# Comparing `tmp/turbx-0.1.2.tar.gz` & `tmp/turbx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.1.2.tar", last modified: Fri Jul  1 07:56:36 2022, max compression
+gzip compressed data, was "turbx-0.2.1.tar", last modified: Thu Apr 13 18:11:17 2023, max compression
```

## Comparing `turbx-0.1.2.tar` & `turbx-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2022-07-01 07:56:36.581682 turbx-0.1.2/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.1.2/LICENSE
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2348 2022-07-01 07:56:36.579794 turbx-0.1.2/PKG-INFO
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1061 2022-07-01 07:43:09.000000 turbx-0.1.2/README.md
--rwxrwxrwx   0 jason     (1000) jason     (1000)       38 2022-07-01 07:56:36.581682 turbx-0.1.2/setup.cfg
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2310 2022-07-01 07:56:06.000000 turbx-0.1.2/setup.py
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2022-07-01 07:56:36.490820 turbx-0.1.2/turbx/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     1814 2022-07-01 07:55:44.000000 turbx-0.1.2/turbx/__init__.py
--rwxrwxrwx   0 jason     (1000) jason     (1000)   607025 2022-06-30 19:44:03.000000 turbx-0.1.2/turbx/turbx.py
-drwxrwxrwx   0 jason     (1000) jason     (1000)        0 2022-07-01 07:56:36.565704 turbx-0.1.2/turbx.egg-info/
--rwxrwxrwx   0 jason     (1000) jason     (1000)     2348 2022-07-01 07:56:35.000000 turbx-0.1.2/turbx.egg-info/PKG-INFO
--rwxrwxrwx   0 jason     (1000) jason     (1000)      203 2022-07-01 07:56:36.000000 turbx-0.1.2/turbx.egg-info/SOURCES.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)        1 2022-07-01 07:56:36.000000 turbx-0.1.2/turbx.egg-info/dependency_links.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)      143 2022-07-01 07:56:36.000000 turbx-0.1.2/turbx.egg-info/requires.txt
--rwxrwxrwx   0 jason     (1000) jason     (1000)        6 2022-07-01 07:56:36.000000 turbx-0.1.2/turbx.egg-info/top_level.txt
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-13 18:11:17.748169 turbx-0.2.1/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.2.1/LICENSE
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2342 2023-04-13 18:11:17.748169 turbx-0.2.1/PKG-INFO
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1061 2022-07-01 07:43:09.000000 turbx-0.2.1/README.md
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2023-04-13 18:11:17.748169 turbx-0.2.1/setup.cfg
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-04-13 18:04:16.000000 turbx-0.2.1/setup.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-13 18:11:17.748169 turbx-0.2.1/turbx/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2937 2023-04-13 18:06:57.000000 turbx-0.2.1/turbx/__init__.py
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1088399 2023-04-13 18:00:07.000000 turbx-0.2.1/turbx/turbx.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-13 18:11:17.748169 turbx-0.2.1/turbx.egg-info/
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2342 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/PKG-INFO
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      143 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/requires.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.1.2/LICENSE` & `turbx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.1.2/PKG-INFO` & `turbx-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.1.2
-Summary: Tools for analysis of turbulent flow datasets.
+Version: 0.2.1
+Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
-Author: Jason Appelbaum
-Maintainer: Jason Appelbaum
+Author: Jason A
+Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `turbx-0.1.2/README.md` & `turbx-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `turbx-0.1.2/setup.py` & `turbx-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 from setuptools import setup
 import sys
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.1.2',
-    description='Tools for analysis of turbulent flow datasets.',
+    version='0.2.1',
+    description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
-    author='Jason Appelbaum',
-    maintainer='Jason Appelbaum',
-    #author_email='jason.appelbaum@icloud.com',
+    author='Jason A',
+    maintainer='Jason A',
+    #author_email='johndoe@gmail.com',
     license='MIT',
     packages=['turbx'],
-    #packages=find_packages(exclude=("tests",)),
+    #packages=find_packages(exclude=('tests',)),
     install_requires=['mpi4py>=3.1',
                       'numpy>=1.22',
                       'scipy>=1.8',
                       'h5py>=3.6',
-                      'matplotlib>=3.5',
+                      'matplotlib>=3.6',
                       'scikit-image>=0.19',
                       'psutil>=5.9',
                       'tqdm>=4.64',
                       'cmocean>=2.0',
                       'colorcet>=3.0',
                       'cmasher>=1.6',
                       ],
```

### Comparing `turbx-0.1.2/turbx.egg-info/PKG-INFO` & `turbx-0.2.1/turbx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.1.2
-Summary: Tools for analysis of turbulent flow datasets.
+Version: 0.2.1
+Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
-Author: Jason Appelbaum
-Maintainer: Jason Appelbaum
+Author: Jason A
+Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

