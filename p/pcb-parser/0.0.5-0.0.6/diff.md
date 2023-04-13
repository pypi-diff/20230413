# Comparing `tmp/pcb-parser-0.0.5.tar.gz` & `tmp/pcb-parser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcb-parser-0.0.5.tar", last modified: Mon Apr 10 04:59:56 2023, max compression
+gzip compressed data, was "pcb-parser-0.0.6.tar", last modified: Thu Apr 13 11:58:17 2023, max compression
```

## Comparing `pcb-parser-0.0.5.tar` & `pcb-parser-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-10 04:59:40.000000 pcb-parser-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.246246 pcb-parser-0.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.247246 pcb-parser-0.0.5/src/pcb_parser/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.5/src/pcb_parser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.5/src/pcb_parser/abs.py
--rwxr-xr-x   0 root         (0) root         (0)    29966 2023-04-10 04:54:03.000000 pcb-parser-0.0.5/src/pcb_parser/geometry.py
--rwxr-xr-x   0 root         (0) root         (0)     6848 2023-04-10 04:59:19.000000 pcb-parser-0.0.5/src/pcb_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-04 08:44:09.000000 pcb-parser-0.0.5/src/pcb_parser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 04:59:56.248246 pcb-parser-0.0.5/src/pcb_parser.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-10 04:59:56.000000 pcb-parser-0.0.5/src/pcb_parser.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.790560 pcb-parser-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-02-20 02:12:16.000000 pcb-parser-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-13 11:58:17.790560 pcb-parser-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-03 04:33:47.000000 pcb-parser-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 11:58:17.791560 pcb-parser-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      688 2023-04-13 11:57:51.000000 pcb-parser-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.784560 pcb-parser-0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.788560 pcb-parser-0.0.6/src/pcb_parser/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-02 23:43:20.000000 pcb-parser-0.0.6/src/pcb_parser/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      924 2023-03-30 05:32:08.000000 pcb-parser-0.0.6/src/pcb_parser/abs.py
+-rwxr-xr-x   0 root         (0) root         (0)    30748 2023-04-13 11:45:07.000000 pcb-parser-0.0.6/src/pcb_parser/geometry.py
+-rwxr-xr-x   0 root         (0) root         (0)     6914 2023-04-13 09:20:09.000000 pcb-parser-0.0.6/src/pcb_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-04-13 09:50:32.000000 pcb-parser-0.0.6/src/pcb_parser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:58:17.789560 pcb-parser-0.0.6/src/pcb_parser.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-13 11:58:17.000000 pcb-parser-0.0.6/src/pcb_parser.egg-info/top_level.txt
```

### Comparing `pcb-parser-0.0.5/LICENSE` & `pcb-parser-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.5/setup.py` & `pcb-parser-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
     
 setuptools.setup(
     name = 'pcb-parser',
-    version = 'v0.0.5',
+    version = 'v0.0.6',
     author = 'Changyun Choi',
     author_email = "cyun9601@gmail.com",
     description = "PCB Parser",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/cyun9601/PCB_Parser",
     package_dir={"": "src"},
```

### Comparing `pcb-parser-0.0.5/src/pcb_parser/abs.py` & `pcb-parser-0.0.6/src/pcb_parser/abs.py`

 * *Files identical despite different names*

### Comparing `pcb-parser-0.0.5/src/pcb_parser/geometry.py` & `pcb-parser-0.0.6/src/pcb_parser/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from matplotlib.patches import Rectangle as mpl_Rect
 from matplotlib.lines import Line2D
 from .abs import Object
 import math
 import numpy as np 
 from typing import Union  
 import cv2
-from .utils import floodfill, img_rot_90
+from .utils import floodfill, img_rot_90, img_folder
 import copy 
+import os 
+from PIL import Image
  
 class Point(Object):
     def __init__(self, x, y):
         self.x = x 
         self.y = y 
         
     def min_x(self):
@@ -616,75 +618,86 @@
             
     def switch_layer(self) -> None:
         self.placed_layer = 'TOP' if self.placed_layer == 'BOTTOM' else 'BOTTOM'
         self.top_area, self.bottom_area = self.bottom_area, self.top_area
         self.top_prohibit_area, self.bottom_prohibit_area = self.bottom_prohibit_area, self.top_prohibit_area
 
     def draw_cv(self, fill='in') -> tuple[np.array, np.array]:
-        # 기존에 그린게 있으면 해당 값을 반환
-        # if 'self.cv_top_img' in locals(): 
-        #     if (self.cv_resolution == resolution) & (self.cv_fill == fill):
-        #         return self.cv_top_img
-        # if 'self.cv_bottom_img' in locals(): 
-        #     if (self.cv_resolution == resolution) & (self.cv_fill == fill):
-        #         return self.cv_bottom_img
-        
-        total_area = self.top_area + self.bottom_area
-        
-        total_h = int(round(total_area.h / self.p_resolution, 0)) + 1
-        total_w = int(round(total_area.w / self.p_resolution, 0)) + 1
-        
-        # TOP
-        total_top_img = np.ones((total_h, total_w)) * 255
-        total_top_img = total_top_img.astype(np.uint8)
-
-        top_img = self.top_area.draw_cv(fill=fill)
+        img_path = os.path.join(img_folder, str(self.p_resolution), self.name)
+        top_img_path = os.path.join(img_path, 'top.png')
+        bottom_img_path = os.path.join(img_path, 'bottom.png')
         
-        if top_img is not None: 
+        if os.path.exists(top_img_path):
+            total_top_img = np.array(Image.open(top_img_path))
+        else:
+            total_area = self.top_area + self.bottom_area
             
-            ## Component의 원점 매핑 시 BBox 계산. 
-            top_moved_min_x = self.top_area.min_x - total_area.min_x
-            top_moved_max_x = self.top_area.max_x - total_area.min_x
-            top_moved_min_y = self.top_area.min_y - total_area.min_y 
-            top_moved_max_y = self.top_area.max_y - total_area.min_y 
+            total_h = int(round(total_area.h / self.p_resolution, 0)) + 1
+            total_w = int(round(total_area.w / self.p_resolution, 0)) + 1
             
-            ## Pixel 영역에서의 BBox 영역 매핑 
-            top_min_pix_h = total_h - 1 - int(round((top_moved_max_y / self.p_resolution), 0))
-            top_max_pix_h = total_h - 1 - int(round((top_moved_min_y / self.p_resolution), 0))
-            top_min_pix_w = int(round((top_moved_min_x / self.p_resolution), 0))
-            top_max_pix_w = int(round((top_moved_max_x / self.p_resolution), 0))
+            # TOP
+            total_top_img = np.ones((total_h, total_w)) * 255
+            total_top_img = total_top_img.astype(np.uint8)
+
+            top_img = self.top_area.draw_cv(fill=fill)
             
-            ## 이미지 삽입 
-            total_top_img[top_min_pix_h:top_min_pix_h+top_img.shape[0], top_min_pix_w:top_min_pix_w+top_img.shape[1]] = top_img 
-    
-        # BOTTOM
-        total_bottom_img = np.ones((total_h, total_w)) * 255
-        total_bottom_img = total_bottom_img.astype(np.uint8)
-        
-        bottom_img = self.bottom_area.draw_cv(fill=fill)
-        
-        if bottom_img is not None: 
-            ## Component의 원점 매핑 시 BBox 계산.
-            bottom_moved_min_x = self.bottom_area.min_x - total_area.min_x
-            bottom_moved_max_x = self.bottom_area.max_x - total_area.min_x
-            bottom_moved_min_y = self.bottom_area.min_y - total_area.min_y 
-            bottom_moved_max_y = self.bottom_area.max_y - total_area.min_y 
-        
-            ## Pixel 영역에서의 BBox 영역 매핑 
-            bottom_min_pix_h = total_h - 1 - int(round((bottom_moved_max_y / self.p_resolution), 0))
-            bottom_max_pix_h = total_h - 1 - int(round((bottom_moved_min_y / self.p_resolution), 0))
-            bottom_min_pix_w = int(round((bottom_moved_min_x / self.p_resolution), 0))
-            bottom_max_pix_w = int(round((bottom_moved_max_x / self.p_resolution), 0))
+            if top_img is not None: 
+                
+                ## Component의 원점 매핑 시 BBox 계산. 
+                top_moved_min_x = self.top_area.min_x - total_area.min_x
+                top_moved_max_x = self.top_area.max_x - total_area.min_x
+                top_moved_min_y = self.top_area.min_y - total_area.min_y 
+                top_moved_max_y = self.top_area.max_y - total_area.min_y 
+                
+                ## Pixel 영역에서의 BBox 영역 매핑 
+                top_min_pix_h = total_h - 1 - int(round((top_moved_max_y / self.p_resolution), 0))
+                top_max_pix_h = total_h - 1 - int(round((top_moved_min_y / self.p_resolution), 0))
+                top_min_pix_w = int(round((top_moved_min_x / self.p_resolution), 0))
+                top_max_pix_w = int(round((top_moved_max_x / self.p_resolution), 0))
+                
+                ## 이미지 삽입 
+                total_top_img[top_min_pix_h:top_min_pix_h+top_img.shape[0], top_min_pix_w:top_min_pix_w+top_img.shape[1]] = top_img 
+
+                im = Image.fromarray(total_top_img)
+                os.makedirs(img_path, exist_ok=True)
+                im.save(top_img_path)
+                
+        if os.path.exists(bottom_img_path):
+            total_bottom_img = np.array(Image.open(bottom_img_path))
+        else: 
+            total_area = self.top_area + self.bottom_area
             
-            ## 이미지 삽입 
-            total_bottom_img[bottom_min_pix_h:bottom_min_pix_h + bottom_img.shape[0], bottom_min_pix_w:bottom_min_pix_w + bottom_img.shape[1]] = bottom_img 
+            total_h = int(round(total_area.h / self.p_resolution, 0)) + 1
+            total_w = int(round(total_area.w / self.p_resolution, 0)) + 1
+            
+            # BOTTOM
+            total_bottom_img = np.ones((total_h, total_w)) * 255
+            total_bottom_img = total_bottom_img.astype(np.uint8)
+            
+            bottom_img = self.bottom_area.draw_cv(fill=fill)
+            
+            if bottom_img is not None: 
+                ## Component의 원점 매핑 시 BBox 계산.
+                bottom_moved_min_x = self.bottom_area.min_x - total_area.min_x
+                bottom_moved_max_x = self.bottom_area.max_x - total_area.min_x
+                bottom_moved_min_y = self.bottom_area.min_y - total_area.min_y 
+                bottom_moved_max_y = self.bottom_area.max_y - total_area.min_y 
+            
+                ## Pixel 영역에서의 BBox 영역 매핑 
+                bottom_min_pix_h = total_h - 1 - int(round((bottom_moved_max_y / self.p_resolution), 0))
+                bottom_max_pix_h = total_h - 1 - int(round((bottom_moved_min_y / self.p_resolution), 0))
+                bottom_min_pix_w = int(round((bottom_moved_min_x / self.p_resolution), 0))
+                bottom_max_pix_w = int(round((bottom_moved_max_x / self.p_resolution), 0))
+                
+                ## 이미지 삽입 
+                total_bottom_img[bottom_min_pix_h:bottom_min_pix_h + bottom_img.shape[0], bottom_min_pix_w:bottom_min_pix_w + bottom_img.shape[1]] = bottom_img 
 
-        self.cv_top_img = total_top_img    
-        self.cv_bottom_img = total_bottom_img   
-        
+            self.cv_top_img = total_top_img    
+            self.cv_bottom_img = total_bottom_img   
+            
         return self.cv_top_img, self.cv_bottom_img     
         
     def draw_mat(self, ax, layer, shift_x=0, shift_y=0, color='k'): 
         if layer == 'TOP':
             self.top_area.draw_mat(ax, shift_x=shift_x, shift_y=shift_y, color=color)
         elif layer == 'BOTTOM':
             self.bottom_area.draw_mat(ax, shift_x=shift_x, shift_y=shift_y, color=color)
@@ -773,21 +786,23 @@
             self.bottom_area.rotation(angle, self.center, inplace=True)
             self.hole_area.rotation(angle, self.center, inplace=True)
             self.top_prohibit_area.rotation(angle, self.center, inplace=True)
             self.bottom_prohibit_area.rotation(angle, self.center, inplace=True) 
             
             # 이미지 회전
             k = angle // 90
-            self.cv_top_img = img_rot_90(self.cv_top_img, k)
-            self.cv_bottom_img = img_rot_90(self.cv_bottom_img, k)
+            
+            if 'cv_top_img' in dir(self):
+                self.cv_top_img = img_rot_90(self.cv_top_img, k)
+            if 'cv_bottom_img' in dir(self):
+                self.cv_bottom_img = img_rot_90(self.cv_bottom_img, k)
             return self
         else:
             new_comp = copy.deepcopy(self)
             return new_comp.rotation(angle, inplace=True)
-        
 
 def merge_polygon(base_img:np.array, background:Polygon, foreground:Polygon, resolution = 0.05, inplace = False) -> np.array:
     if inplace == False:
         base_img = copy.deepcopy(base_img)
     
     back_pix_h = int(round(background.h / resolution, 0)) + 1
     back_pix_w = int(round(background.w / resolution, 0)) + 1
```

### Comparing `pcb-parser-0.0.5/src/pcb_parser/parser.py` & `pcb-parser-0.0.6/src/pcb_parser/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,33 +21,33 @@
         self.board = Polygon(self.pcb_info['BOARD_FIGURE'], p_resolution)
         self.hole_area = Polygon(self.pcb_info['HoleArea'], p_resolution)
         self.prohibit_area = Polygon(self.pcb_info['ProhibitArea'], p_resolution)
         self.components_dict = {comp_info['Name']:Component(comp_info, p_resolution) for comp_info in self.pcb_info['ComponentDict'].values()}
         self.net_list = dict(zip(self.pcb_info['NetDict'].keys(), [Net(net_info) for net_info in list(self.pcb_info['NetDict'].values())]))
         
         # 초기화
-        ## 초기 이미지 생성  
+        ## 초기 Comp 이미지 생성  
         self.initialize_cv_img()
         
         ## Background 초기화 -> self.state 생성  
         self.initialize_background()
         
-        ## Component 초기화 
-        self.initialize_components()
-    
     def initialize_cv_img(self):
         # initialize
         print('Board 이미지 생성 중...')
         self.board.draw_cv()
         self.hole_area.draw_cv()
         self.prohibit_area.draw_cv()         
         print('Component 이미지 생성 중...')
         pbar = tqdm(self.components_dict.values())
         for comp in pbar:
             pbar.set_description(comp.name)
+            
+            print(comp.placed_layer, comp.angle, len(comp.top_area), len(comp.bottom_area))
+            # if './comp_img'
             comp.draw_cv()
     
     def initialize_background(self):
         board_cv_img = self.board.draw_cv(fill='out')
 
         merged_img, collision = self.merge_polygon(board_cv_img, self.board, self.hole_area, inplace=False)
         self.state = [copy.deepcopy(merged_img), copy.deepcopy(merged_img)]
```

### Comparing `pcb-parser-0.0.5/src/pcb_parser/utils.py` & `pcb-parser-0.0.6/src/pcb_parser/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import cv2
 import numpy as np 
 import copy 
+import os 
+
+img_folder = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'comp_img')
 
 
 def img_rot_90(img, k):
     return np.rot90(img, k=k)
 
 def floodfill(img:np.array, fill_area = 'in', fill_val = 100):
     ret, img = cv2.threshold(img, 127, 255, cv2.THRESH_BINARY)
```

