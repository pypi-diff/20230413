# Comparing `tmp/napari-ui-tracer-0.1.1.tar.gz` & `tmp/napari-ui-tracer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-ui-tracer-0.1.1.tar", last modified: Tue Mar 14 17:46:45 2023, max compression
+gzip compressed data, was "napari-ui-tracer-0.1.2.tar", last modified: Thu Apr 13 17:43:08 2023, max compression
```

## Comparing `napari-ui-tracer-0.1.1.tar` & `napari-ui-tracer-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:46:45.465378 napari-ui-tracer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-03-14 17:46:45.465378 napari-ui-tracer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-14 17:46:45.465378 napari-ui-tracer-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:46:45.461378 napari-ui-tracer-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:46:45.465378 napari-ui-tracer-0.1.1/src/napari_ui_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:46:45.465378 napari-ui-tracer-0.1.1/src/napari_ui_tracer/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-14 17:46:20.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 17:46:45.465378 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-03-14 17:46:45.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-14 17:46:45.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 17:46:45.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-14 17:46:45.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-14 17:46:45.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 17:46:45.000000 napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:08.058273 napari-ui-tracer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-13 17:42:50.000000 napari-ui-tracer-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 17:42:50.000000 napari-ui-tracer-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-13 17:43:08.058273 napari-ui-tracer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-13 17:42:50.000000 napari-ui-tracer-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-13 17:42:51.000000 napari-ui-tracer-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 17:43:08.062271 napari-ui-tracer-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:08.058273 napari-ui-tracer-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:08.058273 napari-ui-tracer-0.1.2/src/napari_ui_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 17:42:51.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:08.058273 napari-ui-tracer-0.1.2/src/napari_ui_tracer/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:42:51.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-13 17:42:51.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-13 17:42:51.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-13 17:42:51.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:08.058273 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-13 17:43:08.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 17:43:08.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:43:08.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 17:43:08.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 17:43:08.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 17:43:08.000000 napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/top_level.txt
```

### Comparing `napari-ui-tracer-0.1.1/LICENSE` & `napari-ui-tracer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-ui-tracer-0.1.1/PKG-INFO` & `napari-ui-tracer-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-ui-tracer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin to help understand Napari UI components and check their source code definition
 Home-page: https://github.com/dalthviz/napari-ui-tracer
 Author: Daniel Althviz
 Author-email: dalthviz@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dalthviz/napari-ui-tracer/issues
 Project-URL: Documentation, https://github.com/dalthviz/napari-ui-tracer#README.md
