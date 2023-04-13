# Comparing `tmp/pydwrap-0.5.6.tar.gz` & `tmp/pydwrap-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwrap-0.5.6.tar", max compression
+gzip compressed data, was "pydwrap-0.5.7.tar", max compression
```

## Comparing `pydwrap-0.5.6.tar` & `pydwrap-0.5.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-03-24 13:21:49.321460 pydwrap-0.5.6/LICENSE
--rw-r--r--   0        0        0     1205 2023-03-24 13:53:27.176284 pydwrap-0.5.6/README.md
--rw-r--r--   0        0        0       69 2023-03-30 16:20:21.356084 pydwrap-0.5.6/pydwrap/__init__.py
--rw-r--r--   0        0        0     4078 2023-03-31 16:20:00.757494 pydwrap-0.5.6/pydwrap/main.py
--rw-r--r--   0        0        0     1203 2023-03-31 16:21:00.910249 pydwrap-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 pydwrap-0.5.6/setup.py
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pydwrap-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-03-24 13:21:49.321460 pydwrap-0.5.7/LICENSE
+-rw-r--r--   0        0        0     1205 2023-03-24 13:53:27.176284 pydwrap-0.5.7/README.md
+-rw-r--r--   0        0        0       69 2023-03-30 16:20:21.356084 pydwrap-0.5.7/pydwrap/__init__.py
+-rw-r--r--   0        0        0     4168 2023-04-13 21:03:38.694510 pydwrap-0.5.7/pydwrap/main.py
+-rw-r--r--   0        0        0     1203 2023-04-13 21:05:56.281711 pydwrap-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 pydwrap-0.5.7/setup.py
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pydwrap-0.5.7/PKG-INFO
```

### Comparing `pydwrap-0.5.6/LICENSE` & `pydwrap-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwrap-0.5.6/README.md` & `pydwrap-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pydwrap-0.5.6/pydwrap/main.py` & `pydwrap-0.5.7/pydwrap/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pydantic import BaseModel as OriginalBaseModel
 from pydantic import create_model, root_validator
 from pydantic.fields import ModelField
 from pydantic.typing import is_none_type
 
 _T = TypeVar("_T")
 _V = TypeVar("_V")
+ValidatorOptionValue = TypeVar("ValidatorOptionValue", bound="BaseModel")
 
 
 class Option(Generic[_T]):
     """Type Option in order to correctly handle optional value."""
 
     __value: _T | None
 
@@ -30,15 +31,15 @@
 
     @classmethod
     def __get_validators__(cls):
         yield cls.option_validator
 
     @classmethod
     def option_validator(cls, v: Any, field: ModelField) -> Option[_T]:
-        field_name = field.name.removeprefix("_").removesuffix("_")
+        field_name: str = field.name.removeprefix("_").removesuffix("_")
         if field.outer_type_ is Option:
             raise TypeError("To type an Option, it is necessary to specify a parameter in its generic.")
         if v is None:
             return cls(v)
         if isinstance(v, cls) and v.is_none:
             return v
         validator = _create_validator_option_value(
@@ -105,15 +106,15 @@
     return {
         k: Option()
         for k in properties
         if k in schema.get("required", []) or "default" not in properties[k] and _is_option_type(model_annotations[k])
     }
 
 
-def _create_validator_option_value(field_name: str, field_value: Any, field_type: Type[Any]) -> BaseModel:
+def _create_validator_option_value(field_name: str, field_value: Any, field_type: Type[Any]) -> ValidatorOptionValue:
     return create_model(
         "ValidatorOptionValue",
         __base__=BaseModel,
         **{
             field_name: (
                 field_type,
                 field_value,
```

### Comparing `pydwrap-0.5.6/pyproject.toml` & `pydwrap-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydwrap"
-version = "0.5.6"
+version = "0.5.7"
 description = "pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object."
 authors = ["Georgy howl <howluwqz1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydwrap"}]
 homepage = "https://github.com/luwqz1/pydwrap"
 repository = "https://github.com/luwqz1/pydwrap"
```

### Comparing `pydwrap-0.5.6/setup.py` & `pydwrap-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'pydwrap',
-    'version': '0.5.6',
+    'version': '0.5.7',
     'description': 'pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object.',
     'long_description': '# ♻️ pydwrap pydantic optional fields ♻️\n\n\npydwrap stores a **Option** object to implement unpacking of values if they are not **None**. The **BaseModel** object is also a little extended to work with the **Option** object.\n\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pypi](https://img.shields.io/pypi/v/pydwrap.svg)](https://pypi.python.org/pypi/pydwrap)\n[![versions](https://img.shields.io/pypi/pyversions/pydwrap.svg)](https://github.com/luwqz1/pydwrap)\n[![license](https://img.shields.io/github/license/luwqz1/pydwrap.svg)](https://github.com/luwqz1/pydwrap/blob/main/LICENSE)\n\n\n# ⭐️ A simple example ⭐️\n```python\nfrom pydwrap import BaseModel, Option\n\nclass User(BaseModel):\n    name: Option[str]\n    age: int\n\ndata = {\n    "age": 20\n}\nuser = User(**data)\n#> User(name=Option(None), age=20)\nprint("Hello", user.name.unwrap(error_msg="What\'s your name?") + "!")\n#> ValueError: What\'s your name?\n```\n\n# 📚 Documentation 📚\n* In 🇷🇺 [**Russian**](https://github.com/luwqz1/pydwrap/blob/main/docs/RU.md) 🇷🇺\n* In 🇺🇸 [**English**](https://github.com/luwqz1/pydwrap/blob/main/docs/EN.md) 🇺🇸',
     'author': 'Georgy howl',
     'author_email': 'howluwqz1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luwqz1/pydwrap',
```

### Comparing `pydwrap-0.5.6/PKG-INFO` & `pydwrap-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwrap
-Version: 0.5.6
+Version: 0.5.7
 Summary: pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object.
 Home-page: https://github.com/luwqz1/pydwrap
 License: MIT
 Keywords: python,wrapping,optional handle,basemodel fields,option,pydwrap
 Author: Georgy howl
 Author-email: howluwqz1@gmail.com
 Requires-Python: >=3.9,<4.0
```

