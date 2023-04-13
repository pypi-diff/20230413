# Comparing `tmp/pcalf-0.0.2.tar.gz` & `tmp/pcalf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcalf-0.0.2.tar", last modified: Thu Apr 13 12:48:51 2023, max compression
+gzip compressed data, was "pcalf-0.0.3.tar", last modified: Thu Apr 13 12:58:46 2023, max compression
```

## Comparing `pcalf-0.0.2.tar` & `pcalf-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/
--rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-04-13 11:29:34.000000 pcalf-0.0.2/LICENSE.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       42 2023-04-13 08:49:42.000000 pcalf-0.0.2/MANIFEST.in
--rw-r--r--   0 mmillet    (501) staff       (20)     2320 2023-04-13 12:48:51.000000 pcalf-0.0.2/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)     1854 2023-04-13 08:49:42.000000 pcalf-0.0.2/README.md
--rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-04-13 11:28:33.000000 pcalf-0.0.2/pyproject.toml
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/scripts/
--rw-r--r--   0 mmillet    (501) staff       (20)    13197 2023-04-13 12:45:06.000000 pcalf-0.0.2/scripts/pcalf
--rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-04-13 12:48:51.000000 pcalf-0.0.2/setup.cfg
--rw-r--r--   0 mmillet    (501) staff       (20)     1181 2023-04-13 12:48:33.000000 pcalf-0.0.2/setup.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf/
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:43:28.000000 pcalf-0.0.2/src/pcalf/__init__.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf/core/
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:01:24.000000 pcalf-0.0.2/src/pcalf/core/__init__.py
--rw-r--r--   0 mmillet    (501) staff       (20)     7841 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/core/biohmm.py
--rw-r--r--   0 mmillet    (501) staff       (20)    17748 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/core/bioseq.py
--rw-r--r--   0 mmillet    (501) staff       (20)     1662 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/core/log.py
--rw-r--r--   0 mmillet    (501) staff       (20)    22688 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/core/search.py
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf/datas/
--rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/Gly1.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/Gly1.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/Gly2.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/Gly2.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/Gly3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/Gly3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/GlyX3.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/GlyX3.msa.fa
--rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/__init__.py
--rw-r--r--   0 mmillet    (501) staff       (20)      496 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/accession.txt
--rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/all.hmm
--rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/nterdb.fasta
--rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/nterdb.ref.tsv
--rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-04-13 08:49:42.000000 pcalf-0.0.2/src/pcalf/datas/nterdb.tsv
-drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf.egg-info/
--rw-r--r--   0 mmillet    (501) staff       (20)     2320 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf.egg-info/PKG-INFO
--rw-r--r--   0 mmillet    (501) staff       (20)      796 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf.egg-info/SOURCES.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf.egg-info/dependency_links.txt
--rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:39:50.000000 pcalf-0.0.2/src/pcalf.egg-info/not-zip-safe
--rw-r--r--   0 mmillet    (501) staff       (20)       96 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf.egg-info/requires.txt
--rw-r--r--   0 mmillet    (501) staff       (20)       10 2023-04-13 12:48:51.000000 pcalf-0.0.2/src/pcalf.egg-info/top_level.txt
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/
+-rw-r--r--   0 mmillet    (501) staff       (20)     1069 2023-04-13 11:29:34.000000 pcalf-0.0.3/LICENSE.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       42 2023-04-13 08:49:42.000000 pcalf-0.0.3/MANIFEST.in
+-rw-r--r--   0 mmillet    (501) staff       (20)     2340 2023-04-13 12:58:46.000000 pcalf-0.0.3/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)     1854 2023-04-13 08:49:42.000000 pcalf-0.0.3/README.md
+-rw-r--r--   0 mmillet    (501) staff       (20)       84 2023-04-13 11:28:33.000000 pcalf-0.0.3/pyproject.toml
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/scripts/
+-rw-r--r--   0 mmillet    (501) staff       (20)    13197 2023-04-13 12:45:06.000000 pcalf-0.0.3/scripts/pcalf
+-rw-r--r--   0 mmillet    (501) staff       (20)       38 2023-04-13 12:58:46.000000 pcalf-0.0.3/setup.cfg
+-rw-r--r--   0 mmillet    (501) staff       (20)     1181 2023-04-13 12:55:04.000000 pcalf-0.0.3/setup.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf/
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:43:28.000000 pcalf-0.0.3/src/pcalf/__init__.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf/core/
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 12:01:24.000000 pcalf-0.0.3/src/pcalf/core/__init__.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     7841 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/biohmm.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    17748 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/bioseq.py
+-rw-r--r--   0 mmillet    (501) staff       (20)     1662 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/log.py
+-rw-r--r--   0 mmillet    (501) staff       (20)    22688 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/core/search.py
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf/datas/
+-rw-r--r--   0 mmillet    (501) staff       (20)    29491 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly1.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3440 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly1.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    28897 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly2.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     2819 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly2.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)    27603 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)     3674 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/Gly3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)   106797 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/GlyX3.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    11209 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/GlyX3.msa.fa
+-rw-r--r--   0 mmillet    (501) staff       (20)        0 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/__init__.py
+-rw-r--r--   0 mmillet    (501) staff       (20)      496 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/accession.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)   192788 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/all.hmm
+-rw-r--r--   0 mmillet    (501) staff       (20)    12236 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/nterdb.fasta
+-rw-r--r--   0 mmillet    (501) staff       (20)     6003 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/nterdb.ref.tsv
+-rw-r--r--   0 mmillet    (501) staff       (20)     3188 2023-04-13 08:49:42.000000 pcalf-0.0.3/src/pcalf/datas/nterdb.tsv
+drwxr-xr-x   0 mmillet    (501) staff       (20)        0 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/
+-rw-r--r--   0 mmillet    (501) staff       (20)     2340 2023-04-13 12:58:45.000000 pcalf-0.0.3/src/pcalf.egg-info/PKG-INFO
+-rw-r--r--   0 mmillet    (501) staff       (20)      796 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/SOURCES.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:58:45.000000 pcalf-0.0.3/src/pcalf.egg-info/dependency_links.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)        1 2023-04-13 12:39:50.000000 pcalf-0.0.3/src/pcalf.egg-info/not-zip-safe
+-rw-r--r--   0 mmillet    (501) staff       (20)       96 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/requires.txt
+-rw-r--r--   0 mmillet    (501) staff       (20)       10 2023-04-13 12:58:46.000000 pcalf-0.0.3/src/pcalf.egg-info/top_level.txt
```

### Comparing `pcalf-0.0.2/LICENSE.txt` & `pcalf-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/PKG-INFO` & `pcalf-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pcalf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Search calcyanin in a set of amino acid sequences
 Home-page: https://github.com/K2SOHIGH/pcalf
 Author: Maxime Millet
 Author-email: maxime.luc.millet@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -69,7 +70,9 @@
 
 ## USAGE
 ```bash
 pcalf -i fasta.cds.fa.gz -o pcalf_res
 ```
 
 
