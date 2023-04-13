# Comparing `tmp/os2mo_data_import-5.3.1.tar.gz` & `tmp/os2mo_data_import-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2mo_data_import-5.3.1.tar", max compression
+gzip compressed data, was "os2mo_data_import-5.3.2.tar", max compression
```

## Comparing `os2mo_data_import-5.3.1.tar` & `os2mo_data_import-5.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0        0        0        0 2023-04-13 07:32:50.640488 os2mo_data_import-5.3.1/LICENSES/
--rw-r--r--   0        0        0    11696 2023-04-13 07:32:50.640488 os2mo_data_import-5.3.1/README.rst
--rw-r--r--   0        0        0       99 2023-04-13 07:32:50.640488 os2mo_data_import-5.3.1/kle/__init__.py
--rw-r--r--   0        0        0    13572 2023-04-13 07:32:50.641488 os2mo_data_import-5.3.1/kle/kle_import.py
--rw-r--r--   0        0        0     2261 2023-04-13 07:32:50.641488 os2mo_data_import-5.3.1/kle/payloads.py
--rw-r--r--   0        0        0      332 2023-04-13 07:32:50.641488 os2mo_data_import-5.3.1/mox_helpers/__init__.py
--rw-r--r--   0        0        0     7243 2023-04-13 07:32:50.641488 os2mo_data_import-5.3.1/mox_helpers/mox_helper.py
--rw-r--r--   0        0        0    20756 2023-04-13 07:32:50.641488 os2mo_data_import-5.3.1/mox_helpers/mox_util.py
--rw-r--r--   0        0        0     2736 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/mox_helpers/payloads.py
--rw-r--r--   0        0        0       40 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/mox_helpers/requirements.txt
--rw-r--r--   0        0        0      899 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/mox_helpers/utils.py
--rw-r--r--   0        0        0      397 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/os2mo_data_import/__init__.py
--rw-r--r--   0        0        0     3799 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/os2mo_data_import/caching_import.py
--rw-r--r--   0        0        0     1300 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/os2mo_data_import/defaults.py
--rw-r--r--   0        0        0    19484 2023-04-13 07:32:50.642488 os2mo_data_import-5.3.1/os2mo_data_import/helpers.py
--rw-r--r--   0        0        0    22987 2023-04-13 07:32:50.643489 os2mo_data_import-5.3.1/os2mo_data_import/mora_data_types.py
--rw-r--r--   0        0        0    13436 2023-04-13 07:32:50.643489 os2mo_data_import-5.3.1/os2mo_data_import/mox_data_types.py
--rw-r--r--   0        0        0       99 2023-04-13 07:32:50.643489 os2mo_data_import-5.3.1/os2mo_data_import/tests/__init__.py
--rw-r--r--   0        0        0     1650 2023-04-13 07:32:50.643489 os2mo_data_import-5.3.1/os2mo_data_import/tests/test_utilities.py
--rw-r--r--   0        0        0    27431 2023-04-13 07:32:50.643489 os2mo_data_import-5.3.1/os2mo_data_import/utilities.py
--rw-r--r--   0        0        0      332 2023-04-13 07:32:50.644488 os2mo_data_import-5.3.1/os2mo_helpers/__init__.py
--rw-r--r--   0        0        0    30138 2023-04-13 07:32:50.644488 os2mo_data_import-5.3.1/os2mo_helpers/mora_helpers.py
--rw-r--r--   0        0        0       41 2023-04-13 07:32:50.644488 os2mo_data_import-5.3.1/os2mo_helpers/requirements.txt
--rw-r--r--   0        0        0     1169 2023-04-13 07:32:50.644488 os2mo_data_import-5.3.1/os2mo_helpers/settings.py
--rw-r--r--   0        0        0       99 2023-04-13 07:32:50.644488 os2mo_data_import-5.3.1/os2mo_helpers/tests/__init__.py
--rw-r--r--   0        0        0     3412 2023-04-13 07:32:50.644488 os2mo_data_import-5.3.1/os2mo_helpers/tests/test_morahelpers.py
--rw-r--r--   0        0        0     1082 2023-04-13 07:32:51.888608 os2mo_data_import-5.3.1/pyproject.toml
--rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 os2mo_data_import-5.3.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-13 08:50:57.440809 os2mo_data_import-5.3.2/LICENSES/
+-rw-r--r--   0        0        0    11696 2023-04-13 08:50:57.441809 os2mo_data_import-5.3.2/README.rst
+-rw-r--r--   0        0        0       99 2023-04-13 08:50:57.441809 os2mo_data_import-5.3.2/kle/__init__.py
+-rw-r--r--   0        0        0    13572 2023-04-13 08:50:57.441809 os2mo_data_import-5.3.2/kle/kle_import.py
+-rw-r--r--   0        0        0     2261 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/kle/payloads.py
+-rw-r--r--   0        0        0      332 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/__init__.py
+-rw-r--r--   0        0        0     7243 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/mox_helper.py
+-rw-r--r--   0        0        0    20756 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/mox_util.py
+-rw-r--r--   0        0        0     2736 2023-04-13 08:50:57.442809 os2mo_data_import-5.3.2/mox_helpers/payloads.py
+-rw-r--r--   0        0        0       40 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/mox_helpers/requirements.txt
+-rw-r--r--   0        0        0      899 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/mox_helpers/utils.py
+-rw-r--r--   0        0        0      397 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/__init__.py
+-rw-r--r--   0        0        0     3799 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/caching_import.py
+-rw-r--r--   0        0        0     1300 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/defaults.py
+-rw-r--r--   0        0        0    19484 2023-04-13 08:50:57.443809 os2mo_data_import-5.3.2/os2mo_data_import/helpers.py
+-rw-r--r--   0        0        0    22987 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/mora_data_types.py
+-rw-r--r--   0        0        0    13436 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/mox_data_types.py
+-rw-r--r--   0        0        0       99 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/tests/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/tests/test_utilities.py
+-rw-r--r--   0        0        0    27431 2023-04-13 08:50:57.444810 os2mo_data_import-5.3.2/os2mo_data_import/utilities.py
+-rw-r--r--   0        0        0      332 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/__init__.py
+-rw-r--r--   0        0        0    30138 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/mora_helpers.py
+-rw-r--r--   0        0        0       41 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/settings.py
+-rw-r--r--   0        0        0       99 2023-04-13 08:50:57.445810 os2mo_data_import-5.3.2/os2mo_helpers/tests/__init__.py
+-rw-r--r--   0        0        0     3412 2023-04-13 08:50:57.446810 os2mo_data_import-5.3.2/os2mo_helpers/tests/test_morahelpers.py
+-rw-r--r--   0        0        0     1080 2023-04-13 08:50:58.671979 os2mo_data_import-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.3.2/PKG-INFO
```

### Comparing `os2mo_data_import-5.3.1/README.rst` & `os2mo_data_import-5.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/kle/kle_import.py` & `os2mo_data_import-5.3.2/kle/kle_import.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/kle/payloads.py` & `os2mo_data_import-5.3.2/kle/payloads.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/mox_helpers/mox_helper.py` & `os2mo_data_import-5.3.2/mox_helpers/mox_helper.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/mox_helpers/mox_util.py` & `os2mo_data_import-5.3.2/mox_helpers/mox_util.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/mox_helpers/payloads.py` & `os2mo_data_import-5.3.2/mox_helpers/payloads.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/mox_helpers/utils.py` & `os2mo_data_import-5.3.2/mox_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/caching_import.py` & `os2mo_data_import-5.3.2/os2mo_data_import/caching_import.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/defaults.py` & `os2mo_data_import-5.3.2/os2mo_data_import/defaults.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/helpers.py` & `os2mo_data_import-5.3.2/os2mo_data_import/helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/mora_data_types.py` & `os2mo_data_import-5.3.2/os2mo_data_import/mora_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/mox_data_types.py` & `os2mo_data_import-5.3.2/os2mo_data_import/mox_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/tests/test_utilities.py` & `os2mo_data_import-5.3.2/os2mo_data_import/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_data_import/utilities.py` & `os2mo_data_import-5.3.2/os2mo_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_helpers/mora_helpers.py` & `os2mo_data_import-5.3.2/os2mo_helpers/mora_helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_helpers/settings.py` & `os2mo_data_import-5.3.2/os2mo_helpers/settings.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/os2mo_helpers/tests/test_morahelpers.py` & `os2mo_data_import-5.3.2/os2mo_helpers/tests/test_morahelpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.1/pyproject.toml` & `os2mo_data_import-5.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "os2mo_data_import"
-version = "5.3.1"
+version = "5.3.2"
 description = "A set of tools for OS2MO data import and export"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.rst"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo_data_import"
 keywords = ["os2mo", "dipex"]
 packages = [
     { include = "os2mo_data_import" },
     { include = "os2mo_helpers" },
     { include = "mox_helpers" },
     { include = "kle" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11.0"
+python = "^3.11"
 aiohttp = "^3.8.4"
 anytree = "^2.8.0"
 certifi = "^2022.12.7"
 chardet = "^5.1.0"
 click = "^8.1.3"
 idna = "^3.4"
 openpyxl = "^3.1.2"
```

### Comparing `os2mo_data_import-5.3.1/PKG-INFO` & `os2mo_data_import-5.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: os2mo-data-import
-Version: 5.3.1
+Version: 5.3.2
 Summary: A set of tools for OS2MO data import and export
 Home-page: https://git.magenta.dk/rammearkitektur/os2mo_data_import
 License: MPL-2.0
 Keywords: os2mo,dipex
 Author: Magenta
 Author-email: info@magenta.dk
-Requires-Python: >=3.11.0,<4.0.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: XlsxWriter (>=3.0.9,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: anytree (>=2.8.0,<3.0.0)
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
```

