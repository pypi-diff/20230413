# Comparing `tmp/barsdiary-0.1.4.tar.gz` & `tmp/barsdiary-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barsdiary-0.1.4.tar", max compression
+gzip compressed data, was "barsdiary-0.1.5.tar", max compression
```

## Comparing `barsdiary-0.1.4.tar` & `barsdiary-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       31 2023-04-13 18:31:09.494048 barsdiary-0.1.4/README.md
--rw-r--r--   0        0        0      554 2023-04-13 18:31:09.494048 barsdiary-0.1.4/barsdiary/__init__.py
--rw-r--r--   0        0        0     6790 2023-04-13 18:31:09.494048 barsdiary-0.1.4/barsdiary/aio.py
--rw-r--r--   0        0        0     6125 2023-04-13 18:31:09.494048 barsdiary-0.1.4/barsdiary/sync.py
--rw-r--r--   0        0        0     5091 2023-04-13 18:31:09.494048 barsdiary-0.1.4/barsdiary/types.py
--rw-r--r--   0        0        0     1296 2023-04-13 18:31:09.494048 barsdiary-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 barsdiary-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-04-13 18:38:52.195346 barsdiary-0.1.5/README.md
+-rw-r--r--   0        0        0      554 2023-04-13 18:38:52.195346 barsdiary-0.1.5/barsdiary/__init__.py
+-rw-r--r--   0        0        0     6790 2023-04-13 18:38:52.195346 barsdiary-0.1.5/barsdiary/aio.py
+-rw-r--r--   0        0        0     6125 2023-04-13 18:38:52.195346 barsdiary-0.1.5/barsdiary/sync.py
+-rw-r--r--   0        0        0     5088 2023-04-13 18:38:52.195346 barsdiary-0.1.5/barsdiary/types.py
+-rw-r--r--   0        0        0     1296 2023-04-13 18:38:52.195346 barsdiary-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 barsdiary-0.1.5/PKG-INFO
```

### Comparing `barsdiary-0.1.4/barsdiary/__init__.py` & `barsdiary-0.1.5/barsdiary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     LoginObject,
     ProgressAverageObject,
     SchoolMeetingsObject,
     TotalsObject,
 )
 
 # using in user-agent in requests
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

### Comparing `barsdiary-0.1.4/barsdiary/aio.py` & `barsdiary-0.1.5/barsdiary/aio.py`

 * *Files identical despite different names*

### Comparing `barsdiary-0.1.4/barsdiary/sync.py` & `barsdiary-0.1.5/barsdiary/sync.py`

 * *Files identical despite different names*

### Comparing `barsdiary-0.1.4/barsdiary/types.py` & `barsdiary-0.1.5/barsdiary/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     level: ProgressDataObject
     sub_period: str = Field(alias="subperiod")
 
 
 # /rest/additional_materials
 
 
-class MaterialDataObject(BaseResponse):
+class MaterialDataObject(BaseModel):
     name: str
     file: str  # URL
 
 
 class AdditionalMaterialsObject(BaseResponse):
     kind: Optional[str]
     data: Optional[List[MaterialDataObject]]
```

### Comparing `barsdiary-0.1.4/pyproject.toml` & `barsdiary-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "barsdiary"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python library for working with API \"БАРС.Web-Образование\""
 license = "MIT"
 readme = "README.md"
 authors = ["mironovmeow <71277890+mironovmeow@users.noreply.github.com>"]
 homepage = "https://github.com/mironovmeow/barsdiary"
 repository = "https://github.com/mironovmeow/barsdiary"
 # documentation = "https://barsdiary.readthedocs.io/ru/latest/"
```

### Comparing `barsdiary-0.1.4/PKG-INFO` & `barsdiary-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barsdiary
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library for working with API "БАРС.Web-Образование"
 Home-page: https://github.com/mironovmeow/barsdiary
 License: MIT
 Keywords: python,aiohttp,pydantic,asyncio
 Author: mironovmeow
 Author-email: 71277890+mironovmeow@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
```

