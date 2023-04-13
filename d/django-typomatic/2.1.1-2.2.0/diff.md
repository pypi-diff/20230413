# Comparing `tmp/django-typomatic-2.1.1.tar.gz` & `tmp/django-typomatic-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-typomatic-2.1.1.tar", last modified: Wed Apr  5 23:42:22 2023, max compression
+gzip compressed data, was "django-typomatic-2.2.0.tar", last modified: Thu Apr 13 04:03:06 2023, max compression
```

## Comparing `django-typomatic-2.1.1.tar` & `django-typomatic-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/django_typomatic/
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/django_typomatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/django_typomatic/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/django_typomatic/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/django_typomatic/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/django_typomatic/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/django_typomatic/management/commands/generate_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/django_typomatic/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/django_typomatic/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/django_typomatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-05 23:42:22.000000 django-typomatic-2.1.1/django_typomatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-05 23:42:22.000000 django-typomatic-2.1.1/django_typomatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 23:42:22.000000 django-typomatic-2.1.1/django_typomatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 23:42:22.000000 django-typomatic-2.1.1/django_typomatic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 23:42:22.000000 django-typomatic-2.1.1/django_typomatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 23:42:22.000000 django-typomatic-2.1.1/django_typomatic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 23:42:22.617985 django-typomatic-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-05 23:42:06.000000 django-typomatic-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/management/commands/generate_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/setup.py
```

### Comparing `django-typomatic-2.1.1/LICENSE` & `django-typomatic-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.1.1/PKG-INFO` & `django-typomatic-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.1.1
+Version: 2.2.0
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.1.1/README.md` & `django-typomatic-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.1.1/django_typomatic/__init__.py` & `django-typomatic-2.2.0/django_typomatic/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 from pathlib import Path
 
 from .mappings import mappings
 
 from rest_framework import serializers
 from rest_framework.fields import empty
 
-from .mappings import mappings, format_mappings
+from django.db.models.enums import Choices
+import inspect
+
+from typing import get_type_hints, get_origin, get_args
+
+from .mappings import mappings, format_mappings, primitives_mapping
 
 _LOG = logging.getLogger(f"django-typomatic.{__name__}")
 
 # Serializers
 __serializers = dict()
 # Custom serializers.Field to TS Type mappings
 __field_mappings = dict()
@@ -143,48 +148,125 @@
         field_type = type(field.child)
     elif hasattr(field, 'child_relation'):
         is_many = True
         field_type = type(field.child_relation)
     else:
         is_many = False
         field_type = type(field)
+
     if field_type in __serializers[context]:
         ts_type = __get_trimmed_name(
             field_type.__name__, trim_serializer_output)
     elif field_type in __field_mappings[context]:
         ts_type = __field_mappings[context].get(field_type, 'any')
     elif (context in __mapping_overrides) and (serializer in __mapping_overrides[context]) \
             and field_name in __mapping_overrides[context][serializer]:
         ts_type = __mapping_overrides[context][serializer].get(
             field_name, 'any')
     elif field_type == serializers.PrimaryKeyRelatedField:
         ts_type = "number | string"
     elif (hasattr(field, 'choices') and enum_choices) or (hasattr(field, 'choices') and enum_values):
-        ts_type = f"{''.join(x.title() for x in field_name.split('_'))}ChoiceEnum"
-        if enum_choices:
-            ts_enum = __map_choices_to_enum(ts_type, field_type, field.choices)
-        if enum_values:
-            ts_enum_value = __map_choices_to_enum_values(f'{ts_type}Values', field_type, field.choices)
-
-            if not enum_choices:
-                ts_type = __map_choices_to_union(field_type, field.choices)
+        ts_type, ts_enum, ts_enum_value = __process_choice_field(
+            field_name, field_type, field.choices, enum_choices, enum_values
+        )
     elif hasattr(field, 'choices'):
         ts_type = __map_choices_to_union(field_type, field.choices)
+    elif field_type == serializers.SerializerMethodField:
+        types = []
+        field_function = getattr(serializer, f'get_{field_name}')
+        return_type = get_type_hints(field_function).get('return')
+        is_generic_type = hasattr(return_type, '__origin__')
+        many = False
+
+        # TODO type pass recursively to represent something like a list from a list e.g. List[List[int]]
+        if is_generic_type:
+            return_type, many = __process_generic_type(return_type)
+
+        if isinstance(return_type, list) or isinstance(return_type, tuple) or isinstance(return_type, set):
+            return_types = return_type
+
+            for return_type in return_types:
+                many = False
+                is_generic_type = hasattr(return_type, '__origin__')
+
+                if is_generic_type:
+                    return_type, many = __process_generic_type(return_type)
+
+                ts_type, ts_enum, ts_enum_value = __process_method_field(
+                    field_name, field_type, return_type, enum_choices, enum_values, many
+                )
+                types.append(ts_type)
+        else:
+            ts_type, ts_enum, ts_enum_value = __process_method_field(
+                field_name, field_type, return_type, enum_choices, enum_values, many
+            )
+            types.append(ts_type)
+
+        # Clear duplicate types
+        types = list(dict.fromkeys(types))
+        ts_type = " | ".join(types)
     else:
         ts_type = mappings.get(field_type, 'any')
     if is_many:
         ts_type += '[]'
 
     if camelize:
         field_name_components = field_name.split("_")
         field_name = field_name_components[0] + "".join(x.title() for x in field_name_components[1:])
 
     return field_name, ts_type, ts_enum, ts_enum_value
 
 
