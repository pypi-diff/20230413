# Comparing `tmp/pylife-odbclient-2.0.2rc1.tar.gz` & `tmp/pylife-odbclient-2.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylife-odbclient-2.0.2rc1.tar", last modified: Tue Dec 13 10:55:11 2022, max compression
+gzip compressed data, was "pylife-odbclient-2.0.3rc1.tar", last modified: Thu Apr 13 08:57:30 2023, max compression
```

## Comparing `pylife-odbclient-2.0.2rc1.tar` & `pylife-odbclient-2.0.3rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:11.176862 pylife-odbclient-2.0.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2022-12-13 10:55:11.176862 pylife-odbclient-2.0.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-13 10:55:11.176862 pylife-odbclient-2.0.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:11.172862 pylife-odbclient-2.0.2rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:11.172862 pylife-odbclient-2.0.2rc1/src/odbclient/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/src/odbclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/src/odbclient/odbclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:11.176862 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2022-12-13 10:55:10.000000 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-13 10:55:11.000000 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 10:55:10.000000 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 10:55:10.000000 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-13 10:55:10.000000 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-13 10:55:10.000000 pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:55:11.176862 pylife-odbclient-2.0.2rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   238316 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/tests/beam_3d_hex_quad.odb
--rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/tests/connectivity.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/tests/node_coordinates.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/tests/stress_element_nodal.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/tests/stress_integration_point.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2022-12-13 10:55:07.000000 pylife-odbclient-2.0.2rc1/tests/test_odbclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-13 08:57:30.767831 pylife-odbclient-2.0.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.759831 pylife-odbclient-2.0.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/src/odbclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/src/odbclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/src/odbclient/odbclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 08:57:30.000000 pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:57:30.763831 pylife-odbclient-2.0.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   238316 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/beam_3d_hex_quad.odb
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/connectivity.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/node_coordinates.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/stress_element_nodal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/stress_integration_point.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-13 08:57:24.000000 pylife-odbclient-2.0.3rc1/tests/test_odbclient.py
```

### Comparing `pylife-odbclient-2.0.2rc1/.coveragerc` & `pylife-odbclient-2.0.3rc1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/.gitignore` & `pylife-odbclient-2.0.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/LICENSE` & `pylife-odbclient-2.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/PKG-INFO` & `pylife-odbclient-2.0.3rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbclient
-Version: 2.0.2rc1
+Version: 2.0.3rc1
 Summary: A Python 3 client for odbAccess using pylife-odbserver
 Home-page: https://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Project-URL: Documentation, https://pylife.readthedocs.io
 Platform: any
