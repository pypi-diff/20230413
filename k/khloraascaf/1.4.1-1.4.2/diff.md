# Comparing `tmp/khloraascaf-1.4.1.tar.gz` & `tmp/khloraascaf-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.4.1.tar", last modified: Wed Apr 12 09:22:50 2023, max compression
+gzip compressed data, was "khloraascaf-1.4.2.tar", last modified: Thu Apr 13 09:12:49 2023, max compression
```

## Comparing `khloraascaf-1.4.1.tar` & `khloraascaf-1.4.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.244232 khloraascaf-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)    45979 2023-04-12 09:22:50.244232 khloraascaf-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4599 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 09:22:50.244232 khloraascaf-1.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.226231 khloraascaf-1.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.235231 khloraascaf-1.4.1/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    12407 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5164 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.241232 khloraascaf-1.4.1/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10970 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8303 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    27131 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)     9071 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    20366 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7104 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.237232 khloraascaf-1.4.1/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45979 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 09:22:50.000000 khloraascaf-1.4.1/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:22:50.243232 khloraascaf-1.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13426 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    22646 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-12 09:22:24.000000 khloraascaf-1.4.1/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:12:49.754257 khloraascaf-1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    45979 2023-04-13 09:12:49.752425 khloraascaf-1.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4599 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:12:49.754257 khloraascaf-1.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:12:49.738678 khloraascaf-1.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:12:49.746010 khloraascaf-1.4.2/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12407 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5164 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:12:49.750592 khloraascaf-1.4.2/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10970 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8303 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    22345 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)     9071 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    20366 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7104 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:12:49.747842 khloraascaf-1.4.2/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45979 2023-04-13 09:12:49.000000 khloraascaf-1.4.2/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-13 09:12:49.000000 khloraascaf-1.4.2/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:12:49.000000 khloraascaf-1.4.2/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-13 09:12:49.000000 khloraascaf-1.4.2/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 09:12:49.000000 khloraascaf-1.4.2/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:12:49.752425 khloraascaf-1.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13426 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    22646 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-13 09:12:26.000000 khloraascaf-1.4.2/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.4.1/LICENCE` & `khloraascaf-1.4.2/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/PKG-INFO` & `khloraascaf-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.4.1
+Version: 1.4.2
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf-1.4.1/README.md` & `khloraascaf-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/pyproject.toml` & `khloraascaf-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.4.1"
+version = "1.4.2"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf-1.4.1/src/khloraascaf/__init__.py` & `khloraascaf-1.4.2/src/khloraascaf/__init__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/__main__.py` & `khloraascaf-1.4.2/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.4.2/src/khloraascaf/assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/cli.py` & `khloraascaf-1.4.2/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/exceptions.py` & `khloraascaf-1.4.2/src/khloraascaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/dirf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.4.2/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/inputs.py` & `khloraascaf-1.4.2/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/lib.py` & `khloraascaf-1.4.2/src/khloraascaf/lib.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.4.2/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/outputs.py` & `khloraascaf-1.4.2/src/khloraascaf/outputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/run_metadata.py` & `khloraascaf-1.4.2/src/khloraascaf/run_metadata.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.4.2/src/khloraascaf/scaffolding_methods.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf/utils_debug.py` & `khloraascaf-1.4.2/src/khloraascaf/utils_debug.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.4.2/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.4.1
+Version: 1.4.2
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `khloraascaf-1.4.1/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.4.2/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/tests/test_assembly_graph.py` & `khloraascaf-1.4.2/tests/test_assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/tests/test_exceptions.py` & `khloraascaf-1.4.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/tests/test_toy_examples.py` & `khloraascaf-1.4.2/tests/test_toy_examples.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.4.1/tests/test_utils_debug.py` & `khloraascaf-1.4.2/tests/test_utils_debug.py`

 * *Files identical despite different names*

