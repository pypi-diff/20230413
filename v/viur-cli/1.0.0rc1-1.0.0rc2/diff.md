# Comparing `tmp/viur_cli-1.0.0rc1.tar.gz` & `tmp/viur_cli-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-1.0.0rc1.tar", last modified: Wed Mar 29 05:09:42 2023, max compression
+gzip compressed data, was "viur_cli-1.0.0rc2.tar", last modified: Fri Mar 31 12:15:35 2023, max compression
```

## Comparing `viur_cli-1.0.0rc1.tar` & `viur_cli-1.0.0rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.650011 viur_cli-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-29 05:09:42.650011 viur_cli-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-29 05:09:42.654011 viur_cli-1.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.642011 viur_cli-1.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.646011 viur_cli-1.0.0rc1/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/npm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.650011 viur_cli-1.0.0rc1/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.650011 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.650011 viur_cli-1.0.0rc1/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scripts/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-29 05:09:34.000000 viur_cli-1.0.0rc1/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:09:42.650011 viur_cli-1.0.0rc1/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-29 05:09:42.000000 viur_cli-1.0.0rc1/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-29 05:09:42.000000 viur_cli-1.0.0rc1/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 05:09:42.000000 viur_cli-1.0.0rc1/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-29 05:09:42.000000 viur_cli-1.0.0rc1/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-29 05:09:42.000000 viur_cli-1.0.0rc1/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 05:09:42.000000 viur_cli-1.0.0rc1/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.440485 viur_cli-1.0.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.440485 viur_cli-1.0.0rc2/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/npm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-31 12:15:27.000000 viur_cli-1.0.0rc2/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:15:35.444485 viur_cli-1.0.0rc2/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 12:15:35.000000 viur_cli-1.0.0rc2/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-1.0.0rc1/LICENSE` & `viur_cli-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/PKG-INFO` & `viur_cli-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 1.0.0rc1 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 1.0.0rc2 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.0rc1/README.md` & `viur_cli-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/setup.cfg` & `viur_cli-1.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/build.py` & `viur_cli-1.0.0rc2/src/viur_cli/build.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/cli.py` & `viur_cli-1.0.0rc2/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/conf.py` & `viur_cli-1.0.0rc2/src/viur_cli/conf.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/deploy.py` & `viur_cli-1.0.0rc2/src/viur_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/flare.py` & `viur_cli-1.0.0rc2/src/viur_cli/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/install.py` & `viur_cli-1.0.0rc2/src/viur_cli/install.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/local.py` & `viur_cli-1.0.0rc2/src/viur_cli/local.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/npm.py` & `viur_cli-1.0.0rc2/src/viur_cli/npm.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/script.py` & `viur_cli-1.0.0rc2/src/viur_cli/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import click
-import os
-
-from . import cli
-
-
-@cli.group()
-def script():
-    """run different viur related scripts"""
-
-
-@script.command(name="2to3")
-@click.argument("path")
-@click.option('--dryrun', '-d', is_flag=True, default=False)
-@click.option('--daredevil', '-x', is_flag=True, default=False)
-def two_to_three(path, *args, **kwargs):
-    """viur porting script"""
-    command = f"viur-2to3 {path}"
-    for option, value in kwargs.items():
-        if value:
-            command += f" --{option}"
-
-    os.system(command)
-
-
-@script.command()
-@click.option('--source', '-s')
-@click.option('--target', '-t')
-@click.option('--name', '-n')
-@click.option('--minify', '-m', is_flag=True, default=False)
-@click.option('--compile', '-c', is_flag=True, default=False)
-@click.option('--zip', '-z', is_flag=True, default=False)
-@click.option('--watch', '-w', is_flag=True, default=False)
-def flare(*args, **kwargs):
-    """flare build script"""
-    command = "flare"
-    for option, value in kwargs.items():
-        if value and isinstance(value, bool):
-            command += f" --{option}"
-        elif value:
-            command += f" --{option} {value}"
-    os.system(command)
-
-
-@script.command()
-@click.option('--version', '-v')
-@click.option('--package', '-p')
-@click.option('--target', '-t')
-@click.option('--help', '-h')
-def pyodide(additional_args, version, package, target, help):
-    """run the get_pyodide command"""
-    command = "get-pyodide"
-    if help:
-        os.system("get-pyodide -h")
-
-    if version:
-        command += f" -v {version}"
-
-    if package:
-        command += f" -p {package}"
-
-    if target:
-        command += f" -t {target}"
-
-    os.system(command)
-
-
-@script.command()
-def ssl_fix():
-    """ssl fix for macos"""
-    os.system("chmod +x scripts/macos_certificate_fix.command && ./scripts/macos_certificate_fix.command")
+import click
+import os
+
+from . import cli
+
+
+@cli.group()
+def tool():
+    """run different viur related scripts"""
+
+
+@tool.command(name="2to3")
+@click.argument("path")
+@click.option('--dryrun', '-d', is_flag=True, default=False)
+@click.option('--daredevil', '-x', is_flag=True, default=False)
+def two_to_three(path, *args, **kwargs):
+    """viur porting script"""
+    command = f"viur-2to3 {path}"
+    for option, value in kwargs.items():
+        if value:
+            command += f" --{option}"
+
+    os.system(command)
+
+
+@tool.command()
+@click.option('--source', '-s')
+@click.option('--target', '-t')
+@click.option('--name', '-n')
+@click.option('--minify', '-m', is_flag=True, default=False)
+@click.option('--compile', '-c', is_flag=True, default=False)
+@click.option('--zip', '-z', is_flag=True, default=False)
+@click.option('--watch', '-w', is_flag=True, default=False)
+def flare(*args, **kwargs):
+    """flare build script"""
+    command = "flare"
+    for option, value in kwargs.items():
+        if value and isinstance(value, bool):
+            command += f" --{option}"
+        elif value:
+            command += f" --{option} {value}"
+    os.system(command)
+
+
+@tool.command()
+@click.option('--version', '-v')
+@click.option('--package', '-p')
+@click.option('--target', '-t')
+@click.option('--help', '-h')
+def pyodide(additional_args, version, package, target, help):
+    """run the get_pyodide command"""
+    command = "get-pyodide"
+    if help:
+        os.system("get-pyodide -h")
+
+    if version:
+        command += f" -v {version}"
+
+    if package:
+        command += f" -p {package}"
+
+    if target:
+        command += f" -t {target}"
+
+    os.system(command)
+
+
+@tool.command()
+def ssl_fix():
+    """ssl fix for macos"""
+    os.system("chmod +x scripts/macos_certificate_fix.command && ./scripts/macos_certificate_fix.command")
```

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/cli.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,21 @@
 def build_url(url: str):
     return Config()["base_url"] + "/" + url
 
 viur.request.build_url = staticmethod(build_url)
 
 
 @cli.group()
-def scriptor():
+def script():
     """
     Manage and run scriptor scripts locally on the console
     """
 
 
-@scriptor.command()
+@script.command()
 @click.option('--url', default=None, help='Set the url')
 @click.option('--username', default=None, help='Set the username')
 @click.option('--working_dir', default=None, help='Set the working directory where scripts are stored to')
 def configure(url: str, username: str, working_dir: str):
     """
     Manage configuration settings.
     """
@@ -78,15 +78,15 @@
     if username:
         conf["username"] = username
 
     if working_dir:
         conf["working_dir"] = working_dir.replace("\\", "/")
 
 
-@scriptor.command()
+@script.command()
 def setup():
     """
     Setup user session with a given username and password.
     """
     config = Config()
     base_url = config.get("base_url")
     try:
@@ -123,15 +123,15 @@
 
     response = s.get(base_url+"/vi/user/view/self", cookies=Config().get("cookies", {}))
     if not response.ok:
         click.echo("Invalid session, please run `viur script setup` again.")
         ctx.invoke(setup)
         ctx.close()
 
-@scriptor.command()
+@script.command()
 @click.option('--force', default=False, help='Force replace files from server in local working directory')
 @click.pass_context
 def pull(ctx: click.Context, force: bool):
     """
     Pull contents from server to working_dir.
     """
     check_session(ctx)
@@ -173,15 +173,15 @@
                     create_file()
 
         await tree.for_each(for_each)
 
     asyncio.new_event_loop().run_until_complete(main())
 
 
-@scriptor.command()
+@script.command()
 @click.option('--force', '-f', is_flag=True, default=False,
               help='Force push files from the local working directory onto the server')
 @click.pass_context
 def push(ctx: click.Context, force: bool):
     """
     Push contents of working_dir to server.
     """
@@ -285,15 +285,15 @@
 
                     click.echo(f"Push {_real_file}")
                     await tree.add(_type, args)
 
     asyncio.new_event_loop().run_until_complete(main())
 
 
-@scriptor.command()
+@script.command()
 @click.argument('path', required=True)
 @click.pass_context
 def run(ctx: click.Context, path: str):
     """
     Locally run a script located in the working_dir.
     """
     check_session(ctx)
```

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-1.0.0rc2/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scripts/flare.py` & `viur_cli-1.0.0rc2/src/viur_cli/scripts/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-1.0.0rc2/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-1.0.0rc2/src/viur_cli/scripts/viur_2to3.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/setup.py` & `viur_cli-1.0.0rc2/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli/utils.py` & `viur_cli-1.0.0rc2/src/viur_cli/utils.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.0rc1/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-1.0.0rc2/src/viur_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-cli
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-cli Version: 1.0.0rc1 Summary: Command-line
+Metadata-Version: 2.1 Name: viur-cli Version: 1.0.0rc2 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.0rc1/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-1.0.0rc2/src/viur_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 src/viur_cli/cli.py
 src/viur_cli/conf.py
 src/viur_cli/deploy.py
 src/viur_cli/flare.py
 src/viur_cli/install.py
 src/viur_cli/local.py
 src/viur_cli/npm.py
-src/viur_cli/script.py
 src/viur_cli/setup.py
+src/viur_cli/tool.py
 src/viur_cli/utils.py
 src/viur_cli/version.py
 src/viur_cli.egg-info/PKG-INFO
 src/viur_cli.egg-info/SOURCES.txt
 src/viur_cli.egg-info/dependency_links.txt
 src/viur_cli.egg-info/entry_points.txt
 src/viur_cli.egg-info/requires.txt
```

