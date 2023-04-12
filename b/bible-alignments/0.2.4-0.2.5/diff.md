# Comparing `tmp/bible_alignments-0.2.4.tar.gz` & `tmp/bible_alignments-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bible_alignments-0.2.4.tar", max compression
+gzip compressed data, was "bible_alignments-0.2.5.tar", max compression
```

## Comparing `bible_alignments-0.2.4.tar` & `bible_alignments-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.4/LICENSE
--rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.4/README.md
--rw-r--r--   0        0        0     1706 2023-04-12 23:36:29.238404 bible_alignments-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.4/src/.github/actions/run-checks/action.yml
--rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.4/src/.github/actions/setup-poetry-env/action.yml
--rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529246 bible_alignments-0.2.4/src/.github/workflows/on-merge-to-main.yml
--rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529365 bible_alignments-0.2.4/src/.github/workflows/on-pull-request.yml
--rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.4/src/.github/workflows/on-release-main.yml
--rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.4/src/.github/workflows/validate-codecov-config.yml
--rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.4/src/01-Exploration.ipynb
--rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.4/src/__init__.py
--rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.4/src/catalog.py
--rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.4/src/config.py
--rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.4/src/format/__init__.py
--rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.4/src/format/grapecity.py
--rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702956 bible_alignments-0.2.4/src/gcsource.py
--rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463180 bible_alignments-0.2.4/src/gctarget.py
--rw-r--r--   0        0        0     4536 2023-04-12 23:47:40.528641 bible_alignments-0.2.4/src/grapecity.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 bible_alignments-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.5/LICENSE
+-rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.5/README.md
+-rw-r--r--   0        0        0     1705 2023-04-12 23:54:12.663470 bible_alignments-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.5/src/.github/actions/run-checks/action.yml
+-rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.5/src/.github/actions/setup-poetry-env/action.yml
+-rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529246 bible_alignments-0.2.5/src/.github/workflows/on-merge-to-main.yml
+-rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529365 bible_alignments-0.2.5/src/.github/workflows/on-pull-request.yml
+-rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.5/src/.github/workflows/on-release-main.yml
+-rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.5/src/.github/workflows/validate-codecov-config.yml
+-rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.5/src/01-Exploration.ipynb
+-rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.5/src/__init__.py
+-rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.5/src/catalog.py
+-rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.5/src/config.py
+-rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.5/src/format/__init__.py
+-rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.5/src/format/grapecity.py
+-rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702956 bible_alignments-0.2.5/src/gcsource.py
+-rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463180 bible_alignments-0.2.5/src/gctarget.py
+-rw-r--r--   0        0        0     4536 2023-04-12 23:47:40.528641 bible_alignments-0.2.5/src/grapecity.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 bible_alignments-0.2.5/PKG-INFO
```

### Comparing `bible_alignments-0.2.4/LICENSE` & `bible_alignments-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/README.md` & `bible_alignments-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/pyproject.toml` & `bible_alignments-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bible-alignments"
-version = "0.2.4"
+version = "0.2.5"
 description = "Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments."
 authors = ["Sean Boisen <sean.boisen@clear.bible>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Bible", "alignment", "Bible alignment"]
 repository = "https://github.com/Clear-Bible/bible-alignments"
 #documentation = "https://sboisen.github.io/alignments/"
@@ -21,15 +21,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
+python = ">=3.7,<4.0"
 jsonlines = "^3.1.0"
 tomli = "^2.0.1"
 jupyterlab = "^3.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `bible_alignments-0.2.4/src/.github/actions/run-checks/action.yml` & `bible_alignments-0.2.5/src/.github/actions/run-checks/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/.github/actions/setup-poetry-env/action.yml` & `bible_alignments-0.2.5/src/.github/actions/setup-poetry-env/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/.github/workflows/on-merge-to-main.yml` & `bible_alignments-0.2.5/src/.github/workflows/on-merge-to-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/.github/workflows/on-pull-request.yml` & `bible_alignments-0.2.5/src/.github/workflows/on-pull-request.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/.github/workflows/on-release-main.yml` & `bible_alignments-0.2.5/src/.github/workflows/on-release-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/01-Exploration.ipynb` & `bible_alignments-0.2.5/src/01-Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/catalog.py` & `bible_alignments-0.2.5/src/catalog.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/format/grapecity.py` & `bible_alignments-0.2.5/src/format/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/gcsource.py` & `bible_alignments-0.2.5/src/gcsource.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/gctarget.py` & `bible_alignments-0.2.5/src/gctarget.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/src/grapecity.py` & `bible_alignments-0.2.5/src/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.4/PKG-INFO` & `bible_alignments-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: bible-alignments
-Version: 0.2.4
+Version: 0.2.5
 Summary: Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments.
 Home-page: https://github.com/Clear-Bible/bible-alignments
 License: MIT
 Keywords: Bible,alignment,Bible alignment
 Author: Sean Boisen
 Author-email: sean.boisen@clear.bible
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Religion
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Religion
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: jupyterlab (>=3.6.1,<4.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
```