@@ -28,16 +28,19 @@
 Provides-Extra: pyqt5
 Provides-Extra: pre-commit
 License-File: LICENSE
 
 # napari-ui-tracer
 
 [![License MIT](https://img.shields.io/pypi/l/napari-ui-tracer.svg?color=green)](https://github.com/dalthviz/napari-ui-tracer/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ui-tracer.svg?color=green)](https://python.org)
+[![PyPI](https://img.shields.io/pypi/v/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer)
+[![PyPI download month](https://img.shields.io/pypi/dm/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer/)
+[![conda version](https://img.shields.io/conda/vn/conda-forge/napari-ui-tracer.svg?color=blue)](https://anaconda.org/conda-forge/napari-ui-tracer)
+[![conda download count](https://img.shields.io/conda/d/conda-forge/napari-ui-tracer.svg?color=blue)](https://anaconda.org/conda-forge/napari-ui-tracer)
 [![tests](https://github.com/dalthviz/napari-ui-tracer/workflows/tests/badge.svg)](https://github.com/dalthviz/napari-ui-tracer/actions)
 [![codecov](https://codecov.io/gh/dalthviz/napari-ui-tracer/branch/main/graph/badge.svg?token=E6je6vXOSA)](https://codecov.io/gh/dalthviz/napari-ui-tracer)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-ui-tracer)](https://napari-hub.org/plugins/napari-ui-tracer)
 
 A plugin to help understand Napari UI components and locate their code definition
 
 ----------------------------------
@@ -48,21 +51,22 @@
 
 ## Installation
 
 You can install `napari-ui-tracer` via [pip]:
 
     pip install napari-ui-tracer
 
+Or via [conda]:
 
+    conda install -c conda-forge napari-ui-tracer
 
 To install latest development version :
 
     pip install git+https://github.com/dalthviz/napari-ui-tracer.git
 
-
 ## Usage
 
 1. Show the plugin inside the napari interface:
 
     * You can launch napari with the plugin visible running:
 
             napari -w napari-ui-tracer
@@ -108,7 +112,8 @@
 
 [file an issue]: https://github.com/dalthviz/napari-ui-tracer/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+[conda]: https://docs.conda.io/projects/conda/en/stable/
```

### Comparing `napari-ui-tracer-0.1.1/README.md` & `napari-ui-tracer-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # napari-ui-tracer
 
 [![License MIT](https://img.shields.io/pypi/l/napari-ui-tracer.svg?color=green)](https://github.com/dalthviz/napari-ui-tracer/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ui-tracer.svg?color=green)](https://python.org)
+[![PyPI](https://img.shields.io/pypi/v/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer)
+[![PyPI download month](https://img.shields.io/pypi/dm/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer/)
+[![conda version](https://img.shields.io/conda/vn/conda-forge/napari-ui-tracer.svg?color=blue)](https://anaconda.org/conda-forge/napari-ui-tracer)
+[![conda download count](https://img.shields.io/conda/d/conda-forge/napari-ui-tracer.svg?color=blue)](https://anaconda.org/conda-forge/napari-ui-tracer)
 [![tests](https://github.com/dalthviz/napari-ui-tracer/workflows/tests/badge.svg)](https://github.com/dalthviz/napari-ui-tracer/actions)
 [![codecov](https://codecov.io/gh/dalthviz/napari-ui-tracer/branch/main/graph/badge.svg?token=E6je6vXOSA)](https://codecov.io/gh/dalthviz/napari-ui-tracer)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-ui-tracer)](https://napari-hub.org/plugins/napari-ui-tracer)
 
 A plugin to help understand Napari UI components and locate their code definition
 
 ----------------------------------
@@ -17,21 +20,22 @@
 
 ## Installation
 
 You can install `napari-ui-tracer` via [pip]:
 
     pip install napari-ui-tracer
 
+Or via [conda]:
 
+    conda install -c conda-forge napari-ui-tracer
 
 To install latest development version :
 
     pip install git+https://github.com/dalthviz/napari-ui-tracer.git
 
-
 ## Usage
 
 1. Show the plugin inside the napari interface:
 
     * You can launch napari with the plugin visible running:
 
             napari -w napari-ui-tracer
@@ -77,7 +81,8 @@
 
 [file an issue]: https://github.com/dalthviz/napari-ui-tracer/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+[conda]: https://docs.conda.io/projects/conda/en/stable/
```

### Comparing `napari-ui-tracer-0.1.1/setup.cfg` & `napari-ui-tracer-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-ui-tracer-0.1.1/src/napari_ui_tracer/_tests/test_widget.py` & `napari-ui-tracer-0.1.2/src/napari_ui_tracer/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-ui-tracer-0.1.1/src/napari_ui_tracer/_widget.py` & `napari-ui-tracer-0.1.2/src/napari_ui_tracer/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Widget to show information of the Napari widgets classes and module location.
 
 Uses `Ctrl + Mouse right button press`/`Cmd + Mouse right button press`
-to trigger the tracing when the event filter is installed.
+to trigger the tracing when the Qt event filter is enabled and logging events
+information if the application events logging is enabled.
 """
 # Standard library imports
 import inspect
 from pathlib import Path
 from textwrap import indent
 
 # Third-party imports
@@ -171,15 +172,15 @@
             call_stack = inspect.stack(0)
             for frame in call_stack[2 : 2 + cfg.stack_depth]:
                 fname = _shorten_fname(frame.filename)
                 obj = ""
                 if "self" in frame.frame.f_locals:
                     obj = type(frame.frame.f_locals["self"]).__name__ + "."
                 if obj:
-                    ln = f'  <a href="{frame.filename}">"{fname}", line {frame.lineno}, in {obj}{frame.function}</a>'
+                    ln = f'  <a href="file:///{frame.filename}">"{fname}", line {frame.lineno}, in {obj}{frame.function}</a>'
                     lines.append(ln)
             lines.append("")
 
             # find the first caller in the call stack
             for f in reversed(call_stack):
                 if "self" in f.frame.f_locals:
                     obj_type = type(f.frame.f_locals["self"])
```

### Comparing `napari-ui-tracer-0.1.1/src/napari_ui_tracer.egg-info/PKG-INFO` & `napari-ui-tracer-0.1.2/src/napari_ui_tracer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-ui-tracer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin to help understand Napari UI components and check their source code definition
 Home-page: https://github.com/dalthviz/napari-ui-tracer
 Author: Daniel Althviz
 Author-email: dalthviz@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/dalthviz/napari-ui-tracer/issues
 Project-URL: Documentation, https://github.com/dalthviz/napari-ui-tracer#README.md
@@ -28,16 +28,19 @@
 Provides-Extra: pyqt5
 Provides-Extra: pre-commit
 License-File: LICENSE
 
 # napari-ui-tracer
 
 [![License MIT](https://img.shields.io/pypi/l/napari-ui-tracer.svg?color=green)](https://github.com/dalthviz/napari-ui-tracer/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ui-tracer.svg?color=green)](https://python.org)
+[![PyPI](https://img.shields.io/pypi/v/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer)
+[![PyPI download month](https://img.shields.io/pypi/dm/napari-ui-tracer.svg?color=green)](https://pypi.org/project/napari-ui-tracer/)
+[![conda version](https://img.shields.io/conda/vn/conda-forge/napari-ui-tracer.svg?color=blue)](https://anaconda.org/conda-forge/napari-ui-tracer)
+[![conda download count](https://img.shields.io/conda/d/conda-forge/napari-ui-tracer.svg?color=blue)](https://anaconda.org/conda-forge/napari-ui-tracer)
 [![tests](https://github.com/dalthviz/napari-ui-tracer/workflows/tests/badge.svg)](https://github.com/dalthviz/napari-ui-tracer/actions)
 [![codecov](https://codecov.io/gh/dalthviz/napari-ui-tracer/branch/main/graph/badge.svg?token=E6je6vXOSA)](https://codecov.io/gh/dalthviz/napari-ui-tracer)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-ui-tracer)](https://napari-hub.org/plugins/napari-ui-tracer)
 
 A plugin to help understand Napari UI components and locate their code definition
 
 ----------------------------------
@@ -48,21 +51,22 @@
 
 ## Installation
 
 You can install `napari-ui-tracer` via [pip]:
 
     pip install napari-ui-tracer
 
+Or via [conda]:
 
+    conda install -c conda-forge napari-ui-tracer
 
 To install latest development version :
 
     pip install git+https://github.com/dalthviz/napari-ui-tracer.git
 
-
 ## Usage
 
 1. Show the plugin inside the napari interface:
 
     * You can launch napari with the plugin visible running:
 
             napari -w napari-ui-tracer
@@ -108,7 +112,8 @@
 
 [file an issue]: https://github.com/dalthviz/napari-ui-tracer/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+[conda]: https://docs.conda.io/projects/conda/en/stable/
```

