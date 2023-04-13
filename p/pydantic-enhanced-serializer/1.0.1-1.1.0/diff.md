# Comparing `tmp/pydantic_enhanced_serializer-1.0.1-py3-none-any.whl.zip` & `tmp/pydantic_enhanced_serializer-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,17 @@
-Zip file size: 17154 bytes, number of entries: 16
+Zip file size: 15782 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      309 b- defN 23-Mar-08 23:12 pydantic_enhanced_serializer/__init__.py
 -rw-r--r--  2.0 unx     9416 b- defN 23-Mar-08 23:41 pydantic_enhanced_serializer/fieldsets.py
 -rw-r--r--  2.0 unx     2724 b- defN 23-Mar-08 23:35 pydantic_enhanced_serializer/models.py
 -rw-r--r--  2.0 unx     3960 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/path_put.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/py.typed
 -rw-r--r--  2.0 unx     4222 b- defN 23-Mar-08 23:32 pydantic_enhanced_serializer/render.py
--rw-r--r--  2.0 unx     6235 b- defN 23-Mar-08 23:32 pydantic_enhanced_serializer/schema.py
+-rw-r--r--  2.0 unx     6996 b- defN 23-Apr-13 21:29 pydantic_enhanced_serializer/schema.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-08 23:11 pydantic_enhanced_serializer/integrations/__init__.py
 -rw-r--r--  2.0 unx     1401 b- defN 23-Mar-08 23:47 pydantic_enhanced_serializer/integrations/django_ninja.py
 -rw-r--r--  2.0 unx     6078 b- defN 23-Mar-08 23:14 pydantic_enhanced_serializer/integrations/fastapi.py
--rw-r--r--  2.0 unx     4084 b- defN 23-Mar-08 23:41 pydantic_enhanced_serializer/integrations/flask.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Mar-09 00:53 pydantic_enhanced_serializer-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6019 b- defN 23-Mar-09 00:53 pydantic_enhanced_serializer-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-09 00:53 pydantic_enhanced_serializer-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       29 b- defN 23-Mar-09 00:53 pydantic_enhanced_serializer-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1595 b- defN 23-Mar-09 00:53 pydantic_enhanced_serializer-1.0.1.dist-info/RECORD
-16 files, 47237 bytes uncompressed, 14420 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6021 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       29 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1488 b- defN 23-Apr-13 21:52 pydantic_enhanced_serializer-1.1.0.dist-info/RECORD
+15 files, 43809 bytes uncompressed, 13224 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -24,26 +24,23 @@
 
 Filename: pydantic_enhanced_serializer/integrations/django_ninja.py
 Comment: 
 
 Filename: pydantic_enhanced_serializer/integrations/fastapi.py
 Comment: 
 
-Filename: pydantic_enhanced_serializer/integrations/flask.py
+Filename: pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.0.1.dist-info/LICENSE
+Filename: pydantic_enhanced_serializer-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.0.1.dist-info/METADATA
+Filename: pydantic_enhanced_serializer-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.0.1.dist-info/WHEEL
+Filename: pydantic_enhanced_serializer-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pydantic_enhanced_serializer-1.0.1.dist-info/top_level.txt
-Comment: 
-
-Filename: pydantic_enhanced_serializer-1.0.1.dist-info/RECORD
+Filename: pydantic_enhanced_serializer-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydantic_enhanced_serializer/schema.py

```diff
@@ -1,10 +1,11 @@
 import inspect
 from collections import defaultdict
 from functools import partial
+from itertools import chain
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Set,
@@ -128,26 +129,30 @@
 
         else:
             field_names = set(_fully_list_fieldvalue(fieldsets[fieldset_name]))
 
         for field_name in field_names:
             fieldsets_per_field[field_name].add(fieldset_name)
 
-    for field_name, fieldset_names in fieldsets_per_field.items():
-        if not fieldset_names:
-            continue
+    for field_name in set(chain(model.__fields__.keys(), fieldsets_per_field.keys())):
+        fieldset_names = fieldsets_per_field.get(field_name) or set()
 
         if "default" in fieldset_names and len(fieldset_names) == 1:
             continue
 
-        description = (
-            "Included in fieldset(s): "
-            + ", ".join([f for f in sorted(fieldset_names) if f != "default"])
-            + "."
-        )
+        if len(fieldset_names) > 0:
+            description = (
+                "Request using fieldset(s): "
+                + ", ".join(
+                    [f"`{f}`" for f in sorted(fieldset_names) if f != "default"]
+                )
+                + "."
+            )
+        else:
+            description = "Not returned by default.  Request this field by name."
 
         schema["properties"][field_name]["description"] = (
             schema["properties"][field_name].get("description", "") + description
         )
 
     if callable(original_schema_extra):
         _deep_update(schema, original_schema_extra(schema, model) or {})
@@ -185,7 +190,26 @@
             key in into_dict
             and isinstance(from_dict[key], dict)
             and isinstance(into_dict[key], dict)
         ):
             _deep_update(into_dict[key], from_dict[key])
         else:
             into_dict[key] = from_dict[key]
+
+
+def model_has_fieldsets_defined(model: Any) -> bool:
+    if is_optional(model):
+        model = get_optional_type(model)
+
+    if inspect.isclass(model) and issubclass(model, BaseModel):
+        if getattr(model.__config__, "fieldsets", None):
+            return True
+
+        else:
+            return any(
+                [
+                    model_has_fieldsets_defined(field.type_)
+                    for field in model.__fields__.values()
+                ]
+            )
+
+    return False
```

