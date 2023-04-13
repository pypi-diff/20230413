# Comparing `tmp/powerk8s-0.7.0.tar.gz` & `tmp/powerk8s-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerk8s-0.7.0.tar", max compression
+gzip compressed data, was "powerk8s-0.8.0.tar", max compression
```

## Comparing `powerk8s-0.7.0.tar` & `powerk8s-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2022-11-11 20:41:58.276193 powerk8s-0.7.0/LICENSE
--rw-r--r--   0        0        0     2203 2022-11-11 20:41:58.276193 powerk8s-0.7.0/README.md
--rw-r--r--   0        0        0     3625 2022-11-11 20:41:58.280193 powerk8s-0.7.0/powerk8s.py
--rw-r--r--   0        0        0      910 2022-11-11 20:41:58.280193 powerk8s-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 powerk8s-0.7.0/setup.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 powerk8s-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-13 19:29:43.786850 powerk8s-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2203 2023-04-13 19:29:43.786850 powerk8s-0.8.0/README.md
+-rw-r--r--   0        0        0     3580 2023-04-13 19:29:43.786850 powerk8s-0.8.0/powerk8s.py
+-rw-r--r--   0        0        0      842 2023-04-13 19:29:43.786850 powerk8s-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 powerk8s-0.8.0/PKG-INFO
```

### Comparing `powerk8s-0.7.0/LICENSE` & `powerk8s-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powerk8s-0.7.0/README.md` & `powerk8s-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `powerk8s-0.7.0/powerk8s.py` & `powerk8s-0.8.0/powerk8s.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
 KUBERNETES_LOGO: str = "\U00002388 "
 
 
 class SegmentArg(Enum):
     """All possible Powerline segment argument types for Powerk8s."""
 
-    SHOW_KUBERNETES_LOGO: str = "show_kube_logo"
-    SHOW_CLUSTER: str = "show_cluster"
-    SHOW_NAMESPACE: str = "show_namespace"
-    SHOW_DEFAULT_NAMESPACE: str = "show_default_namespace"
+    SHOW_KUBERNETES_LOGO = "show_kube_logo"
+    SHOW_CLUSTER = "show_cluster"
+    SHOW_NAMESPACE = "show_namespace"
+    SHOW_DEFAULT_NAMESPACE = "show_default_namespace"
 
 
 class HighlightGroup(Enum):
     """All possible highlight groups for Powerk8s."""
 
-    KUBERNETES_CLUSTER_ALERT: str = "kubernetes_cluster:alert"
-    KUBERNETES_CLUSTER: str = "kubernetes_cluster"
-    KUBERNETES_DIVIDER: str = "kubernetes:divider"
-    KUBERNETES_NAMESPACE_ALERT: str = "kubernetes_namespace:alert"
-    KUBERNETES_NAMESPACE: str = "kubernetes_namespace"
+    KUBERNETES_CLUSTER_ALERT = "kubernetes_cluster:alert"
+    KUBERNETES_CLUSTER = "kubernetes_cluster"
+    KUBERNETES_DIVIDER = "kubernetes:divider"
+    KUBERNETES_NAMESPACE_ALERT = "kubernetes_namespace:alert"
+    KUBERNETES_NAMESPACE = "kubernetes_namespace"
 
 
 @dataclass
 class SegmentData:
     """Encapsulates data for a Powerk8s segment."""
 
     # pylint: disable=unsubscriptable-object
```

### Comparing `powerk8s-0.7.0/pyproject.toml` & `powerk8s-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 [tool.poetry]
 name = "powerk8s"
-version = "0.7.0"
+version = "0.8.0"
 description = "Powerline Segment for Kubernetes"
 authors = ["George Kontridze <george.kontridze@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gkze/powerk8s"
 repository = "https://github.com/gkze/powerk8s"
 documentation = "https://gkze.github.io/powerk8s/powerk8s.html"
 keywords = ["kubernetes", "powerline", "tools"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyYAML = "^6.0"
-kubernetes = ">=24.2,<26.0"
+kubernetes = "^26.1"
 powerline-status = "^2.7"
 
 [tool.poetry.dev-dependencies]
-pdoc = "^12.0"
-pymultilint = "^0.14"
+pdoc = "^13.1"
+pymultilint = "^1.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.multilint]
 src_paths = ["*.py"]
 
 [tool.autoflake]
-recursive = true
-in_place = true
-ignore_init_module_imports = true
-remove_all_unused_imports = true
-remove_unused_variables = true
-verbose = true
+in-place = true
+remove-unused-variables = true
+remove-rhs-for-unused-variables = true
 
 [tool.mypy]
 files = ["*.py"]
```

### Comparing `powerk8s-0.7.0/PKG-INFO` & `powerk8s-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: powerk8s
-Version: 0.7.0
+Version: 0.8.0
 Summary: Powerline Segment for Kubernetes
 Home-page: https://github.com/gkze/powerk8s
 License: MIT
 Keywords: kubernetes,powerline,tools
 Author: George Kontridze
 Author-email: george.kontridze@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: kubernetes (>=24.2,<26.0)
+Requires-Dist: kubernetes (>=26.1,<27.0)
 Requires-Dist: powerline-status (>=2.7,<3.0)
 Project-URL: Documentation, https://gkze.github.io/powerk8s/powerk8s.html
 Project-URL: Repository, https://github.com/gkze/powerk8s
 Description-Content-Type: text/markdown
 
 # ☸️ powerk8s: Powerline Plugin for Kubernetes ☸️
```

