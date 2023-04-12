# Comparing `tmp/jaxrie-4.tar.gz` & `tmp/jaxrie-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-4.tar", last modified: Wed Apr 12 22:21:58 2023, max compression
+gzip compressed data, was "jaxrie-5.tar", last modified: Wed Apr 12 22:33:12 2023, max compression
```

## Comparing `jaxrie-4.tar` & `jaxrie-5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-4/README.md
--rw-r--r--   0        0        0     3959 2023-04-12 22:21:58.309314 jaxrie-4/pyproject.toml
--rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-4/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-12 22:20:31.621114 jaxrie-4/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      183 2023-04-07 20:42:03.402217 jaxrie-4/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-4/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-4/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-4/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-4/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-4/src/jaxrie/modules/__init__.py
--rw-r--r--   0        0        0     4816 2023-04-12 22:19:22.534152 jaxrie-4/src/jaxrie/modules/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-4/src/jaxrie/nets/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-4/src/jaxrie/nets/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-4/src/jaxrie/py.typed
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-4/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-5/README.md
+-rw-r--r--   0        0        0     3959 2023-04-12 22:33:12.584873 jaxrie-5/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-04-11 06:06:22.543202 jaxrie-5/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-12 22:32:34.319643 jaxrie-5/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-5/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-5/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     4749 2023-04-12 22:31:42.778318 jaxrie-5/src/jaxrie/manifold/euclidean.py
+-rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-5/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-5/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-5/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-5/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4816 2023-04-12 22:19:22.534152 jaxrie-5/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-5/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-5/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-5/src/jaxrie/py.typed
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-5/PKG-INFO
```

### Comparing `jaxrie-4/pyproject.toml` & `jaxrie-5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     "jaxlib>=0.4.6",
     "dm-haiku>=0.0.9",
     "optax>=0.1.4",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 dynamic = []
-version = "4"
+version = "5"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-4/src/jaxrie/manifold/base.py` & `jaxrie-5/src/jaxrie/manifold/base.py`

 * *Files identical despite different names*

### Comparing `jaxrie-4/src/jaxrie/manifold/lorentz.py` & `jaxrie-5/src/jaxrie/manifold/lorentz.py`

 * *Files identical despite different names*

### Comparing `jaxrie-4/src/jaxrie/manifold/math.py` & `jaxrie-5/src/jaxrie/manifold/math.py`

 * *Files identical despite different names*

### Comparing `jaxrie-4/src/jaxrie/manifold/stereographic.py` & `jaxrie-5/src/jaxrie/manifold/stereographic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-4/src/jaxrie/modules/basic.py` & `jaxrie-5/src/jaxrie/modules/basic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-4/src/jaxrie/nets/basic.py` & `jaxrie-5/src/jaxrie/nets/basic.py`

 * *Files identical despite different names*

