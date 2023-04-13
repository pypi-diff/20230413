# Comparing `tmp/doc-ufcn-0.1.9rc2.tar.gz` & `tmp/doc-ufcn-0.1.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-ufcn-0.1.9rc2.tar", last modified: Fri Feb 24 09:30:16 2023, max compression
+gzip compressed data, was "doc-ufcn-0.1.9rc3.tar", last modified: Thu Apr 13 09:42:56 2023, max compression
```

## Comparing `doc-ufcn-0.1.9rc2.tar` & `doc-ufcn-0.1.9rc3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    20040 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/doc_ufcn/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/image.py
--rw-rw-rw-   0 root         (0) root         (0)     6050 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/main.py
--rw-rw-rw-   0 root         (0) root         (0)     8821 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1622 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/prediction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/doc_ufcn/train/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     7109 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/evaluate.py
--rw-rw-rw-   0 root         (0) root         (0)    11206 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     5398 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/mlflow_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/normalization_params.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/predict.py
--rw-rw-rw-   0 root         (0) root         (0)     8159 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/
--rw-rw-rw-   0 root         (0) root         (0)     6881 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9836 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     8020 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/object_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/pixel_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     8788 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     4479 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/training.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/training_pixel_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/doc_ufcn/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20040 2023-02-24 09:30:16.000000 doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1191 2023-02-24 09:30:16.000000 doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 09:30:16.000000 doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      262 2023-02-24 09:30:16.000000 doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-24 09:30:16.000000 doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/hugging_face/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/hugging_face/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/hugging_face/app.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/hugging_face/config.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      822 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 09:30:16.335434 doc-ufcn-0.1.9rc2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    19803 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     5284 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    11105 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/tests/test_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-02-24 09:20:11.000000 doc-ufcn-0.1.9rc2/training-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21620 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    21314 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     6050 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     8821 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/prediction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn/train/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     7109 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11206 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5398 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/mlflow_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/normalization_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)     8159 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9836 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8020 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/object_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/pixel_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3891 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     8788 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training_pixel_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21620 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/hugging_face/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7282 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/app.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      822 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19803 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     5284 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11105 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/training-requirements.txt
```

### Comparing `doc-ufcn-0.1.9rc2/LICENSE` & `doc-ufcn-0.1.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/PKG-INFO` & `doc-ufcn-0.1.9rc3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: doc-ufcn
-Version: 0.1.9rc2
-Summary: Doc-UFCN
-Home-page: https://gitlab.com/teklia/dla/doc-ufcn
-Author: Mélodie Boillet
-Author-email: boillet@teklia.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: training
-License-File: LICENSE
-
 # Doc-UFCN
 
 This Python 3 library contains a public implementation of Doc-UFCN, a fully convolutional network presented in the paper [Multiple Document Datasets Pre-training Improves Text Line Detection With Deep Neural Networks](https://teklia.com/research/publications/boillet2020/). This library has been developed by the original authors from [Teklia](https://teklia.com).
 
 The model is designed to run various Document Layout Analysis (DLA) tasks like the text line detection or page segmentation.
 
 ![Model schema](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
@@ -304,50 +291,78 @@
   - Set the value of the `loss` at `"initial"`;
   - Set the `same_classes` parameter to `False` if the classes used for training the new model are different from the classes used during the pre-training.
 
 Once these parameters have been updated, the training can be started and followed as described above.
 
 ## HuggingFace app
 
-You may easily create and deploy a web application to demo the prediction of your Doc-UFCN models. This application can be integrated in a [HuggingFace space](https://huggingface.co/spaces).
+You may easily create and deploy a web application to demo the prediction of your Doc-UFCN models. This application can be easily integrated in a [HuggingFace space](https://huggingface.co/spaces): an example of a *HuggingFace Space* generated using this code is available [here](https://huggingface.co/spaces/Teklia/doc-ufcn).
 
 To use HuggingFace app, it is necessary to install gradio using pip:
 
 ```shell
 pip install gradio
 ```
 The code was last tested with `gradio==3.18.0`.
 
 
-![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/HuggingFace_Line_Historical.png)
+![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
+
+An example is available in the `huggingface/` folder. You need to create a YAML configuration file with the following parameters:
+
+| Parameter        | Description                                                                                                        | Default value                 |
+| ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
+| `title`          | Title of the app (supports Markdown)                                                                                                   |                           **Required**|
+| `description`    | Description of the app (supports Markdown)                                                                                           |                           **Required**|
+| `examples`       | Paths towards the image examples                                                                                  |                           **Required**|
+| `models`       | List of models                                                                                  |                           **Required**|
 
-An example is available in the `huggingface/` folder. You need to create a JSON configuration file with the following parameters:
+In models parameter, for each model, fill in the following parameters:
 
 | Parameter        | Description                                                                                                        | Default value                 |
 | ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
-| `model_name`     | Name of the model                                                                                             |`doc-ufcn-generic-historical-line`|
-| `classes_colors` | List with the colors of the classes                                                                                |                    `["green"]`|
-| `title`          | Title of the app                                                                                                   |                           **Required**|
-| `description`    | Description of the app                                                                                             |                           **Required**|
-| `examples`       | Paths towards the image examples.                                                                                  |                           **Required**|
+| `model_name`     | Name of the model                                                                                             |**Required**|
+| `title`          | Title of the model (supports Markdown)                                                                                                   |                           **Required**|
+| `description`    | Description of the model (supports Markdown)                                                                                           |                           **Required**|
+| `classes_colors` | List with the colors of the classes                                                                                |                    **Required**|
 
-A ready-to-use configuration file is available in `huggingface/config.json`. You may update it to your needs.
+A ready-to-use configuration file is available in `huggingface/config.yaml`. You may update it to your needs.
 
 Once the configuration file is ready, just run the following command:
 
 ```shell
-$ python3 hugging_face/app.py --config hugging_face/config.json
+$ python3 hugging_face/app.py --config hugging_face/config.yaml
 ```
 
 If the `--public` argument is specified, the script will generate a public, shareable link that you can send to anyone. More information about public links on gradio is available in the [gradio documentation](https://gradio.app/sharing-your-app/).
 
 To generate the shareable link, use the following command:
 
 ```shell
-$ python3 hugging_face/app.py --config hugging_face/config.json --public
+$ python3 hugging_face/app.py --config hugging_face/config.yaml --public
+```
+
+The model's predictions will be shown on the application in JSON format:
+
+A dictionary mapping an object idx (starting from 1) to a dictionary describing the detected object:
+- `polygon` key : list, the coordinates of the points of the polygon,
+- `confidence` key : float, confidence of the model,
+- `channel` key : str, the name of the predicted class.
+
+```
+[
+  {
+    "polygon": [[],..,[]]
+    ,
+    "confidence": 0.91
+    ,
+    "channel": "text_line"
+  },
+  ..
+]
 ```
 
 ## Cite us!
 
 If you want to cite us in one of your works, please use the following citation.
 ```latex
 @inproceedings{boillet2020,
@@ -361,9 +376,7 @@
     doi = {10.1109/ICPR48806.2021.9412447}
 }
 ```
 
 ## License
 
 This library is under the 3-Clause BSD License.
-
-
```

### Comparing `doc-ufcn-0.1.9rc2/README.md` & `doc-ufcn-0.1.9rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: doc-ufcn
+Version: 0.1.9rc3
+Summary: Doc-UFCN
+Home-page: https://gitlab.com/teklia/dla/doc-ufcn
+Author: Mélodie Boillet
+Author-email: boillet@teklia.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Provides-Extra: training
+License-File: LICENSE
+
 # Doc-UFCN
 
 This Python 3 library contains a public implementation of Doc-UFCN, a fully convolutional network presented in the paper [Multiple Document Datasets Pre-training Improves Text Line Detection With Deep Neural Networks](https://teklia.com/research/publications/boillet2020/). This library has been developed by the original authors from [Teklia](https://teklia.com).
 
 The model is designed to run various Document Layout Analysis (DLA) tasks like the text line detection or page segmentation.
 
 ![Model schema](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
@@ -291,50 +304,78 @@
   - Set the value of the `loss` at `"initial"`;
   - Set the `same_classes` parameter to `False` if the classes used for training the new model are different from the classes used during the pre-training.
 
 Once these parameters have been updated, the training can be started and followed as described above.
 
 ## HuggingFace app
 
-You may easily create and deploy a web application to demo the prediction of your Doc-UFCN models. This application can be integrated in a [HuggingFace space](https://huggingface.co/spaces).
+You may easily create and deploy a web application to demo the prediction of your Doc-UFCN models. This application can be easily integrated in a [HuggingFace space](https://huggingface.co/spaces): an example of a *HuggingFace Space* generated using this code is available [here](https://huggingface.co/spaces/Teklia/doc-ufcn).
 
 To use HuggingFace app, it is necessary to install gradio using pip:
 
 ```shell
 pip install gradio
 ```
 The code was last tested with `gradio==3.18.0`.
 
 
-![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/HuggingFace_Line_Historical.png)
+![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
+
+An example is available in the `huggingface/` folder. You need to create a YAML configuration file with the following parameters:
+
+| Parameter        | Description                                                                                                        | Default value                 |
+| ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
+| `title`          | Title of the app (supports Markdown)                                                                                                   |                           **Required**|
+| `description`    | Description of the app (supports Markdown)                                                                                           |                           **Required**|
+| `examples`       | Paths towards the image examples                                                                                  |                           **Required**|
+| `models`       | List of models                                                                                  |                           **Required**|
 
-An example is available in the `huggingface/` folder. You need to create a JSON configuration file with the following parameters:
+In models parameter, for each model, fill in the following parameters:
 
 | Parameter        | Description                                                                                                        | Default value                 |
 | ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
-| `model_name`     | Name of the model                                                                                             |`doc-ufcn-generic-historical-line`|
-| `classes_colors` | List with the colors of the classes                                                                                |                    `["green"]`|
-| `title`          | Title of the app                                                                                                   |                           **Required**|
-| `description`    | Description of the app                                                                                             |                           **Required**|
-| `examples`       | Paths towards the image examples.                                                                                  |                           **Required**|
+| `model_name`     | Name of the model                                                                                             |**Required**|
+| `title`          | Title of the model (supports Markdown)                                                                                                   |                           **Required**|
+| `description`    | Description of the model (supports Markdown)                                                                                           |                           **Required**|
+| `classes_colors` | List with the colors of the classes                                                                                |                    **Required**|
 
-A ready-to-use configuration file is available in `huggingface/config.json`. You may update it to your needs.
+A ready-to-use configuration file is available in `huggingface/config.yaml`. You may update it to your needs.
 
 Once the configuration file is ready, just run the following command:
 
 ```shell
-$ python3 hugging_face/app.py --config hugging_face/config.json
+$ python3 hugging_face/app.py --config hugging_face/config.yaml
 ```
 
 If the `--public` argument is specified, the script will generate a public, shareable link that you can send to anyone. More information about public links on gradio is available in the [gradio documentation](https://gradio.app/sharing-your-app/).
 
 To generate the shareable link, use the following command:
 
 ```shell
-$ python3 hugging_face/app.py --config hugging_face/config.json --public
+$ python3 hugging_face/app.py --config hugging_face/config.yaml --public
+```
+
+The model's predictions will be shown on the application in JSON format:
+
+A dictionary mapping an object idx (starting from 1) to a dictionary describing the detected object:
+- `polygon` key : list, the coordinates of the points of the polygon,
+- `confidence` key : float, confidence of the model,
+- `channel` key : str, the name of the predicted class.
+
+```
+[
+  {
+    "polygon": [[],..,[]]
+    ,
+    "confidence": 0.91
+    ,
+    "channel": "text_line"
+  },
+  ..
+]
 ```
 
 ## Cite us!
 
 If you want to cite us in one of your works, please use the following citation.
 ```latex
 @inproceedings{boillet2020,
@@ -348,7 +389,9 @@
     doi = {10.1109/ICPR48806.2021.9412447}
 }
 ```
 
 ## License
 
 This library is under the 3-Clause BSD License.
+
+
```

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/image.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/image.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/main.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/main.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/model.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/model.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/models.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/models.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/prediction.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/prediction.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/cli.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         help="Path towards an experiment or global configuration file. All files will be merged in order.",
     )
 
     return parser.parse_args()
 
 
 def main():
-
     args = parse_args()
 
     # Parse all configuration files provided from CLI
     config = parse_configurations(args.config)
 
     # Ensure we have at least one step to run
     if len(config["steps"]) == 0:
```

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/configuration.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/configuration.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/evaluate.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/experiment.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/experiment.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/mask.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/mask.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/mlflow_utils.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/normalization_params.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/normalization_params.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/predict.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/predict.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/training.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/training.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/__init__.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         dict_index: values for dict_index, values in bucket.items() if len(values) > 0
     }
     return bucket
 
 
 class Sampler(torch.utils.data.Sampler):
     def __init__(self, data, bin_size=20, batch_size=None, nb_params=None):
-
         self.bin_size = bin_size
         self.batch_size = batch_size
         self.nb_params = nb_params
 
         self.data_sizes = [image["size"] for image in data]
 
         self.vertical = {
```

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/evaluation.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/object_metrics.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/object_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/pixel_metrics.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/pixel_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/prediction.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/preprocessing.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/training.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/train/utils/training_pixel_metrics.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training_pixel_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn/utils.py` & `doc-ufcn-0.1.9rc3/doc_ufcn/utils.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/PKG-INFO` & `doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-ufcn
-Version: 0.1.9rc2
+Version: 0.1.9rc3
 Summary: Doc-UFCN
 Home-page: https://gitlab.com/teklia/dla/doc-ufcn
 Author: Mélodie Boillet
 Author-email: boillet@teklia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -304,50 +304,78 @@
   - Set the value of the `loss` at `"initial"`;
   - Set the `same_classes` parameter to `False` if the classes used for training the new model are different from the classes used during the pre-training.
 
 Once these parameters have been updated, the training can be started and followed as described above.
 
 ## HuggingFace app
 
-You may easily create and deploy a web application to demo the prediction of your Doc-UFCN models. This application can be integrated in a [HuggingFace space](https://huggingface.co/spaces).
+You may easily create and deploy a web application to demo the prediction of your Doc-UFCN models. This application can be easily integrated in a [HuggingFace space](https://huggingface.co/spaces): an example of a *HuggingFace Space* generated using this code is available [here](https://huggingface.co/spaces/Teklia/doc-ufcn).
 
 To use HuggingFace app, it is necessary to install gradio using pip:
 
 ```shell
 pip install gradio
 ```
 The code was last tested with `gradio==3.18.0`.
 
 
-![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/HuggingFace_Line_Historical.png)
+![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
 
-An example is available in the `huggingface/` folder. You need to create a JSON configuration file with the following parameters:
+An example is available in the `huggingface/` folder. You need to create a YAML configuration file with the following parameters:
 
 | Parameter        | Description                                                                                                        | Default value                 |
 | ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
-| `model_name`     | Name of the model                                                                                             |`doc-ufcn-generic-historical-line`|
-| `classes_colors` | List with the colors of the classes                                                                                |                    `["green"]`|
-| `title`          | Title of the app                                                                                                   |                           **Required**|
-| `description`    | Description of the app                                                                                             |                           **Required**|
-| `examples`       | Paths towards the image examples.                                                                                  |                           **Required**|
+| `title`          | Title of the app (supports Markdown)                                                                                                   |                           **Required**|
+| `description`    | Description of the app (supports Markdown)                                                                                           |                           **Required**|
+| `examples`       | Paths towards the image examples                                                                                  |                           **Required**|
+| `models`       | List of models                                                                                  |                           **Required**|
 
-A ready-to-use configuration file is available in `huggingface/config.json`. You may update it to your needs.
+In models parameter, for each model, fill in the following parameters:
+
+| Parameter        | Description                                                                                                        | Default value                 |
+| ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
+| `model_name`     | Name of the model                                                                                             |**Required**|
+| `title`          | Title of the model (supports Markdown)                                                                                                   |                           **Required**|
+| `description`    | Description of the model (supports Markdown)                                                                                           |                           **Required**|
+| `classes_colors` | List with the colors of the classes                                                                                |                    **Required**|
+
+A ready-to-use configuration file is available in `huggingface/config.yaml`. You may update it to your needs.
 
 Once the configuration file is ready, just run the following command:
 
 ```shell
-$ python3 hugging_face/app.py --config hugging_face/config.json
+$ python3 hugging_face/app.py --config hugging_face/config.yaml
 ```
 
 If the `--public` argument is specified, the script will generate a public, shareable link that you can send to anyone. More information about public links on gradio is available in the [gradio documentation](https://gradio.app/sharing-your-app/).
 
 To generate the shareable link, use the following command:
 
 ```shell
-$ python3 hugging_face/app.py --config hugging_face/config.json --public
+$ python3 hugging_face/app.py --config hugging_face/config.yaml --public
+```
+
+The model's predictions will be shown on the application in JSON format:
+
+A dictionary mapping an object idx (starting from 1) to a dictionary describing the detected object:
+- `polygon` key : list, the coordinates of the points of the polygon,
+- `confidence` key : float, confidence of the model,
+- `channel` key : str, the name of the predicted class.
+
+```
+[
+  {
+    "polygon": [[],..,[]]
+    ,
+    "confidence": 0.91
+    ,
+    "channel": "text_line"
+  },
+  ..
+]
 ```
 
 ## Cite us!
 
 If you want to cite us in one of your works, please use the following citation.
 ```latex
 @inproceedings{boillet2020,
```

### Comparing `doc-ufcn-0.1.9rc2/doc_ufcn.egg-info/SOURCES.txt` & `doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 doc_ufcn/train/utils/prediction.py
 doc_ufcn/train/utils/preprocessing.py
 doc_ufcn/train/utils/training.py
 doc_ufcn/train/utils/training_pixel_metrics.py
 hugging_face/__init__.py
 hugging_face/app.py
 hugging_face/config.py
+hugging_face/tools.py
 tests/__init__.py
 tests/conftest.py
 tests/test_image.py
 tests/test_main.py
 tests/test_mask.py
 tests/test_model.py
 tests/test_models.py
```

### Comparing `doc-ufcn-0.1.9rc2/setup.py` & `doc-ufcn-0.1.9rc3/setup.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/conftest.py` & `doc-ufcn-0.1.9rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/test_image.py` & `doc-ufcn-0.1.9rc3/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/test_main.py` & `doc-ufcn-0.1.9rc3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/test_mask.py` & `doc-ufcn-0.1.9rc3/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/test_model.py` & `doc-ufcn-0.1.9rc3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/test_models.py` & `doc-ufcn-0.1.9rc3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc2/tests/test_prediction.py` & `doc-ufcn-0.1.9rc3/tests/test_prediction.py`

 * *Files identical despite different names*

