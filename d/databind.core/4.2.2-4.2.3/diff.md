# Comparing `tmp/databind.core-4.2.2.tar.gz` & `tmp/databind.core-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind.core-4.2.2.tar", max compression
+gzip compressed data, was "databind.core-4.2.3.tar", max compression
```

## Comparing `databind.core-4.2.2.tar` & `databind.core-4.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1727 2022-11-30 15:24:22.313944 databind.core-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     1245 2022-11-28 15:36:02.170436 databind.core-4.2.2/readme.md
--rw-r--r--   0        0        0       22 2022-11-30 15:24:22.313944 databind.core-4.2.2/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5559 2022-11-21 16:31:06.132972 databind.core-4.2.2/src/databind/core/context.py
--rw-r--r--   0        0        0     4869 2022-11-21 16:31:06.132972 databind.core-4.2.2/src/databind/core/converter.py
--rw-r--r--   0        0        0     4100 2022-11-21 16:31:06.132972 databind.core-4.2.2/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2022-11-21 16:31:06.132972 databind.core-4.2.2/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2022-11-21 16:31:06.132972 databind.core-4.2.2/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2022-11-21 16:31:06.132972 databind.core-4.2.2/src/databind/core/py.typed
--rw-r--r--   0        0        0    15139 2022-11-21 16:31:06.136972 databind.core-4.2.2/src/databind/core/schema.py
--rw-r--r--   0        0        0    26831 2022-11-30 15:24:15.341984 databind.core-4.2.2/src/databind/core/settings.py
--rw-r--r--   0        0        0     8709 2022-11-21 16:31:06.136972 databind.core-4.2.2/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2022-11-21 16:31:06.136972 databind.core-4.2.2/src/databind/core/utils.py
--rw-r--r--   0        0        0     2186 2022-11-30 15:25:07.877947 databind.core-4.2.2/setup.py
--rw-r--r--   0        0        0     2343 2022-11-30 15:25:07.878360 databind.core-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1727 2023-04-12 21:58:45.391794 databind.core-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1245 2023-03-01 15:01:37.487224 databind.core-4.2.3/readme.md
+-rw-r--r--   0        0        0       22 2023-04-12 21:58:45.391794 databind.core-4.2.3/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5558 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/context.py
+-rw-r--r--   0        0        0     4869 2023-04-12 21:47:28.043974 databind.core-4.2.3/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15320 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/schema.py
+-rw-r--r--   0        0        0    26830 2023-04-12 21:58:39.471732 databind.core-4.2.3/src/databind/core/settings.py
+-rw-r--r--   0        0        0     8709 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2023-03-01 15:01:37.487224 databind.core-4.2.3/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2186 2023-04-12 21:58:57.866877 databind.core-4.2.3/setup.py
+-rw-r--r--   0        0        0     2343 2023-04-12 21:58:57.867233 databind.core-4.2.3/PKG-INFO
```

### Comparing `databind.core-4.2.2/pyproject.toml` & `databind.core-4.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.2.2"
+version = "4.2.3"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "databind/core", from = "src"}]
 
 [tool.poetry.urls]
```

### Comparing `databind.core-4.2.2/readme.md` & `databind.core-4.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.2/src/databind/core/context.py` & `databind.core-4.2.3/src/databind/core/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,14 @@
 def format_context_trace(ctx: Context) -> str:
     """Formats a trace for the given context that is convenient to inspect in case of errors to understand where the
     context is pointing to in the payload that is being converted."""
 
     lines = []
     prev_filename: t.Union[str, None] = None
     for ctx in reversed(list(ctx.iter_hierarchy_up())):
-
         # On the first context, or if the filename changed, we output the filename.
         if ctx.location.filename != prev_filename and ctx.location.filename is not None:
             lines.append(f'In "{ctx.location.filename}"')
             prev_filename = ctx.location.filename
 
         if ctx.key is Context.ROOT:
             key = "$"
```

### Comparing `databind.core-4.2.2/src/databind/core/converter.py` & `databind.core-4.2.3/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.2/src/databind/core/dataclasses.py` & `databind.core-4.2.3/src/databind/core/dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
 
 def _field_has_default(field: Field) -> bool:
     return any(x != MISSING for x in (field.default, field.default_factory))  # type: ignore
 
 
 def _process_class(cls, **kwargs):
-
     # Collect a list of the fields that have no default values but follow after a default argument.
     no_default_fields: t.List[str] = []
     existing_fields = getattr(cls, "__dataclass_fields__", {})  # For subclasses of dataclasses
     annotations = getattr(cls, "__annotations__", {})
     if "__annotations__" not in cls.__dict__:
         # Make sure that __annotations__ exists on the class itself.
         cls.__annotations__ = annotations