## Comparing `pydantic_enhanced_serializer-1.0.1.dist-info/LICENSE` & `pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pydantic_enhanced_serializer-1.0.1.dist-info/METADATA` & `pydantic_enhanced_serializer-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydantic-enhanced-serializer
-Version: 1.0.1
-Summary: Pydantic extension that allows user selection of object fields or expanded inline when serializing models
+Version: 1.1.0
+Summary: Pydantic extension that allows user selection of object fields or expansions inline when serializing models
 Home-page: https://github.com/adamsussman/pydantic-enhanced-serializer
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
 Classifier: Framework :: FastAPI
```

## Comparing `pydantic_enhanced_serializer-1.0.1.dist-info/RECORD` & `pydantic_enhanced_serializer-1.1.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 pydantic_enhanced_serializer/__init__.py,sha256=YDA4Ntaq4mBBR0nDyHFXlvqE_OWJ6mzsCHlxjX71nYc,309
 pydantic_enhanced_serializer/fieldsets.py,sha256=beBS5m3KAyOqmyOhoU9qenIKIF3F-SP3Ss3HsmBHbXA,9416
 pydantic_enhanced_serializer/models.py,sha256=ZGoQZ9cHTT9icObGvfWFkeBYRSQUKYYbligdsiDvX94,2724
 pydantic_enhanced_serializer/path_put.py,sha256=CPqpjErHgzvipU6B326A-XpSbhTtWJzGeV9UODzMUjY,3960
 pydantic_enhanced_serializer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/render.py,sha256=OsnGmTjDr93Xi1vYWcM5YgNDpsZbpsAa5Ct724-BxBw,4222
-pydantic_enhanced_serializer/schema.py,sha256=YJVELl6cqf8rBK0KZ6IUYa-JSkI-EmMH0RqmMbwrEdg,6235
+pydantic_enhanced_serializer/schema.py,sha256=p3kUgONZMZ3qMdoCw7qMYgQHjHL39I2kh39fT_gwaks,6996
 pydantic_enhanced_serializer/integrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pydantic_enhanced_serializer/integrations/django_ninja.py,sha256=Z60LR0vfM4wbpvWo_qfEhcsUn4ufXU80xwD4zbPGIdI,1401
 pydantic_enhanced_serializer/integrations/fastapi.py,sha256=6qBNdbafvEAmVDBVS0h_AedDnevh_Ilv3bztF3pcYHY,6078
-pydantic_enhanced_serializer/integrations/flask.py,sha256=1MOTlNY-qo21rGrh1edlhgh-5vmFZbgRx9Pig6Xjxdc,4084
-pydantic_enhanced_serializer-1.0.1.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-pydantic_enhanced_serializer-1.0.1.dist-info/METADATA,sha256=PrQOSjMM8hwUBTPmiP7NRbYJM32dRdqZE7voVTGXcV4,6019
-pydantic_enhanced_serializer-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pydantic_enhanced_serializer-1.0.1.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
-pydantic_enhanced_serializer-1.0.1.dist-info/RECORD,,
+pydantic_enhanced_serializer-1.1.0.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+pydantic_enhanced_serializer-1.1.0.dist-info/METADATA,sha256=e2yGk8ACb6cyr30jglEslf0tRD5XpUnzoBFb1ijwvao,6021
+pydantic_enhanced_serializer-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pydantic_enhanced_serializer-1.1.0.dist-info/top_level.txt,sha256=QCypSWZi8vRHdmuu-4xOAqUWN78nQShuGw0yMB4RLI4,29
+pydantic_enhanced_serializer-1.1.0.dist-info/RECORD,,
```

