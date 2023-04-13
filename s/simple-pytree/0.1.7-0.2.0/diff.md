# Comparing `tmp/simple_pytree-0.1.7.tar.gz` & `tmp/simple_pytree-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pytree-0.1.7.tar", max compression
+gzip compressed data, was "simple_pytree-0.2.0.tar", max compression
```

## Comparing `simple_pytree-0.1.7.tar` & `simple_pytree-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-03-19 17:40:03.820615 simple_pytree-0.1.7/LICENSE
--rw-r--r--   0        0        0     3455 2023-03-19 17:40:03.820615 simple_pytree-0.1.7/README.md
--rw-r--r--   0        0        0      512 2023-03-19 17:40:03.820615 simple_pytree-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      118 2023-03-19 17:40:03.820615 simple_pytree-0.1.7/simple_pytree/__init__.py
--rw-r--r--   0        0        0     8512 2023-03-19 17:40:03.820615 simple_pytree-0.1.7/simple_pytree/pytree.py
--rw-r--r--   0        0        0     4008 1970-01-01 00:00:00.000000 simple_pytree-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-13 17:46:32.740828 simple_pytree-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3554 2023-04-13 17:46:32.740828 simple_pytree-0.2.0/README.md
+-rw-r--r--   0        0        0      595 2023-04-13 17:46:32.744828 simple_pytree-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-04-13 17:46:32.744828 simple_pytree-0.2.0/simple_pytree/__init__.py
+-rw-r--r--   0        0        0     2293 2023-04-13 17:46:32.744828 simple_pytree-0.2.0/simple_pytree/dataclass.py
+-rw-r--r--   0        0        0     8421 2023-04-13 17:46:32.744828 simple_pytree-0.2.0/simple_pytree/pytree.py
+-rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 simple_pytree-0.2.0/PKG-INFO
```

### Comparing `simple_pytree-0.1.7/LICENSE` & `simple_pytree-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_pytree-0.1.7/README.md` & `simple_pytree-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,32 +68,34 @@
 assert foo.x == -1 and foo.y == 2
 ```
 
 Static fields are not included in the pytree leaves, they
 are passed as pytree metadata instead.
 
 ### Dataclasses
-You can seamlessly use the `dataclasses.dataclass` decorator with `Pytree` classes.
-Since `static_field` returns instances of `dataclasses.Field` these it will work as expected:
+`simple_pytree` provides a `dataclass` decorator you can use with classes
+that contain `static_field`s:
 
 ```python
 import jax
-from dataclasses import dataclass
-from simple_pytree import Pytree, static_field
+from simple_pytree import Pytree, dataclass, static_field
 
 @dataclass
 class Foo(Pytree):
     x: int
-    y: int = static_field(2) # with default value
+    y: int = static_field(default=2)
     
 foo = Foo(1)
 foo = jax.tree_map(lambda x: -x, foo) # y is not modified
 
 assert foo.x == -1 and foo.y == 2
 ```
+`simple_pytree.dataclass` is just a wrapper around `dataclasses.dataclass` but
+when used static analysis tools and IDEs will understand that `static_field` is a 
+field specifier just like `dataclasses.field`.
 
 ### Mutability
 `Pytree` objects are immutable by default after `__init__`:
 
 ```python
 from simple_pytree import Pytree, static_field
```

### Comparing `simple_pytree-0.1.7/pyproject.toml` & `simple_pytree-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [tool.poetry]
 name = "simple-pytree"
