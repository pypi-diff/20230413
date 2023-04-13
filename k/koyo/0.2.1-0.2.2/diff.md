# Comparing `tmp/koyo-0.2.1.tar.gz` & `tmp/koyo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koyo-0.2.1.tar", last modified: Thu Apr 13 13:48:54 2023, max compression
+gzip compressed data, was "koyo-0.2.2.tar", last modified: Thu Apr 13 13:55:21 2023, max compression
```

## Comparing `koyo-0.2.1.tar` & `koyo-0.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.207282 koyo-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.203282 koyo-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 13:48:36.000000 koyo-0.2.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 13:48:36.000000 koyo-0.2.1/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 13:48:36.000000 koyo-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.203282 koyo-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-13 13:48:36.000000 koyo-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-13 13:48:36.000000 koyo-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-13 13:48:36.000000 koyo-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 13:48:36.000000 koyo-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 13:48:54.207282 koyo-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 13:48:36.000000 koyo-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 13:48:36.000000 koyo-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:48:54.207282 koyo-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.199282 koyo-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.203282 koyo-0.2.1/src/koyo/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 13:48:54.000000 koyo-0.2.1/src/koyo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 13:48:36.000000 koyo-0.2.1/src/koyo/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.203282 koyo-0.2.1/src/koyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 13:48:54.000000 koyo-0.2.1/src/koyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 13:48:54.000000 koyo-0.2.1/src/koyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:48:54.000000 koyo-0.2.1/src/koyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 13:48:54.000000 koyo-0.2.1/src/koyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 13:48:54.000000 koyo-0.2.1/src/koyo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:48:54.207282 koyo-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_koyo.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 13:48:36.000000 koyo-0.2.1/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.660050 koyo-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.648050 koyo-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.648050 koyo-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-13 13:55:02.000000 koyo-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-13 13:55:02.000000 koyo-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-13 13:55:02.000000 koyo-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 13:55:02.000000 koyo-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 13:55:21.660050 koyo-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 13:55:02.000000 koyo-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 13:55:02.000000 koyo-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:55:21.660050 koyo-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.648050 koyo-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.656050 koyo-0.2.2/src/koyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-13 13:55:02.000000 koyo-0.2.2/src/koyo/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.656050 koyo-0.2.2/src/koyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 13:55:21.000000 koyo-0.2.2/src/koyo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:55:21.660050 koyo-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_koyo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-13 13:55:02.000000 koyo-0.2.2/tests/test_utilities.py
```

### Comparing `koyo-0.2.1/.github/workflows/ci.yml` & `koyo-0.2.2/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
       - uses: softprops/action-gh-release@v1
         with:
           generate_release_notes: true
 
   deploy:
     name: Deploy
-    needs: test
+    needs: deploy_test
     if: success() && startsWith(github.ref, 'refs/tags/') && github.event_name != 'schedule'
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
```

### Comparing `koyo-0.2.1/.pre-commit-config.yaml` & `koyo-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/LICENSE` & `koyo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/PKG-INFO` & `koyo-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koyo-0.2.1/README.md` & `koyo-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/pyproject.toml` & `koyo-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/containers.py` & `koyo-0.2.2/src/koyo/containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/decorators.py` & `koyo-0.2.2/src/koyo/decorators.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/download.py` & `koyo-0.2.2/src/koyo/download.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/image.py` & `koyo-0.2.2/src/koyo/image.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/json.py` & `koyo-0.2.2/src/koyo/json.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/numpy.py` & `koyo-0.2.2/src/koyo/numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/secret.py` & `koyo-0.2.2/src/koyo/secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/spectrum.py` & `koyo-0.2.2/src/koyo/spectrum.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/timer.py` & `koyo-0.2.2/src/koyo/timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/toml.py` & `koyo-0.2.2/src/koyo/toml.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/typing.py` & `koyo-0.2.2/src/koyo/typing.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/utilities.py` & `koyo-0.2.2/src/koyo/utilities.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo/visuals.py` & `koyo-0.2.2/src/koyo/visuals.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/src/koyo.egg-info/PKG-INFO` & `koyo-0.2.2/src/koyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koyo-0.2.1/src/koyo.egg-info/SOURCES.txt` & `koyo-0.2.2/src/koyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/tests/test_containers.py` & `koyo-0.2.2/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/tests/test_numpy.py` & `koyo-0.2.2/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/tests/test_secret.py` & `koyo-0.2.2/tests/test_secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/tests/test_timer.py` & `koyo-0.2.2/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.1/tests/test_utilities.py` & `koyo-0.2.2/tests/test_utilities.py`

 * *Files identical despite different names*

