# Comparing `tmp/fastapi_myhelper-0.1.6.tar.gz` & `tmp/fastapi_myhelper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_myhelper-0.1.6.tar", max compression
+gzip compressed data, was "fastapi_myhelper-0.1.7.tar", max compression
```

## Comparing `fastapi_myhelper-0.1.6.tar` & `fastapi_myhelper-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        0 2023-02-03 07:51:10.857527 fastapi_myhelper-0.1.6/fastapi_myhelper/__init__.py
--rw-r--r--   0        0        0       28 2023-03-23 10:28:40.538865 fastapi_myhelper-0.1.6/fastapi_myhelper/pydantic/__init__.py
--rw-r--r--   0        0        0     4342 2023-03-27 10:57:11.408077 fastapi_myhelper-0.1.6/fastapi_myhelper/pydantic/meta.py
--rw-r--r--   0        0        0        0 2023-02-03 10:26:54.940734 fastapi_myhelper-0.1.6/fastapi_myhelper/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1367 2023-02-03 10:26:54.941812 fastapi_myhelper-0.1.6/fastapi_myhelper/sqlalchemy/pagination.py
--rw-r--r--   0        0        0     2287 2023-04-13 12:20:07.464551 fastapi_myhelper-0.1.6/fastapi_myhelper/sqlalchemy/utils.py
--rw-r--r--   0        0        0       36 2023-03-23 10:28:40.539623 fastapi_myhelper-0.1.6/fastapi_myhelper/sqlmodel/__init__.py
--rw-r--r--   0        0        0      167 2023-03-25 13:25:21.863943 fastapi_myhelper-0.1.6/fastapi_myhelper/sqlmodel/meta.py
--rw-r--r--   0        0        0      420 2023-04-12 12:27:09.142691 fastapi_myhelper-0.1.6/fastapi_myhelper/sqlmodel/utils.py
--rw-r--r--   0        0        0      149 2023-04-07 08:52:16.724050 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/__init__.py
--rw-r--r--   0        0        0      509 2023-02-03 07:51:10.858340 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/decorators.py
--rw-r--r--   0        0        0     3480 2023-02-03 07:51:10.877180 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/exceptions.py
--rw-r--r--   0        0        0       22 2023-02-03 07:51:10.876992 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/extentions/__init__.py
--rw-r--r--   0        0        0     2358 2023-02-03 07:51:10.876819 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/extentions/errors.py
--rw-r--r--   0        0        0     2570 2023-04-10 07:23:04.112037 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/relationship.py
--rw-r--r--   0        0        0       26 2023-02-03 07:51:10.859100 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/__init__.py
--rw-r--r--   0        0        0     4053 2023-03-23 10:28:40.540283 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/meta.py
--rw-r--r--   0        0        0     1898 2023-02-03 07:51:10.876431 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/pagination.py
--rw-r--r--   0        0        0     1139 2023-02-03 07:56:07.978675 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/schema.py
--rw-r--r--   0        0        0     1502 2023-02-03 07:51:10.876010 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/type.py
--rw-r--r--   0        0        0       56 2023-04-11 11:38:41.537044 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2557 2023-04-11 11:38:41.533046 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlalchemy/query.py
--rw-r--r--   0        0        0      572 2023-04-11 11:38:41.528316 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlalchemy/utils.py
--rw-r--r--   0        0        0       39 2023-02-03 07:51:10.875460 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlmodel/__init__.py
--rw-r--r--   0        0        0      547 2023-02-03 07:51:10.875291 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlmodel/utils.py
--rw-r--r--   0        0        0      326 2023-04-07 08:07:59.584631 fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/utils.py
--rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860735 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860888 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/__init__.py
--rw-r--r--   0        0        0     4734 2023-02-03 07:52:15.846049 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_pydantic.py
--rw-r--r--   0        0        0     3390 2023-02-03 07:51:34.114284 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_schema.py
--rw-r--r--   0        0        0     1242 2023-02-03 07:51:10.874520 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py
--rw-r--r--   0        0        0      984 2023-02-03 07:51:10.874285 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_sqlmodel.py
--rw-r--r--   0        0        0     2037 2023-02-03 07:52:06.953217 fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_validator.py
--rw-r--r--   0        0        0      786 2023-04-13 12:20:07.468773 fastapi_myhelper-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.6/setup.py
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-03 07:51:10.857527 fastapi_myhelper-0.1.7/fastapi_myhelper/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-23 10:28:40.538865 fastapi_myhelper-0.1.7/fastapi_myhelper/pydantic/__init__.py
+-rw-r--r--   0        0        0     4342 2023-03-27 10:57:11.408077 fastapi_myhelper-0.1.7/fastapi_myhelper/pydantic/meta.py
+-rw-r--r--   0        0        0        0 2023-02-03 10:26:54.940734 fastapi_myhelper-0.1.7/fastapi_myhelper/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1367 2023-02-03 10:26:54.941812 fastapi_myhelper-0.1.7/fastapi_myhelper/sqlalchemy/pagination.py
+-rw-r--r--   0        0        0     2517 2023-04-13 12:49:12.428999 fastapi_myhelper-0.1.7/fastapi_myhelper/sqlalchemy/utils.py
+-rw-r--r--   0        0        0       36 2023-03-23 10:28:40.539623 fastapi_myhelper-0.1.7/fastapi_myhelper/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      167 2023-03-25 13:25:21.863943 fastapi_myhelper-0.1.7/fastapi_myhelper/sqlmodel/meta.py
+-rw-r--r--   0        0        0      420 2023-04-12 12:27:09.142691 fastapi_myhelper-0.1.7/fastapi_myhelper/sqlmodel/utils.py
+-rw-r--r--   0        0        0      149 2023-04-07 08:52:16.724050 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/__init__.py
+-rw-r--r--   0        0        0      509 2023-02-03 07:51:10.858340 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/decorators.py
+-rw-r--r--   0        0        0     3480 2023-02-03 07:51:10.877180 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/exceptions.py
+-rw-r--r--   0        0        0       22 2023-02-03 07:51:10.876992 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/extentions/__init__.py
+-rw-r--r--   0        0        0     2358 2023-02-03 07:51:10.876819 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/extentions/errors.py
+-rw-r--r--   0        0        0     2570 2023-04-10 07:23:04.112037 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/relationship.py
+-rw-r--r--   0        0        0       26 2023-02-03 07:51:10.859100 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/__init__.py
+-rw-r--r--   0        0        0     4053 2023-03-23 10:28:40.540283 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/meta.py
+-rw-r--r--   0        0        0     1898 2023-02-03 07:51:10.876431 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/pagination.py
+-rw-r--r--   0        0        0     1139 2023-02-03 07:56:07.978675 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/schema.py
+-rw-r--r--   0        0        0     1502 2023-02-03 07:51:10.876010 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/type.py
+-rw-r--r--   0        0        0       56 2023-04-11 11:38:41.537044 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2557 2023-04-11 11:38:41.533046 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlalchemy/query.py
+-rw-r--r--   0        0        0      572 2023-04-11 11:38:41.528316 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlalchemy/utils.py
+-rw-r--r--   0        0        0       39 2023-02-03 07:51:10.875460 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      547 2023-02-03 07:51:10.875291 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlmodel/utils.py
+-rw-r--r--   0        0        0      326 2023-04-07 08:07:59.584631 fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/utils.py
+-rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860735 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-03 07:51:10.860888 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/__init__.py
+-rw-r--r--   0        0        0     4734 2023-02-03 07:52:15.846049 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_pydantic.py
+-rw-r--r--   0        0        0     3390 2023-02-03 07:51:34.114284 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_schema.py
+-rw-r--r--   0        0        0     1242 2023-02-03 07:51:10.874520 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py
+-rw-r--r--   0        0        0      984 2023-02-03 07:51:10.874285 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_sqlmodel.py
+-rw-r--r--   0        0        0     2037 2023-02-03 07:52:06.953217 fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_validator.py
+-rw-r--r--   0        0        0      786 2023-04-13 12:50:37.830204 fastapi_myhelper-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.7/setup.py
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 fastapi_myhelper-0.1.7/PKG-INFO
```

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/pydantic/meta.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/pydantic/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/sqlalchemy/pagination.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/sqlalchemy/pagination.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/sqlalchemy/utils.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/sqlalchemy/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ]
 
 
 async def get_non_unique_fields(
         model,
         data,
         session: AsyncSession,
-) -> list[str]:
+) -> tuple[list[str], list[tuple[str, ...]]]:
     fields = get_unique_columns(model.__table__)
     constraint_fields = get_unique_constraint_columns(model.__table__)
     selects = []
     for field in fields:
         model_field = getattr(model, field)
         value = getattr(data, field, None)
         qs = None
@@ -59,12 +59,17 @@
             values, None
         )
         selects.append(
             select(*values.keys()).where(where).scalar_subquery().exists()
         )
 
     result = (await session.execute(select(*selects))).one_or_none()
-    non_unique = []
-    for i, field in enumerate(fields + constraint_fields):
+    non_unique_fields = []
+    non_unique_constraints = []
+    n = len(fields)
+    for i, field in enumerate(fields):
         if result[i]:
-            non_unique.append(field)
-    return non_unique
+            non_unique_fields.append(field)
+    for i, field in enumerate(constraint_fields):
+        if result[n+i]:
+            non_unique_constraints.append(field)
+    return non_unique_fields, non_unique_constraints
```

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/exceptions.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/extentions/errors.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/extentions/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/relationship.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/relationship.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/meta.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/pagination.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/schema.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/schemas/type.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/schemas/type.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlalchemy/query.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlalchemy/query.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlalchemy/utils.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/strawberry/sqlmodel/utils.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/strawberry/sqlmodel/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_pydantic.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_schema.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_sqlmodel.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/fastapi_myhelper/tests/strawberry/test_validator.py` & `fastapi_myhelper-0.1.7/fastapi_myhelper/tests/strawberry/test_validator.py`

 * *Files identical despite different names*

### Comparing `fastapi_myhelper-0.1.6/pyproject.toml` & `fastapi_myhelper-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-myhelper"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["MihaTeam1 <sarsern2004@gmail.com>"]
 packages = [{include = "fastapi_myhelper"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 strawberry-graphql = {version = "^0.155.3", optional = true}
```

### Comparing `fastapi_myhelper-0.1.6/setup.py` & `fastapi_myhelper-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'sqlmodel': ['sqlmodel>=0.0.8,<0.0.9',
               'sqlalchemy>=1.4.17,<=1.4.41',
               'pydantic>=1.10.4,<2.0.0'],
  'strawberry': ['strawberry-graphql>=0.155.3,<0.156.0']}
 
 setup_kwargs = {
     'name': 'fastapi-myhelper',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': 'None',
     'author': 'MihaTeam1',
     'author_email': 'sarsern2004@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fastapi_myhelper-0.1.6/PKG-INFO` & `fastapi_myhelper-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-myhelper
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: MihaTeam1
 Author-email: sarsern2004@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