@@ -50,22 +50,14 @@
 pip install pylife-odbclient
 ```
 
 * See the <a href="../odbserver/">instructions in `pylife-odbserver`</a> on how
   to install the server.
 
 
-Once there are released versions the installation will be easier.
-
-* Install the server using `pip install pylife-odbserver` in a python-2.0
-  environment that is usable from the current Abaqus python engine.
-
-* Install the client package using `pip install pylife-odbclient`.
-
-
 ## Usage
 
 Usually you only will see the `OdbClient` class interface when you access an
 odb file. The only point you care about the server is when you instantiate an
 `OdbClient` object. You need to know the following things
 
 * The path to the Abaqus executable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.2rc1 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc1 Summary: A
 Python 3 client for odbAccess using pylife-odbserver Home-page: https://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Project-URL: Documentation,
 https://pylife.readthedocs.io Platform: any Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Requires-Python: >=3
 Description-Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing
 License-File: LICENSE License-File: AUTHORS.rst # pylife-odbclient A Python 3
@@ -16,26 +16,22 @@
 is querying data from the `odbAccess` interface and returning them in a pickle
 object. This package comes with a python class `OdbClient` that spawns the
 server in the background when an instance of `OdbClient` is instantiated. Then
 the client object can be used to transparently access data from the odb file
 via the server. Once the client object goes out of scope i.e. is deleted, the
 server process is stopped automatically. ## Installation * Install the
 odbclient using `pip` with the command ``` pip install pylife-odbclient ``` *
-See the instructions_in_`pylife-odbserver` on how to install the server. Once
-there are released versions the installation will be easier. * Install the
-server using `pip install pylife-odbserver` in a python-2.0 environment that is
-usable from the current Abaqus python engine. * Install the client package
-using `pip install pylife-odbclient`. ## Usage Usually you only will see the
-`OdbClient` class interface when you access an odb file. The only point you
-care about the server is when you instantiate an `OdbClient` object. You need
-to know the following things * The path to the Abaqus executable * The path to
-the python environment `pylife-server` is installed into. Then you can
-instantiate a `OdbClient` object using ```python import odbclient as CL client
-= CL.OdbClient("yourodb.odb") ``` See the [API docs of `OdbClient`][1] for
-details. ## Limitations ### Limited functionality Only a subset of Abaqus
-variable locations are supported. These are: nodal, element nodal, whole
-element and centroid. Integration point variables are extrapolated to element
-nodal. You can only extract data from an odb file, not write to it. ### String
-literals So far only names made of `ascii` strings are supported. That means
-that instance names, node that names and the like containing non-ascii
-characters like German umlauts will not work. ___ [1]: https://
-pylife.readthedocs.io/en/latest/tools/odbclient/odbclient.html
+See the instructions_in_`pylife-odbserver` on how to install the server. ##
+Usage Usually you only will see the `OdbClient` class interface when you access
+an odb file. The only point you care about the server is when you instantiate
+an `OdbClient` object. You need to know the following things * The path to the
+Abaqus executable * The path to the python environment `pylife-server` is
+installed into. Then you can instantiate a `OdbClient` object using ```python
+import odbclient as CL client = CL.OdbClient("yourodb.odb") ``` See the [API
+docs of `OdbClient`][1] for details. ## Limitations ### Limited functionality
+Only a subset of Abaqus variable locations are supported. These are: nodal,
+element nodal, whole element and centroid. Integration point variables are
+extrapolated to element nodal. You can only extract data from an odb file, not
+write to it. ### String literals So far only names made of `ascii` strings are
+supported. That means that instance names, node that names and the like
+containing non-ascii characters like German umlauts will not work. ___ [1]:
+https://pylife.readthedocs.io/en/latest/tools/odbclient/odbclient.html
```

### Comparing `pylife-odbclient-2.0.2rc1/README.md` & `pylife-odbclient-2.0.3rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,22 +32,14 @@
 pip install pylife-odbclient
 ```
 
 * See the <a href="../odbserver/">instructions in `pylife-odbserver`</a> on how
   to install the server.
 
 
-Once there are released versions the installation will be easier.
-
-* Install the server using `pip install pylife-odbserver` in a python-2.0
-  environment that is usable from the current Abaqus python engine.
-
-* Install the client package using `pip install pylife-odbclient`.
-
-
 ## Usage
 
 Usually you only will see the `OdbClient` class interface when you access an
 odb file. The only point you care about the server is when you instantiate an
 `OdbClient` object. You need to know the following things
 
 * The path to the Abaqus executable
```

#### html2text {}

```diff
@@ -9,25 +9,22 @@
 returning them in a pickle object. This package comes with a python class
 `OdbClient` that spawns the server in the background when an instance of
 `OdbClient` is instantiated. Then the client object can be used to
 transparently access data from the odb file via the server. Once the client
 object goes out of scope i.e. is deleted, the server process is stopped
 automatically. ## Installation * Install the odbclient using `pip` with the
 command ``` pip install pylife-odbclient ``` * See the instructions_in_`pylife-
