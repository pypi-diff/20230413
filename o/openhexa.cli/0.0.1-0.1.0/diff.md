# Comparing `tmp/openhexa.cli-0.0.1.tar.gz` & `tmp/openhexa.cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.cli-0.0.1.tar", last modified: Thu Apr 13 08:17:00 2023, max compression
+gzip compressed data, was "openhexa.cli-0.1.0.tar", last modified: Thu Apr 13 13:07:22 2023, max compression
```

## Comparing `openhexa.cli-0.0.1.tar` & `openhexa.cli-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2023-04-13 08:17:00.141006 openhexa.cli-0.0.1/
--rw-r--r--   0 quentin    (501) staff       (20)     1057 2023-04-12 12:53:35.000000 openhexa.cli-0.0.1/LICENCE
--rw-r--r--   0 quentin    (501) staff       (20)      452 2023-04-13 08:17:00.141080 openhexa.cli-0.0.1/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)        0 2023-04-12 12:52:19.000000 openhexa.cli-0.0.1/README.md
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2023-04-13 08:17:00.139319 openhexa.cli-0.0.1/openhexa/
--rw-r--r--   0 quentin    (501) staff       (20)       22 2023-04-12 13:53:32.000000 openhexa.cli-0.0.1/openhexa/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)     6377 2023-04-12 14:43:39.000000 openhexa.cli-0.0.1/openhexa/api.py
--rw-r--r--   0 quentin    (501) staff       (20)     7646 2023-04-12 15:05:42.000000 openhexa.cli-0.0.1/openhexa/cli.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2023-04-13 08:17:00.140709 openhexa.cli-0.0.1/openhexa.cli.egg-info/
--rw-r--r--   0 quentin    (501) staff       (20)      452 2023-04-13 08:17:00.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)      353 2023-04-13 08:17:00.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/SOURCES.txt
--rw-r--r--   0 quentin    (501) staff       (20)        1 2023-04-13 08:17:00.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/dependency_links.txt
--rw-r--r--   0 quentin    (501) staff       (20)       46 2023-04-13 08:17:00.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/entry_points.txt
--rw-r--r--   0 quentin    (501) staff       (20)       41 2023-04-13 08:17:00.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/requires.txt
--rw-r--r--   0 quentin    (501) staff       (20)        9 2023-04-13 08:17:00.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/top_level.txt
--rw-r--r--   0 quentin    (501) staff       (20)        1 2023-04-12 15:06:01.000000 openhexa.cli-0.0.1/openhexa.cli.egg-info/zip-safe
--rw-r--r--   0 quentin    (501) staff       (20)       89 2023-04-12 12:44:06.000000 openhexa.cli-0.0.1/pyproject.toml
--rw-r--r--   0 quentin    (501) staff       (20)      763 2023-04-13 08:17:00.141422 openhexa.cli-0.0.1/setup.cfg
--rw-r--r--   0 quentin    (501) staff       (20)       89 2023-04-12 09:28:16.000000 openhexa.cli-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:07:22.949430 openhexa.cli-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-13 13:07:22.949430 openhexa.cli-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:07:22.949430 openhexa.cli-0.1.0/openhexa/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/openhexa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/openhexa/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/openhexa/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:07:22.949430 openhexa.cli-0.1.0/openhexa.cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-13 13:07:22.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 13:07:22.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:07:22.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 13:07:22.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 13:07:22.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 13:07:22.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:07:13.000000 openhexa.cli-0.1.0/openhexa.cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 13:07:22.949430 openhexa.cli-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 13:07:07.000000 openhexa.cli-0.1.0/setup.py
```

### Comparing `openhexa.cli-0.0.1/LICENCE` & `openhexa.cli-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `openhexa.cli-0.0.1/openhexa/api.py` & `openhexa.cli-0.1.0/openhexa/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import base64
 import configparser
-import click
-import sys
-import os
+import importlib
 import io
-import requests
+import os
+import sys
 import typing
 from zipfile import ZipFile
-import base64
-import importlib
+
+import click
+import requests
+
 from . import __version__
 
 CONFIGFILE_PATH = os.path.expanduser("~") + "/.openhexa.ini"
 
 
 def is_debug(config: configparser.ConfigParser):
     return config.getboolean("openhexa", "debug", fallback=False)
```

### Comparing `openhexa.cli-0.0.1/openhexa/cli.py` & `openhexa.cli-0.1.0/openhexa/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import click
-import sys
 import os
+import sys
+
+import click
+
+from . import __version__
 from .api import (
-    open_config,
-    save_config,
-    get_workspace,
-    get_pipelines,
-    get_pipeline,
     create_pipeline,
+    get_pipeline,
+    get_pipelines,
+    get_workspace,
     import_pipeline,
     is_debug,
+    open_config,
+    save_config,
     upload_pipeline,
 )
-from . import __version__
 
 
 @click.group()
 @click.option("--debug/--no-debug", default=False, envvar="DEBUG")
 @click.version_option(__version__)
 @click.pass_context
 def app(ctx, debug):
```

### Comparing `openhexa.cli-0.0.1/setup.cfg` & `openhexa.cli-0.1.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -20,22 +20,29 @@
 include_package_data = True
 install_requires = 
 	click
 	requests
 
 [options.extras_require]
 dev = 
-	black
-	flake8
+	black==22.3.0
+	flake8==4.0.1
 	build
+	pre-commit
 
 [options.package_data]
 * = README.md
 
 [options.entry_points]
 console_scripts = 
 	openhexa = openhexa.cli:app
 
+[flake8]
+ignore = W293, E501, W503, F841, E203
+max-line-length = 120
+per-file-ignores = 
+	__init__.py: F401
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

