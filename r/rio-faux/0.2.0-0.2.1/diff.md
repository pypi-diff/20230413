# Comparing `tmp/rio-faux-0.2.0.tar.gz` & `tmp/rio-faux-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-faux-0.2.0.tar", last modified: Tue Oct 25 16:15:17 2022, max compression
+gzip compressed data, was "rio-faux-0.2.1.tar", last modified: Thu Apr 13 16:56:51 2023, max compression
```

## Comparing `rio-faux-0.2.0.tar` & `rio-faux-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      212 2022-10-25 16:15:04.345990 rio-faux-0.2.0/.bumpversion.cfg
--rw-r--r--   0        0        0      136 2022-10-25 16:15:04.345990 rio-faux-0.2.0/.flake8
--rw-r--r--   0        0        0     1172 2022-10-25 16:15:04.345990 rio-faux-0.2.0/.gitignore
--rw-r--r--   0        0        0      674 2022-10-25 16:15:04.345990 rio-faux-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1517 2022-10-25 16:15:04.345990 rio-faux-0.2.0/LICENSE
--rw-r--r--   0        0        0     2663 2022-10-25 16:15:04.345990 rio-faux-0.2.0/README.md
--rw-r--r--   0        0        0     1618 2022-10-25 16:15:04.345990 rio-faux-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       60 2022-10-25 16:15:04.345990 rio-faux-0.2.0/rio_faux/__init__.py
--rw-r--r--   0        0        0     4311 2022-10-25 16:15:04.345990 rio-faux-0.2.0/rio_faux/cli.py
--rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 rio-faux-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-04-13 16:56:40.102023 rio-faux-0.2.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2023-04-13 16:56:40.102023 rio-faux-0.2.1/.gitignore
+-rw-r--r--   0        0        0      822 2023-04-13 16:56:40.102023 rio-faux-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1517 2023-04-13 16:56:40.102023 rio-faux-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2663 2023-04-13 16:56:40.102023 rio-faux-0.2.1/README.md
+-rw-r--r--   0        0        0     2094 2023-04-13 16:56:40.102023 rio-faux-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-04-13 16:56:40.102023 rio-faux-0.2.1/rio_faux/__init__.py
+-rw-r--r--   0        0        0     5183 2023-04-13 16:56:40.102023 rio-faux-0.2.1/rio_faux/cli.py
+-rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 rio-faux-0.2.1/PKG-INFO
```

### Comparing `rio-faux-0.2.0/.gitignore` & `rio-faux-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rio-faux-0.2.0/LICENSE` & `rio-faux-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rio-faux-0.2.0/README.md` & `rio-faux-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rio-faux-0.2.0/pyproject.toml` & `rio-faux-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ]
 
 [project.urls]
 Source = "https://github.com/cogeotiff/rio-faux"
 Documentation = "https://cogeotiff.github.io/rio-faux/"
 
 [project.entry-points."rasterio.rio_plugins"]
-cogeo = "rio_faux.cli:faux"
+faux = "rio_faux.cli:faux"
 
 [build-system]
 requires = ["flit>=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.module]
 name = "rio_faux"
@@ -58,20 +58,40 @@
     ".github/",
     "CHANGES.md",
     "codecov.yml",
     "CONTRIBUTING.md",
     "mkdocs.yml",
 ]
 
+[tool.coverage.run]
+branch = true
+parallel = true
+
+[tool.coverage.report]
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
 [tool.isort]
 profile = "black"
 known_first_party = ["rio_fake"]
 known_third_party = ["rasterio", "click"]
 default_section = "THIRDPARTY"
 
 [tool.mypy]
-no_strict_optional = "True"
-ignore_missing_imports = "True"
+no_strict_optional = true
 
-[tool.pydocstyle]
-select = "D1"
-match = "(?!test).*.py"
+[tool.ruff]
+select = [
+    "D1",  # pydocstyle errors
+    "E",  # pycodestyle errors
+    "W",  # pycodestyle warnings
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+]
+ignore = [
+    "E501",  # line too long, handled by black
+    "B008",  # do not perform function calls in argument defaults
+    "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
+]
```

### Comparing `rio-faux-0.2.0/PKG-INFO` & `rio-faux-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-faux
-Version: 0.2.0
+Version: 0.2.1
 Summary: Create empty image from a model.
 Keywords: rasterio
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rio-faux Version: 0.2.0 Summary: Create empty image
+Metadata-Version: 2.1 Name: rio-faux Version: 0.2.1 Summary: Create empty image
 from a model. Keywords: rasterio Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

