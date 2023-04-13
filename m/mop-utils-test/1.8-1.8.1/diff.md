# Comparing `tmp/mop_utils_test-1.8.tar.gz` & `tmp/mop_utils_test-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mop_utils_test-1.8.tar", last modified: Wed Apr 12 07:40:59 2023, max compression
+gzip compressed data, was "mop_utils_test-1.8.1.tar", last modified: Thu Apr 13 06:59:43 2023, max compression
```

## Comparing `mop_utils_test-1.8.tar` & `mop_utils_test-1.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:40:59.452151 mop_utils_test-1.8/
--rw-rw-rw-   0        0        0      113 2023-04-12 07:40:59.451151 mop_utils_test-1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 07:40:59.398148 mop_utils_test-1.8/mop_utils/
--rw-rw-rw-   0        0        0       89 2023-02-13 07:03:05.000000 mop_utils_test-1.8/mop_utils/__init__.py
--rw-rw-rw-   0        0        0     4528 2023-04-12 05:51:09.000000 mop_utils_test-1.8/mop_utils/base_model_wrapper.py
--rw-rw-rw-   0        0        0       39 2023-02-16 07:10:11.000000 mop_utils_test-1.8/mop_utils/constant.py
--rw-rw-rw-   0        0        0     6264 2023-03-31 08:33:06.000000 mop_utils_test-1.8/mop_utils/inference_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:40:59.449149 mop_utils_test-1.8/mop_utils_test.egg-info/
--rw-rw-rw-   0        0        0      113 2023-04-12 07:40:59.000000 mop_utils_test-1.8/mop_utils_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-12 07:40:59.000000 mop_utils_test-1.8/mop_utils_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:40:59.000000 mop_utils_test-1.8/mop_utils_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-12 07:40:59.000000 mop_utils_test-1.8/mop_utils_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-12 07:40:59.000000 mop_utils_test-1.8/mop_utils_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 07:40:59.452151 mop_utils_test-1.8/setup.cfg
--rw-rw-rw-   0        0        0      350 2023-04-12 05:52:08.000000 mop_utils_test-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:59:43.904690 mop_utils_test-1.8.1/
+-rw-rw-rw-   0        0        0      115 2023-04-13 06:59:43.903692 mop_utils_test-1.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 06:59:43.874692 mop_utils_test-1.8.1/mop_utils/
+-rw-rw-rw-   0        0        0       89 2023-02-13 07:03:05.000000 mop_utils_test-1.8.1/mop_utils/__init__.py
+-rw-rw-rw-   0        0        0     4529 2023-04-13 06:22:23.000000 mop_utils_test-1.8.1/mop_utils/base_model_wrapper.py
+-rw-rw-rw-   0        0        0       39 2023-02-16 07:10:11.000000 mop_utils_test-1.8.1/mop_utils/constant.py
+-rw-rw-rw-   0        0        0     6264 2023-03-31 08:33:06.000000 mop_utils_test-1.8.1/mop_utils/inference_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:59:43.902690 mop_utils_test-1.8.1/mop_utils_test.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-04-13 06:59:43.000000 mop_utils_test-1.8.1/mop_utils_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-13 06:59:43.000000 mop_utils_test-1.8.1/mop_utils_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:59:43.000000 mop_utils_test-1.8.1/mop_utils_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-13 06:59:43.000000 mop_utils_test-1.8.1/mop_utils_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 06:59:43.000000 mop_utils_test-1.8.1/mop_utils_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:59:43.904690 mop_utils_test-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-04-13 06:28:58.000000 mop_utils_test-1.8.1/setup.py
```

### Comparing `mop_utils_test-1.8/mop_utils/base_model_wrapper.py` & `mop_utils_test-1.8.1/mop_utils/base_model_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def height(self, height: int) -> None:
         self.__height__ = height
 
     @property
     def images(self) -> str:
         return self.__images__
 
-    @image.setter
+    @images.setter
     def images(self, images: str) -> None:
         self.__images__ = images
 
 
 class InferenceInput(MopInferenceInput):
     '''this is a subclass to be compatible with old version'''
```

### Comparing `mop_utils_test-1.8/mop_utils/inference_wrapper.py` & `mop_utils_test-1.8.1/mop_utils/inference_wrapper.py`

 * *Files identical despite different names*

