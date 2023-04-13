# Comparing `tmp/WaBach-0.1.1.tar.gz` & `tmp/WaBach-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaBach-0.1.1.tar", last modified: Wed Jan 11 19:29:12 2023, max compression
+gzip compressed data, was "WaBach-0.1.2.tar", last modified: Thu Apr 13 11:19:50 2023, max compression
```

## Comparing `WaBach-0.1.1.tar` & `WaBach-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-01-11 19:29:12.923239 WaBach-0.1.1/
--rw-r--r--   0 simon      (502) staff       (20)     1073 2023-01-11 13:10:10.000000 WaBach-0.1.1/LICENSE
--rw-r--r--   0 simon      (502) staff       (20)      824 2023-01-11 19:29:12.923103 WaBach-0.1.1/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      170 2023-01-11 13:10:12.000000 WaBach-0.1.1/README.md
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-01-11 19:29:12.922538 WaBach-0.1.1/WaBach.egg-info/
--rw-r--r--   0 simon      (502) staff       (20)      824 2023-01-11 19:29:12.000000 WaBach-0.1.1/WaBach.egg-info/PKG-INFO
--rw-r--r--   0 simon      (502) staff       (20)      241 2023-01-11 19:29:12.000000 WaBach-0.1.1/WaBach.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-01-11 19:29:12.000000 WaBach-0.1.1/WaBach.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (502) staff       (20)        1 2023-01-11 19:27:51.000000 WaBach-0.1.1/WaBach.egg-info/not-zip-safe
--rw-r--r--   0 simon      (502) staff       (20)       15 2023-01-11 19:29:12.000000 WaBach-0.1.1/WaBach.egg-info/requires.txt
--rw-r--r--   0 simon      (502) staff       (20)        7 2023-01-11 19:29:12.000000 WaBach-0.1.1/WaBach.egg-info/top_level.txt
--rw-r--r--   0 simon      (502) staff       (20)       38 2023-01-11 19:29:12.923283 WaBach-0.1.1/setup.cfg
--rw-r--r--   0 simon      (502) staff       (20)      997 2023-01-11 19:27:45.000000 WaBach-0.1.1/setup.py
-drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-01-11 19:29:12.922793 WaBach-0.1.1/wabach/
--rw-r--r--   0 simon      (502) staff       (20)        0 2023-01-11 19:23:30.000000 WaBach-0.1.1/wabach/__init__.py
--rw-r--r--   0 simon      (502) staff       (20)     3215 2023-01-11 13:42:54.000000 WaBach-0.1.1/wabach/tensors.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:19:50.389907 WaBach-0.1.2/
+-rw-r--r--   0 simon      (502) staff       (20)     1073 2023-01-11 13:10:10.000000 WaBach-0.1.2/LICENSE
+-rw-r--r--   0 simon      (502) staff       (20)      824 2023-04-13 11:19:50.389621 WaBach-0.1.2/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      376 2023-01-11 19:53:18.000000 WaBach-0.1.2/README.md
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:19:50.388828 WaBach-0.1.2/WaBach.egg-info/
+-rw-r--r--   0 simon      (502) staff       (20)      824 2023-04-13 11:19:50.000000 WaBach-0.1.2/WaBach.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (502) staff       (20)      241 2023-04-13 11:19:50.000000 WaBach-0.1.2/WaBach.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-04-13 11:19:50.000000 WaBach-0.1.2/WaBach.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (502) staff       (20)        1 2023-01-11 19:27:51.000000 WaBach-0.1.2/WaBach.egg-info/not-zip-safe
+-rw-r--r--   0 simon      (502) staff       (20)       15 2023-04-13 11:19:50.000000 WaBach-0.1.2/WaBach.egg-info/requires.txt
+-rw-r--r--   0 simon      (502) staff       (20)        7 2023-04-13 11:19:50.000000 WaBach-0.1.2/WaBach.egg-info/top_level.txt
+-rw-r--r--   0 simon      (502) staff       (20)       38 2023-04-13 11:19:50.389992 WaBach-0.1.2/setup.cfg
+-rw-r--r--   0 simon      (502) staff       (20)      997 2023-04-13 11:18:39.000000 WaBach-0.1.2/setup.py
+drwxr-xr-x   0 simon      (502) staff       (20)        0 2023-04-13 11:19:50.389221 WaBach-0.1.2/wabach/
+-rw-r--r--   0 simon      (502) staff       (20)        0 2023-01-11 19:23:30.000000 WaBach-0.1.2/wabach/__init__.py
+-rw-r--r--   0 simon      (502) staff       (20)     3515 2023-04-13 11:16:02.000000 WaBach-0.1.2/wabach/tensors.py
```

### Comparing `WaBach-0.1.1/LICENSE` & `WaBach-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WaBach-0.1.1/PKG-INFO` & `WaBach-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaBach
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the Weyl tensor and the Bach tensor into Gravipy
 Home-page: 
 Author: Simon Knoska
 Author-email: knoskas@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `WaBach-0.1.1/WaBach.egg-info/PKG-INFO` & `WaBach-0.1.2/WaBach.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaBach
-Version: 0.1.1
+Version: 0.1.2
 Summary: Implementation of the Weyl tensor and the Bach tensor into Gravipy
 Home-page: 
 Author: Simon Knoska
 Author-email: knoskas@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `WaBach-0.1.1/setup.py` & `WaBach-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="WaBach",
-    version="0.1.1",
+    version="0.1.2",
     description="Implementation of the Weyl tensor and the Bach tensor into Gravipy",
     url="",
     author="Simon Knoska",
     author_email="knoskas@gmail.com",
     license="BSD",
     packages=["wabach"],
     include_package_data=True,
```

### Comparing `WaBach-0.1.1/wabach/tensors.py` & `WaBach-0.1.2/wabach/tensors.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,8 +58,18 @@
                      Rational(1,2)*self.Ri(c,d)*self.W(idxs[0],-c,idxs[1],-d)
                      for c in self.index_values[1])
                      for d in self.index_values[1])
                     ).together().simplify()
         self.components.update({idxs: component})
         if self.apply_tensor_symmetry:
                 self.components.update({(idxs[1], idxs[0]): component})
-        return component
+        return component
+
+    def square(self):
+        if self._s is None:
+            self._s = sum(
+                self(k, l) * self(-k, -l) for k, l in
+                list(variations(self.index_values[1], 4, True))
+            ).together().simplify()
+            return self._s
+        else:
+            return self._s
```

