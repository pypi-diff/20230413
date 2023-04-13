# Comparing `tmp/crosspredict-1.1.6.tar.gz` & `tmp/crosspredict-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosspredict-1.1.6.tar", last modified: Wed Oct  5 07:01:08 2022, max compression
+gzip compressed data, was "crosspredict-1.1.7.tar", last modified: Thu Apr 13 14:28:36 2023, max compression
```

## Comparing `crosspredict-1.1.6.tar` & `crosspredict-1.1.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.485944 crosspredict-1.1.6/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1074 2022-09-26 07:29:13.000000 crosspredict-1.1.6/LICENSE
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       58 2022-09-26 07:29:13.000000 crosspredict-1.1.6/MANIFEST.in
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2022-10-05 07:01:08.485814 crosspredict-1.1.6/PKG-INFO
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5151 2022-09-26 07:59:16.000000 crosspredict-1.1.6/README.md
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.478003 crosspredict-1.1.6/crosspredict/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       44 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.478951 crosspredict-1.1.6/crosspredict/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      206 2022-09-26 08:25:52.000000 crosspredict-1.1.6/crosspredict/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     4094 2022-09-26 08:26:01.000000 crosspredict-1.1.6/crosspredict/__pycache__/iterator.cpython-39.pyc
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.480015 crosspredict-1.1.6/crosspredict/crossval/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      241 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/crossval/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.483074 crosspredict-1.1.6/crosspredict/crossval/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      380 2022-09-26 08:25:52.000000 crosspredict-1.1.6/crosspredict/crossval/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3213 2022-09-26 08:26:02.000000 crosspredict-1.1.6/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7803 2022-10-01 14:55:03.000000 crosspredict-1.1.6/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2885 2022-09-26 08:57:16.000000 crosspredict-1.1.6/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1763 2022-09-26 08:26:01.000000 crosspredict-1.1.6/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3869 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/crossval/_catboost.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    11666 2022-10-01 14:58:40.000000 crosspredict-1.1.6/crosspredict/crossval/_crossval.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3848 2022-09-26 08:57:01.000000 crosspredict-1.1.6/crosspredict/crossval/_lightgbm.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2331 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/crossval/_xgboost.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     4965 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/iterator.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.483415 crosspredict-1.1.6/crosspredict/nodes/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      215 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/nodes/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12526 2022-10-05 06:59:32.000000 crosspredict-1.1.6/crosspredict/nodes/_nodes.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1580 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/parameters.yml
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.483890 crosspredict-1.1.6/crosspredict/report_binary/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      138 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/report_binary/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.484518 crosspredict-1.1.6/crosspredict/report_binary/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      323 2022-09-26 08:27:01.000000 crosspredict-1.1.6/crosspredict/report_binary/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     8585 2022-09-26 08:27:01.000000 crosspredict-1.1.6/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     9111 2022-09-26 08:27:01.000000 crosspredict-1.1.6/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7860 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/report_binary/_curves.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12423 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/report_binary/_report_binary.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.484908 crosspredict-1.1.6/crosspredict/target_encoder/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      174 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/target_encoder/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2836 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/target_encoder/_crosstargetencoder.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3471 2022-09-26 07:29:13.000000 crosspredict-1.1.6/crosspredict/target_encoder/_target_encoder.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.478608 crosspredict-1.1.6/crosspredict.egg-info/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2022-10-05 07:01:08.000000 crosspredict-1.1.6/crosspredict.egg-info/PKG-INFO
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1470 2022-10-05 07:01:08.000000 crosspredict-1.1.6/crosspredict.egg-info/SOURCES.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)        1 2022-10-05 07:01:08.000000 crosspredict-1.1.6/crosspredict.egg-info/dependency_links.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      247 2022-10-05 07:01:08.000000 crosspredict-1.1.6/crosspredict.egg-info/requires.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       19 2022-10-05 07:01:08.000000 crosspredict-1.1.6/crosspredict.egg-info/top_level.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      246 2022-09-26 08:59:16.000000 crosspredict-1.1.6/requirements.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       38 2022-10-05 07:01:08.485986 crosspredict-1.1.6/setup.cfg
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1272 2022-10-05 07:00:36.000000 crosspredict-1.1.6/setup.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2022-10-05 07:01:08.485555 crosspredict-1.1.6/tests/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)        0 2022-09-26 07:29:13.000000 crosspredict-1.1.6/tests/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      556 2022-09-26 07:29:13.000000 crosspredict-1.1.6/tests/conftest.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7765 2022-09-26 08:47:46.000000 crosspredict-1.1.6/tests/test_binary.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2518 2022-09-26 07:29:13.000000 crosspredict-1.1.6/tests/test_iterator.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.817636 crosspredict-1.1.7/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1074 2022-09-26 07:29:13.000000 crosspredict-1.1.7/LICENSE
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       58 2022-09-26 07:29:13.000000 crosspredict-1.1.7/MANIFEST.in
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-04-13 14:28:36.817513 crosspredict-1.1.7/PKG-INFO
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5151 2022-09-26 07:59:16.000000 crosspredict-1.1.7/README.md
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.808367 crosspredict-1.1.7/crosspredict/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       44 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.809363 crosspredict-1.1.7/crosspredict/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      206 2022-09-26 08:25:52.000000 crosspredict-1.1.7/crosspredict/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     4094 2022-09-26 08:26:01.000000 crosspredict-1.1.7/crosspredict/__pycache__/iterator.cpython-39.pyc
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.810357 crosspredict-1.1.7/crosspredict/crossval/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      241 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/crossval/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.811351 crosspredict-1.1.7/crosspredict/crossval/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      380 2022-09-26 08:25:52.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3213 2022-09-26 08:26:02.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7803 2022-10-01 14:55:03.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2885 2022-09-26 08:57:16.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1763 2022-09-26 08:26:01.000000 crosspredict-1.1.7/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3869 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/crossval/_catboost.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12175 2023-04-13 13:11:46.000000 crosspredict-1.1.7/crosspredict/crossval/_crossval.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3848 2022-09-26 08:57:01.000000 crosspredict-1.1.7/crosspredict/crossval/_lightgbm.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2331 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/crossval/_xgboost.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     4965 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/iterator.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.811673 crosspredict-1.1.7/crosspredict/nodes/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      215 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/nodes/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12522 2023-04-13 13:11:46.000000 crosspredict-1.1.7/crosspredict/nodes/_nodes.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1580 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/parameters.yml
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.813274 crosspredict-1.1.7/crosspredict/report_binary/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      138 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/report_binary/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.814702 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      323 2022-09-26 08:27:01.000000 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     8585 2022-09-26 08:27:01.000000 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     9111 2022-09-26 08:27:01.000000 crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7896 2023-04-13 13:11:46.000000 crosspredict-1.1.7/crosspredict/report_binary/_curves.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12423 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/report_binary/_report_binary.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.815164 crosspredict-1.1.7/crosspredict/target_encoder/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      174 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/target_encoder/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2836 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/target_encoder/_crosstargetencoder.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3471 2022-09-26 07:29:13.000000 crosspredict-1.1.7/crosspredict/target_encoder/_target_encoder.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.809037 crosspredict-1.1.7/crosspredict.egg-info/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/PKG-INFO
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1470 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/SOURCES.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)        1 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/dependency_links.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      247 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/requires.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       19 2023-04-13 14:28:36.000000 crosspredict-1.1.7/crosspredict.egg-info/top_level.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      246 2022-09-26 08:59:16.000000 crosspredict-1.1.7/requirements.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       38 2023-04-13 14:28:36.817679 crosspredict-1.1.7/setup.cfg
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1272 2023-04-13 13:12:24.000000 crosspredict-1.1.7/setup.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-04-13 14:28:36.817190 crosspredict-1.1.7/tests/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)        0 2022-09-26 07:29:13.000000 crosspredict-1.1.7/tests/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      556 2022-09-26 07:29:13.000000 crosspredict-1.1.7/tests/conftest.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7765 2022-09-26 08:47:46.000000 crosspredict-1.1.7/tests/test_binary.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2518 2022-09-26 07:29:13.000000 crosspredict-1.1.7/tests/test_iterator.py
```

### Comparing `crosspredict-1.1.6/LICENSE` & `crosspredict-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/PKG-INFO` & `crosspredict-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosspredict
-Version: 1.1.6
+Version: 1.1.7
 Summary: package for easy crossvalidation
 Home-page: UNKNOWN
 Author: Vladislav Boyadzhi
 Author-email: vladislav.boyadzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crosspredict-1.1.6/README.md` & `crosspredict-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/__pycache__/iterator.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/__pycache__/iterator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/_catboost.py` & `crosspredict-1.1.7/crosspredict/crossval/_catboost.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/_crossval.py` & `crosspredict-1.1.7/crosspredict/crossval/_crossval.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,23 +138,33 @@
                 log.info(
                     f'\tCROSSVALIDATION FOLD {fold % self.iterator.n_splits} ENDS with best `{self.params["metric"]}` = {best_auc}')
 
         if self.valid:
             self.scores = pd.DataFrame(
                 dict([(k, pd.Series(v)) for k, v in scores.items()]))
             mask = self.scores.isnull().sum(axis=1) == 0