+
+
```

### Comparing `pcalf-0.0.2/README.md` & `pcalf-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/scripts/pcalf` & `pcalf-0.0.3/scripts/pcalf`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/setup.py` & `pcalf-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pcalf',
-    version='0.0.2',
+    version='0.0.3',
     description='Search calcyanin in a set of amino acid sequences',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url='https://github.com/K2SOHIGH/pcalf',
     author='Maxime Millet',
     author_email='maxime.luc.millet@gmail.com',
     license='MIT',
```

### Comparing `pcalf-0.0.2/src/pcalf/core/biohmm.py` & `pcalf-0.0.3/src/pcalf/core/biohmm.py`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/core/bioseq.py` & `pcalf-0.0.3/src/pcalf/core/bioseq.py`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/core/log.py` & `pcalf-0.0.3/src/pcalf/core/log.py`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/core/search.py` & `pcalf-0.0.3/src/pcalf/core/search.py`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/Gly1.hmm` & `pcalf-0.0.3/src/pcalf/datas/Gly1.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/Gly1.msa.fa` & `pcalf-0.0.3/src/pcalf/datas/Gly1.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/Gly2.hmm` & `pcalf-0.0.3/src/pcalf/datas/Gly2.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/Gly2.msa.fa` & `pcalf-0.0.3/src/pcalf/datas/Gly2.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/Gly3.hmm` & `pcalf-0.0.3/src/pcalf/datas/Gly3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/Gly3.msa.fa` & `pcalf-0.0.3/src/pcalf/datas/Gly3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/GlyX3.hmm` & `pcalf-0.0.3/src/pcalf/datas/GlyX3.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/GlyX3.msa.fa` & `pcalf-0.0.3/src/pcalf/datas/GlyX3.msa.fa`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/all.hmm` & `pcalf-0.0.3/src/pcalf/datas/all.hmm`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/nterdb.fasta` & `pcalf-0.0.3/src/pcalf/datas/nterdb.fasta`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/nterdb.ref.tsv` & `pcalf-0.0.3/src/pcalf/datas/nterdb.ref.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf/datas/nterdb.tsv` & `pcalf-0.0.3/src/pcalf/datas/nterdb.tsv`

 * *Files identical despite different names*

### Comparing `pcalf-0.0.2/src/pcalf.egg-info/PKG-INFO` & `pcalf-0.0.3/src/pcalf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pcalf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Search calcyanin in a set of amino acid sequences
 Home-page: https://github.com/K2SOHIGH/pcalf
 Author: Maxime Millet
 Author-email: maxime.luc.millet@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -69,7 +70,9 @@
 
 ## USAGE
 ```bash
 pcalf -i fasta.cds.fa.gz -o pcalf_res
 ```
 
 
+
+
```

### Comparing `pcalf-0.0.2/src/pcalf.egg-info/SOURCES.txt` & `pcalf-0.0.3/src/pcalf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

