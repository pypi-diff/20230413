# Comparing `tmp/pylife-odbclient-2.0.3rc1.tar.gz` & `tmp/pylife-odbclient-2.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylife-odbclient-2.0.3rc1.tar", last modified: Thu Apr 13 08:57:30 2023, max compression
+gzip compressed data, was "pylife-odbclient-2.0.3rc2.tar", last modified: Thu Apr 13 11:11:21 2023, max compression
```

## Comparing `pylife-odbclient-2.0.3rc1.tar` & `pylife-odbclient-2.0.3rc2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-13 08:57:30.767831 pylife-odbclient-2.0.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.759831 pylife-odbclient-2.0.3rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/src/odbclient/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/src/odbclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/src/odbclient/odbclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   238316 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/beam_3d_hex_quad.odb
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/connectivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/node_coordinates.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/stress_element_nodal.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/stress_integration_point.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/test_odbclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.916126 pylife-odbclient-2.0.3rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.916126 pylife-odbclient-2.0.3rc2/src/odbclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/src/odbclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/src/odbclient/odbclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.916126 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 11:11:21.000000 pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:11:21.920126 pylife-odbclient-2.0.3rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   238316 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/beam_3d_hex_quad.odb
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/connectivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/node_coordinates.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/stress_element_nodal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/stress_integration_point.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-13 11:11:18.000000 pylife-odbclient-2.0.3rc2/tests/test_odbclient.py
```

### Comparing `pylife-odbclient-2.0.3rc1/.coveragerc` & `pylife-odbclient-2.0.3rc2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/.gitignore` & `pylife-odbclient-2.0.3rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/LICENSE` & `pylife-odbclient-2.0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/PKG-INFO` & `pylife-odbclient-2.0.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbclient
-Version: 2.0.3rc1
+Version: 2.0.3rc2
 Summary: A Python 3 client for odbAccess using pylife-odbserver
 Home-page: https://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Project-URL: Documentation, https://pylife.readthedocs.io
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc1 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc2 Summary: A
 Python 3 client for odbAccess using pylife-odbserver Home-page: https://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Project-URL: Documentation,
 https://pylife.readthedocs.io Platform: any Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Requires-Python: >=3
 Description-Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing
 License-File: LICENSE License-File: AUTHORS.rst # pylife-odbclient A Python 3
```

### Comparing `pylife-odbclient-2.0.3rc1/README.md` & `pylife-odbclient-2.0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/demo.ipynb` & `pylife-odbclient-2.0.3rc2/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/setup.cfg` & `pylife-odbclient-2.0.3rc2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	pandas
+	pandas<2.0.0
 	numpy==1.23.5
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `pylife-odbclient-2.0.3rc1/setup.py` & `pylife-odbclient-2.0.3rc2/setup.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/src/odbclient/__init__.py` & `pylife-odbclient-2.0.3rc2/src/odbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/src/odbclient/odbclient.py` & `pylife-odbclient-2.0.3rc2/src/odbclient/odbclient.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/PKG-INFO` & `pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbclient
-Version: 2.0.3rc1
+Version: 2.0.3rc2
 Summary: A Python 3 client for odbAccess using pylife-odbserver
 Home-page: https://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Project-URL: Documentation, https://pylife.readthedocs.io
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc1 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc2 Summary: A
 Python 3 client for odbAccess using pylife-odbserver Home-page: https://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Project-URL: Documentation,
 https://pylife.readthedocs.io Platform: any Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Requires-Python: >=3
 Description-Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing
 License-File: LICENSE License-File: AUTHORS.rst # pylife-odbclient A Python 3
```

### Comparing `pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/SOURCES.txt` & `pylife-odbclient-2.0.3rc2/src/pylife_odbclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/tests/beam_3d_hex_quad.odb` & `pylife-odbclient-2.0.3rc2/tests/beam_3d_hex_quad.odb`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/tests/node_coordinates.csv` & `pylife-odbclient-2.0.3rc2/tests/node_coordinates.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/tests/stress_element_nodal.csv` & `pylife-odbclient-2.0.3rc2/tests/stress_element_nodal.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/tests/stress_integration_point.csv` & `pylife-odbclient-2.0.3rc2/tests/stress_integration_point.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.3rc1/tests/test_odbclient.py` & `pylife-odbclient-2.0.3rc2/tests/test_odbclient.py`

 * *Files identical despite different names*