-            self.num_boost_optimal = np.argmax(
-                self.scores[mask].mean(axis=1).values)
-            self.score_max = self.scores[mask].mean(
-                axis=1)[self.num_boost_optimal]
+            if self.params['metric'] in ('auc'):
+                self.num_boost_optimal = np.argmax(self.scores[mask].mean(axis=1).values)
+
+            elif self.params['metric'] in (
+                'binary_logloss', 'binary', 'l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2',
+                'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse',
+                'root_mean_squared_error', 'l2_root'):
+                self.num_boost_optimal = np.argmin(self.scores[mask].mean(axis=1).values)
+
+            self.score_max = self.scores[mask].mean(axis=1)[self.num_boost_optimal]
+            loss = self.score_max
+            if self.params['metric'] in ('auc'):
+                loss = -self.score_max
+
             # self.score_max = np.mean(scores_avg)
             self.std = self.scores[mask].std(axis=1)[self.num_boost_optimal]
             # self.std = np.std(scores_avg)
 
-            result = {'loss': -self.score_max,
+            result = {'loss': loss,
                       'status': STATUS_OK,
                       'std': self.std,
                       'score_max': self.score_max,
                       'scores_all': scores_avg,
                       'num_boost': int(self.num_boost_optimal),
                       }
             log.info(result)
```

### Comparing `crosspredict-1.1.6/crosspredict/crossval/_lightgbm.py` & `crosspredict-1.1.7/crosspredict/crossval/_lightgbm.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/crossval/_xgboost.py` & `crosspredict-1.1.7/crosspredict/crossval/_xgboost.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/iterator.py` & `crosspredict-1.1.7/crosspredict/iterator.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/nodes/_nodes.py` & `crosspredict-1.1.7/crosspredict/nodes/_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                                              valid=True,
                                              random_state=0,
                                              col_target=col_target,
                                              cols_cat=cols_cat
                                              )
 
             result = model_class.fit(df)
