# Comparing `tmp/jaxrie-6.tar.gz` & `tmp/jaxrie-7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrie-6.tar", last modified: Thu Apr 13 02:06:37 2023, max compression
+gzip compressed data, was "jaxrie-7.tar", last modified: Thu Apr 13 02:13:07 2023, max compression
```

## Comparing `jaxrie-6.tar` & `jaxrie-7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-6/README.md
--rw-r--r--   0        0        0     3959 2023-04-13 02:06:37.149303 jaxrie-6/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-13 02:05:54.392649 jaxrie-6/src/jaxrie/__init__.py
--rw-r--r--   0        0        0       18 2023-04-13 02:06:07.285490 jaxrie-6/src/jaxrie/__version__.py
--rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-6/src/jaxrie/manifold/__init__.py
--rw-r--r--   0        0        0     4015 2023-04-11 05:01:03.595132 jaxrie-6/src/jaxrie/manifold/base.py
--rw-r--r--   0        0        0     4749 2023-04-12 22:31:42.778318 jaxrie-6/src/jaxrie/manifold/euclidean.py
--rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-6/src/jaxrie/manifold/lorentz.py
--rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-6/src/jaxrie/manifold/math.py
--rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-6/src/jaxrie/manifold/stereographic.py
--rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-6/src/jaxrie/modules/__init__.py
--rw-r--r--   0        0        0     4816 2023-04-12 22:19:22.534152 jaxrie-6/src/jaxrie/modules/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-6/src/jaxrie/nets/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-6/src/jaxrie/nets/basic.py
--rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-6/src/jaxrie/py.typed
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-6/PKG-INFO
+-rw-r--r--   0        0        0      114 2023-04-11 06:28:18.666689 jaxrie-7/README.md
+-rw-r--r--   0        0        0     3959 2023-04-13 02:13:07.887664 jaxrie-7/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-13 02:05:54.392649 jaxrie-7/src/jaxrie/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-13 02:12:42.523822 jaxrie-7/src/jaxrie/__version__.py
+-rw-r--r--   0        0        0      274 2023-04-12 22:32:25.869284 jaxrie-7/src/jaxrie/manifold/__init__.py
+-rw-r--r--   0        0        0     4120 2023-04-13 02:10:13.893763 jaxrie-7/src/jaxrie/manifold/base.py
+-rw-r--r--   0        0        0     4749 2023-04-12 22:31:42.778318 jaxrie-7/src/jaxrie/manifold/euclidean.py
+-rw-r--r--   0        0        0     1456 2023-03-14 02:52:02.061979 jaxrie-7/src/jaxrie/manifold/lorentz.py
+-rw-r--r--   0        0        0    22649 2023-04-11 05:00:33.822418 jaxrie-7/src/jaxrie/manifold/math.py
+-rw-r--r--   0        0        0     5304 2023-04-11 05:01:59.603887 jaxrie-7/src/jaxrie/manifold/stereographic.py
+-rw-r--r--   0        0        0       93 2023-04-11 06:05:54.838637 jaxrie-7/src/jaxrie/modules/__init__.py
+-rw-r--r--   0        0        0     4816 2023-04-12 22:19:22.534152 jaxrie-7/src/jaxrie/modules/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:52:43.064397 jaxrie-7/src/jaxrie/nets/__init__.py
+-rw-r--r--   0        0        0     2282 2023-04-12 22:18:13.252978 jaxrie-7/src/jaxrie/nets/basic.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:36:46.927134 jaxrie-7/src/jaxrie/py.typed
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 jaxrie-7/PKG-INFO
```

### Comparing `jaxrie-6/pyproject.toml` & `jaxrie-7/pyproject.toml`

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
-version = "6"
+version = "7"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `jaxrie-6/src/jaxrie/manifold/base.py` & `jaxrie-7/src/jaxrie/manifold/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 
 Array = jax.Array
 
 
 class Manifold(metaclass=ABCMeta):
   """Manifold base."""
 
+  @property
+  def name(self) -> str:
+    """Name of the manifold."""
+    return self.__class__.__name__
+
   @staticmethod
   @abstractmethod
   def add(x: Array, y: Array, k: ArrayLike, eps: float = EPS) -> Array:
     """Addition on manifold with curvature k."""
     raise NotImplementedError
 
   @staticmethod
```

### Comparing `jaxrie-6/src/jaxrie/manifold/euclidean.py` & `jaxrie-7/src/jaxrie/manifold/euclidean.py`

 * *Files identical despite different names*

### Comparing `jaxrie-6/src/jaxrie/manifold/lorentz.py` & `jaxrie-7/src/jaxrie/manifold/lorentz.py`

 * *Files identical despite different names*

### Comparing `jaxrie-6/src/jaxrie/manifold/math.py` & `jaxrie-7/src/jaxrie/manifold/math.py`

 * *Files identical despite different names*

### Comparing `jaxrie-6/src/jaxrie/manifold/stereographic.py` & `jaxrie-7/src/jaxrie/manifold/stereographic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-6/src/jaxrie/modules/basic.py` & `jaxrie-7/src/jaxrie/modules/basic.py`

 * *Files identical despite different names*

### Comparing `jaxrie-6/src/jaxrie/nets/basic.py` & `jaxrie-7/src/jaxrie/nets/basic.py`

 * *Files identical despite different names*