-version = "0.1.7"
+version = "0.2.0"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "simple_pytree"}]
+packages = [{ include = "simple_pytree" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 jax = "*"
 jaxlib = "*"
+typing-extensions = "*"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.1"
 pytest-cov = ">=4.0.0"
 pre-commit = ">=3.0.4"
 black = "23.1.0"
 isort = "5.12.0"
 flax = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.coverage.report]
+exclude_lines = ["@tp.overload"]
```

### Comparing `simple_pytree-0.1.7/simple_pytree/pytree.py` & `simple_pytree-0.2.0/simple_pytree/pytree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,131 +1,107 @@
 import dataclasses
 import importlib.util
-import itertools
+import inspect
 import typing as tp
 from abc import ABCMeta
 from copy import copy
 from functools import partial
+from types import MappingProxyType
 
 import jax
 
 P = tp.TypeVar("P", bound="Pytree")
 
 
-def field(
-    default: tp.Any = dataclasses.MISSING,
-    *,
-    pytree_node: bool = True,
-    default_factory: tp.Any = dataclasses.MISSING,
-    init: bool = True,
-    repr: bool = True,
-    hash: tp.Optional[bool] = None,
-    compare: bool = True,
-    metadata: tp.Optional[tp.Mapping[str, tp.Any]] = None,
-):
-    if metadata is None:
-        metadata = {}
-    else:
-        metadata = dict(metadata)
-
-    if "pytree_node" in metadata:
-        raise ValueError("'pytree_node' found in metadata")
-
-    metadata["pytree_node"] = pytree_node
-
-    return dataclasses.field(
-        default=default,
-        default_factory=default_factory,
-        init=init,
-        repr=repr,
-        hash=hash,
-        compare=compare,
-        metadata=metadata,
-    )
-
-
-def static_field(
-    default: tp.Any = dataclasses.MISSING,
-    *,
-    default_factory: tp.Any = dataclasses.MISSING,
-    init: bool = True,
-    repr: bool = True,
-    hash: tp.Optional[bool] = None,
-    compare: bool = True,
-    metadata: tp.Optional[tp.Mapping[str, tp.Any]] = None,
-):
-    return field(
-        default=default,
-        pytree_node=False,
-        default_factory=default_factory,
-        init=init,
-        repr=repr,
-        hash=hash,
-        compare=compare,
-        metadata=metadata,
-    )
-
-
 class PytreeMeta(ABCMeta):
-    def __call__(self: tp.Type[P], *args: tp.Any, **kwargs: tp.Any) -> P:
-        obj: P = self.__new__(self, *args, **kwargs)
+    def __call__(cls: tp.Type[P], *args: tp.Any, **kwargs: tp.Any) -> P:
+        obj: P = cls.__new__(cls, *args, **kwargs)
         obj.__dict__["_pytree__initializing"] = True
         try:
             obj.__init__(*args, **kwargs)
         finally:
             del obj.__dict__["_pytree__initializing"]
+
+        vars_dict = vars(obj)
+        vars_dict["_pytree__node_fields"] = tuple(
+            sorted(
+                field for field in vars_dict if field not in cls._pytree__static_fields
+            )
+        )
         return obj
 
 
 class Pytree(metaclass=PytreeMeta):
     _pytree__initializing: bool
     _pytree__class_is_mutable: bool
-    _pytree__static_fields: tp.FrozenSet[str]
+    _pytree__static_fields: tp.Tuple[str, ...]
+    _pytree__node_fields: tp.Tuple[str, ...]
     _pytree__setter_descriptors: tp.FrozenSet[str]
 
     def __init_subclass__(cls, mutable: bool = False):
         super().__init_subclass__()
 
         # gather class info
         class_vars = vars(cls)
         setter_descriptors = set()
         static_fields = _inherited_static_fields(cls)
 
+        # add special static fields
+        static_fields.add("_pytree__node_fields")
+
         for field, value in class_vars.items():
             if isinstance(value, dataclasses.Field) and not value.metadata.get(
                 "pytree_node", True
             ):
                 static_fields.add(field)
 
             # add setter descriptors
             if hasattr(value, "__set__"):
                 setter_descriptors.add(field)
 
+        static_fields = tuple(sorted(static_fields))
+
         # init class variables
         cls._pytree__initializing = False
         cls._pytree__class_is_mutable = mutable
-        cls._pytree__static_fields = frozenset(static_fields)
+        cls._pytree__static_fields = static_fields
         cls._pytree__setter_descriptors = frozenset(setter_descriptors)
 
+        # TODO: clean up this in the future once minimal supported version is 0.4.7
         if hasattr(jax.tree_util, "register_pytree_with_keys"):
-            jax.tree_util.register_pytree_with_keys(
-                cls,
-                partial(
-                    cls._pytree__flatten,
-                    cls._pytree__static_fields,
-                    with_key_paths=True,
-                ),
-                cls._pytree__unflatten,
-            )
+            if (
+                "flatten_func"
+                in inspect.signature(jax.tree_util.register_pytree_with_keys).parameters
+            ):
+                jax.tree_util.register_pytree_with_keys(
+                    cls,
+                    partial(
+                        cls._pytree__flatten,
+                        with_key_paths=True,
+                    ),
+                    cls._pytree__unflatten,
+                    flatten_func=partial(
+                        cls._pytree__flatten,
+                        with_key_paths=False,
+                    ),
+                )
+            else:
+                jax.tree_util.register_pytree_with_keys(
+                    cls,
+                    partial(
+                        cls._pytree__flatten,
+                        with_key_paths=True,
+                    ),
+                    cls._pytree__unflatten,
+                )
         else:
             jax.tree_util.register_pytree_node(
                 cls,
                 partial(
                     cls._pytree__flatten,
-                    cls._pytree__static_fields,
                     with_key_paths=False,
                 ),
                 cls._pytree__unflatten,
             )
 
         # flax serialization support
         if importlib.util.find_spec("flax") is not None:
@@ -136,67 +112,66 @@
                 partial(cls._to_flax_state_dict, cls._pytree__static_fields),
                 partial(cls._from_flax_state_dict, cls._pytree__static_fields),
             )
 
     @classmethod
     def _pytree__flatten(
         cls,
-        static_field_names: tp.FrozenSet[str],
         pytree: "Pytree",
         *,
         with_key_paths: bool,
-    ) -> tp.Tuple[
-        tp.List[tp.Any],
-        tp.Tuple[tp.List[str], tp.List[tp.Tuple[str, tp.Any]]],
-    ]:
-        static_fields = []
-        node_names = []
-        node_values = []
-        # sort to ensure deterministic order
-        for field in sorted(vars(pytree)):
-            value = getattr(pytree, field)
-            if field in static_field_names:
-                static_fields.append((field, value))
-            else:
-                if with_key_paths:
-                    value = (jax.tree_util.GetAttrKey(field), value)
-                node_names.append(field)
-                node_values.append(value)
+    ) -> tp.Tuple[tp.Tuple[tp.Any, ...], tp.Mapping[str, tp.Any],]:
+        all_vars = vars(pytree).copy()
+        static = {k: all_vars.pop(k) for k in pytree._pytree__static_fields}
+
+        if with_key_paths:
+            node_values = tuple(
+                (jax.tree_util.GetAttrKey(field), all_vars.pop(field))
+                for field in pytree._pytree__node_fields
+            )
+        else:
+            node_values = tuple(
+                all_vars.pop(field) for field in pytree._pytree__node_fields
+            )
 