-odbserver` on how to install the server. Once there are released versions the
-installation will be easier. * Install the server using `pip install pylife-
-odbserver` in a python-2.0 environment that is usable from the current Abaqus
-python engine. * Install the client package using `pip install pylife-
-odbclient`. ## Usage Usually you only will see the `OdbClient` class interface
-when you access an odb file. The only point you care about the server is when
-you instantiate an `OdbClient` object. You need to know the following things *
-The path to the Abaqus executable * The path to the python environment `pylife-
-server` is installed into. Then you can instantiate a `OdbClient` object using
-```python import odbclient as CL client = CL.OdbClient("yourodb.odb") ``` See
-the [API docs of `OdbClient`][1] for details. ## Limitations ### Limited
-functionality Only a subset of Abaqus variable locations are supported. These
-are: nodal, element nodal, whole element and centroid. Integration point
-variables are extrapolated to element nodal. You can only extract data from an
-odb file, not write to it. ### String literals So far only names made of
-`ascii` strings are supported. That means that instance names, node that names
-and the like containing non-ascii characters like German umlauts will not work.
-___ [1]: https://pylife.readthedocs.io/en/latest/tools/odbclient/odbclient.html
+odbserver` on how to install the server. ## Usage Usually you only will see the
+`OdbClient` class interface when you access an odb file. The only point you
+care about the server is when you instantiate an `OdbClient` object. You need
+to know the following things * The path to the Abaqus executable * The path to
+the python environment `pylife-server` is installed into. Then you can
+instantiate a `OdbClient` object using ```python import odbclient as CL client
+= CL.OdbClient("yourodb.odb") ``` See the [API docs of `OdbClient`][1] for
+details. ## Limitations ### Limited functionality Only a subset of Abaqus
+variable locations are supported. These are: nodal, element nodal, whole
+element and centroid. Integration point variables are extrapolated to element
+nodal. You can only extract data from an odb file, not write to it. ### String
+literals So far only names made of `ascii` strings are supported. That means
+that instance names, node that names and the like containing non-ascii
+characters like German umlauts will not work. ___ [1]: https://
+pylife.readthedocs.io/en/latest/tools/odbclient/odbclient.html
```

### Comparing `pylife-odbclient-2.0.2rc1/demo.ipynb` & `pylife-odbclient-2.0.3rc1/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/setup.cfg` & `pylife-odbclient-2.0.3rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	pandas
+	numpy==1.23.5
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `pylife-odbclient-2.0.2rc1/setup.py` & `pylife-odbclient-2.0.3rc1/setup.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/src/odbclient/__init__.py` & `pylife-odbclient-2.0.3rc1/src/odbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/src/odbclient/odbclient.py` & `pylife-odbclient-2.0.3rc1/src/odbclient/odbclient.py`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/PKG-INFO` & `pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylife-odbclient
-Version: 2.0.2rc1
+Version: 2.0.3rc1
 Summary: A Python 3 client for odbAccess using pylife-odbserver
 Home-page: https://github.com/boschresearch/pylife
 Author: Johannes Mueller
 Author-email: johannes.mueller4@de.bosch.com
 License: Apache-2
 Project-URL: Documentation, https://pylife.readthedocs.io
 Platform: any
