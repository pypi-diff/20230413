# Comparing `tmp/py3dchart-0.2.1.tar.gz` & `tmp/py3dchart-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dchart-0.2.1.tar", last modified: Thu Apr 13 14:22:41 2023, max compression
+gzip compressed data, was "py3dchart-0.2.2.tar", last modified: Thu Apr 13 14:49:40 2023, max compression
```

## Comparing `py3dchart-0.2.1.tar` & `py3dchart-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:22:41.717187 py3dchart-0.2.1/
--rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      692 2023-04-13 14:22:41.716187 py3dchart-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 14:22:41.699185 py3dchart-0.2.1/py3dchart/
--rw-rw-rw-   0        0        0       60 2023-04-13 13:56:09.000000 py3dchart-0.2.1/py3dchart/__init__.py
--rw-rw-rw-   0        0        0     3031 2023-04-13 14:22:13.000000 py3dchart-0.2.1/py3dchart/chart.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:22:41.713191 py3dchart-0.2.1/py3dchart.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 14:22:41.000000 py3dchart-0.2.1/py3dchart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 14:22:41.718194 py3dchart-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     3927 2023-04-13 14:22:20.000000 py3dchart-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:49:40.470720 py3dchart-0.2.2/
+-rw-rw-rw-   0        0        0     1100 2023-04-13 03:12:28.000000 py3dchart-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      692 2023-04-13 14:49:40.468721 py3dchart-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 03:12:28.000000 py3dchart-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:49:40.448723 py3dchart-0.2.2/py3dchart/
+-rw-rw-rw-   0        0        0       60 2023-04-13 13:56:09.000000 py3dchart-0.2.2/py3dchart/__init__.py
+-rw-rw-rw-   0        0        0     2999 2023-04-13 14:49:11.000000 py3dchart-0.2.2/py3dchart/chart.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:49:40.466748 py3dchart-0.2.2/py3dchart.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-04-13 14:49:40.000000 py3dchart-0.2.2/py3dchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-13 14:49:40.000000 py3dchart-0.2.2/py3dchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:49:40.000000 py3dchart-0.2.2/py3dchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 14:49:40.000000 py3dchart-0.2.2/py3dchart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:49:40.470720 py3dchart-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     3927 2023-04-13 14:49:19.000000 py3dchart-0.2.2/setup.py
```

### Comparing `py3dchart-0.2.1/LICENSE` & `py3dchart-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dchart-0.2.1/PKG-INFO` & `py3dchart-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.2.1/py3dchart/chart.py` & `py3dchart-0.2.2/py3dchart/chart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 from tkinter import *
 import numpy
 import math
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__ = 'WangLvyuan'
 
 class chart3d:
-    fontSize = 12
-    x1 = 20
-    y1 = 20
-    x2 = 220
-    y2 = 220
+    
+    fontSize1 = 12
+    xx1 = 20
+    yy1 = 20
+    xx2 = 220
+    yy2 = 220
 
     def fontSize(self, num):
-         chart3d.fontSize = num
+         chart3d.fontSize1 = num
          return
 
     def x1(self, num):
-         chart3d.x1 = num
+         chart3d.xx1 = num
          return
     
     def x2(self, num):
-         chart3d.x2 = num
+         chart3d.xx2 = num
          return
     
     def y1(self, num):
-         chart3d.y1 = num
+         chart3d.yy1 = num
          return
     
     def y2(self, num):
-         chart3d.y2 = num
+         chart3d.yy2 = num
          return
 
-    def pieData(data2):
-        rate = []
-        s = sum(data2)
-        for x in data2:
-            rate.append('{:.4f}'.format(x/s))
-        rate = numpy.array(rate, dtype = numpy.float64)
-        return rate
-    
-    def locationCal(degree):
-        rad = math.radians(degree)
-        xLocation1 = round(round(math.cos(-rad),2) * (chart3d.x2-chart3d.x1)/4 + (chart3d.x2+chart3d.x1)/2)
-        yLocation1 = round(round(math.sin(-rad),2) * (chart3d.x2-chart3d.x1)/4 + (chart3d.y2+chart3d.y1)/2)
-        xLocation2 = round(round(math.cos(-rad),2) * (chart3d.x2-chart3d.x1)/2-10 + (chart3d.x2+chart3d.x1)/2)
-        yLocation2 = round(round(math.sin(-rad),2) * (chart3d.x2-chart3d.x1)/2-10 + (chart3d.y2+chart3d.y1)/2)
-        return [xLocation1, yLocation1, xLocation2, yLocation2]
-    
-    # the pie apart
+# the pie apart
     def drawPie(self, pie_data_as_array, pie_lable_as_llist):
         rate = chart3d.pieData(pie_data_as_array)
         root = Tk()
