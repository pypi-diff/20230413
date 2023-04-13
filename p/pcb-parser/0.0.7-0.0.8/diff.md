# Comparing `tmp/pcb-parser-0.0.7.tar.gz` & `tmp/pcb-parser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcb-parser-0.0.7.tar", last modified: Thu Apr 13 12:32:20 2023, max compression
+gzip compressed data, was "pcb-parser-0.0.8.tar", last modified: Thu Apr 13 13:57:32 2023, max compression
```

## Comparing `pcb-parser-0.0.7.tar` & `pcb-parser-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-13 12:31:54.000000 pcb-parser-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.404513 pcb-parser-0.0.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.405514 pcb-parser-0.0.7/src/pcb_parser/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.7/src/pcb_parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.7/src/pcb_parser/abs.py
--rwxr-xr-x   0 root         (0) root         (0)    30746 2023-04-13 12:31:21.000000 pcb-parser-0.0.7/src/pcb_parser/geometry.py
--rwxr-xr-x   0 root         (0) root         (0)     6914 2023-04-13 09:20:09.000000 pcb-parser-0.0.7/src/pcb_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 09:50:32.000000 pcb-parser-0.0.7/src/pcb_parser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:32:20.406514 pcb-parser-0.0.7/src/pcb_parser.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-13 12:32:20.000000 pcb-parser-0.0.7/src/pcb_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 13:57:32.480419 pcb-parser-0.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-13 13:56:58.000000 pcb-parser-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.478419 pcb-parser-0.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/src/pcb_parser/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.8/src/pcb_parser/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.8/src/pcb_parser/abs.py
+-rwxr-xr-x   0 root         (0) root         (0)    30746 2023-04-13 13:56:15.000000 pcb-parser-0.0.8/src/pcb_parser/geometry.py
+-rwxr-xr-x   0 root         (0) root         (0)     6779 2023-04-13 13:56:01.000000 pcb-parser-0.0.8/src/pcb_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 13:56:14.000000 pcb-parser-0.0.8/src/pcb_parser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 13:57:32.479419 pcb-parser-0.0.8/src/pcb_parser.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-13 13:57:32.000000 pcb-parser-0.0.8/src/pcb_parser.egg-info/top_level.txt
```

### Comparing `pcb-parser-0.0.7/LICENSE` & `pcb-parser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.7/setup.py` & `pcb-parser-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
     
 setuptools.setup(
     name = 'pcb-parser',
-    version = 'v0.0.7',
+    version = 'v0.0.8',
     author = 'Changyun Choi',
     author_email = "cyun9601@gmail.com",
     description = "PCB Parser",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/cyun9601/PCB_Parser",
     package_dir={"": "src"},
```

### Comparing `pcb-parser-0.0.7/src/pcb_parser/abs.py` & `pcb-parser-0.0.8/src/pcb_parser/abs.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.7/src/pcb_parser/geometry.py` & `pcb-parser-0.0.8/src/pcb_parser/geometry.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.7/src/pcb_parser/parser.py` & `pcb-parser-0.0.8/src/pcb_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,14 @@
         self.board.draw_cv()
         self.hole_area.draw_cv()
         self.prohibit_area.draw_cv()         
         print('Component 이미지 생성 중...')
         pbar = tqdm(self.components_dict.values())
         for comp in pbar:
             pbar.set_description(comp.name)
-            
-            print(comp.placed_layer, comp.angle, len(comp.top_area), len(comp.bottom_area))
-            # if './comp_img'
             comp.draw_cv()
     
     def initialize_background(self):
         board_cv_img = self.board.draw_cv(fill='out')
 
         merged_img, collision = self.merge_polygon(board_cv_img, self.board, self.hole_area, inplace=False)
         self.state = [copy.deepcopy(merged_img), copy.deepcopy(merged_img)]
```

### Comparing `pcb-parser-0.0.7/src/pcb_parser/utils.py` & `pcb-parser-0.0.8/src/pcb_parser/utils.py`

 * *Files identical despite different names*

