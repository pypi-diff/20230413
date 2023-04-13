# Comparing `tmp/loci-sarif-0.3.0.tar.gz` & `tmp/loci-sarif-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loci-sarif-0.3.0.tar", last modified: Mon Mar 27 02:18:46 2023, max compression
+gzip compressed data, was "loci-sarif-0.3.1.tar", last modified: Thu Apr 13 02:47:34 2023, max compression
```

## Comparing `loci-sarif-0.3.0.tar` & `loci-sarif-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 02:18:46.652089 loci-sarif-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      839 2023-03-27 02:18:46.653089 loci-sarif-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 02:18:46.650089 loci-sarif-0.3.0/loci_sarif/
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-03-27 02:18:44.000000 loci-sarif-0.3.0/loci_sarif/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3256 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/loci_sarif/add.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/loci_sarif/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/loci_sarif/summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5150 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/loci_sarif/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 02:18:46.652089 loci-sarif-0.3.0/loci_sarif.egg-info/
--rw-r--r--   0 root         (0) root         (0)      839 2023-03-27 02:18:46.000000 loci-sarif-0.3.0/loci_sarif.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      344 2023-03-27 02:18:46.000000 loci-sarif-0.3.0/loci_sarif.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 02:18:46.000000 loci-sarif-0.3.0/loci_sarif.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-27 02:18:46.000000 loci-sarif-0.3.0/loci_sarif.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-27 02:18:46.000000 loci-sarif-0.3.0/loci_sarif.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-27 02:18:46.000000 loci-sarif-0.3.0/loci_sarif.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-03-27 02:18:46.653089 loci-sarif-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-03-27 02:18:32.000000 loci-sarif-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:47:34.064591 loci-sarif-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      839 2023-04-13 02:47:34.064591 loci-sarif-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:47:34.062761 loci-sarif-0.3.1/loci_sarif/
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-04-13 02:47:31.000000 loci-sarif-0.3.1/loci_sarif/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/loci_sarif/add.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/loci_sarif/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/loci_sarif/summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5150 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/loci_sarif/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 02:47:34.064591 loci-sarif-0.3.1/loci_sarif.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      839 2023-04-13 02:47:34.000000 loci-sarif-0.3.1/loci_sarif.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      344 2023-04-13 02:47:34.000000 loci-sarif-0.3.1/loci_sarif.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 02:47:34.000000 loci-sarif-0.3.1/loci_sarif.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-13 02:47:34.000000 loci-sarif-0.3.1/loci_sarif.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-13 02:47:34.000000 loci-sarif-0.3.1/loci_sarif.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-13 02:47:34.000000 loci-sarif-0.3.1/loci_sarif.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-13 02:47:34.065507 loci-sarif-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-13 02:47:20.000000 loci-sarif-0.3.1/setup.py
```

### Comparing `loci-sarif-0.3.0/LICENSE` & `loci-sarif-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loci-sarif-0.3.0/PKG-INFO` & `loci-sarif-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loci-sarif
-Version: 0.3.0
+Version: 0.3.1
 Summary: The official Loci Notes SARIF processor.
 Home-page: https://gitlab.com/loci-notes/loci-sarif
 Author: TheTwitchy
 Author-email: thetwitchy@thetwitchy.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loci-sarif-0.3.0/README.md` & `loci-sarif-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `loci-sarif-0.3.0/loci_sarif/add.py` & `loci-sarif-0.3.1/loci_sarif/add.py`

 * *Files identical despite different names*

### Comparing `loci-sarif-0.3.0/loci_sarif/main.py` & `loci-sarif-0.3.1/loci_sarif/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import click
 import loci
 import loci.cli
 
-from loci_sarif import PROG_NAME
+from loci_sarif import PROG_NAME, __version__
 from loci_sarif.add import add
 from loci_sarif.summary import summary
 
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
-    loci.cli.print_version(PROG_NAME)
+    loci.cli.print_version(PROG_NAME, __version__)
     ctx.exit()
 
 
 @click.group()
 @click.option("-v", "--version", is_flag=True, callback=print_version, expose_value=False, is_eager=True)
 def loci_sarif():
     pass
```

### Comparing `loci-sarif-0.3.0/loci_sarif/summary.py` & `loci-sarif-0.3.1/loci_sarif/summary.py`

 * *Files identical despite different names*

### Comparing `loci-sarif-0.3.0/loci_sarif/utils.py` & `loci-sarif-0.3.1/loci_sarif/utils.py`

 * *Files identical despite different names*

### Comparing `loci-sarif-0.3.0/loci_sarif.egg-info/PKG-INFO` & `loci-sarif-0.3.1/loci_sarif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loci-sarif
-Version: 0.3.0
+Version: 0.3.1
 Summary: The official Loci Notes SARIF processor.
 Home-page: https://gitlab.com/loci-notes/loci-sarif
 Author: TheTwitchy
 Author-email: thetwitchy@thetwitchy.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loci-sarif-0.3.0/setup.py` & `loci-sarif-0.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author_email="thetwitchy@thetwitchy.com",
     description="The official Loci Notes SARIF processor.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/loci-notes/loci-sarif",
     packages=setuptools.find_packages(),
     install_requires=[
-        "loci-cli",
+        "loci-cli>=0.10.1",
     ],
     entry_points={
         "console_scripts": [
             "loci-sarif = loci_sarif.main:root_entry",
         ],
     },
 )
```

