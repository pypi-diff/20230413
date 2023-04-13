# Comparing `tmp/markdown_link_attr_modifier-0.2.0.tar.gz` & `tmp/markdown_link_attr_modifier-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_link_attr_modifier-0.2.0.tar", last modified: Mon Feb 15 17:17:41 2021, max compression
+gzip compressed data, was "markdown_link_attr_modifier-0.2.1.tar", last modified: Thu Apr 13 15:56:58 2023, max compression
```

## Comparing `markdown_link_attr_modifier-0.2.0.tar` & `markdown_link_attr_modifier-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2021-02-15 17:17:41.584645 markdown_link_attr_modifier-0.2.0/
--rw-r--r--   0 shen       (501) staff       (20)    35149 2020-10-04 14:28:16.000000 markdown_link_attr_modifier-0.2.0/LICENSE
--rw-r--r--   0 shen       (501) staff       (20)       29 2020-10-06 14:27:56.000000 markdown_link_attr_modifier-0.2.0/MANIFEST.in
--rw-r--r--   0 shen       (501) staff       (20)      870 2021-02-15 17:17:41.584400 markdown_link_attr_modifier-0.2.0/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      159 2020-10-04 20:25:46.000000 markdown_link_attr_modifier-0.2.0/Readme.PyPI.md
--rw-r--r--   0 shen       (501) staff       (20)     5459 2021-02-15 16:31:17.000000 markdown_link_attr_modifier-0.2.0/Readme.md
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2021-02-15 17:17:41.584044 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/
--rw-r--r--   0 shen       (501) staff       (20)      870 2021-02-15 17:17:41.000000 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      338 2021-02-15 17:17:41.000000 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/SOURCES.txt
--rw-r--r--   0 shen       (501) staff       (20)        1 2021-02-15 17:17:41.000000 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/dependency_links.txt
--rw-r--r--   0 shen       (501) staff       (20)       12 2021-02-15 17:17:41.000000 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/requires.txt
--rw-r--r--   0 shen       (501) staff       (20)       28 2021-02-15 17:17:41.000000 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/top_level.txt
--rwxr-xr-x   0 shen       (501) staff       (20)    22267 2021-02-15 16:55:42.000000 markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.py
--rw-r--r--   0 shen       (501) staff       (20)       38 2021-02-15 17:17:41.584724 markdown_link_attr_modifier-0.2.0/setup.cfg
--rwxr-xr-x   0 shen       (501) staff       (20)     1170 2021-02-15 17:14:40.000000 markdown_link_attr_modifier-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:56:58.126470 markdown_link_attr_modifier-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-13 15:56:48.000000 markdown_link_attr_modifier-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-13 15:56:48.000000 markdown_link_attr_modifier-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-13 15:56:58.126470 markdown_link_attr_modifier-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      159 2023-04-13 15:56:48.000000 markdown_link_attr_modifier-0.2.1/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-04-13 15:56:48.000000 markdown_link_attr_modifier-0.2.1/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:56:58.126470 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-13 15:56:58.000000 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-13 15:56:58.000000 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:56:58.000000 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 15:56:58.000000 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-13 15:56:58.000000 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    17104 2023-04-13 15:56:48.000000 markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 15:56:58.126470 markdown_link_attr_modifier-0.2.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1150 2023-04-13 15:56:48.000000 markdown_link_attr_modifier-0.2.1/setup.py
```

### Comparing `markdown_link_attr_modifier-0.2.0/LICENSE` & `markdown_link_attr_modifier-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_link_attr_modifier-0.2.0/PKG-INFO` & `markdown_link_attr_modifier-0.2.1/markdown_link_attr_modifier.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
-Name: markdown_link_attr_modifier
-Version: 0.2.0
+Name: markdown-link-attr-modifier
+Version: 0.2.1
 Summary: A Python-Markdown extension to modify attributes of <a> tag links
 Home-page: https://github.com/Phuker/markdown_link_attr_modifier
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
-Description: [Project homepage](https://github.com/Phuker/markdown_link_attr_modifier)
-        
-        [Readme](https://github.com/Phuker/markdown_link_attr_modifier/blob/main/Readme.md)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[Project homepage](https://github.com/Phuker/markdown_link_attr_modifier)
+
+[Readme](https://github.com/Phuker/markdown_link_attr_modifier/blob/main/Readme.md)
```

### Comparing `markdown_link_attr_modifier-0.2.0/Readme.md` & `markdown_link_attr_modifier-0.2.1/Readme.md`

 * *Files identical despite different names*

### Comparing `markdown_link_attr_modifier-0.2.0/markdown_link_attr_modifier.egg-info/PKG-INFO` & `markdown_link_attr_modifier-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
-Name: markdown-link-attr-modifier
-Version: 0.2.0
+Name: markdown_link_attr_modifier
+Version: 0.2.1
 Summary: A Python-Markdown extension to modify attributes of <a> tag links
 Home-page: https://github.com/Phuker/markdown_link_attr_modifier
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
-Description: [Project homepage](https://github.com/Phuker/markdown_link_attr_modifier)
-        
-        [Readme](https://github.com/Phuker/markdown_link_attr_modifier/blob/main/Readme.md)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[Project homepage](https://github.com/Phuker/markdown_link_attr_modifier)
+
+[Readme](https://github.com/Phuker/markdown_link_attr_modifier/blob/main/Readme.md)
```

### Comparing `markdown_link_attr_modifier-0.2.0/setup.py` & `markdown_link_attr_modifier-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 from setuptools import setup
 
 # Impossible? to update only Readme.md but keep version number in PyPI.
-# Gancui use a dummy readme instead.
+# Gancui use a dummy readme file instead.
 with open("Readme.PyPI.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "markdown_link_attr_modifier",
-    version = "0.2.0",
+    version = "0.2.1",
     description = "A Python-Markdown extension to modify attributes of <a> tag links",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = "Phuker",
     author_email = 'Phuker@users.noreply.github.com',
     url = "https://github.com/Phuker/markdown_link_attr_modifier",
     license = "GNU General Public License v3.0",
@@ -23,13 +23,12 @@
     scripts = [],
     install_requires = [
         'markdown>=3',
     ],
     classifiers = [
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Topic :: Text Processing :: Markup :: Markdown',
     ],
-    python_requires = '>=3.6'
+    python_requires = '>=3.6', # PEP 498, f-strings
 )
```

