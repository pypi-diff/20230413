# Comparing `tmp/admath1-0.0.2.tar.gz` & `tmp/admath1-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admath1-0.0.2.tar", last modified: Thu Apr 13 18:42:05 2023, max compression
+gzip compressed data, was "admath1-0.0.3.tar", last modified: Thu Apr 13 19:27:26 2023, max compression
```

## Comparing `admath1-0.0.2.tar` & `admath1-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:42:05.723292 admath1-0.0.2/
--rw-rw-rw-   0        0        0     1099 2023-04-12 19:44:25.000000 admath1-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1802 2023-04-13 18:42:05.723292 admath1-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-04-12 19:43:18.000000 admath1-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 18:42:05.718793 admath1-0.0.2/admath1/
--rw-rw-rw-   0        0        0      870 2023-04-13 18:17:23.000000 admath1-0.0.2/admath1/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-04-13 12:00:07.000000 admath1-0.0.2/admath1/area.py
--rw-rw-rw-   0        0        0     2158 2023-04-13 12:46:53.000000 admath1-0.0.2/admath1/parameter.py
--rw-rw-rw-   0        0        0      693 2023-04-13 07:55:38.000000 admath1-0.0.2/admath1/trignometry.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:42:05.722279 admath1-0.0.2/admath1.egg-info/
--rw-rw-rw-   0        0        0     1802 2023-04-13 18:42:05.000000 admath1-0.0.2/admath1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-13 18:42:05.000000 admath1-0.0.2/admath1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:42:05.000000 admath1-0.0.2/admath1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 18:42:05.000000 admath1-0.0.2/admath1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 18:42:05.723292 admath1-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-04-13 18:41:47.000000 admath1-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:26.647560 admath1-0.0.3/
+-rw-rw-rw-   0        0        0     1099 2023-04-12 19:44:25.000000 admath1-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1802 2023-04-13 19:27:26.647315 admath1-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-04-12 19:43:18.000000 admath1-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:26.643397 admath1-0.0.3/admath1/
+-rw-rw-rw-   0        0        0      145 2023-04-13 19:09:22.000000 admath1-0.0.3/admath1/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-04-13 12:00:07.000000 admath1-0.0.3/admath1/area.py
+-rw-rw-rw-   0        0        0     2194 2023-04-13 19:16:49.000000 admath1-0.0.3/admath1/parameter.py
+-rw-rw-rw-   0        0        0      693 2023-04-13 07:55:38.000000 admath1-0.0.3/admath1/trignometry.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:26.646341 admath1-0.0.3/admath1.egg-info/
+-rw-rw-rw-   0        0        0     1802 2023-04-13 19:27:26.000000 admath1-0.0.3/admath1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-13 19:27:26.000000 admath1-0.0.3/admath1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:27:26.000000 admath1-0.0.3/admath1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 19:27:26.000000 admath1-0.0.3/admath1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:27:26.647560 admath1-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-04-13 19:27:05.000000 admath1-0.0.3/setup.py
```

### Comparing `admath1-0.0.2/LICENSE.txt` & `admath1-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admath1-0.0.2/PKG-INFO` & `admath1-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admath1
-Version: 0.0.2
+Version: 0.0.3
 Summary: maths library with some intermediate and advanced function
 Home-page: 
 Author: Subhash Kumar
 Author-email: subhashfreelancer2004@gmail.com
 License: MIT
 Keywords: maths,advance math,math,math formula,formula
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `admath1-0.0.2/README.txt` & `admath1-0.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `admath1-0.0.2/admath1/area.py` & `admath1-0.0.3/admath1/area.py`

 * *Files identical despite different names*

### Comparing `admath1-0.0.2/admath1/parameter.py` & `admath1-0.0.3/admath1/parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,26 @@
 def regular_polygon(
         side:float,
         number_side:float
 ) -> None:
     '''Find Perimeter of Regular_Polygon'''
     return side*number_side
 
-def circle(
-        radius:float
+def cube(
+        side:float
 ) -> None:
-    '''Find Perimeter of Circle'''
-    return round(2*PI*radius,3)
-def circle(
-        radius:float
+    '''Find Perimeter of Cube'''
+    return 12*side
+def cuboid(
+        lenght:float,
+        breadth:float,
+        height:float,
 ) -> None:
-    '''Find Perimeter of Circle'''
-    return round(2*PI*radius,3)
+    '''Find Perimeter of Cuboid'''
+    return 4*(lenght+breadth+height)
 
 
 def trapezoid(
         top_base:float,
         bottom_base:float,
         right_height:float,
         left_height:float
@@ -103,7 +105,8 @@
         outer_radius:float,
         inner_radius:float
 ) -> None:
     '''Find Perimeter of Annulus'''
     return round(2*PI*(outer_radius+inner_radius),3)
 
 
+
```

### Comparing `admath1-0.0.2/admath1/trignometry.py` & `admath1-0.0.3/admath1/trignometry.py`

 * *Files identical despite different names*

### Comparing `admath1-0.0.2/admath1.egg-info/PKG-INFO` & `admath1-0.0.3/admath1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admath1
-Version: 0.0.2
+Version: 0.0.3
 Summary: maths library with some intermediate and advanced function
 Home-page: 
 Author: Subhash Kumar
 Author-email: subhashfreelancer2004@gmail.com
 License: MIT
 Keywords: maths,advance math,math,math formula,formula
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `admath1-0.0.2/setup.py` & `admath1-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION ='0.0.2'
+VERSION ='0.0.3'
 
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'Operating System :: Unix',
   'Operating System :: MacOS :: MacOS X',
```

