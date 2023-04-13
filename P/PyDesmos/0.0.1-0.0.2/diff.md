# Comparing `tmp/PyDesmos-0.0.1.tar.gz` & `tmp/PyDesmos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDesmos-0.0.1.tar", last modified: Thu Apr 13 03:39:52 2023, max compression
+gzip compressed data, was "PyDesmos-0.0.2.tar", last modified: Thu Apr 13 03:46:32 2023, max compression
```

## Comparing `PyDesmos-0.0.1.tar` & `PyDesmos-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:39:52.532591 PyDesmos-0.0.1/
--rw-rw-rw-   0        0        0       82 2023-04-13 03:10:00.000000 PyDesmos-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2023-04-13 03:39:08.000000 PyDesmos-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1872 2023-04-13 03:39:52.531593 PyDesmos-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 03:39:52.515636 PyDesmos-0.0.1/PyDesmos/
--rw-rw-rw-   0        0        0     6843 2023-04-13 03:34:16.000000 PyDesmos-0.0.1/PyDesmos/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.1/PyDesmos/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-13 03:39:52.530596 PyDesmos-0.0.1/PyDesmos.egg-info/
--rw-rw-rw-   0        0        0     1872 2023-04-13 03:39:52.000000 PyDesmos-0.0.1/PyDesmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 03:39:52.000000 PyDesmos-0.0.1/PyDesmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:39:52.000000 PyDesmos-0.0.1/PyDesmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 03:39:52.000000 PyDesmos-0.0.1/PyDesmos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 03:39:52.000000 PyDesmos-0.0.1/PyDesmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1179 2023-04-13 03:38:28.000000 PyDesmos-0.0.1/README.md
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.1/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 03:39:52.532591 PyDesmos-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-04-13 03:39:47.000000 PyDesmos-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:46:32.826739 PyDesmos-0.0.2/
+-rw-rw-rw-   0        0        0      147 2023-04-13 03:46:15.000000 PyDesmos-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2023-04-13 03:39:08.000000 PyDesmos-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1937 2023-04-13 03:46:32.825742 PyDesmos-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 03:46:32.805795 PyDesmos-0.0.2/PyDesmos/
+-rw-rw-rw-   0        0        0     6843 2023-04-13 03:34:16.000000 PyDesmos-0.0.2/PyDesmos/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.2/PyDesmos/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-13 03:46:32.824744 PyDesmos-0.0.2/PyDesmos.egg-info/
+-rw-rw-rw-   0        0        0     1937 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1179 2023-04-13 03:38:28.000000 PyDesmos-0.0.2/README.md
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.2/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:46:32.826739 PyDesmos-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-04-13 03:45:57.000000 PyDesmos-0.0.2/setup.py
```

### Comparing `PyDesmos-0.0.1/LICENSE.txt` & `PyDesmos-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.1/PKG-INFO` & `PyDesmos-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy-to-use python to desmos html compiler via the desmos api.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -39,7 +39,11 @@
 
 Change Log
 ==========
 
 0.0.1 (12/04/2023)
 -------------------
 - First Release
+
+0.0.2 (12/04/2023)
+-------------------
+- Fixed requirements
```

### Comparing `PyDesmos-0.0.1/PyDesmos/__init__.py` & `PyDesmos-0.0.2/PyDesmos/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.1/PyDesmos/logo.png` & `PyDesmos-0.0.2/PyDesmos/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.1/PyDesmos.egg-info/PKG-INFO` & `PyDesmos-0.0.2/PyDesmos.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy-to-use python to desmos html compiler via the desmos api.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -39,7 +39,11 @@
 
 Change Log
 ==========
 
 0.0.1 (12/04/2023)
 -------------------
 - First Release
+
+0.0.2 (12/04/2023)
+-------------------
+- Fixed requirements
```

### Comparing `PyDesmos-0.0.1/README.md` & `PyDesmos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.1/logo.png` & `PyDesmos-0.0.2/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.1/setup.py` & `PyDesmos-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='PyDesmos',
-    version='0.0.1',
+    version='0.0.2',
     description='An easy-to-use python to desmos html compiler via the desmos api.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
     keywords=['math', 'graph', 'desmos', 'graphing software', 'html', 'sympy'],
     classifiers=classifiers,
     packages=find_packages(),
-    install_requires=['sympy', 'webbrowser']
+    install_requires=['sympy']
 )
```