```

### Comparing `databind.core-4.2.2/src/databind/core/dataclasses.pyi` & `databind.core-4.2.3/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.2/src/databind/core/mapper.py` & `databind.core-4.2.3/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.2/src/databind/core/schema.py` & `databind.core-4.2.3/src/databind/core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,18 @@
 
     annotations = []
     if isinstance(hint, AnnotatedTypeHint):
         annotations = list(hint.metadata)
         hint = hint[0]
 
     if isinstance(hint, ClassTypeHint) and dataclasses.is_dataclass(hint.type):
-        schema = convert_dataclass_to_schema(hint.type)
+        schema = convert_dataclass_to_schema(hint)
     elif isinstance(hint, ClassTypeHint) and is_typed_dict(hint.type):
+        # TODO(@NiklasRosenstein): Pass in the original TypeHint which will contain information about
+        #   TypeVar parametrization that is lost when we just pass the generic type.
         schema = convert_typed_dict_to_schema(hint.type)
     else:
         raise ValueError(f"cannot be converted to a schema (not a dataclass or TypedDict): {type_repr(original_hint)}")
 
     schema.annotations.extend(annotations)
     return schema
 
@@ -300,15 +302,14 @@
     assert is_typed_dict(typed_dict), typed_dict
 
     eval_context = vars(sys.modules[typed_dict.__module__])
 
     annotations = get_annotations(t.cast(type, typed_dict))
     fields: t.Dict[str, Field] = {}
     for key in typed_dict.__required_keys__ | typed_dict.__optional_keys__:
-
         field_hint = TypeHint(annotations[key]).evaluate(eval_context)
 
         has_default = hasattr(typed_dict, key)
         required = _is_required(field_hint, not has_default)
         fields[key] = Field(
             datatype=field_hint,
             required=required and typed_dict.__total__,
```

### Comparing `databind.core-4.2.2/src/databind/core/settings.py` & `databind.core-4.2.3/src/databind/core/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 
     def __init__(self) -> None:
         if type(self) is Setting:
             raise TypeError("Setting cannot be directly instantiated")
 
 
 class ClassDecoratorSetting(Setting):
-
     bound_to: t.Optional[type] = None
 
     def __init__(self) -> None:
         if type(self) is ClassDecoratorSetting:
             raise TypeError("ClassDecoratorSetting cannot be directly instantiated")
         super().__init__()
```

### Comparing `databind.core-4.2.2/src/databind/core/union.py` & `databind.core-4.2.3/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.2/src/databind/core/utils.py` & `databind.core-4.2.3/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind.core-4.2.2/setup.py` & `databind.core-4.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nr-date>=2.0.0,<3.0.0',
  'nr-stream>=1.0.0,<2.0.0',
  'typeapi>=1.2.1,<2.0.0',
  'typing-extensions>=3.10.0']
 
 setup_kwargs = {
     'name': 'databind.core',
-    'version': '4.2.2',
+    'version': '4.2.3',
     'description': 'Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.',
     'long_description': '# databind.core\n\n`databind.core` provides a jackson-databind inspired framework for data de-/serialization in Python. Unless you\nare looking to implement support for de-/serializing new data formats, the `databind.core` package alone might\nnot be what you are looking for (unless you want to use `databind.core.dataclasses` as a drop-in replacement to\nthe standard library `dataclasses` module, for that check out the section at the bottom).\n\n### Known implementations\n\n* [databind.json](https://pypi.org/project/databind.json)\n\n### Dataclass extension\n\nThe standard library `dataclasses` module does not allow to define non-default arguments after default arguments.\nYou can use `databind.core.dataclasses` as a drop-in replacement to get this feature. It behaves exactly like the\nstandard library, only that non-default arguments may follow default arguments. Such arguments can be passed to\nthe constructor as positional or keyword arguments.\n\n```py\nfrom databind.core import dataclasses\n\n@dataclasses.dataclass\nclass A:\n  value1: int = 42\n\n@dataclasses.dataclass\nclass B(A):\n  value2: str\n\nprint(B(0, \'Hello, World!\'))\nprint(B(value2=\'Answer to the universe\'))\n```\n\n---\n\n<p align="center">Copyright &copy; 2020 &ndash; Niklas Rosenstein</p>\n',
     'author': 'Niklas Rosenstein',
     'author_email': 'rosensteinniklas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `databind.core-4.2.2/PKG-INFO` & `databind.core-4.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.2.2
+Version: 4.2.3
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.7 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