-            score = result['score_max']
+            score = -result['loss']
 
             if score > top_score:
                 top_score = score
                 top_feature = f
 
         log.info("{} features left to select ...".format(len(set(feature_name) - set(selected_features)) - 1))
         scores.append(top_score)
```

### Comparing `crosspredict-1.1.6/crosspredict/parameters.yml` & `crosspredict-1.1.7/crosspredict/parameters.yml`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc` & `crosspredict-1.1.7/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/report_binary/_curves.py` & `crosspredict-1.1.7/crosspredict/report_binary/_curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         super().__init__(col_score, col_target, name=name)
         self.series_auc = None
         self._col_generation_deals = col_generation_deals
         self.count = None
 
     def fit(self, df):
         self.count = df.groupby(self._col_generation_deals).size()
-        self.series_auc = df[~df[self.col_score].isnull()].groupby(self._col_generation_deals).apply(
+        self.series_auc = df[(~df[self.col_score].isnull()) & (~df[self.col_target].isnull())].groupby(self._col_generation_deals).apply(
             lambda x: 100 * (2 * roc_auc_score(x[self.col_target], x[self.col_score]) - 1) if len(
                 x[self.col_target].unique()) > 1 else None)
         self.series_auc = self.series_auc.reindex(index=self.count.index)
         return self
 
     def plot(self, ax=None, title=None, **kwargs):
         ax_twinx = kwargs['ax_twinx']
```

### Comparing `crosspredict-1.1.6/crosspredict/report_binary/_report_binary.py` & `crosspredict-1.1.7/crosspredict/report_binary/_report_binary.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/target_encoder/_crosstargetencoder.py` & `crosspredict-1.1.7/crosspredict/target_encoder/_crosstargetencoder.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict/target_encoder/_target_encoder.py` & `crosspredict-1.1.7/crosspredict/target_encoder/_target_encoder.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/crosspredict.egg-info/PKG-INFO` & `crosspredict-1.1.7/crosspredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosspredict
-Version: 1.1.6
+Version: 1.1.7
 Summary: package for easy crossvalidation
 Home-page: UNKNOWN
 Author: Vladislav Boyadzhi
 Author-email: vladislav.boyadzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crosspredict-1.1.6/crosspredict.egg-info/SOURCES.txt` & `crosspredict-1.1.7/crosspredict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/setup.py` & `crosspredict-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open('{0}/requirements.txt'.format(dir_path), 'r') as reqs:
         requirements = reqs.readlines()
     return requirements
 
 if __name__ == "__main__":
     setup(
         name="crosspredict",
-        version="1.1.6",
+        version="1.1.7",
         author="Vladislav Boyadzhi",
         author_email="vladislav.boyadzhi@gmail.com",
         description='package for easy crossvalidation',
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=find_packages(),
         classifiers=[
```

### Comparing `crosspredict-1.1.6/tests/conftest.py` & `crosspredict-1.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/tests/test_binary.py` & `crosspredict-1.1.7/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.6/tests/test_iterator.py` & `crosspredict-1.1.7/tests/test_iterator.py`

 * *Files identical despite different names*

