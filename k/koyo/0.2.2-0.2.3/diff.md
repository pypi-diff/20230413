# Comparing `tmp/koyo-0.2.2.tar.gz` & `tmp/koyo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koyo-0.2.2.tar", last modified: Thu Apr 13 13:55:21 2023, max compression
+gzip compressed data, was "koyo-0.2.3.tar", last modified: Thu Apr 13 17:17:48 2023, max compression
```

## Comparing `koyo-0.2.2.tar` & `koyo-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.660050 koyo-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.648050 koyo-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.648050 koyo-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-13 13:55:02.000000 koyo-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-13 13:55:02.000000 koyo-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 13:55:02.000000 koyo-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 13:55:21.660050 koyo-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 13:55:02.000000 koyo-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 13:55:02.000000 koyo-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:55:21.660050 koyo-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.648050 koyo-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.656050 koyo-0.2.2/src/koyo/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.656050 koyo-0.2.2/src/koyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.660050 koyo-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_koyo.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.570429 koyo-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.562429 koyo-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.566429 koyo-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-13 17:17:34.000000 koyo-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-13 17:17:34.000000 koyo-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-13 17:17:34.000000 koyo-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 17:17:34.000000 koyo-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 17:17:48.570429 koyo-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 17:17:34.000000 koyo-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-13 17:17:34.000000 koyo-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:17:48.570429 koyo-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.562429 koyo-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.566429 koyo-0.2.3/src/koyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 17:17:34.000000 koyo-0.2.3/src/koyo/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.570429 koyo-0.2.3/src/koyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 17:17:48.000000 koyo-0.2.3/src/koyo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:48.570429 koyo-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_koyo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 17:17:34.000000 koyo-0.2.3/tests/test_utilities.py
```

### Comparing `koyo-0.2.2/.github/workflows/ci.yml` & `koyo-0.2.3/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -122,12 +122,12 @@
           twine check dist/*
           ls -lh dist
 
       - name: Build and publish
         run: twine upload dist/*
         env:
           TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.PYPI_ALL_TOKEN }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
 
       - uses: softprops/action-gh-release@v1
         with:
           generate_release_notes: true
```

### Comparing `koyo-0.2.2/.pre-commit-config.yaml` & `koyo-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/LICENSE` & `koyo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/PKG-INFO` & `koyo-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koyo-0.2.2/README.md` & `koyo-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/pyproject.toml` & `koyo-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -47,18 +47,17 @@
 ]
 dev = [
     "black",
     "ipython",
     "mypy",
     "pdbpp",
     "pre-commit",
-    "pytest-cov",
-    "pytest",
     "rich",
     "ruff",
+    "koyo[test]"
 ]
 
 [project.urls]
 homepage = "https://github.com/vandeplaslab/koyo"
 repository = "https://github.com/vandeplaslab/koyo"
 
 # same as console_scripts entry point
@@ -110,15 +109,14 @@
     "D401", # First line should be in imperative mood
     "D413", # Missing blank line after last section
     "D416", # Section name should end with a colon
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D", "S"]
-"setup.py" = ["D"]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = ["error"]
```

### Comparing `koyo-0.2.2/src/koyo/containers.py` & `koyo-0.2.3/src/koyo/containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/decorators.py` & `koyo-0.2.3/src/koyo/decorators.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/download.py` & `koyo-0.2.3/src/koyo/download.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/json.py` & `koyo-0.2.3/src/koyo/json.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/numpy.py` & `koyo-0.2.3/src/koyo/numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/secret.py` & `koyo-0.2.3/src/koyo/secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/timer.py` & `koyo-0.2.3/src/koyo/timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/toml.py` & `koyo-0.2.3/src/koyo/toml.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/typing.py` & `koyo-0.2.3/src/koyo/typing.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/utilities.py` & `koyo-0.2.3/src/koyo/utilities.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo/visuals.py` & `koyo-0.2.3/src/koyo/visuals.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/src/koyo.egg-info/PKG-INFO` & `koyo-0.2.3/src/koyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koyo-0.2.2/src/koyo.egg-info/SOURCES.txt` & `koyo-0.2.3/src/koyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/tests/test_containers.py` & `koyo-0.2.3/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/tests/test_numpy.py` & `koyo-0.2.3/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/tests/test_secret.py` & `koyo-0.2.3/tests/test_secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/tests/test_timer.py` & `koyo-0.2.3/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.2/tests/test_utilities.py` & `koyo-0.2.3/tests/test_utilities.py`

 * *Files identical despite different names*

