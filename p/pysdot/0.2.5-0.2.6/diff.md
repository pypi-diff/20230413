# Comparing `tmp/pysdot-0.2.5.tar.gz` & `tmp/pysdot-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdot-0.2.5.tar", last modified: Mon Mar 13 15:40:41 2023, max compression
+gzip compressed data, was "pysdot-0.2.6.tar", last modified: Thu Apr 13 04:49:46 2023, max compression
```

## Comparing `pysdot-0.2.5.tar` & `pysdot-0.2.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.760716 pysdot-0.2.5/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       29 2023-01-20 07:48:21.000000 pysdot-0.2.5/MANIFEST.in
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      490 2023-03-13 15:40:41.760716 pysdot-0.2.5/PKG-INFO
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.752716 pysdot-0.2.5/pysdot/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     5417 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/OptimalTransport.py
--rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)    16769 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/PowerDiagram.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       86 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.756716 pysdot-0.2.5/pysdot/cpp/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       25 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/cpp/__init__.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      204 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/cpp/comb_types.h
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      295 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/cpp/cpp_module.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    14376 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/cpp/inferno_color_map.h
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    44123 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/cpp/pybind_sdot.cpp
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      719 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/cpp/pybind_sdot_Arfd.cpp
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.756716 pysdot-0.2.5/pysdot/domain_types/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     3094 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/domain_types/ConvexPolyhedraAssembly.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1230 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/domain_types/ScaledImage.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       98 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/domain_types/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.756716 pysdot-0.2.5/pysdot/radial_funcs/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      592 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/RadialFuncArfd.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      253 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/RadialFuncEntropy.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      264 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/RadialFuncInBall.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      256 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/RadialFuncPpWmR2.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      224 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/RadialFuncR2.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      222 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/RadialFuncUnit.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      268 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/radial_funcs/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.760716 pysdot-0.2.5/pysdot/solvers/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      630 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/solvers/CuPyx.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      929 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/solvers/Petsc.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      493 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/solvers/Scipy.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        0 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/solvers/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.760716 pysdot-0.2.5/pysdot/util/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     2557 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/util/FastMarching.py
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       39 2023-01-20 07:48:21.000000 pysdot-0.2.5/pysdot/util/__init__.py
-drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-03-13 15:40:41.756716 pysdot-0.2.5/pysdot.egg-info/
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      490 2023-03-13 15:40:41.000000 pysdot-0.2.5/pysdot.egg-info/PKG-INFO
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      930 2023-03-13 15:40:41.000000 pysdot-0.2.5/pysdot.egg-info/SOURCES.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        1 2023-03-13 15:40:41.000000 pysdot-0.2.5/pysdot.egg-info/dependency_links.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        6 2023-03-13 15:40:41.000000 pysdot-0.2.5/pysdot.egg-info/requires.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       68 2023-03-13 15:40:41.000000 pysdot-0.2.5/pysdot.egg-info/top_level.txt
--rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       38 2023-03-13 15:40:41.760716 pysdot-0.2.5/setup.cfg
--rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)     3372 2023-03-13 15:16:38.000000 pysdot-0.2.5/setup.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.432959 pysdot-0.2.6/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       29 2023-01-20 07:48:21.000000 pysdot-0.2.6/MANIFEST.in
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      490 2023-04-13 04:49:46.432959 pysdot-0.2.6/PKG-INFO
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.428959 pysdot-0.2.6/pysdot/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     5417 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/OptimalTransport.py
+-rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)    16769 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/PowerDiagram.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       86 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.428959 pysdot-0.2.6/pysdot/cpp/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       25 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/cpp/__init__.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      204 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/cpp/comb_types.h
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      295 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/cpp/cpp_module.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    14376 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/cpp/inferno_color_map.h
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)    44123 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/cpp/pybind_sdot.cpp
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      719 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/cpp/pybind_sdot_Arfd.cpp
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.428959 pysdot-0.2.6/pysdot/domain_types/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     3094 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/domain_types/ConvexPolyhedraAssembly.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     1230 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/domain_types/ScaledImage.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       98 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/domain_types/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.428959 pysdot-0.2.6/pysdot/radial_funcs/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      592 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/RadialFuncArfd.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      253 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/RadialFuncEntropy.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      264 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/RadialFuncInBall.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      256 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/RadialFuncPpWmR2.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      224 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/RadialFuncR2.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      222 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/RadialFuncUnit.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      268 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/radial_funcs/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.432959 pysdot-0.2.6/pysdot/solvers/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      630 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/solvers/CuPyx.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      929 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/solvers/Petsc.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      493 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/solvers/Scipy.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        0 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/solvers/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.432959 pysdot-0.2.6/pysdot/util/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)     2557 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/util/FastMarching.py
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       39 2023-01-20 07:48:21.000000 pysdot-0.2.6/pysdot/util/__init__.py
+drwxrwxr-x   0 leclerc   (1000) leclerc   (1000)        0 2023-04-13 04:49:46.428959 pysdot-0.2.6/pysdot.egg-info/
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      490 2023-04-13 04:49:46.000000 pysdot-0.2.6/pysdot.egg-info/PKG-INFO
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)      930 2023-04-13 04:49:46.000000 pysdot-0.2.6/pysdot.egg-info/SOURCES.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        1 2023-04-13 04:49:46.000000 pysdot-0.2.6/pysdot.egg-info/dependency_links.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)        6 2023-04-13 04:49:46.000000 pysdot-0.2.6/pysdot.egg-info/requires.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       68 2023-04-13 04:49:46.000000 pysdot-0.2.6/pysdot.egg-info/top_level.txt
+-rw-rw-r--   0 leclerc   (1000) leclerc   (1000)       38 2023-04-13 04:49:46.432959 pysdot-0.2.6/setup.cfg
+-rwxrwxr-x   0 leclerc   (1000) leclerc   (1000)     3372 2023-04-13 04:47:39.000000 pysdot-0.2.6/setup.py
```

### Comparing `pysdot-0.2.5/pysdot/OptimalTransport.py` & `pysdot-0.2.6/pysdot/OptimalTransport.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/PowerDiagram.py` & `pysdot-0.2.6/pysdot/PowerDiagram.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/cpp/inferno_color_map.h` & `pysdot-0.2.6/pysdot/cpp/inferno_color_map.h`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/cpp/pybind_sdot.cpp` & `pysdot-0.2.6/pysdot/cpp/pybind_sdot.cpp`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/cpp/pybind_sdot_Arfd.cpp` & `pysdot-0.2.6/pysdot/cpp/pybind_sdot_Arfd.cpp`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/domain_types/ConvexPolyhedraAssembly.py` & `pysdot-0.2.6/pysdot/domain_types/ConvexPolyhedraAssembly.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/domain_types/ScaledImage.py` & `pysdot-0.2.6/pysdot/domain_types/ScaledImage.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/radial_funcs/RadialFuncArfd.py` & `pysdot-0.2.6/pysdot/radial_funcs/RadialFuncArfd.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/solvers/CuPyx.py` & `pysdot-0.2.6/pysdot/solvers/CuPyx.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/solvers/Petsc.py` & `pysdot-0.2.6/pysdot/solvers/Petsc.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot/util/FastMarching.py` & `pysdot-0.2.6/pysdot/util/FastMarching.py`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/pysdot.egg-info/SOURCES.txt` & `pysdot-0.2.6/pysdot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysdot-0.2.5/setup.py` & `pysdot-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             subprocess.check_call(['git', 'clone', 'https://github.com/eigenteam/eigen-git-mirror.git', 'ext/eigen3'])
         if not os.path.isdir('./ext/pybind11'):
             subprocess.check_call(['git', 'clone', 'https://github.com/pybind/pybind11.git', 'ext/pybind11'])
         setuptools.command.build_py.build_py.run(self)
 
 setup(
     name='pysdot',
-    version='0.2.5',
+    version='0.2.6',
     packages=find_packages(exclude=[
         'hugo', 'ext', 'build', 'dist',
         'examples', 'results', 'tests'
     ]),
     cmdclass={
         'build_py': BuildPyCommand,
     },
```