-        return node_values, (node_names, static_fields)
+        if all_vars:
+            raise ValueError(
+                f"Unexpected fields in {cls.__name__}: {', '.join(all_vars.keys())}"
+            )
+
+        return node_values, MappingProxyType(static)
 
     @classmethod
     def _pytree__unflatten(
         cls: tp.Type[P],
-        metadata: tp.Tuple[tp.List[str], tp.List[tp.Tuple[str, tp.Any]]],
-        node_values: tp.List[tp.Any],
+        static_fields: tp.Mapping[str, tp.Any],
+        node_values: tp.Tuple[tp.Any, ...],
     ) -> P:
-        node_names, static_fields = metadata
-        node_fields = dict(zip(node_names, node_values))
         pytree = object.__new__(cls)
-        pytree.__dict__.update(node_fields, **dict(static_fields))
+        pytree.__dict__.update(zip(static_fields["_pytree__node_fields"], node_values))
+        pytree.__dict__.update(static_fields)
         return pytree
 
     @classmethod
     def _to_flax_state_dict(
-        cls, static_field_names: tp.FrozenSet[str], pytree: "Pytree"
+        cls, static_field_names: tp.Tuple[str, ...], pytree: "Pytree"
     ) -> tp.Dict[str, tp.Any]:
         from flax import serialization
 
         state_dict = {
             name: serialization.to_state_dict(getattr(pytree, name))
             for name in pytree.__dict__
             if name not in static_field_names
         }
         return state_dict
 
     @classmethod
     def _from_flax_state_dict(
         cls,
-        static_field_names: tp.FrozenSet[str],
+        static_field_names: tp.Tuple[str, ...],
         pytree: P,
         state: tp.Dict[str, tp.Any],
     ) -> P:
         """Restore the state of a data class."""
         from flax import serialization
 
         state = state.copy()  # copy the state so we can pop the restored fields.