+def __process_generic_type(return_type):
+    origin = get_origin(return_type)
+    args = get_args(return_type)
+    is_many = False
+
+    if origin == list or origin == tuple or origin == set:
+        is_many = True
+        return_type = args[0]
+    return return_type, is_many
+
+
+def __process_choice_field(field_name, field_type, choices, enum_choices, enum_values):
+    ts_enum = None
+    ts_enum_value = None
+
+    ts_type = f"{''.join(x.title() for x in field_name.split('_'))}ChoiceEnum"
+    if enum_choices:
+        ts_enum = __map_choices_to_enum(ts_type, field_type, choices)
+    if enum_values:
+        ts_enum_value = __map_choices_to_enum_values(f'{ts_type}Values', field_type, choices)
+
+        if not enum_choices:
+            ts_type = __map_choices_to_union(field_type, choices)
+    return ts_type, ts_enum, ts_enum_value
+
+
+def __process_method_field(field_name, field_type, return_type, enum_choices, enum_values, many=False):
+    ts_enum = None
+    ts_enum_value = None
+
+    if inspect.isclass(return_type) and issubclass(return_type, Choices):
+        choices = {key: value for key, value in return_type.choices}
+
+        ts_type, ts_enum, ts_enum_value = __process_choice_field(
+            field_name, field_type, choices, enum_choices, enum_values
+        )
+
+        if not enum_choices:
+            ts_type = __map_choices_to_union(field_type, choices)
+        return ts_type, ts_enum, ts_enum_value
+
+    ts_type = primitives_mapping.get(return_type, 'any')
+    ts_type = ts_type if not many else f'{ts_type}[]'
+
+    return ts_type, ts_enum, ts_enum_value
+
+
 def __get_ts_interface_and_enums(serializer, context, trim_serializer_output, camelize, enum_choices, enum_values,
                                  annotations):
     '''
     Generates and returns a Typescript Interface by iterating
     through the serializer fields of the DRF Serializer class
     passed in as a parameter, and mapping them to the appropriate Typescript
     data type.
@@ -213,15 +295,16 @@
             ts_property = ts_property + "?"
 
         if value.allow_null:
             ts_type = ts_type + " | null"
 
         if annotations:
             annotations_list = __get_annotations(value, ts_type)
-            ts_fields.append('\n'.join(annotations_list))
+            if annotations_list:
+                ts_fields.append('\n'.join(annotations_list))
 
         ts_fields.append(f"    {ts_property}: {ts_type};")
     collapsed_fields = '\n'.join(ts_fields)
     return f'export interface {name} {{\n{collapsed_fields}\n}}\n\n', enums
 
 
 def __generate_interfaces_and_enums(context, trim_serializer_output, camelize, enum_choices, enum_values, annotations):
@@ -277,14 +360,18 @@
     field_type = type(field)
 
     if field_type in format_mappings:
         annotations.append(f'    * @format {format_mappings[field_type]}')
 
     annotations.append('    */')
 
+    # Clear annotations header and footer if nothing to include
+    if len(annotations) == 2:
+        annotations = []
+
     return annotations
 
 
 def generate_ts(output_path, context='default', trim_serializer_output=False, camelize=False,
                 enum_choices=False, enum_values=False, annotations=False):
     '''
     When this function is called, a Typescript interface will be generated
```

### Comparing `django-typomatic-2.1.1/django_typomatic/management/commands/generate_ts.py` & `django-typomatic-2.2.0/django_typomatic/management/commands/generate_ts.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.1.1/django_typomatic/mappings.py` & `django-typomatic-2.2.0/django_typomatic/mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,40 @@
 mappings = {
     serializers.BooleanField: 'boolean',
     serializers.CharField: 'string',
     serializers.EmailField: 'string',
     serializers.RegexField: 'string',
     serializers.SlugField: 'string',
     serializers.URLField: 'string',
+    serializers.DictField: 'string',
     serializers.UUIDField: 'string',
     serializers.FilePathField: 'string',
+    serializers.FileField: 'File',
+    serializers.ImageField: 'File',
     serializers.IPAddressField: 'string',
     serializers.IntegerField: 'number',
     serializers.FloatField: 'number',
     serializers.DecimalField: 'number',
     serializers.DateTimeField: 'string',
     serializers.DateField: 'string',
     serializers.TimeField: 'string',
     serializers.DurationField: 'string',
-    serializers.DictField: 'Map'
 }
 
 format_mappings = {
     serializers.EmailField: 'email',
     serializers.URLField: 'url',
     serializers.UUIDField: 'uuid',
     serializers.DateTimeField: 'date-time',
     serializers.DateField: 'date',
     serializers.TimeField: 'time',
     serializers.FloatField: 'double',
 }
