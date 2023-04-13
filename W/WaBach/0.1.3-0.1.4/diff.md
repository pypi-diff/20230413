# Comparing `tmp/WaBach-0.1.3.tar.gz` & `tmp/WaBach-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaBach-0.1.3.tar", last modified: Thu Apr 13 11:25:44 2023, max compression
+gzip compressed data, was "WaBach-0.1.4.tar", last modified: Thu Apr 13 11:30:27 2023, max compression
```

## Comparing `WaBach-0.1.3.tar` & `WaBach-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:25:44.650924 WaBach-0.1.3/
--rw-r--r--   0 simon      (502) staff       (20)     1073 2023-01-11 13:10:10.000000 WaBach-0.1.3/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)      824 2023-04-13 11:25:44.650676 WaBach-0.1.3/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      376 2023-01-11 19:53:18.000000 WaBach-0.1.3/README.md
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:25:44.649906 WaBach-0.1.3/WaBach.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)      824 2023-04-13 11:25:44.000000 WaBach-0.1.3/WaBach.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      241 2023-04-13 11:25:44.000000 WaBach-0.1.3/WaBach.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-04-13 11:25:44.000000 WaBach-0.1.3/WaBach.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-01-11 19:27:51.000000 WaBach-0.1.3/WaBach.egg-info/not-zip-safe
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-04-13 11:25:44.000000 WaBach-0.1.3/WaBach.egg-info/requires.txt
--rw-r--r--   0 simon      (502) staff       (20)        7 2023-04-13 11:25:44.000000 WaBach-0.1.3/WaBach.egg-info/top_level.txt
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-04-13 11:25:44.650994 WaBach-0.1.3/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      997 2023-04-13 11:25:16.000000 WaBach-0.1.3/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:25:44.650260 WaBach-0.1.3/wabach/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-01-11 19:23:30.000000 WaBach-0.1.3/wabach/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)     3547 2023-04-13 11:24:55.000000 WaBach-0.1.3/wabach/tensors.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:30:27.121967 WaBach-0.1.4/
+-rw-r--r--   0 simon      (502) staff       (20)     1073 2023-01-11 13:10:10.000000 WaBach-0.1.4/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)      824 2023-04-13 11:30:27.121741 WaBach-0.1.4/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      376 2023-01-11 19:53:18.000000 WaBach-0.1.4/README.md
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:30:27.121032 WaBach-0.1.4/WaBach.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)      824 2023-04-13 11:30:27.000000 WaBach-0.1.4/WaBach.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      241 2023-04-13 11:30:27.000000 WaBach-0.1.4/WaBach.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-04-13 11:30:27.000000 WaBach-0.1.4/WaBach.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-01-11 19:27:51.000000 WaBach-0.1.4/WaBach.egg-info/not-zip-safe
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-04-13 11:30:27.000000 WaBach-0.1.4/WaBach.egg-info/requires.txt
+-rw-r--r--   0 simon      (502) staff       (20)        7 2023-04-13 11:30:27.000000 WaBach-0.1.4/WaBach.egg-info/top_level.txt
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-04-13 11:30:27.122028 WaBach-0.1.4/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      997 2023-04-13 11:29:57.000000 WaBach-0.1.4/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:30:27.121366 WaBach-0.1.4/wabach/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-01-11 19:23:30.000000 WaBach-0.1.4/wabach/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)     3539 2023-04-13 11:29:30.000000 WaBach-0.1.4/wabach/tensors.py
```

### Comparing `WaBach-0.1.3/LICENSE` & `WaBach-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `WaBach-0.1.3/PKG-INFO` & `WaBach-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaBach
-Version: 0.1.3
+Version: 0.1.4
 Summary: Implementation of the Weyl tensor and the Bach tensor into Gravipy
 Home-page: 
 Author: Simon Knoska
 Author-email: knoskas@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `WaBach-0.1.3/WaBach.egg-info/PKG-INFO` & `WaBach-0.1.4/WaBach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaBach
-Version: 0.1.3
+Version: 0.1.4
 Summary: Implementation of the Weyl tensor and the Bach tensor into Gravipy
 Home-page: 
 Author: Simon Knoska
 Author-email: knoskas@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `WaBach-0.1.3/setup.py` & `WaBach-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="WaBach",
-    version="0.1.3",
+    version="0.1.4",
     description="Implementation of the Weyl tensor and the Bach tensor into Gravipy",
     url="",
     author="Simon Knoska",
     author_email="knoskas@gmail.com",
     license="BSD",
     packages=["wabach"],
     include_package_data=True,
```

### Comparing `WaBach-0.1.3/wabach/tensors.py` & `WaBach-0.1.4/wabach/tensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         
 class Bach(Tensor):
     def __init__(self, symbol, metric, RicciT, WeylT, *args, **kwargs):
         self._connection_required(metric)
         super(Bach, self).__init__(symbol, 2, metric, metric.conn, *args, **kwargs)
         self.Ri = RicciT
         self.W = WeylT
-        
+
         self._s = None
 
     def _compute_covariant_component(self, idxs):
         component = (sum(sum(self.W.covariantD(idxs[0],-c,idxs[1],-d,c,d) +
                      Rational(1,2)*self.Ri(c,d)*self.W(idxs[0],-c,idxs[1],-d)
                      for c in self.index_values[1])
                      for d in self.index_values[1])
@@ -66,12 +66,12 @@
                 self.components.update({(idxs[1], idxs[0]): component})
         return component
 
     def square(self):
         if self._s is None:
             self._s = sum(
                 self(k, l) * self(-k, -l) for k, l in
-                list(variations(self.index_values[1], 4, True))
+                list(variations(self.index_values[1], 2, True))
             ).together().simplify()
             return self._s
         else:
             return self._s
```

