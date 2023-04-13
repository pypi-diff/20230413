# Comparing `tmp/PyDesmos-0.0.3.tar.gz` & `tmp/PyDesmos-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDesmos-0.0.3.tar", last modified: Thu Apr 13 03:53:42 2023, max compression
+gzip compressed data, was "PyDesmos-0.1.0.tar", last modified: Thu Apr 13 09:36:35 2023, max compression
```

## Comparing `PyDesmos-0.0.3.tar` & `PyDesmos-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:53:42.394868 PyDesmos-0.0.3/
--rw-rw-rw-   0        0        0      213 2023-04-13 03:53:18.000000 PyDesmos-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       37 2023-04-13 03:39:08.000000 PyDesmos-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2003 2023-04-13 03:53:42.393870 PyDesmos-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 03:53:42.376915 PyDesmos-0.0.3/PyDesmos/
--rw-rw-rw-   0        0        0     6777 2023-04-13 03:52:47.000000 PyDesmos-0.0.3/PyDesmos/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.3/PyDesmos/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-13 03:53:42.392872 PyDesmos-0.0.3/PyDesmos.egg-info/
--rw-rw-rw-   0        0        0     2003 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 03:53:42.000000 PyDesmos-0.0.3/PyDesmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1179 2023-04-13 03:38:28.000000 PyDesmos-0.0.3/README.md
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.0.3/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 03:53:42.394868 PyDesmos-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-04-13 03:53:04.000000 PyDesmos-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:36:35.979521 PyDesmos-0.1.0/
+-rw-rw-rw-   0        0        0      188 2023-04-13 09:35:45.000000 PyDesmos-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3530 2023-04-13 09:36:35.978523 PyDesmos-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 09:36:35.959574 PyDesmos-0.1.0/PyDesmos/
+-rw-rw-rw-   0        0        0     9189 2023-04-13 09:33:06.000000 PyDesmos-0.1.0/PyDesmos/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.0/PyDesmos/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-13 09:36:35.977526 PyDesmos-0.1.0/PyDesmos.egg-info/
+-rw-rw-rw-   0        0        0     3530 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 09:36:35.000000 PyDesmos-0.1.0/PyDesmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2725 2023-04-13 09:34:37.000000 PyDesmos-0.1.0/README.md
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.0/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:36:35.979521 PyDesmos-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      869 2023-04-13 09:34:52.000000 PyDesmos-0.1.0/setup.py
```

### Comparing `PyDesmos-0.0.3/LICENSE.txt` & `PyDesmos-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.3/PyDesmos/logo.png` & `PyDesmos-0.1.0/PyDesmos/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.3/logo.png` & `PyDesmos-0.1.0/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.0.3/setup.py` & `PyDesmos-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 classifiers = [
-    'Development Status :: 2 - Pre-Alpha',
+    'Development Status :: 3 - Alpha',
     'Intended Audience :: Education',
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='PyDesmos',
-    version='0.0.3',
-    description='An easy-to-use python to desmos html compiler via the desmos api.',
+    version='0.1.0',
+    description='An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
-    keywords=['math', 'graph', 'desmos', 'graphing software', 'html', 'sympy'],
+    keywords=['math', 'graph', 'desmos', 'graphing software', 'html', 'sympy', 'api'],
     classifiers=classifiers,
     packages=find_packages(),
     install_requires=['sympy']
 )
```

