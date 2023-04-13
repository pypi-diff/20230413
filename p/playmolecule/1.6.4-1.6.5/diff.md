# Comparing `tmp/playmolecule-1.6.4.tar.gz` & `tmp/playmolecule-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.6.4.tar", last modified: Wed Apr 12 13:44:59 2023, max compression
+gzip compressed data, was "playmolecule-1.6.5.tar", last modified: Thu Apr 13 08:27:22 2023, max compression
```

## Comparing `playmolecule-1.6.4.tar` & `playmolecule-1.6.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:44:59.987275 playmolecule-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-12 13:44:49.000000 playmolecule-1.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 13:44:49.000000 playmolecule-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 13:44:59.987275 playmolecule-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 13:44:49.000000 playmolecule-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:44:59.987275 playmolecule-1.6.4/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:44:59.987275 playmolecule-1.6.4/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 13:44:49.000000 playmolecule-1.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:44:59.987275 playmolecule-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-12 13:44:49.000000 playmolecule-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:27:22.582073 playmolecule-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-13 08:27:04.000000 playmolecule-1.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 08:27:04.000000 playmolecule-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 08:27:22.582073 playmolecule-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 08:27:04.000000 playmolecule-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:27:22.578072 playmolecule-1.6.5/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32899 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 08:27:04.000000 playmolecule-1.6.5/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:27:22.578072 playmolecule-1.6.5/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 08:27:22.000000 playmolecule-1.6.5/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 08:27:22.000000 playmolecule-1.6.5/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:27:22.000000 playmolecule-1.6.5/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 08:27:22.000000 playmolecule-1.6.5/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 08:27:22.000000 playmolecule-1.6.5/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 08:27:04.000000 playmolecule-1.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:27:22.582073 playmolecule-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 08:27:04.000000 playmolecule-1.6.5/setup.py
```

### Comparing `playmolecule-1.6.4/LICENSE.md` & `playmolecule-1.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/PKG-INFO` & `playmolecule-1.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.4
+Version: 1.6.5
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.4/playmolecule/__init__.py` & `playmolecule-1.6.5/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/_test_funcs.py` & `playmolecule-1.6.5/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/config.py` & `playmolecule-1.6.5/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/datacenter.py` & `playmolecule-1.6.5/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/devutils.py` & `playmolecule-1.6.5/playmolecule/devutils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/func2argparse.py` & `playmolecule-1.6.5/playmolecule/func2argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,44 +177,46 @@
                 )
 
         if type(argtype) == tuple:
             raise RuntimeError(
                 f"Failed to get type annotation for argument '{argname}'"
             )
 
-        if nargs is None and argtype == bool:
-            if default:
-                raise RuntimeError(
-                    "func2argparse does not allow boolean flags with default value True"
+        if argtype == bool:
+            if nargs is None:
+                if default:
+                    raise RuntimeError(
+                        "func2argparse does not allow boolean flags with default value True"
+                    )
+                parser.add_argument(
+                    f"--{argname.replace('_', '-')}",
+                    f"-{abbrevs[argname]}",
+                    help=argdocs[argname]["doc"].strip(),
+                    action="store_true",
+                )
+            else:
+                parser.add_argument(
+                    f"--{argname.replace('_', '-')}",
+                    f"-{abbrevs[argname]}",
+                    help=argdocs[argname]["doc"].strip(),
+                    default=default,
+                    type=str_to_bool,
+                    required=params.default == inspect._empty,
+                    nargs=nargs,
                 )
-            parser.add_argument(
-                f"--{argname.replace('_', '-')}",
-                f"-{abbrevs[argname]}",
-                help=argdocs[argname]["doc"].strip(),
-                action="store_true",
-            )
-        elif nargs is not None and argtype == bool:
-            parser.add_argument(
-                f"--{argname.replace('_', '-')}",
-                f"-{abbrevs[argname]}",
-                help=argdocs[argname]["doc"].strip(),
-                default=default,
-                type=str_to_bool,
-                choices=argdocs[argname]["choices"],
-                required=params.default == inspect._empty,
-                nargs=nargs,
-            )
         else:
+            help = argdocs[argname]["doc"].strip()
+            choices = argdocs[argname]["choices"]
             parser.add_argument(
                 f"--{argname.replace('_', '-')}",
                 f"-{abbrevs[argname]}",
-                help=argdocs[argname]["doc"].strip(),
+                help=help,
                 default=default,
                 type=argtype,
-                choices=argdocs[argname]["choices"],
+                choices=choices,
                 required=params.default == inspect._empty,
                 nargs=nargs,
             )
 
     return parser
```

### Comparing `playmolecule-1.6.4/playmolecule/job.py` & `playmolecule-1.6.5/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/jsonlogger.py` & `playmolecule-1.6.5/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/local.py` & `playmolecule-1.6.5/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/playqueue.py` & `playmolecule-1.6.5/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule/session.py` & `playmolecule-1.6.5/playmolecule/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,53 +48,42 @@
 
 
 def _request_url(*args, **kwargs):
     return _requestURL(*args, **kwargs, _throwError=_throw_error)
 
 
 def _describe_app(python_obj, job=None):
-    columns = "{:<30} {:<20} {:<20} {:<30} {:<40}"
-    print(
-        columns.format(
-            "Name",
-            "Type",
-            "Mandatory",
-            "Value" if job else "Default",
-            "Description",
-        )
-    )
-
     nonprivparams = [param for param in python_obj["params"] if param["name"][0] != "_"]
     mandatoryparams = sorted(
         [param for param in nonprivparams if param["mandatory"]],
         key=lambda param: param["name"],
     )
     optionalparams = sorted(
         [param for param in nonprivparams if not param["mandatory"]],
         key=lambda param: param["name"],
     )
     printparams = mandatoryparams + optionalparams
 
+    print("Parameters\n----------")
     for param in printparams:
-        print(
-            columns.format(
-                param["name"],
-                param["type"],
-                "True" if param["mandatory"] else "False",
-                str(getattr(job, param["name"])) if job else param["value"],
-                param["description"],
-            )
-        )
-
-    if "periodicities" in python_obj and len(python_obj["periodicities"]):
-        columns = "{:<30} {:<20} {:<20}"
-        print(columns.format("Name", "param", "value"))
-        for p in python_obj["periodicities"]:
-            if p["name"][0] != "_":
-                print(columns.format(p["name"], p["param"], p["value"]))
+        atype = param["type"]
+        if atype == "str_to_bool":
+            atype = "bool"
+        if param["nargs"] is not None:
+            atype = f"list[{atype}]"
+        helpstr = f"{param['name']} : {atype}"
+        if param["mandatory"]:
+            helpstr += " [Required]"
+        choices = param["choices"]
+        if choices is not None:
+            choices = '", "'.join(choices)
+            helpstr += f', choices=("{choices}")'
+        print(helpstr)
+        descr = param["description"]
+        print("    " + descr)
 
 
 def _find_token(token):
     """Searches for the token file in the default locations and env vars"""
     if token is not None:
         return token
```

### Comparing `playmolecule-1.6.4/playmolecule/utils.py` & `playmolecule-1.6.5/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.6.5/playmolecule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.4
+Version: 1.6.5
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.4/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.6.5/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.4/setup.py` & `playmolecule-1.6.5/setup.py`

 * *Files identical despite different names*

