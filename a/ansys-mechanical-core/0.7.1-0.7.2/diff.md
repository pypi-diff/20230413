# Comparing `tmp/ansys-mechanical-core-0.7.1.tar.gz` & `tmp/ansys-mechanical-core-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mechanical-core-0.7.1.tar", last modified: Mon Apr 10 12:41:59 2023, max compression
+gzip compressed data, was "ansys-mechanical-core-0.7.2.tar", last modified: Thu Apr 13 16:27:32 2023, max compression
```

## Comparing `ansys-mechanical-core-0.7.1.tar` & `ansys-mechanical-core-0.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-04-10 12:41:47.449289 ansys-mechanical-core-0.7.1/LICENSE
--rw-r--r--   0        0        0     5456 2023-04-10 12:41:47.449289 ansys-mechanical-core-0.7.1/README.rst
--rw-r--r--   0        0        0     3922 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      167 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     4811 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     1344 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     2022 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/logging.py
--rw-r--r--   0        0        0      852 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2992 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    83310 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25079 2023-04-10 12:41:47.457289 ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-13 16:27:09.947751 ansys-mechanical-core-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5456 2023-04-13 16:27:09.947751 ansys-mechanical-core-0.7.2/README.rst
+-rw-r--r--   0        0        0     3922 2023-04-13 16:27:09.955751 ansys-mechanical-core-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      167 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     4811 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     1344 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     2022 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/logging.py
+-rw-r--r--   0        0        0      852 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2992 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    83310 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25079 2023-04-13 16:27:09.959751 ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.7.2/PKG-INFO
```

### Comparing `ansys-mechanical-core-0.7.1/LICENSE` & `ansys-mechanical-core-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/README.rst` & `ansys-mechanical-core-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/pyproject.toml` & `ansys-mechanical-core-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.7.1"
+version = "0.7.2"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -44,29 +44,29 @@
 Documentation = "https://mechanical.docs.pyansys.com"
 Source = "https://github.com/pyansys/pymechanical"
 Homepage = "https://github.com/pyansys/pymechanical"
 Tracker = "https://github.com/pyansys/pymechanical/issues"
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.2.2",
+    "pytest==7.3.0",
     "pytest-cov==4.0.0",
     "pytest-print==0.3.1",
 ]
 doc = [
     "Sphinx==5.3.0",
-    "ansys-sphinx-theme==0.9.6",
+    "ansys-sphinx-theme==0.9.7",
     "grpcio==1.53.0",
     "imageio-ffmpeg==0.4.8",
     "imageio==2.27.0",
     "jupyter_sphinx==0.4.0",
     "jupyterlab>=3.2.8",
     "matplotlib==3.7.1",
     "numpydoc==1.5.0",
-    "plotly==5.14.0",
+    "plotly==5.14.1",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
     "pyvista==0.38.5",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.22",
     "sphinx-copybutton==0.5.1",
```

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/__init__.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/_version.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/app.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/app.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/config.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/imports.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/initializer.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/initializer.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/loader.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/logging.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/resolver.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/runtime.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/embedding/shims.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/errors.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/examples/downloads.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/launcher.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/logging.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/mechanical.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/misc.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/src/ansys/mechanical/core/pool.py` & `ansys-mechanical-core-0.7.2/src/ansys/mechanical/core/pool.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.7.1/PKG-INFO` & `ansys-mechanical-core-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,36 +21,36 @@
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: protobuf>=3.12.2,<3.21.0
 Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: tqdm>=4.45.0
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.6 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
 Requires-Dist: grpcio==1.53.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: imageio==2.27.0 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: jupyterlab>=3.2.8 ; extra == "doc"
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: plotly==5.14.0 ; extra == "doc"
+Requires-Dist: plotly==5.14.1 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pythreejs==2.4.2 ; extra == "doc"
 Requires-Dist: pyvista==0.38.5 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
 Requires-Dist: sphinx_design==0.3.0 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
-Requires-Dist: pytest==7.2.2 ; extra == "tests"
+Requires-Dist: pytest==7.3.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Requires-Dist: pytest-print==0.3.1 ; extra == "tests"
 Project-URL: Documentation, https://mechanical.docs.pyansys.com
 Project-URL: Homepage, https://github.com/pyansys/pymechanical
 Project-URL: Source, https://github.com/pyansys/pymechanical
 Project-URL: Tracker, https://github.com/pyansys/pymechanical/issues
 Provides-Extra: doc
```

