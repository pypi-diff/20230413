# Comparing `tmp/text2mapviewer-0.1.0.tar.gz` & `tmp/text2mapviewer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2mapviewer-0.1.0.tar", last modified: Thu Apr 13 11:51:10 2023, max compression
+gzip compressed data, was "text2mapviewer-0.2.0.tar", last modified: Thu Apr 13 12:38:26 2023, max compression
```

## Comparing `text2mapviewer-0.1.0.tar` & `text2mapviewer-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 11:51:10.281214 text2mapviewer-0.1.0/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapviewer-0.1.0/LICENSE
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       40 2023-04-13 11:39:22.000000 text2mapviewer-0.1.0/MANIFEST.in
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2455 2023-04-13 11:51:10.281214 text2mapviewer-0.1.0/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1887 2023-04-13 08:53:29.000000 text2mapviewer-0.1.0/README.md
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      801 2023-04-13 10:44:59.000000 text2mapviewer-0.1.0/pyproject.toml
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     4130 2023-04-13 11:33:40.000000 text2mapviewer-0.1.0/requirements.txt
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 11:51:10.277214 text2mapviewer-0.1.0/scr/
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 11:51:10.277214 text2mapviewer-0.1.0/scr/text2mapviewer/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapviewer-0.1.0/scr/text2mapviewer/__init__.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 11:51:10.277214 text2mapviewer-0.1.0/scr/text2mapviewer/examples/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapviewer-0.1.0/scr/text2mapviewer/examples/map_embedding.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 11:51:10.277214 text2mapviewer-0.1.0/scr/text2mapviewer/fondamental/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapviewer-0.1.0/scr/text2mapviewer/fondamental/bases.py
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapviewer-0.1.0/scr/text2mapviewer/main.py
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 11:51:10.281214 text2mapviewer-0.1.0/setup.cfg
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 11:51:10.281214 text2mapviewer-0.1.0/text2mapviewer.egg-info/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2455 2023-04-13 11:51:10.000000 text2mapviewer-0.1.0/text2mapviewer.egg-info/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      393 2023-04-13 11:51:10.000000 text2mapviewer-0.1.0/text2mapviewer.egg-info/SOURCES.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 11:51:10.000000 text2mapviewer-0.1.0/text2mapviewer.egg-info/dependency_links.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1300 2023-04-13 11:51:10.000000 text2mapviewer-0.1.0/text2mapviewer.egg-info/requires.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        4 2023-04-13 11:51:10.000000 text2mapviewer-0.1.0/text2mapviewer.egg-info/top_level.txt
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/LICENSE
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       40 2023-04-13 11:39:22.000000 text2mapviewer-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1889 2023-04-13 12:35:34.000000 text2mapviewer-0.2.0/README.md
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      801 2023-04-13 12:35:47.000000 text2mapviewer-0.2.0/pyproject.toml
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     4130 2023-04-13 11:33:40.000000 text2mapviewer-0.2.0/requirements.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/setup.cfg
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.370601 text2mapviewer-0.2.0/text2mapviewer/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapviewer-0.2.0/text2mapviewer/__init__.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/text2mapviewer/examples/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/text2mapviewer/examples/map_embedding.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/text2mapviewer/fondamental/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/text2mapviewer/fondamental/bases.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapviewer-0.2.0/text2mapviewer/main.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 12:38:26.374601 text2mapviewer-0.2.0/text2mapviewer.egg-info/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      377 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1300 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/requires.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       15 2023-04-13 12:38:26.000000 text2mapviewer-0.2.0/text2mapviewer.egg-info/top_level.txt
```

### Comparing `text2mapviewer-0.1.0/LICENSE` & `text2mapviewer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.1.0/PKG-INFO` & `text2mapviewer-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2mapviewer
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapviewer
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 To install the necessary dependencies, run the following command:
 
 ```bash
 python -m venv mymapenv 
 source mymapenv/bin/activate
 pip install --upgrade pip 
-pip install text2mapdata
+pip install text2mapviewer
 ```
 
 ## Supported Transformer Models from Hugging Face 
 
 This project supports a variety of transformer models, including models from the Hugging Face Model Hub and sentence-transformers. Below are some examples:
     - Hugging Face Model: 'prajjwal1/bert-mini'
     - Hugging Face Model: 'Sahajtomar/french_semantic'  (french version for semantic search embedding)
```

### Comparing `text2mapviewer-0.1.0/README.md` & `text2mapviewer-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 To install the necessary dependencies, run the following command:
 
 ```bash
 python -m venv mymapenv 
 source mymapenv/bin/activate
 pip install --upgrade pip 
-pip install text2mapdata
+pip install text2mapviewer
 ```
 
 ## Supported Transformer Models from Hugging Face 
 
 This project supports a variety of transformer models, including models from the Hugging Face Model Hub and sentence-transformers. Below are some examples:
     - Hugging Face Model: 'prajjwal1/bert-mini'
     - Hugging Face Model: 'Sahajtomar/french_semantic'  (french version for semantic search embedding)
```

### Comparing `text2mapviewer-0.1.0/pyproject.toml` & `text2mapviewer-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2mapviewer"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     {name= "Papa Séga WADE", email= "pasega.wade@gmail.com"}
 ]
 
 description = "A python package to map your own csv files data using Atlas from NOMIC"
 readme={file = "README.md", content-type = "text/markdown"} 
 keywords=[
```

### Comparing `text2mapviewer-0.1.0/requirements.txt` & `text2mapviewer-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.1.0/scr/text2mapviewer/fondamental/bases.py` & `text2mapviewer-0.2.0/text2mapviewer/fondamental/bases.py`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.1.0/scr/text2mapviewer/main.py` & `text2mapviewer-0.2.0/text2mapviewer/main.py`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.1.0/text2mapviewer.egg-info/PKG-INFO` & `text2mapviewer-0.2.0/text2mapviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2mapviewer
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapviewer
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 To install the necessary dependencies, run the following command:
 
 ```bash
 python -m venv mymapenv 
 source mymapenv/bin/activate
 pip install --upgrade pip 
-pip install text2mapdata
+pip install text2mapviewer
 ```
 
 ## Supported Transformer Models from Hugging Face 
 
 This project supports a variety of transformer models, including models from the Hugging Face Model Hub and sentence-transformers. Below are some examples:
     - Hugging Face Model: 'prajjwal1/bert-mini'
     - Hugging Face Model: 'Sahajtomar/french_semantic'  (french version for semantic search embedding)
```

### Comparing `text2mapviewer-0.1.0/text2mapviewer.egg-info/requires.txt` & `text2mapviewer-0.2.0/text2mapviewer.egg-info/requires.txt`

 * *Files identical despite different names*

