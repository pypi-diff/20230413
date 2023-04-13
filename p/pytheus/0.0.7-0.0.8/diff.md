# Comparing `tmp/pytheus-0.0.7.tar.gz` & `tmp/pytheus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.0.7.tar", last modified: Wed Apr 12 22:38:58 2023, max compression
+gzip compressed data, was "pytheus-0.0.8.tar", last modified: Thu Apr 13 00:45:36 2023, max compression
```

## Comparing `pytheus-0.0.7.tar` & `pytheus-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.914042 pytheus-0.0.7/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.7/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 22:38:58.913841 pytheus-0.0.7/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.7/README.md
--rw-r--r--   0 llandy     (501) staff       (20)     1089 2023-04-12 22:38:15.000000 pytheus-0.0.7/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.912402 pytheus-0.0.7/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.7/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.913302 pytheus-0.0.7/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.7/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.7/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.7/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.7/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-12 22:30:13.000000 pytheus-0.0.7/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    18563 2023-04-12 19:31:40.000000 pytheus-0.0.7/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.7/pytheus/registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      230 2023-04-12 22:36:32.000000 pytheus-0.0.7/pytheus/utils.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.912937 pytheus-0.0.7/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)      176 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-12 22:38:58.000000 pytheus-0.0.7/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-12 22:38:58.914089 pytheus-0.0.7/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.7/setup.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-12 22:38:58.913673 pytheus-0.0.7/tests/
--rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-04-12 22:30:37.000000 pytheus-0.0.7/tests/test_exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    22327 2023-04-12 19:31:40.000000 pytheus-0.0.7/tests/test_metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.7/tests/test_registry.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.964037 pytheus-0.0.8/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.8/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-13 00:45:36.963844 pytheus-0.0.8/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.8/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1089 2023-04-13 00:45:03.000000 pytheus-0.0.8/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.961103 pytheus-0.0.8/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.8/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.962678 pytheus-0.0.8/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.8/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.8/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.8/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.8/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-12 22:30:13.000000 pytheus-0.0.8/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    18655 2023-04-13 00:44:01.000000 pytheus-0.0.8/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.8/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      230 2023-04-12 22:36:32.000000 pytheus-0.0.8/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.961861 pytheus-0.0.8/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      176 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-13 00:45:36.964082 pytheus-0.0.8/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.8/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.963477 pytheus-0.0.8/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-04-12 22:30:37.000000 pytheus-0.0.8/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    22719 2023-04-13 00:36:59.000000 pytheus-0.0.8/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.8/tests/test_registry.py
```

### Comparing `pytheus-0.0.7/LICENSE` & `pytheus-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/PKG-INFO` & `pytheus-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.7
+Version: 0.0.8
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pytheus-0.0.7/README.md` & `pytheus-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/pyproject.toml` & `pytheus-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytheus"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Llandy Riveron Del Risco", email="llandy3d@gmail.com" },
 ]
 description = "playing with metrics"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pytheus-0.0.7/pytheus/backends/base.py` & `pytheus-0.0.8/pytheus/backends/base.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/pytheus/backends/redis.py` & `pytheus-0.0.8/pytheus/backends/redis.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/pytheus/exposition.py` & `pytheus-0.0.8/pytheus/exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/pytheus/metrics.py` & `pytheus-0.0.8/pytheus/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,37 +221,38 @@
         if self._collector._default_labels:
             default_labels = self._collector._default_labels.copy()
             default_labels.update(labels_)
             labels_count = len(default_labels)
         else:
             labels_count = len(labels_)
 
+        # __init__ arguments for the child
+        child_kwargs = {
+            "name": self.name,
+            "description": self.description,
+            "collector": self._collector,
+            "labels": labels_,
+            "registry": self._registry,
+        }
+
+        # pass down buckets list to the child
+        if isinstance(self, Histogram):
+            child_kwargs["buckets"] = self._upper_bounds
+
         assert self._collector._required_labels is not None
         if labels_count != len(self._collector._required_labels):
             # does not add to collector
-            return self.__class__(
-                self.name,
-                self.description,
-                collector=self._collector,
-                labels=labels_,
-                registry=self._registry,
-            )
+            return self.__class__(**child_kwargs)  # type: ignore
 
         # add to collector
         sorted_label_values = tuple(v for _, v in sorted(labels_.items()))
         if sorted_label_values in self._collector._labeled_metrics:
             metric = self._collector._labeled_metrics[sorted_label_values]
         else:
-            metric = self.__class__(
-                self.name,
-                self.description,
-                collector=self._collector,
-                labels=labels_,
-                registry=self._registry,
-            )
+            metric = self.__class__(**child_kwargs)  # type: ignore
             self._collector._labeled_metrics[sorted_label_values] = metric
         return metric
 
     def collect(self) -> Iterable[Sample]:
         raise NotImplementedError
 
     def _get_sample(self) -> Sample:
```

### Comparing `pytheus-0.0.7/pytheus/registry.py` & `pytheus-0.0.8/pytheus/registry.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/pytheus.egg-info/PKG-INFO` & `pytheus-0.0.8/pytheus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.7
+Version: 0.0.8
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pytheus-0.0.7/tests/test_exposition.py` & `pytheus-0.0.8/tests/test_exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.7/tests/test_metrics.py` & `pytheus-0.0.8/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,14 +516,21 @@
         histogram = Histogram("name", "desc", required_labels=["bob"])
         histogram = histogram.labels({"bob": "cat"})
         assert histogram._sum is not None
         assert histogram._count is not None
         assert histogram._buckets is not None
         assert len(histogram._buckets) == len(histogram._upper_bounds)
 
+    def test_labeled_observable_respects_custom_buckets(self):
+        buckets = [0.2, 0.5, 1]
+        histogram = Histogram("name", "desc", required_labels=["bob"], buckets=buckets)
+        child_histogram = histogram.labels({"bob": "cat"})
+        assert child_histogram._upper_bounds == histogram._upper_bounds
+        assert len(child_histogram._buckets) == len(histogram._upper_bounds)
+
     def test_collect(self):
         buckets = [0.2, 0.5, 1]
         histogram = Histogram("name", "desc", buckets=buckets)
         samples = histogram.collect()
         samples = list(samples)
 
         assert "le" in samples[0].labels
```

### Comparing `pytheus-0.0.7/tests/test_registry.py` & `pytheus-0.0.8/tests/test_registry.py`

 * *Files identical despite different names*

