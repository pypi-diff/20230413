# Comparing `tmp/text2mapview-0.2.0.tar.gz` & `tmp/text2mapview-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2mapview-0.2.0.tar", last modified: Thu Apr 13 09:30:06 2023, max compression
+gzip compressed data, was "text2mapview-0.2.1.tar", last modified: Thu Apr 13 09:57:33 2023, max compression
```

## Comparing `text2mapview-0.2.0.tar` & `text2mapview-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:30:06.938807 text2mapview-0.2.0/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapview-0.2.0/LICENSE
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2451 2023-04-13 09:30:06.938807 text2mapview-0.2.0/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1887 2023-04-13 08:53:29.000000 text2mapview-0.2.0/README.md
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      797 2023-04-13 09:11:52.000000 text2mapview-0.2.0/pyproject.toml
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       60 2023-04-13 08:39:45.000000 text2mapview-0.2.0/requirements.txt
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:30:06.938807 text2mapview-0.2.0/scr/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapview-0.2.0/scr/__init__.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:30:06.938807 text2mapview-0.2.0/scr/examples/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapview-0.2.0/scr/examples/map_embedding.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:30:06.938807 text2mapview-0.2.0/scr/fondamental/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapview-0.2.0/scr/fondamental/bases.py
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapview-0.2.0/scr/main.py
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 09:30:06.938807 text2mapview-0.2.0/setup.cfg
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:30:06.938807 text2mapview-0.2.0/text2mapview.egg-info/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2451 2023-04-13 09:30:06.000000 text2mapview-0.2.0/text2mapview.egg-info/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      311 2023-04-13 09:30:06.000000 text2mapview-0.2.0/text2mapview.egg-info/SOURCES.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 09:30:06.000000 text2mapview-0.2.0/text2mapview.egg-info/dependency_links.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       59 2023-04-13 09:30:06.000000 text2mapview-0.2.0/text2mapview.egg-info/requires.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        4 2023-04-13 09:30:06.000000 text2mapview-0.2.0/text2mapview.egg-info/top_level.txt
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:57:33.963342 text2mapview-0.2.1/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapview-0.2.1/LICENSE
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2451 2023-04-13 09:57:33.963342 text2mapview-0.2.1/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1887 2023-04-13 08:53:29.000000 text2mapview-0.2.1/README.md
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      797 2023-04-13 09:57:15.000000 text2mapview-0.2.1/pyproject.toml
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       60 2023-04-13 08:39:45.000000 text2mapview-0.2.1/requirements.txt
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:57:33.959342 text2mapview-0.2.1/scr/
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:57:33.959342 text2mapview-0.2.1/scr/text2mapview/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapview-0.2.1/scr/text2mapview/__init__.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:57:33.959342 text2mapview-0.2.1/scr/text2mapview/examples/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapview-0.2.1/scr/text2mapview/examples/map_embedding.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:57:33.963342 text2mapview-0.2.1/scr/text2mapview/fondamental/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapview-0.2.1/scr/text2mapview/fondamental/bases.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapview-0.2.1/scr/text2mapview/main.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 09:57:33.963342 text2mapview-0.2.1/setup.cfg
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 09:57:33.963342 text2mapview-0.2.1/text2mapview.egg-info/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2451 2023-04-13 09:57:33.000000 text2mapview-0.2.1/text2mapview.egg-info/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      363 2023-04-13 09:57:33.000000 text2mapview-0.2.1/text2mapview.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 09:57:33.000000 text2mapview-0.2.1/text2mapview.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       59 2023-04-13 09:57:33.000000 text2mapview-0.2.1/text2mapview.egg-info/requires.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        4 2023-04-13 09:57:33.000000 text2mapview-0.2.1/text2mapview.egg-info/top_level.txt
```

### Comparing `text2mapview-0.2.0/LICENSE` & `text2mapview-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `text2mapview-0.2.0/PKG-INFO` & `text2mapview-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2mapview
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapview
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `text2mapview-0.2.0/README.md` & `text2mapview-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `text2mapview-0.2.0/pyproject.toml` & `text2mapview-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2mapview"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name= "Papa Séga WADE", email= "pasega.wade@gmail.com"}
 ]
 
 description = "A python package to map your own csv files data using Atlas from NOMIC"
 readme={file = "README.md", content-type = "text/markdown"} 
 keywords=[
```

### Comparing `text2mapview-0.2.0/scr/fondamental/bases.py` & `text2mapview-0.2.1/scr/text2mapview/fondamental/bases.py`

 * *Files identical despite different names*

### Comparing `text2mapview-0.2.0/scr/main.py` & `text2mapview-0.2.1/scr/text2mapview/main.py`

 * *Files identical despite different names*

### Comparing `text2mapview-0.2.0/text2mapview.egg-info/PKG-INFO` & `text2mapview-0.2.1/text2mapview.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2mapview
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapview
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

