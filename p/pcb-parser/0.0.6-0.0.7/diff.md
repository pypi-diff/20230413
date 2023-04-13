# Comparing `tmp/pcb-parser-0.0.6.tar.gz` & `tmp/pcb-parser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcb-parser-0.0.6.tar", last modified: Thu Apr 13 11:58:17 2023, max compression
+gzip compressed data, was "pcb-parser-0.0.7.tar", last modified: Thu Apr 13 12:32:20 2023, max compression
```

## Comparing `pcb-parser-0.0.6.tar` & `pcb-parser-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.790560 pcb-parser-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-13 11:58:17.790560 pcb-parser-0.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 11:58:17.791560 pcb-parser-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-13 11:57:51.000000 pcb-parser-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.784560 pcb-parser-0.0.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.788560 pcb-parser-0.0.6/src/pcb_parser/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.6/src/pcb_parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.6/src/pcb_parser/abs.py
--rwxr-xr-x   0 root         (0) root         (0)    30748 2023-04-13 11:45:07.000000 pcb-parser-0.0.6/src/pcb_parser/geometry.py
--rwxr-xr-x   0 root         (0) root         (0)     6914 2023-04-13 09:20:09.000000 pcb-parser-0.0.6/src/pcb_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 09:50:32.000000 pcb-parser-0.0.6/src/pcb_parser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.789560 pcb-parser-0.0.6/src/pcb_parser.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-13 12:31:54.000000 pcb-parser-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.404513 pcb-parser-0.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.405514 pcb-parser-0.0.7/src/pcb_parser/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.7/src/pcb_parser/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.7/src/pcb_parser/abs.py
+-rwxr-xr-x   0 root         (0) root         (0)    30746 2023-04-13 12:31:21.000000 pcb-parser-0.0.7/src/pcb_parser/geometry.py
+-rwxr-xr-x   0 root         (0) root         (0)     6914 2023-04-13 09:20:09.000000 pcb-parser-0.0.7/src/pcb_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 09:50:32.000000 pcb-parser-0.0.7/src/pcb_parser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/src/pcb_parser.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/top_level.txt
```

### Comparing `pcb-parser-0.0.6/LICENSE` & `pcb-parser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.6/setup.py` & `pcb-parser-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
     
 setuptools.setup(
     name = 'pcb-parser',
-    version = 'v0.0.6',
+    version = 'v0.0.7',
     author = 'Changyun Choi',
     author_email = "cyun9601@gmail.com",
     description = "PCB Parser",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/cyun9601/PCB_Parser",
     package_dir={"": "src"},
```

### Comparing `pcb-parser-0.0.6/src/pcb_parser/abs.py` & `pcb-parser-0.0.7/src/pcb_parser/abs.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.6/src/pcb_parser/geometry.py` & `pcb-parser-0.0.7/src/pcb_parser/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,15 @@
             self.group = data['Group']
         else:
             NotImplementedError
 
         self.p_resolution = p_resolution
 
         # Component 초기화 
-        # self.initialize()
+        self.initialize()
         
     def initialize(self) -> None:
         # unfixed component 에 대한 처리
         if self.fixed == False: 
             ## placed layer에 따라 스위칭
             if self.placed_layer == 'BOTTOM': 
                 self.switch_layer()
```

### Comparing `pcb-parser-0.0.6/src/pcb_parser/parser.py` & `pcb-parser-0.0.7/src/pcb_parser/parser.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.6/src/pcb_parser/utils.py` & `pcb-parser-0.0.7/src/pcb_parser/utils.py`

 * *Files identical despite different names*

