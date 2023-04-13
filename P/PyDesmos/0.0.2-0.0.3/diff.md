# Comparing `tmp/PyDesmos-0.0.2.tar.gz` & `tmp/PyDesmos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDesmos-0.0.2.tar", last modified: Thu Apr 13 03:46:32 2023, max compression
+gzip compressed data, was "PyDesmos-0.0.3.tar", last modified: Thu Apr 13 03:53:42 2023, max compression
```

## Comparing `PyDesmos-0.0.2.tar` & `PyDesmos-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:46:32.826739 PyDesmos-0.0.2/
--rw-rw-rw-   0        0        0      147 2023-04-13 03:46:15.000000 PyDesmos-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2023-04-13 03:39:08.000000 PyDesmos-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1937 2023-04-13 03:46:32.825742 PyDesmos-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 03:46:32.805795 PyDesmos-0.0.2/PyDesmos/
--rw-rw-rw-   0        0        0     6843 2023-04-13 03:34:16.000000 PyDesmos-0.0.2/PyDesmos/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.2/PyDesmos/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-13 03:46:32.824744 PyDesmos-0.0.2/PyDesmos.egg-info/
--rw-rw-rw-   0        0        0     1937 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 03:46:32.000000 PyDesmos-0.0.2/PyDesmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1179 2023-04-13 03:38:28.000000 PyDesmos-0.0.2/README.md
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.2/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 03:46:32.826739 PyDesmos-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-04-13 03:45:57.000000 PyDesmos-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 03:53:42.394868 PyDesmos-0.0.3/
+-rw-rw-rw-   0        0        0      213 2023-04-13 03:53:18.000000 PyDesmos-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       37 2023-04-13 03:39:08.000000 PyDesmos-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2003 2023-04-13 03:53:42.393870 PyDesmos-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 03:53:42.376915 PyDesmos-0.0.3/PyDesmos/
+-rw-rw-rw-   0        0        0     6777 2023-04-13 03:52:47.000000 PyDesmos-0.0.3/PyDesmos/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.3/PyDesmos/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-13 03:53:42.392872 PyDesmos-0.0.3/PyDesmos.egg-info/
+-rw-rw-rw-   0        0        0     2003 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1179 2023-04-13 03:38:28.000000 PyDesmos-0.0.3/README.md
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.3/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-13 03:53:42.394868 PyDesmos-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-04-13 03:53:04.000000 PyDesmos-0.0.3/setup.py
```

### Comparing `PyDesmos-0.0.2/LICENSE.txt` & `PyDesmos-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.2/PKG-INFO` & `PyDesmos-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy-to-use python to desmos html compiler via the desmos api.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,7 +43,11 @@
 0.0.1 (12/04/2023)
 -------------------
 - First Release
 
 0.0.2 (12/04/2023)
 -------------------
 - Fixed requirements
+
+0.0.3 (12/04/2023)
+-------------------
+- Removed broken logo
```

### Comparing `PyDesmos-0.0.2/PyDesmos/__init__.py` & `PyDesmos-0.0.3/PyDesmos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 
 
 class Graph:
     def __init__(self, graph_name='temp', api_key="dcb31709b452b1cf9dc26972add0fda6"):
         self.graph_name = graph_name
         self.file_name = graph_name + '.html'
         self.html = f'<body style="background-color:#2A2A2A;" marginwidth="0px" marginheight="0px">\n' \
-                    f'<center><img src="logo.png"></center>\n' \
                     f'<script src="https://www.desmos.com/api/v1.7/calculator.js?apiKey={api_key}"></script>\n' \
                     f'<div id="calculator"></div>\n' \
                     f'<script>\n' \
                     f'var elt = document.getElementById("calculator");\n' \
                     f'var calculator = Desmos.GraphingCalculator(elt);\n'
         self.expressions = 0
         for key, value in desmos_symbols.items():
```

### Comparing `PyDesmos-0.0.2/PyDesmos/logo.png` & `PyDesmos-0.0.3/PyDesmos/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.2/PyDesmos.egg-info/PKG-INFO` & `PyDesmos-0.0.3/PyDesmos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy-to-use python to desmos html compiler via the desmos api.
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,7 +43,11 @@
 0.0.1 (12/04/2023)
 -------------------
 - First Release
 
 0.0.2 (12/04/2023)
 -------------------
 - Fixed requirements
+
+0.0.3 (12/04/2023)
+-------------------
+- Removed broken logo
```

### Comparing `PyDesmos-0.0.2/README.md` & `PyDesmos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.2/logo.png` & `PyDesmos-0.0.3/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.2/setup.py` & `PyDesmos-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='PyDesmos',
-    version='0.0.2',
+    version='0.0.3',
     description='An easy-to-use python to desmos html compiler via the desmos api.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
```

