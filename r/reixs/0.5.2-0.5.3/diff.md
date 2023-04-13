# Comparing `tmp/reixs-0.5.2.tar.gz` & `tmp/reixs-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.5.2.tar", last modified: Fri Jan 27 17:30:22 2023, max compression
+gzip compressed data, was "reixs-0.5.3.tar", last modified: Thu Apr 13 17:51:43 2023, max compression
```

## Comparing `reixs-0.5.2.tar` & `reixs-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:30:22.969780 reixs-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-27 17:30:10.000000 reixs-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-01-27 17:30:22.969780 reixs-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-01-27 17:30:10.000000 reixs-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-27 17:30:10.000000 reixs-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-27 17:30:22.973780 reixs-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:30:22.965780 reixs-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:30:22.969780 reixs-0.5.2/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    53721 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-01-27 17:30:10.000000 reixs-0.5.2/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 17:30:22.969780 reixs-0.5.2/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-01-27 17:30:22.000000 reixs-0.5.2/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-27 17:30:22.000000 reixs-0.5.2/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 17:30:22.000000 reixs-0.5.2/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-27 17:30:22.000000 reixs-0.5.2/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 17:30:22.000000 reixs-0.5.2/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.327485 reixs-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-13 17:51:26.000000 reixs-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 17:51:43.327485 reixs-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-13 17:51:26.000000 reixs-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 17:51:26.000000 reixs-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-13 17:51:43.331485 reixs-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.323485 reixs-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.327485 reixs-0.5.3/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    53721 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-13 17:51:26.000000 reixs-0.5.3/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:43.327485 reixs-0.5.3/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 17:51:43.000000 reixs-0.5.3/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.5.2/LICENSE` & `reixs-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/PKG-INFO` & `reixs-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.2
+Version: 0.5.3
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.2/README.md` & `reixs-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/setup.cfg` & `reixs-0.5.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.5.2
+version = 0.5.3
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.5.2/src/reixs/LoadData.py` & `reixs-0.5.3/src/reixs/LoadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/ReadData.py` & `reixs-0.5.3/src/reixs/ReadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/add_subtract.py` & `reixs-0.5.3/src/reixs/add_subtract.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/mca.py` & `reixs-0.5.3/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/mesh.py` & `reixs-0.5.3/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/parser.py` & `reixs-0.5.3/src/reixs/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-import parser
 from .util import doesMatchPattern
 from numpy import log as ln
 from numpy import log10 as log
 from numpy import exp
 from numpy import max, min
 
 
@@ -20,27 +19,29 @@
     # drop all empty strings from re.split
     quantity_str_dict = dict()
 
     # Check all stripped strings individually and evaluate
     for i, string in enumerate(split_expr):
         if string != "":
             try:
-                float(string) # Check if string is float
+                float(string)  # Check if string is float
             except:
                 # Use math expressions to allow logs and exps
-                math_expressions = ['ln', 'log', 'exp','max','min']
+                math_expressions = ['ln', 'log', 'exp', 'max', 'min']
 
                 if string in math_expressions:
                     pass
 
                 else:
                     # Need to allow special case where negative numbers can be assigned in ET scan
-                    if string.endswith("ET["): # This will only be triggered if the arguments of [] are negative, otherwise the string will not be split
-                        string += '-' + split_expr[i+1] # Add the negative sign back in and add to current scan descriptor
-                        del split_expr[i+1] # Drop the extra element
+                    # This will only be triggered if the arguments of [] are negative, otherwise the string will not be split
+                    if string.endswith("ET["):
+                        # Add the negative sign back in and add to current scan descriptor
+                        string += '-' + split_expr[i+1]
+                        del split_expr[i+1]  # Drop the extra element
 
                     # Assign generic "val{i}" key to string literal in compliance with
                     # python supported syntax for variables
                     quantity_str_dict[f"val{i}"] = string
 
     # Parser does not support special string literals (ROIs) due to inproper python variable naming syntax
     # Replace them with generic key as per dictionary
@@ -66,9 +67,8 @@
                 locals()[k] = get_data(v, data, arg, background, REIXSObj)
             else:
                 numerator = get_data(v, data, arg, background, REIXSObj)
                 mesh = data[arg].mesh_current
                 locals()[k] = numerator/mesh
 
     # Return the calculated result
-    code = parser.expr(formula).compile()
-    return eval(code)
+    return eval(formula)
```

### Comparing `reixs-0.5.2/src/reixs/rixs_readutil.py` & `reixs-0.5.3/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/rsxs_mcp.py` & `reixs-0.5.3/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/rsxs_readutil.py` & `reixs-0.5.3/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/sca.py` & `reixs-0.5.3/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/simplemath.py` & `reixs-0.5.3/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/spec_config.py` & `reixs-0.5.3/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/util.py` & `reixs-0.5.3/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs/xeol.py` & `reixs-0.5.3/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.5.2/src/reixs.egg-info/PKG-INFO` & `reixs-0.5.3/src/reixs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.5.2
+Version: 0.5.3
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.5.2/src/reixs.egg-info/SOURCES.txt` & `reixs-0.5.3/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

