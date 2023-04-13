# Comparing `tmp/playmolecule-1.6.6.tar.gz` & `tmp/playmolecule-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.6.6.tar", last modified: Thu Apr 13 08:37:39 2023, max compression
+gzip compressed data, was "playmolecule-1.6.7.tar", last modified: Thu Apr 13 09:02:39 2023, max compression
```

## Comparing `playmolecule-1.6.6.tar` & `playmolecule-1.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:37:39.542734 playmolecule-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-13 08:37:29.000000 playmolecule-1.6.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 08:37:29.000000 playmolecule-1.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 08:37:39.542734 playmolecule-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 08:37:29.000000 playmolecule-1.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:37:39.542734 playmolecule-1.6.6/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33006 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 08:37:29.000000 playmolecule-1.6.6/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:37:39.542734 playmolecule-1.6.6/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 08:37:39.000000 playmolecule-1.6.6/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 08:37:39.000000 playmolecule-1.6.6/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:37:39.000000 playmolecule-1.6.6/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 08:37:39.000000 playmolecule-1.6.6/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 08:37:39.000000 playmolecule-1.6.6/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 08:37:29.000000 playmolecule-1.6.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:37:39.542734 playmolecule-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 08:37:29.000000 playmolecule-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:39.700542 playmolecule-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-13 09:02:28.000000 playmolecule-1.6.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 09:02:28.000000 playmolecule-1.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 09:02:39.700542 playmolecule-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 09:02:28.000000 playmolecule-1.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:39.700542 playmolecule-1.6.7/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 09:02:28.000000 playmolecule-1.6.7/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:02:39.700542 playmolecule-1.6.7/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 09:02:39.000000 playmolecule-1.6.7/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 09:02:28.000000 playmolecule-1.6.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:02:39.700542 playmolecule-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 09:02:28.000000 playmolecule-1.6.7/setup.py
```

### Comparing `playmolecule-1.6.6/LICENSE.md` & `playmolecule-1.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/PKG-INFO` & `playmolecule-1.6.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.6
+Version: 1.6.7
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.6/playmolecule/__init__.py` & `playmolecule-1.6.7/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/_test_funcs.py` & `playmolecule-1.6.7/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/config.py` & `playmolecule-1.6.7/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/datacenter.py` & `playmolecule-1.6.7/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/devutils.py` & `playmolecule-1.6.7/playmolecule/devutils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/func2argparse.py` & `playmolecule-1.6.7/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/job.py` & `playmolecule-1.6.7/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/jsonlogger.py` & `playmolecule-1.6.7/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/local.py` & `playmolecule-1.6.7/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/playqueue.py` & `playmolecule-1.6.7/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule/session.py` & `playmolecule-1.6.7/playmolecule/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,29 @@
 import json
 import os
 
 
 logger = logging.getLogger(__name__)
 
 
+class fg:
+    black = "\u001b[30m"
+    red = "\u001b[31m"
+    green = "\u001b[32m"
+    yellow = "\u001b[33m"
+    blue = "\u001b[34m"
+    magenta = "\u001b[35m"
+    cyan = "\u001b[36m"
+    white = "\u001b[37m"
+    end = "\033[0m"
+
+    def rgb(r, g, b):
+        return f"\u001b[38;2;{r};{g};{b}m"
+
+
 class UserNotFoundError(Exception):
     pass
 
 
 class UserFailedRegistrationError(Exception):
     pass
 
@@ -59,29 +74,29 @@
     )
     optionalparams = sorted(
         [param for param in nonprivparams if not param["mandatory"]],
         key=lambda param: param["name"],
     )
     printparams = mandatoryparams + optionalparams
 
-    print("Parameters\n----------")
+    print(f"{fg.yellow}Parameters\n----------{fg.end}")
     for param in printparams:
         atype = param["type"]
         if atype == "str_to_bool":
             atype = "bool"
         if param["nargs"] is not None:
             atype = f"list[{atype}]"
         default = param["value"] if param["type"] != "str" else f"\"{param['value']}\""
-        helpstr = f"{param['name']} : {atype}, default={default}"
+        helpstr = f"{fg.yellow}{param['name']}{fg.end} : {fg.blue}{atype}{fg.end}, {fg.green}default={default}{fg.end}"
         if param["mandatory"]:
-            helpstr += " [Required]"
+            helpstr += f" {fg.red}[Required]{fg.end}"
         choices = param["choices"]
         if choices is not None:
             choices = '", "'.join(choices)
-            helpstr += f', choices=("{choices}")'
+            helpstr += f', {fg.magenta}choices=("{choices}"){fg.end}'
         print(helpstr)
         descr = param["description"]
         print("    " + descr)
 
 
 def _find_token(token):
     """Searches for the token file in the default locations and env vars"""
```

### Comparing `playmolecule-1.6.6/playmolecule/utils.py` & `playmolecule-1.6.7/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.6.7/playmolecule.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.6
+Version: 1.6.7
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.6/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.6.7/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.6/setup.py` & `playmolecule-1.6.7/setup.py`

 * *Files identical despite different names*