-        coord = chart3d.x1, chart3d.y1, chart3d.x2, chart3d.y2
-        shadow = chart3d.x1 + 10, chart3d.y1 + 10, chart3d.x2 + 10, chart3d.y2 + 10
-        center = chart3d.x1 + 80, chart3d.y1 + 80, chart3d.x2 - 80, chart3d.y2 - 80
-        centerShadow = chart3d.x1 + 90, chart3d.y1 + 90, chart3d.x2 - 70, chart3d.y2 - 70
+        coord = chart3d.xx1, chart3d.yy1, chart3d.xx2, chart3d.yy2
+        shadow = chart3d.xx1 + 10, chart3d.yy1 + 10, chart3d.xx2 + 10, chart3d.yy2 + 10
+        center = chart3d.xx1 + 80, chart3d.yy1 + 80, chart3d.xx2 - 80, chart3d.yy2 - 80
+        centerShadow = chart3d.xx1 + 90, chart3d.yy1 + 90, chart3d.xx2 - 70, chart3d.yy2 - 70
         cv = Canvas(root, bg='white')
         cv.pack(fill = 'both',expand ='yes')
     
         # the 3D shadow, will not move
         cv.create_oval(shadow, fill="white")
 
         #generate pie
         startPoint: float = 0
         for x,y in zip(rate, pie_lable_as_llist):
             degree: float = float('{:.2f}'.format(x*360))
             print(chart3d.locationCal(startPoint + degree/2)) 
             location = chart3d.locationCal(startPoint + degree/2)#data type: int in list
             cv.create_arc(coord, start=startPoint, extent=degree, fill="white")
             cv.create_text(location[0], location[1], text=str(round((x*100),1)) + '%')
-            cv.create_text(location[2], location[3], text=y, font=("Arial", chart3d.fontSize))
+            cv.create_text(location[2], location[3], text=y, font=("Arial", chart3d.fontSize1))
             location = []
             startPoint += degree
     
         #generate center hole
         cv.create_oval(center, fill="white")
         cv.create_arc(centerShadow, style="arc", start=71, extent=135)
-    
-        #generate label
-        # for x in label:
-             
 
         cv.pack()
         root.mainloop()
 
+    def pieData(data2):
+        rate = []
+        s = sum(data2)
+        for x in data2:
+            rate.append('{:.4f}'.format(x/s))
+        rate = numpy.array(rate, dtype = numpy.float64)
+        return rate
+    
+    def locationCal(degree):
+        rad = math.radians(degree)
+        xLocation1 = round(round(math.cos(-rad),2) * (chart3d.xx2-chart3d.xx1)/4 + (chart3d.xx2+chart3d.xx1)/2)
+        yLocation1 = round(round(math.sin(-rad),2) * (chart3d.xx2-chart3d.xx1)/4 + (chart3d.yy2+chart3d.yy1)/2)
+        xLocation2 = round(round(math.cos(-rad),2) * (chart3d.xx2-chart3d.xx1)/2-10 + (chart3d.xx2+chart3d.xx1)/2)
+        yLocation2 = round(round(math.sin(-rad),2) * (chart3d.xx2-chart3d.xx1)/2-10 + (chart3d.yy2+chart3d.yy1)/2)
+        return [xLocation1, yLocation1, xLocation2, yLocation2]
+
 def main():
      print('test main')
 		
 if __name__ == '__main__':
 	main()
```

### Comparing `py3dchart-0.2.1/py3dchart.egg-info/PKG-INFO` & `py3dchart-0.2.2/py3dchart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3dchart
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple tool for my classmate to finish their classwork
 Home-page: https://github.com/Niggoss/Wang-Lvyuan.git
 Author: Wang Lvyuan
 Author-email: lvyuanw@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `py3dchart-0.2.1/setup.py` & `py3dchart-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'py3dchart'
 DESCRIPTION = 'A simple tool for my classmate to finish their classwork'
 URL = 'https://github.com/Niggoss/Wang-Lvyuan.git'
 EMAIL = 'lvyuanw@gmail.com'
 AUTHOR = 'Wang Lvyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
   # 'tkinter', 'numpy'
 ]
 
 # What packages are optional?
```