@@ -242,19 +217,21 @@
         pytree = copy(self)
         pytree.__dict__.update(kwargs)
         return pytree
 
     if not tp.TYPE_CHECKING:
 
         def __setattr__(self: P, field: str, value: tp.Any):
-            if (
-                not self._pytree__initializing
-                and not self._pytree__class_is_mutable
-                and field not in self._pytree__setter_descriptors
-            ):
+            if self._pytree__initializing or field in self._pytree__setter_descriptors:
+                pass
+            elif not hasattr(self, field) and not self._pytree__initializing:
+                raise AttributeError(
+                    f"Cannot add new fields to {type(self)} after initialization"
+                )
+            elif not self._pytree__class_is_mutable:
                 raise AttributeError(
                     f"{type(self)} is immutable, trying to update field {field}"
                 )
 
             object.__setattr__(self, field, value)
```

### Comparing `simple_pytree-0.1.7/PKG-INFO` & `simple_pytree-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: simple-pytree
-Version: 0.1.7
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Cristian Garcia
 Author-email: cgarcia.e88@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jax
 Requires-Dist: jaxlib
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 
 <!-- codecov badge -->
 [![codecov](https://codecov.io/gh/cgarciae/simple-pytree/branch/main/graph/badge.svg?token=3IKEUAU3C8)](https://codecov.io/gh/cgarciae/simple-pytree)
 
 
@@ -86,32 +87,34 @@
 assert foo.x == -1 and foo.y == 2
 ```
 
 Static fields are not included in the pytree leaves, they
 are passed as pytree metadata instead.
 
 ### Dataclasses
-You can seamlessly use the `dataclasses.dataclass` decorator with `Pytree` classes.
-Since `static_field` returns instances of `dataclasses.Field` these it will work as expected:
+`simple_pytree` provides a `dataclass` decorator you can use with classes
+that contain `static_field`s:
 
 ```python
 import jax
-from dataclasses import dataclass
-from simple_pytree import Pytree, static_field
+from simple_pytree import Pytree, dataclass, static_field
 
 @dataclass
 class Foo(Pytree):
     x: int
-    y: int = static_field(2) # with default value
+    y: int = static_field(default=2)
     
 foo = Foo(1)
 foo = jax.tree_map(lambda x: -x, foo) # y is not modified
 
 assert foo.x == -1 and foo.y == 2
 ```
+`simple_pytree.dataclass` is just a wrapper around `dataclasses.dataclass` but
+when used static analysis tools and IDEs will understand that `static_field` is a 
+field specifier just like `dataclasses.field`.
 
 ### Mutability
 `Pytree` objects are immutable by default after `__init__`:
 
 ```python
 from simple_pytree import Pytree, static_field
```

