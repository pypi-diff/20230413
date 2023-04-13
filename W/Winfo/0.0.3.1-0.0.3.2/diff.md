# Comparing `tmp/Winfo-0.0.3.1.tar.gz` & `tmp/Winfo-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.3.1.tar", last modified: Thu Apr 13 19:34:06 2023, max compression
+gzip compressed data, was "Winfo-0.0.3.2.tar", last modified: Thu Apr 13 19:36:32 2023, max compression
```

## Comparing `Winfo-0.0.3.1.tar` & `Winfo-0.0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:34:06.306155 Winfo-0.0.3.1/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6162 2023-04-13 19:34:06.305156 Winfo-0.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5714 2023-04-11 23:13:18.000000 Winfo-0.0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 19:34:06.285156 Winfo-0.0.3.1/Winfo/
--rw-rw-rw-   0        0        0     2686 2023-04-11 23:02:28.000000 Winfo-0.0.3.1/Winfo/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.3.1/Winfo/cpu.py
--rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.3.1/Winfo/disk.py
--rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.3.1/Winfo/ethernet.py
--rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.3.1/Winfo/gpu.py
--rw-rw-rw-   0        0        0      628 2023-04-11 23:07:57.000000 Winfo-0.0.3.1/Winfo/internet.py
--rw-rw-rw-   0        0        0     1312 2023-04-13 19:32:57.000000 Winfo-0.0.3.1/Winfo/memory.py
--rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.3.1/Winfo/motherboard.py
--rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.3.1/Winfo/software.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:34:06.303156 Winfo-0.0.3.1/Winfo.egg-info/
--rw-rw-rw-   0        0        0     6162 2023-04-13 19:34:06.000000 Winfo-0.0.3.1/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-04-13 19:34:06.000000 Winfo-0.0.3.1/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:34:06.000000 Winfo-0.0.3.1/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 19:34:06.000000 Winfo-0.0.3.1/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 19:34:06.306155 Winfo-0.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-13 19:33:43.000000 Winfo-0.0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:36:32.773516 Winfo-0.0.3.2/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     6162 2023-04-13 19:36:32.772516 Winfo-0.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5714 2023-04-11 23:13:18.000000 Winfo-0.0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 19:36:32.759517 Winfo-0.0.3.2/Winfo/
+-rw-rw-rw-   0        0        0     2686 2023-04-11 23:02:28.000000 Winfo-0.0.3.2/Winfo/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.3.2/Winfo/cpu.py
+-rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.3.2/Winfo/disk.py
+-rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.3.2/Winfo/ethernet.py
+-rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.3.2/Winfo/gpu.py
+-rw-rw-rw-   0        0        0      607 2023-04-13 19:35:23.000000 Winfo-0.0.3.2/Winfo/internet.py
+-rw-rw-rw-   0        0        0     1312 2023-04-13 19:32:57.000000 Winfo-0.0.3.2/Winfo/memory.py
+-rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.3.2/Winfo/motherboard.py
+-rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.3.2/Winfo/software.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:36:32.771517 Winfo-0.0.3.2/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     6162 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:36:32.773516 Winfo-0.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-04-13 19:36:05.000000 Winfo-0.0.3.2/setup.py
```

### Comparing `Winfo-0.0.3.1/LICENSE` & `Winfo-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/PKG-INFO` & `Winfo-0.0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Winfo-0.0.3.1/README.md` & `Winfo-0.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/__init__.py` & `Winfo-0.0.3.2/Winfo/__init__.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/cpu.py` & `Winfo-0.0.3.2/Winfo/cpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/disk.py` & `Winfo-0.0.3.2/Winfo/disk.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/ethernet.py` & `Winfo-0.0.3.2/Winfo/ethernet.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/gpu.py` & `Winfo-0.0.3.2/Winfo/gpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/memory.py` & `Winfo-0.0.3.2/Winfo/memory.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo/software.py` & `Winfo-0.0.3.2/Winfo/software.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.1/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.3.2/Winfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Winfo-0.0.3.1/setup.py` & `Winfo-0.0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.3.1",
+    version="0.0.3.2",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
```

