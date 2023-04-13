# Comparing `tmp/doc-ufcn-0.1.9rc3.tar.gz` & `tmp/doc-ufcn-0.1.9rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-ufcn-0.1.9rc3.tar", last modified: Thu Apr 13 09:42:56 2023, max compression
+gzip compressed data, was "doc-ufcn-0.1.9rc4.tar", last modified: Thu Apr 13 10:27:53 2023, max compression
```

## Comparing `doc-ufcn-0.1.9rc3.tar` & `doc-ufcn-0.1.9rc4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    21620 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    21314 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/image.py
--rw-rw-rw-   0 root         (0) root         (0)     6050 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/main.py
--rw-rw-rw-   0 root         (0) root         (0)     8821 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1622 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/prediction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn/train/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     7109 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/evaluate.py
--rw-rw-rw-   0 root         (0) root         (0)    11206 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     5398 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/mlflow_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/normalization_params.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/predict.py
--rw-rw-rw-   0 root         (0) root         (0)     8159 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/
--rw-rw-rw-   0 root         (0) root         (0)     6880 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9836 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     8020 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/object_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/pixel_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     8788 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     4479 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training_pixel_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/doc_ufcn/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.889626 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21620 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-13 09:42:56.000000 doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/hugging_face/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7282 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/app.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/hugging_face/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      822 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:42:56.893626 doc-ufcn-0.1.9rc3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    19803 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     5284 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    11105 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/tests/test_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-13 09:34:52.000000 doc-ufcn-0.1.9rc3/training-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.422901 doc-ufcn-0.1.9rc4/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21620 2023-04-13 10:27:53.422901 doc-ufcn-0.1.9rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    21314 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.418901 doc-ufcn-0.1.9rc4/doc_ufcn/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     6050 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     8821 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/prediction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.418901 doc-ufcn-0.1.9rc4/doc_ufcn/train/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     7109 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11206 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5398 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/mlflow_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/normalization_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)     8159 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.418901 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9836 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8020 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/object_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/pixel_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3891 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     8788 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/training_pixel_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/doc_ufcn/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.418901 doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21620 2023-04-13 10:27:53.000000 doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-04-13 10:27:53.000000 doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:27:53.000000 doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      283 2023-04-13 10:27:53.000000 doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-13 10:27:53.000000 doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.422901 doc-ufcn-0.1.9rc4/hugging_face/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/hugging_face/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7282 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/hugging_face/app.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/hugging_face/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/hugging_face/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 10:27:53.422901 doc-ufcn-0.1.9rc4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      822 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:27:53.422901 doc-ufcn-0.1.9rc4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19803 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     5284 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11105 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/tests/test_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-13 10:27:18.000000 doc-ufcn-0.1.9rc4/training-requirements.txt
```

### Comparing `doc-ufcn-0.1.9rc3/LICENSE` & `doc-ufcn-0.1.9rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/PKG-INFO` & `doc-ufcn-0.1.9rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-ufcn
-Version: 0.1.9rc3
+Version: 0.1.9rc4
 Summary: Doc-UFCN
 Home-page: https://gitlab.com/teklia/dla/doc-ufcn
 Author: Mélodie Boillet
 Author-email: boillet@teklia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `doc-ufcn-0.1.9rc3/README.md` & `doc-ufcn-0.1.9rc4/README.md`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/image.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/image.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/main.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/main.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/model.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/model.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/models.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/models.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/prediction.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/prediction.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/cli.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/cli.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/configuration.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/configuration.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/evaluate.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/experiment.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/experiment.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/mask.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/mask.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/mlflow_utils.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/normalization_params.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/normalization_params.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/predict.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/predict.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/training.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/training.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/__init__.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/evaluation.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/object_metrics.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/object_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/pixel_metrics.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/pixel_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/prediction.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/preprocessing.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/training.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/train/utils/training_pixel_metrics.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/train/utils/training_pixel_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn/utils.py` & `doc-ufcn-0.1.9rc4/doc_ufcn/utils.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/PKG-INFO` & `doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-ufcn
-Version: 0.1.9rc3
+Version: 0.1.9rc4
 Summary: Doc-UFCN
 Home-page: https://gitlab.com/teklia/dla/doc-ufcn
 Author: Mélodie Boillet
 Author-email: boillet@teklia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `doc-ufcn-0.1.9rc3/doc_ufcn.egg-info/SOURCES.txt` & `doc-ufcn-0.1.9rc4/doc_ufcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/hugging_face/app.py` & `doc-ufcn-0.1.9rc4/hugging_face/app.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/hugging_face/config.py` & `doc-ufcn-0.1.9rc4/hugging_face/config.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/hugging_face/tools.py` & `doc-ufcn-0.1.9rc4/hugging_face/tools.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/setup.py` & `doc-ufcn-0.1.9rc4/setup.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/conftest.py` & `doc-ufcn-0.1.9rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/test_image.py` & `doc-ufcn-0.1.9rc4/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/test_main.py` & `doc-ufcn-0.1.9rc4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/test_mask.py` & `doc-ufcn-0.1.9rc4/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/test_model.py` & `doc-ufcn-0.1.9rc4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/test_models.py` & `doc-ufcn-0.1.9rc4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.1.9rc3/tests/test_prediction.py` & `doc-ufcn-0.1.9rc4/tests/test_prediction.py`

 * *Files identical despite different names*

