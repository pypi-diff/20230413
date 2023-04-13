# Comparing `tmp/durguestprofile-1.1.4.tar.gz` & `tmp/durguestprofile-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durguestprofile-1.1.4.tar", last modified: Thu Apr 13 20:22:50 2023, max compression
+gzip compressed data, was "durguestprofile-1.1.5.tar", last modified: Thu Apr 13 20:35:19 2023, max compression
```

## Comparing `durguestprofile-1.1.4.tar` & `durguestprofile-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:22:50.423270 durguestprofile-1.1.4/
--rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3590 2023-04-13 20:22:50.424275 durguestprofile-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:22:50.357233 durguestprofile-1.1.4/durguestprofile/
--rw-rw-rw-   0        0        0     1013 2023-04-13 17:43:54.000000 durguestprofile-1.1.4/durguestprofile/__init__.py
--rw-rw-rw-   0        0        0    16938 2023-04-13 19:57:06.000000 durguestprofile-1.1.4/durguestprofile/functions.py
--rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.1.4/durguestprofile/guest_profile.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:22:50.421270 durguestprofile-1.1.4/durguestprofile/support/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.4/durguestprofile/support/__init__.py
--rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.4/durguestprofile/utilities.py
--rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.4/durguestprofile/xmltodict.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:22:50.416270 durguestprofile-1.1.4/durguestprofile.egg-info/
--rw-rw-rw-   0        0        0     3590 2023-04-13 20:22:50.000000 durguestprofile-1.1.4/durguestprofile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-04-13 20:22:50.000000 durguestprofile-1.1.4/durguestprofile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:22:50.000000 durguestprofile-1.1.4/durguestprofile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-13 20:22:50.000000 durguestprofile-1.1.4/durguestprofile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 20:22:50.000000 durguestprofile-1.1.4/durguestprofile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2023-04-13 20:22:50.430272 durguestprofile-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1758 2023-04-13 20:22:41.000000 durguestprofile-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.410365 durguestprofile-1.1.5/
+-rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3642 2023-04-13 20:35:19.410419 durguestprofile-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.370359 durguestprofile-1.1.5/durguestprofile/
+-rw-rw-rw-   0        0        0     1013 2023-04-13 20:35:14.000000 durguestprofile-1.1.5/durguestprofile/__init__.py
+-rw-rw-rw-   0        0        0    16938 2023-04-13 19:57:06.000000 durguestprofile-1.1.5/durguestprofile/functions.py
+-rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.1.5/durguestprofile/guest_profile.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.408370 durguestprofile-1.1.5/durguestprofile/support/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.5/durguestprofile/support/__init__.py
+-rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.5/durguestprofile/utilities.py
+-rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.5/durguestprofile/xmltodict.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.405366 durguestprofile-1.1.5/durguestprofile.egg-info/
+-rw-rw-rw-   0        0        0     3642 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2023-04-13 20:35:19.416365 durguestprofile-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-04-13 20:35:06.000000 durguestprofile-1.1.5/setup.py
```

### Comparing `durguestprofile-1.1.4/LICENSE` & `durguestprofile-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.4/PKG-INFO` & `durguestprofile-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.1.4
+Version: 1.1.5
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
-License: MIT
+License: BSD
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Software Development :: Version Control :: Git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # durguestprofile
```

### Comparing `durguestprofile-1.1.4/README.md` & `durguestprofile-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.4/durguestprofile/__init__.py` & `durguestprofile-1.1.5/durguestprofile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "1.1.5"
 
 missing_python = []
 try:
     import struct
     version = struct.calcsize("P") * 8
 except ImportError as e:
     missing_python.append(f"{version}: {e}")
```

### Comparing `durguestprofile-1.1.4/durguestprofile/functions.py` & `durguestprofile-1.1.5/durguestprofile/functions.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.4/durguestprofile/utilities.py` & `durguestprofile-1.1.5/durguestprofile/utilities.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.4/durguestprofile/xmltodict.py` & `durguestprofile-1.1.5/durguestprofile/xmltodict.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.4/durguestprofile.egg-info/PKG-INFO` & `durguestprofile-1.1.5/durguestprofile.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.1.4
+Version: 1.1.5
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
-License: MIT
+License: BSD
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Software Development :: Version Control :: Git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # durguestprofile
```

### Comparing `durguestprofile-1.1.4/setup.py` & `durguestprofile-1.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     """
     with open(os.path.join(os.path.dirname(__file__),fname), encoding="utf8") as f:
         contents = f.read()
 
     return contents
 
 
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 DESCRIPTION = 'Dur Guest Data Accuracy Measurement Tool'
 LONG_DESCRIPTION = read("README.md")
 
 # Setting up
 setup(
     # the name must match the folder name
     name="durguestprofile",
     version=VERSION,
-    license='MIT',
+    license='BSD',
     author="ROInsight.com - Muhammad Khlef",
     author_email="<support@roinsight.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
@@ -47,14 +47,15 @@
     ],
     url="",
     keywords=['python', 'dur', 'guest', 'opera', 'profile', 'audit'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Interpreters",
         "Topic :: Software Development :: Version Control :: Git",
     ]
 )
```