@@ -50,22 +50,14 @@
 pip install pylife-odbclient
 ```
 
 * See the <a href="../odbserver/">instructions in `pylife-odbserver`</a> on how
   to install the server.
 
 
-Once there are released versions the installation will be easier.
-
-* Install the server using `pip install pylife-odbserver` in a python-2.0
-  environment that is usable from the current Abaqus python engine.
-
-* Install the client package using `pip install pylife-odbclient`.
-
-
 ## Usage
 
 Usually you only will see the `OdbClient` class interface when you access an
 odb file. The only point you care about the server is when you instantiate an
 `OdbClient` object. You need to know the following things
 
 * The path to the Abaqus executable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.2rc1 Summary: A
+Metadata-Version: 2.1 Name: pylife-odbclient Version: 2.0.3rc1 Summary: A
 Python 3 client for odbAccess using pylife-odbserver Home-page: https://
 github.com/boschresearch/pylife Author: Johannes Mueller Author-email:
 johannes.mueller4@de.bosch.com License: Apache-2 Project-URL: Documentation,
 https://pylife.readthedocs.io Platform: any Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python Requires-Python: >=3
 Description-Content-Type: text/markdown; charset=UTF-8 Provides-Extra: testing
 License-File: LICENSE License-File: AUTHORS.rst # pylife-odbclient A Python 3
@@ -16,26 +16,22 @@
 is querying data from the `odbAccess` interface and returning them in a pickle
 object. This package comes with a python class `OdbClient` that spawns the
 server in the background when an instance of `OdbClient` is instantiated. Then
 the client object can be used to transparently access data from the odb file
 via the server. Once the client object goes out of scope i.e. is deleted, the
 server process is stopped automatically. ## Installation * Install the
 odbclient using `pip` with the command ``` pip install pylife-odbclient ``` *
-See the instructions_in_`pylife-odbserver` on how to install the server. Once
-there are released versions the installation will be easier. * Install the
-server using `pip install pylife-odbserver` in a python-2.0 environment that is
-usable from the current Abaqus python engine. * Install the client package
-using `pip install pylife-odbclient`. ## Usage Usually you only will see the
-`OdbClient` class interface when you access an odb file. The only point you
-care about the server is when you instantiate an `OdbClient` object. You need
-to know the following things * The path to the Abaqus executable * The path to
-the python environment `pylife-server` is installed into. Then you can
-instantiate a `OdbClient` object using ```python import odbclient as CL client
-= CL.OdbClient("yourodb.odb") ``` See the [API docs of `OdbClient`][1] for
-details. ## Limitations ### Limited functionality Only a subset of Abaqus
-variable locations are supported. These are: nodal, element nodal, whole
-element and centroid. Integration point variables are extrapolated to element
-nodal. You can only extract data from an odb file, not write to it. ### String
-literals So far only names made of `ascii` strings are supported. That means
-that instance names, node that names and the like containing non-ascii
-characters like German umlauts will not work. ___ [1]: https://
-pylife.readthedocs.io/en/latest/tools/odbclient/odbclient.html
+See the instructions_in_`pylife-odbserver` on how to install the server. ##
+Usage Usually you only will see the `OdbClient` class interface when you access
+an odb file. The only point you care about the server is when you instantiate
+an `OdbClient` object. You need to know the following things * The path to the
+Abaqus executable * The path to the python environment `pylife-server` is
+installed into. Then you can instantiate a `OdbClient` object using ```python
+import odbclient as CL client = CL.OdbClient("yourodb.odb") ``` See the [API
+docs of `OdbClient`][1] for details. ## Limitations ### Limited functionality
+Only a subset of Abaqus variable locations are supported. These are: nodal,
+element nodal, whole element and centroid. Integration point variables are
+extrapolated to element nodal. You can only extract data from an odb file, not
+write to it. ### String literals So far only names made of `ascii` strings are
+supported. That means that instance names, node that names and the like
+containing non-ascii characters like German umlauts will not work. ___ [1]:
+https://pylife.readthedocs.io/en/latest/tools/odbclient/odbclient.html
```

### Comparing `pylife-odbclient-2.0.2rc1/src/pylife_odbclient.egg-info/SOURCES.txt` & `pylife-odbclient-2.0.3rc1/src/pylife_odbclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/tests/beam_3d_hex_quad.odb` & `pylife-odbclient-2.0.3rc1/tests/beam_3d_hex_quad.odb`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/tests/node_coordinates.csv` & `pylife-odbclient-2.0.3rc1/tests/node_coordinates.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/tests/stress_element_nodal.csv` & `pylife-odbclient-2.0.3rc1/tests/stress_element_nodal.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/tests/stress_integration_point.csv` & `pylife-odbclient-2.0.3rc1/tests/stress_integration_point.csv`

 * *Files identical despite different names*

### Comparing `pylife-odbclient-2.0.2rc1/tests/test_odbclient.py` & `pylife-odbclient-2.0.3rc1/tests/test_odbclient.py`

 * *Files identical despite different names*

