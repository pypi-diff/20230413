# Comparing `tmp/fal_serverless-0.6.27.tar.gz` & `tmp/fal_serverless-0.6.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.27.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.28.tar", max compression
```

## Comparing `fal_serverless-0.6.27.tar` & `fal_serverless-0.6.28.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0        0 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/README.md
--rw-r--r--   0        0        0      956 2023-04-12 23:53:57.363851 fal_serverless-0.6.27/pyproject.toml
--rw-r--r--   0        0        0      294 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    14760 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2390 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5292 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    11503 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-04-12 23:53:49.771829 fal_serverless-0.6.27/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     1127 2023-04-12 23:53:36.911797 fal_serverless-0.6.27/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-04-12 23:53:36.915797 fal_serverless-0.6.27/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-04-12 23:53:36.915797 fal_serverless-0.6.27/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-04-12 23:53:36.915797 fal_serverless-0.6.27/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    14988 2023-04-12 23:53:36.915797 fal_serverless-0.6.27/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 fal_serverless-0.6.27/setup.py
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 fal_serverless-0.6.27/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/README.md
+-rw-r--r--   0        0        0      956 2023-04-13 08:34:59.200602 fal_serverless-0.6.28/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    14760 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2390 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5292 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    11503 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-04-13 08:34:51.100543 fal_serverless-0.6.28/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     1127 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-04-13 08:34:34.788432 fal_serverless-0.6.28/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    14988 2023-04-13 08:34:34.792433 fal_serverless-0.6.28/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     3300 2023-04-13 08:34:34.792433 fal_serverless-0.6.28/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 fal_serverless-0.6.28/setup.py
+-rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 fal_serverless-0.6.28/PKG-INFO
```

### Comparing `fal_serverless-0.6.27/pyproject.toml` & `fal_serverless-0.6.28/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.27"
+version = "0.6.28"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = "0.11.1", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "^0.0.23"
+isolate-proto = "^0.0.26"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "^2.9.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
```

### Comparing `fal_serverless-0.6.27/src/fal_serverless/api.py` & `fal_serverless-0.6.28/src/fal_serverless/api.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.28/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.28/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.28/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/cli.py` & `fal_serverless-0.6.28/src/fal_serverless/cli.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.28/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.28/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.28/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.28/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.28/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.28/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.28/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/src/fal_serverless/sdk.py` & `fal_serverless-0.6.28/src/fal_serverless/sdk.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.27/setup.py` & `fal_serverless-0.6.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client>=2.9.0,<3.0.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto>=0.0.23,<0.0.24',
+ 'isolate-proto>=0.0.26,<0.0.27',
  'isolate[build]==0.11.1',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=13.3.2,<14.0.0',
  'structlog>=22.3.0,<23.0.0',
@@ -36,15 +36,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.27',
+    'version': '0.6.28',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.27/PKG-INFO` & `fal_serverless-0.6.28/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.27
+Version: 0.6.28
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (>=2.9.0,<3.0.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (>=0.0.23,<0.0.24)
+Requires-Dist: isolate-proto (>=0.0.26,<0.0.27)
 Requires-Dist: isolate[build] (==0.11.1)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
```

