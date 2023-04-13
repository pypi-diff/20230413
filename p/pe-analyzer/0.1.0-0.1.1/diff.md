# Comparing `tmp/pe_analyzer-0.1.0.tar.gz` & `tmp/pe_analyzer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe_analyzer-0.1.0.tar", max compression
+gzip compressed data, was "pe_analyzer-0.1.1.tar", max compression
```

## Comparing `pe_analyzer-0.1.0.tar` & `pe_analyzer-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       35 2023-04-13 03:49:51.301406 pe_analyzer-0.1.0/pe_analyzer/__init__.py
--rw-r--r--   0        0        0     4904 2023-04-13 04:48:19.073194 pe_analyzer-0.1.0/pe_analyzer/pe_analyzer.py
--rw-r--r--   0        0        0      916 2023-04-13 05:14:12.592949 pe_analyzer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1244 2023-04-13 04:22:07.270312 pe_analyzer-0.1.0/README.md
--rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 pe_analyzer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2023-04-13 03:49:51.301406 pe_analyzer-0.1.1/pe_analyzer/__init__.py
+-rw-r--r--   0        0        0     4899 2023-04-13 05:36:16.328086 pe_analyzer-0.1.1/pe_analyzer/pe_analyzer.py
+-rw-r--r--   0        0        0      916 2023-04-13 05:37:53.890421 pe_analyzer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1244 2023-04-13 04:22:07.270312 pe_analyzer-0.1.1/README.md
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 pe_analyzer-0.1.1/PKG-INFO
```

### Comparing `pe_analyzer-0.1.0/pe_analyzer/pe_analyzer.py` & `pe_analyzer-0.1.1/pe_analyzer/pe_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import sys
 import os
 
 
 class PEAnalyzer:
     def __init__(self, file_path):
-        self.file_path = self.file_path.replace('\\', '/')
+        self.file_path = file_path.replace('\\', '/')
         if not os.path.isfile(self.file_path):
             raise ValueError("Couldn't find the target file")
         else:
             self.pe = pefile.PE(file_path)
 
     def analyze(self):
         analysis = {
```

### Comparing `pe_analyzer-0.1.0/pyproject.toml` & `pe_analyzer-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pe-analyzer"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python module to analyze Portable Executable (PE) files on Windows systems. It parses and extracts various details about the file header, optional header, sections, imports, and exports. The module provides an easy-to-use class, PEAnalyzer, which returns analysis data in JSON format and supports pretty-printing of the information when used with the print() function."
 authors = [
 	"DJ Stomp <85457381+DJStompZone@users.noreply.github.com>",
 ]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pe_analyzer"}]
```

### Comparing `pe_analyzer-0.1.0/README.md` & `pe_analyzer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pe_analyzer-0.1.0/PKG-INFO` & `pe_analyzer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-analyzer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python module to analyze Portable Executable (PE) files on Windows systems. It parses and extracts various details about the file header, optional header, sections, imports, and exports. The module provides an easy-to-use class, PEAnalyzer, which returns analysis data in JSON format and supports pretty-printing of the information when used with the print() function.
 License: MIT
 Author: DJ Stomp
 Author-email: 85457381+DJStompZone@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

