# Comparing `tmp/typeapi-1.4.1.tar.gz` & `tmp/typeapi-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeapi-1.4.1.tar", max compression
+gzip compressed data, was "typeapi-1.4.2.tar", max compression
```

## Comparing `typeapi-1.4.1.tar` & `typeapi-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      991 2023-03-01 15:02:00.051150 typeapi-1.4.1/LICENSE
--rw-r--r--   0        0        0     2215 2023-03-23 10:32:08.876438 typeapi-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     4481 2023-03-23 10:30:24.377082 typeapi-1.4.1/readme.md
--rw-r--r--   0        0        0      595 2023-03-23 10:32:08.876438 typeapi-1.4.1/src/typeapi/__init__.py
--rw-r--r--   0        0        0     4883 2023-03-02 10:19:24.777783 typeapi-1.4.1/src/typeapi/backport/inspect.py
--rw-r--r--   0        0        0     5452 2023-03-01 15:02:00.051150 typeapi-1.4.1/src/typeapi/future/astrewrite.py
--rw-r--r--   0        0        0     2342 2023-03-23 10:28:28.261353 typeapi-1.4.1/src/typeapi/future/fake.py
--rw-r--r--   0        0        0     1570 2023-03-01 15:02:00.051150 typeapi-1.4.1/src/typeapi/future/fake_test.py
--rw-r--r--   0        0        0        0 2023-03-01 15:02:00.051150 typeapi-1.4.1/src/typeapi/py.typed
--rw-r--r--   0        0        0    14944 2023-03-01 15:24:22.286372 typeapi-1.4.1/src/typeapi/typehint.py
--rw-r--r--   0        0        0    14662 2023-03-01 15:05:41.738336 typeapi-1.4.1/src/typeapi/typehint_test.py
--rw-r--r--   0        0        0    13292 2023-03-23 10:20:40.926339 typeapi-1.4.1/src/typeapi/utils.py
--rw-r--r--   0        0        0    15733 2023-03-23 10:30:37.945516 typeapi-1.4.1/src/typeapi/utils_test.py
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 typeapi-1.4.1/setup.py
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 typeapi-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      991 2023-03-01 15:02:00.051150 typeapi-1.4.2/LICENSE
+-rw-r--r--   0        0        0     2215 2023-04-12 22:39:01.286876 typeapi-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4481 2023-03-23 10:30:24.377082 typeapi-1.4.2/readme.md
+-rw-r--r--   0        0        0      595 2023-04-12 22:39:01.286876 typeapi-1.4.2/src/typeapi/__init__.py
+-rw-r--r--   0        0        0     4883 2023-03-02 10:19:24.777783 typeapi-1.4.2/src/typeapi/backport/inspect.py
+-rw-r--r--   0        0        0     5505 2023-04-12 22:28:15.607915 typeapi-1.4.2/src/typeapi/future/astrewrite.py
+-rw-r--r--   0        0        0     2342 2023-04-12 22:36:27.277248 typeapi-1.4.2/src/typeapi/future/fake.py
+-rw-r--r--   0        0        0     1570 2023-03-01 15:02:00.051150 typeapi-1.4.2/src/typeapi/future/fake_test.py
+-rw-r--r--   0        0        0        0 2023-03-01 15:02:00.051150 typeapi-1.4.2/src/typeapi/py.typed
+-rw-r--r--   0        0        0    15204 2023-04-12 22:18:08.512957 typeapi-1.4.2/src/typeapi/typehint.py
+-rw-r--r--   0        0        0    14932 2023-04-12 22:20:39.278551 typeapi-1.4.2/src/typeapi/typehint_test.py
+-rw-r--r--   0        0        0    13473 2023-04-12 22:18:08.516957 typeapi-1.4.2/src/typeapi/utils.py
+-rw-r--r--   0        0        0    16298 2023-04-12 22:29:54.749041 typeapi-1.4.2/src/typeapi/utils_test.py
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 typeapi-1.4.2/setup.py
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 typeapi-1.4.2/PKG-INFO
```

### Comparing `typeapi-1.4.1/LICENSE` & `typeapi-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typeapi-1.4.1/pyproject.toml` & `typeapi-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # NOTE(NiklasRosenstein): We pin this version so we can keep using the old way that Slap supports installing
 #                         the "docs" extra without Poetry complaining about invalid format of the requirements.
 requires = ["poetry-core==1.1.0a6"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "typeapi"
-version = "1.4.1"
+version = "1.4.2"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "typeapi", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `typeapi-1.4.1/readme.md` & `typeapi-1.4.2/readme.md`

 * *Files identical despite different names*

### Comparing `typeapi-1.4.1/src/typeapi/__init__.py` & `typeapi-1.4.2/src/typeapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 from .typehint import (
     AnnotatedTypeHint,
     ClassTypeHint,
     ForwardRefTypeHint,
     LiteralTypeHint,
     TupleTypeHint,
```

### Comparing `typeapi-1.4.1/src/typeapi/backport/inspect.py` & `typeapi-1.4.2/src/typeapi/backport/inspect.py`

 * *Files identical despite different names*

### Comparing `typeapi-1.4.1/src/typeapi/future/astrewrite.py` & `typeapi-1.4.2/src/typeapi/future/astrewrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 T_AST = t.TypeVar("T_AST", bound=ast.AST)
 
 
 def rewrite_expr(source: str, lookup_target: str) -> CodeType:
     expr = ast.parse(source, "<expr>", "eval")
     expr = DynamicLookupRewriter(lookup_target).visit(expr)
     ast.fix_missing_locations(expr)
-    return t.cast(CodeType, compile(expr, "<expr>", "eval"))
+    return t.cast(CodeType, compile(expr, "<expr>", "eval"))  # type: ignore[redundant-cast]  # Redundant in 3.7+
 
 
 @dataclasses.dataclass
 class DynamicLookupRewriter(ast.NodeTransformer):
     # TODO(NiklasRosenstein): Handle more nodes that define local variables and := operator.
 
     #: The variable name of the target object that name resolution should occur through.
```

### Comparing `typeapi-1.4.1/src/typeapi/future/fake.py` & `typeapi-1.4.2/src/typeapi/future/fake.py`

 * *Files identical despite different names*

### Comparing `typeapi-1.4.1/src/typeapi/future/fake_test.py` & `typeapi-1.4.2/src/typeapi/future/fake_test.py`

 * *Files identical despite different names*

### Comparing `typeapi-1.4.1/src/typeapi/typehint.py` & `typeapi-1.4.2/src/typeapi/typehint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import abc
+import sys
+from collections import ChainMap
 from types import ModuleType
-from typing import Any, Dict, Generic, Iterator, List, Mapping, Tuple, TypeVar, Union, overload
+from typing import Any, Dict, Generic, Iterator, List, Mapping, MutableMapping, Tuple, TypeVar, Union, cast, overload
 
 from typing_extensions import Annotated
 
 from .utils import (
     ForwardRef,
     HasGetitem,
     get_subscriptable_type_hint_from_origin,
@@ -232,15 +234,20 @@
                 "to which we could fall back to. Specify the `context` argument or make sure that the type "
                 "hint's `.source` is set."
             )
         if isinstance(self.source, ModuleType):
             return vars(self.source)
         if isinstance(self.source, Mapping):
             return self.source
-        return vars(self.source.__module__)  # type: ignore[no-any-return] # Should be a function or class, something that has __module__  # noqa: E501
+        if isinstance(self.source, type):
+            return ChainMap(
+                cast(MutableMapping[str, Any], vars(self.source)),
+                cast(MutableMapping[str, Any], vars(sys.modules[self.source.__module__])),
+            )
+        raise RuntimeError(f"Unable to determine TypeHint.source context from source={self.source!r}")
 
 
 class ClassTypeHint(TypeHint):
     def __init__(self, hint: object, source: "Any | None" = None) -> None:
         super().__init__(hint, source)
         assert isinstance(self.hint, type) or isinstance(self.origin, type), (
             "ClassTypeHint must be initialized from a real type or a generic that points to a real type. "
```

### Comparing `typeapi-1.4.1/src/typeapi/typehint_test.py` & `typeapi-1.4.2/src/typeapi/typehint_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,14 +365,26 @@
 
     hint = TypeHint(List["str"]).evaluate(Mapping())
     item_hint = hint[0]
     assert isinstance(item_hint, ClassTypeHint)
     assert item_hint.type is int
 
 
+def test__TypeHint__evaluate_forward_reference_on_class_level() -> None:
+    class A:
+        class B:
+            pass
+
+    hint = TypeHint("B", A)
+    assert hint.evaluate() == TypeHint(A.B)
+
+    hint = TypeHint("str", A)
+    assert hint.evaluate() == TypeHint(str)
+
+
 def test__TypeHint__caching_same_named_type_hints() -> None:
     """
     This test ensures that type hint caching is stable if two different
     definitions with the same are encountered.
     """
 
     class A:
```

### Comparing `typeapi-1.4.1/src/typeapi/utils.py` & `typeapi-1.4.2/src/typeapi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import sys
 import types
 import typing
 import warnings
 from types import FrameType, FunctionType, ModuleType
-from typing import Any, Callable, Dict, Generic, Optional, Set, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, Generic, MutableMapping, Optional, Set, Tuple, TypeVar, Union, cast
 
 import typing_extensions
 from typing_extensions import Protocol, TypeGuard
 
 from .backport.inspect import get_annotations as _inspect_get_annotations
 
 IS_PYTHON_AT_LAST_3_6 = sys.version_info[:2] <= (3, 6)
@@ -327,16 +327,19 @@
             assert hasattr(module, "__dict__"), module
             globalns = vars(module)
 
     from collections import ChainMap
 
     from .typehint import TypeHint
 
-    def eval_callback(obj: str, globals: Any, locals: Any) -> Any:
-        hint = TypeHint(obj, ChainMap(locals or {}, globals or {}))
+    def eval_callback(hint_expr: str, globals: Any, locals: Any) -> Any:
+        chainmap = ChainMap(locals or {}, globals or {})
+        if isinstance(obj, type):
+            chainmap = chainmap.new_child(cast(MutableMapping[str, Any], vars(obj)))
+        hint = TypeHint(hint_expr, chainmap)
         return hint.evaluate().hint
 
     annotations = _inspect_get_annotations(obj, globals=globalns, locals=localns, eval_str=eval_str, eval=eval_callback)
 
     if isinstance(obj, type) and include_bases:
         annotations = {}
         for base in obj.__mro__:
```

### Comparing `typeapi-1.4.1/src/typeapi/utils_test.py` & `typeapi-1.4.2/src/typeapi/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import typing as t
 from typing import Any, Dict, Generic, List, Mapping, MutableMapping, Optional, TypeVar, Union
 
 import pytest
 import typing_extensions
 
 from typeapi.utils import (
+    IS_PYTHON_AT_LEAST_3_7,
+    IS_PYTHON_AT_LEAST_3_9,
     ForwardRef,
     get_annotations,
     get_subscriptable_type_hint_from_origin,
     get_type_hint_args,
     get_type_hint_origin_or_none,
     get_type_hint_original_bases,
     get_type_hint_parameters,
@@ -425,38 +427,59 @@
     assert get_subscriptable_type_hint_from_origin(dict) is Dict
     assert get_subscriptable_type_hint_from_origin(Mapping) is Mapping
     assert get_subscriptable_type_hint_from_origin(collections.abc.Mapping) is Mapping
     assert get_subscriptable_type_hint_from_origin(T) is T
     assert get_subscriptable_type_hint_from_origin(int) is int
 
 
-def test__get_annotations_does_not_evaluate_strings() -> None:
+def test__get_annotations__does_not_evaluate_strings() -> None:
     class A:
         a: "str | None"
 
     assert get_annotations(A, eval_str=False) == {"a": "str | None"}
 
 
-def test__get_annotations_includes_bases() -> None:
+def test__get_annotations__includes_bases() -> None:
     class A:
         a: "str | None"
         b: int
 
     class B(A):
         b: "str"
         c: Optional[int]
 
     assert get_annotations(B, include_bases=True, eval_str=False) == {"a": "str | None", "b": "str", "c": Optional[int]}
 
 
-def test__get_annotations_can_evaluate_future_type_hints() -> None:
+def test__get_annotations__can_evaluate_future_type_hints() -> None:
     class A:
         a: "str | None"
 
     annotations = get_annotations(A)
     assert annotations == {"a": Optional[str]}
 
-    from typing import _UnionGenericAlias  # type: ignore
-
     # NOTE(@NiklasRosenstein): Even though `str | None` is of type `types.UnionType` in Python 3.10+,
     #   our fake evaluation will still return legacy type hints.
-    assert type(annotations["a"]) is _UnionGenericAlias
+    if IS_PYTHON_AT_LEAST_3_9:
+        from typing import _UnionGenericAlias  # type: ignore
+
+        assert type(annotations["a"]) is _UnionGenericAlias
+
+    elif IS_PYTHON_AT_LEAST_3_7:
+        from typing import _GenericAlias  # type: ignore
+
+        assert type(annotations["a"]) is _GenericAlias
+
+    else:
+        assert str(type(annotations["a"])) == "typing.Union"
+
+
+def test__get_annotations__evaluate_forward_references_on_class_level() -> None:
+    class A:
+        class B:
+            pass
+
+        a: "str"
+        b: "B"
+
+    annotations = get_annotations(A)
+    assert annotations == {"a": str, "b": A.B}
```

### Comparing `typeapi-1.4.1/setup.py` & `typeapi-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['typing-extensions>=3.0.0']
 
 setup_kwargs = {
     'name': 'typeapi',
-    'version': '1.4.1',
+    'version': '1.4.2',
     'description': '',
     'long_description': '# typeapi\n\n[![Python](https://github.com/NiklasRosenstein/python-typeapi/actions/workflows/python.yml/badge.svg)](https://github.com/NiklasRosenstein/python-typeapi/actions/workflows/python.yml)\n\n  [PEP484]: https://peps.python.org/pep-0484/\n  [PEP585]: https://peps.python.org/pep-0585/\n  [PEP604]: https://peps.python.org/pep-0604/\n\n__Compatibility__: Python 3.6.3+\n\nThe `typeapi` package provides an object-oriented interface for introspecting [PEP484][] type hints at runtime,\nincluding forward references that make use of the more recent [PEP585][] and [PEP604][] type hint features in\nPython versions that don\'t natively support them.\n\nThe main API of this module is comprised of:\n\n* `typeapi.TypeHint()` &ndash; A class to parse low-level type hints and present them in a consistent, object-oriented API.\n* `typeapi.get_annotations()` &ndash; Retrieve an object\'s `__annotations__` with support for evaluating future type hints ([PEP585][], [PEP604][]).\n\nThe following kinds of type hints are currently supported:\n\n| Concrete type | Description | Added in |\n| ------------- | ----------- | -------- |\n| `ClassTypeHint` | For any normal or generic type as well as `typing.Any`. Provides access to the underlying type, the type arguments and parameters, if any. | 1.0.0 |\n| `UnionTypeHint` | Represents `Union` type hint and gives access to the union members. | 1.0.0 |\n| `LiteralTypeHint` | Represents a `Literal` type hint and gives access to the literal values. | 1.0.0 |\n| `AnnotatedTypeHint` | Represents an `Annotated` type hint and gives access to the annotated type as well as the metadata. | 1.0.0 |\n| `TypeVarTypeHint` | Represents a `TypeVar` type hint and gives an interface to access the variable\'s metadata (such as constarints, variance, ...). | 1.0.0 |\n| `ForwardRefTypeHint` | Represents a forward reference. Can be evaluated in Python 3.6+ even if it contains [PEP585][] and [PEP604][] expressions. <sup>1)</sup> | 1.0.0, future support in 1.3.0 |\n| `TupleTypeHint` | Reperesents a `Tuple` type hint, allowing you to differentiate between repeated and explicitly sized tuples. | 1.2.0 |\n\n<sup>1)</sup> New-style type union evaluation will continue to return a `typing.Union`, even if the same syntax\nevaluated natively by Python 3.10+ results in a `types.UnionType`.\n\n## Examples\n\nInspect a `List[int]` type hint:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import ClassTypeHint, TypeHint\nfrom typing import List\n\nhint = TypeHint(List[int])\nassert isinstance(hint, ClassTypeHint)\nassert hint.type is list\n\nitem_hint = hint[0]\nassert isinstance(item_hint, ClassTypeHint)\nassert item_hint.type is int\n```\n\nRetrieve the metadata from an `Annotated[...]` type hint:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import AnnotatedTypeHint, ClassTypeHint, TypeHint\nfrom typing_extensions import Annotated\n\nhint = TypeHint(Annotated[int, 42])\nassert isinstance(hint, AnnotatedTypeHint)\nassert hint.type is int\nassert hint.metadata == (42,)\n\nsub_hint = hint[0]\nassert isinstance(sub_hint, ClassTypeHint)\nassert sub_hint.type is int\n```\n\nParameterize one type hint with the parameterization of a generic alias:\n\n```py\n# cat <<EOF | python -\nfrom dataclasses import dataclass\nfrom typeapi import ClassTypeHint, TypeHint\nfrom typing import Generic, TypeVar\nfrom typing_extensions import Annotated\n\nT = TypeVar("T")\n\n@dataclass\nclass MyGeneric(Generic[T]):\n  value: T\n\nhint = TypeHint(MyGeneric[int])\nassert isinstance(hint, ClassTypeHint)\nassert hint.get_parameter_map() == {T: int}\n\nmember_hint = TypeHint(T).parameterize(hint.get_parameter_map())\nassert isinstance(member_hint, ClassTypeHint)\nassert member_hint.type is int\n```\n\nEvaluate forward references with `get_annotations()`:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import get_annotations\nfrom typing import Optional\nfrom sys import version_info\n\nclass MyType:\n  a: "str | None"\n\nannotations = get_annotations(MyType)\n\nif version_info[:2] < (3, 10):\n  assert annotations == {"a": Optional[str]}\nelse:\n  assert annotations == {"a": str | None}\n```\n\nEvaluating forward references with the `TypeHint` API:\n\n```py\n# cat <<EOF | python -\nfrom typeapi import ClassTypeHint, ForwardRefTypeHint, TypeHint\n\nMyVector = "list[MyType]"\n\nclass MyType:\n  pass\n\nhint = TypeHint(MyVector).evaluate(globals())\nprint(hint)  # TypeHint(typing.List[__main__.MyType])\nassert isinstance(hint, ClassTypeHint)\nassert hint.type is list\n\nitem_hint = hint[0]\nassert isinstance(item_hint, ClassTypeHint)\nassert item_hint.type is MyType\n```\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `typeapi-1.4.1/PKG-INFO` & `typeapi-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeapi
-Version: 1.4.1
+Version: 1.4.2
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