+
+primitives_mapping = {
+    str: 'string',
+    int: 'number',
+    float: 'number',
+    bool: 'boolean',
+    dict: 'string',
+    None: 'null'
+}
```

### Comparing `django-typomatic-2.1.1/django_typomatic/test__init__.py` & `django-typomatic-2.2.0/django_typomatic/test__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import io
+import random
+from typing import List
+
 import pytest
 from rest_framework import serializers
 from django.db import models
 from unittest.mock import patch, mock_open, MagicMock
 from . import ts_interface, generate_ts, get_ts
 
 
@@ -37,14 +40,15 @@
     email_field = serializers.EmailField()
     date_field = serializers.DateField()
     datetime_field = serializers.DateTimeField()
     time_field = serializers.TimeField()
     uuid_field = serializers.UUIDField()
     url_field = serializers.URLField(default='https://google.com')
     float_field = serializers.FloatField()
+    empty_annotation = serializers.CharField()
 
 
 class ActionType(models.TextChoices):
     ACTION1 = "Action1", ("Action1")
     ACTION2 = "Action2", ("Action2")
     ACTION3 = "Action3", ("Action3")
 
@@ -63,14 +67,48 @@
 
 @ts_interface('enumChoices')
 class EnumChoiceSerializer(serializers.Serializer):
     action = serializers.ChoiceField(choices=ActionType.choices)
     num = serializers.ChoiceField(choices=NumberType.choices)
 
 
+@ts_interface('files')
+class FileSerializer(serializers.Serializer):
+    image = serializers.ImageField()
+    file = serializers.FileField()
+
+
+@ts_interface('methodFields')
+class MethodFieldsSerializer(serializers.Serializer):
+    integer_field = serializers.SerializerMethodField()
+    string_field = serializers.SerializerMethodField()
+    float_field = serializers.SerializerMethodField()
+    choice_field = serializers.SerializerMethodField()
+    multiple_return = serializers.SerializerMethodField()
+    various_type_return = serializers.SerializerMethodField()
+
+    def get_integer_field(self) -> int:
+        return 5
+
+    def get_string_field(self) -> str:
+        return 'test'
+
+    def get_float_field(self) -> float:
+        return 1.1
+
+    def get_choice_field(self) -> ActionType:
+        return ActionType.ACTION1
+
+    def get_multiple_return(self) -> List[int]:
+        return [1, 2]
+
+    def get_various_type_return(self) -> [int, str]:
+        return random.choice([1, 'test'])
+
+
 def test_get_ts():
     expected = """export interface FooSerializer {
     some_field: number[];
     another_field: string;
     null_field: string | null;
 }
 
@@ -224,14 +262,15 @@
     * @format url
     */
     url_field?: string;
     /**
     * @format double
     */
     float_field: number;
+    empty_annotation: string;
 }
 
 """
     interfaces = get_ts('annotations', annotations=True)
     assert interfaces == expected
 
 
@@ -247,7 +286,40 @@
     action: "Action1" | "Action2" | "Action3";
     num: 1 | 2 | 3;
 }
 
 """
     interfaces = get_ts('enumChoices', enum_values=True, enum_choices=False)
     assert interfaces == expected
+
+
+def test_file_serializer():
+    expected = """export interface FileSerializer {
+    image: File;
+    file: File;
+}
+
+"""
+    interfaces = get_ts('files')
+    assert interfaces == expected
+
+
+def test_method_fields_serializer():
+    expected = """export enum ChoiceFieldChoiceEnum {
+    ACTION1 = 'Action1',
+    ACTION2 = 'Action2',
+    ACTION3 = 'Action3',
+}
+
+
+export interface MethodFieldsSerializer {
+    integer_field?: number;
+    string_field?: string;
+    float_field?: number;
+    choice_field?: ChoiceFieldChoiceEnum;
+    multiple_return?: number[];
+    various_type_return?: number | string;
+}
+
+"""
+    interfaces = get_ts('methodFields', enum_choices=True)
+    assert interfaces == expected
```

### Comparing `django-typomatic-2.1.1/django_typomatic.egg-info/PKG-INFO` & `django-typomatic-2.2.0/django_typomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.1.1
+Version: 2.2.0
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.1.1/setup.py` & `django-typomatic-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as file:
     long_description = file.read()
 
 setuptools.setup(
     name="django-typomatic",
-    version="2.1.1",
+    version="2.2.0",
     url="https://github.com/adenh93/django-typomatic",
 
     author="Aden Herold",
     author_email="aden.herold1@gmail.com",
 
     description="A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.",
     long_description=long_description,
```

