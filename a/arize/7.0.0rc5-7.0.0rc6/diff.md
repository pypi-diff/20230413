# Comparing `tmp/arize-7.0.0rc5.tar.gz` & `tmp/arize-7.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.0rc5.tar", last modified: Tue Apr 11 17:47:12 2023, max compression
+gzip compressed data, was "arize-7.0.0rc6.tar", last modified: Thu Apr 13 01:46:58 2023, max compression
```

## Comparing `arize-7.0.0rc5.tar` & `arize-7.0.0rc6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.976723 arize-7.0.0rc5/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc5/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc5/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-11 17:47:12.977262 arize-7.0.0rc5/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc5/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.885802 arize-7.0.0rc5/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    25743 2023-04-10 23:06:12.000000 arize-7.0.0rc5/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.898800 arize-7.0.0rc5/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.918558 arize-7.0.0rc5/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.931183 arize-7.0.0rc5/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-04-10 21:49:18.000000 arize-7.0.0rc5/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.932173 arize-7.0.0rc5/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.935576 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-10 22:55:57.000000 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12188 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    21965 2023-04-11 17:42:13.000000 arize-7.0.0rc5/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.938444 arize-7.0.0rc5/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-04-10 03:28:13.000000 arize-7.0.0rc5/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.941342 arize-7.0.0rc5/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    22704 2023-04-10 23:06:12.000000 arize-7.0.0rc5/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    59911 2023-04-11 01:26:42.000000 arize-7.0.0rc5/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   167320 2023-04-11 17:42:13.000000 arize-7.0.0rc5/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.949832 arize-7.0.0rc5/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc5/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-04-10 23:06:12.000000 arize-7.0.0rc5/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    22046 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7229 2023-04-11 17:42:22.000000 arize-7.0.0rc5/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.890054 arize-7.0.0rc5/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12608 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-11 17:47:12.000000 arize-7.0.0rc5/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc5/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1561 2023-04-11 17:47:12.979870 arize-7.0.0rc5/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-11 17:47:12.975172 arize-7.0.0rc5/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    43569 2023-04-10 03:28:13.000000 arize-7.0.0rc5/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc5/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.220308 arize-7.0.0rc6/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.0rc6/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.0rc6/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-13 01:46:58.220851 arize-7.0.0rc6/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.0rc6/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.148036 arize-7.0.0rc6/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-13 01:46:45.000000 arize-7.0.0rc6/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26240 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.169092 arize-7.0.0rc6/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.170804 arize-7.0.0rc6/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.182041 arize-7.0.0rc6/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-04-10 21:49:18.000000 arize-7.0.0rc6/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.182921 arize-7.0.0rc6/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.200864 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-10 22:55:57.000000 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12188 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22747 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.202383 arize-7.0.0rc6/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-04-10 03:28:13.000000 arize-7.0.0rc6/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.204990 arize-7.0.0rc6/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    23189 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    60237 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)   167683 2023-04-13 01:39:58.000000 arize-7.0.0rc6/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.210885 arize-7.0.0rc6/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.0rc6/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4177 2023-04-10 23:06:12.000000 arize-7.0.0rc6/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    22046 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7229 2023-04-11 17:42:22.000000 arize-7.0.0rc6/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.161838 arize-7.0.0rc6/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-13 01:46:58.000000 arize-7.0.0rc6/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.0rc6/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-04-13 01:46:58.224384 arize-7.0.0rc6/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-13 01:46:58.213599 arize-7.0.0rc6/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    44544 2023-04-13 01:39:58.000000 arize-7.0.0rc6/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.0rc6/tests/test_utils.py
```

### Comparing `arize-7.0.0rc5/LICENSE.md` & `arize-7.0.0rc6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/PKG-INFO` & `arize-7.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc5
+Version: 7.0.0rc6
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
```

### Comparing `arize-7.0.0rc5/README.md` & `arize-7.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/api.py` & `arize-7.0.0rc6/arize/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import concurrent.futures as cf
 import time
 from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
+from arize.pandas.validation.errors import InvalidAdditionalHeaders
 from arize.utils.utils import MAX_PREDICTION_ID_LEN, MIN_PREDICTION_ID_LEN
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.wrappers_pb2 import DoubleValue
 from requests_futures.sessions import FuturesSession
 
 from . import public_pb2 as pb2
 from .__init__ import __version__
@@ -39,45 +40,52 @@
         self,
         api_key: str,
         space_key: str,
         uri: Optional[str] = "https://api.arize.com/v1",
         max_workers: Optional[int] = 8,
         max_queue_bound: Optional[int] = 5000,
         timeout: Optional[int] = 200,
+        additional_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         """
         :param api_key (str): Arize provided API key associated with your account. Located on the
         data upload page.
         :param space_key (str): Arize provided identifier to connect records to spaces. Located on
         the data upload page.
         :param uri (str, optional): URI to send your records to Arize AI. Defaults to
         "https://api.arize.com/v1".
         :param max_workers (int, optional): maximum number of concurrent requests to Arize. Defaults
         to 8.
         :param max_queue_bound (int, optional): maximum number of concurrent future objects
         generated for publishing to Arize. Defaults to 5000.
         :param timeout (int, optional): How long to wait for the server to send data before giving
         up. Defaults to 200.
+        :param additional_headers (Dict[str, str], optional): Dictionary of additional headers to
+        append to request
         """
 
         if not isinstance(space_key, str):
             raise TypeError(f"space_key {space_key} is type {type(space_key)}, but must be a str")
-        self._uri = uri + "/log"
+        self._uri = f"{uri}/log"
         self._api_key = api_key
         self._space_key = space_key
         self._timeout = timeout
         self._session = FuturesSession(executor=BoundedExecutor(max_queue_bound, max_workers))
         # Grpc-Metadata prefix is required to pass non-standard md through via grpc-gateway
         self._header = {
             "authorization": api_key,
             "Grpc-Metadata-space": space_key,
             "Grpc-Metadata-python-version": get_python_version(),
             "Grpc-Metadata-sdk-version": __version__,
             "Grpc-Metadata-sdk": "py",
         }
+        if additional_headers is not None:
+            if conflicting_keys := self._header.keys() & additional_headers.keys():
+                raise InvalidAdditionalHeaders(conflicting_keys)
+            self._header.update(additional_headers)
 
     def log(
         self,
         model_id: str,
         model_type: ModelTypes,
         environment: Environments,
         model_version: Optional[str] = None,
```

### Comparing `arize-7.0.0rc5/arize/bounded_executor.py` & `arize-7.0.0rc6/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/examples/bulk_client.py` & `arize-7.0.0rc6/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/examples/bulk_client_shap.py` & `arize-7.0.0rc6/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/examples/client_shap_values.py` & `arize-7.0.0rc6/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/examples/log_client.py` & `arize-7.0.0rc6/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/examples/log_pandas_dataframe.py` & `arize-7.0.0rc6/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/examples/preproduction_client.py` & `arize-7.0.0rc6/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.0rc6/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/embeddings/base_generators.py` & `arize-7.0.0rc6/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.0rc6/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/embeddings/models.py` & `arize-7.0.0rc6/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.0rc6/arize/pandas/embeddings/nlp_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,12 +82,12 @@
             raise TypeError("text_col must be a pandas Series")
 
         ds = Dataset.from_dict({"text": text_col})
 
         ds.set_transform(partial(self.tokenize, text_feat_name="text"))
         logger.info("Generating embedding vectors")
         ds = ds.map(
-            lambda batch: self._get_embedding_vector(batch, "avg_token"),
+            lambda batch: self._get_embedding_vector(batch, "cls_token"),
             batched=True,
             batch_size=self.batch_size,
         )
         return cast(pd.DataFrame, ds.to_pandas())["embedding_vector"]
```

### Comparing `arize-7.0.0rc5/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.0rc6/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.0rc6/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/logger.py` & `arize-7.0.0rc6/arize/pandas/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # type: ignore[pb2]
 import base64
 import tempfile
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 import pandas as pd
 import pandas.api.types as ptypes
 import pyarrow as pa
 import requests
 
 from .. import public_pb2 as pb2
@@ -31,26 +31,43 @@
     """
 
     def __init__(
         self,
         api_key: str,
         space_key: str,
         uri: Optional[str] = "https://api.arize.com/v1",
+        additional_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         """
         :param api_key (str): Arize provided API key associated with your account. Located on the
         data upload page.
         :param space_key (str): Arize provided identifier to connect records to spaces. Located on
         the data upload page.
         :param uri (str, optional): URI endpoint to send your records to Arize AI. Defaults to
         "https://api.arize.com/v1".
+        :param additional_headers (Dict[str, str], optional): Dictionary of additional headers to
+        append to request
         """
         self._api_key = api_key
         self._space_key = space_key
         self._files_uri = uri + "/pandas_arrow"
+        self._additional_headers = {}
+        if additional_headers is not None:
+            reserved_headers = {
+                "authorization",
+                "space",
+                "sdk-version",
+                "schema",
+                "sdk",
+                "python-version",
+                "sync",
+            }
+            if conflicting_keys := reserved_headers & additional_headers.keys():
+                raise err.InvalidAdditionalHeaders(conflicting_keys)
+            self._additional_headers.update(additional_headers)
 
     def log(
         self,
         dataframe: pd.DataFrame,
         schema: Schema,
         environment: Environments,
         model_id: str,
@@ -439,14 +456,15 @@
                 "authorization": self._api_key,
                 "space": self._space_key,
                 "schema": schema,
                 "python-version": get_python_version(),
                 "sdk-version": __version__,
                 "sdk": "py",
             }
+            headers.update(self._additional_headers)
             if sync:
                 headers["sync"] = "1"
             return requests.post(
                 self._files_uri,
                 timeout=timeout,
                 data=f,
                 headers=headers,
```

### Comparing `arize-7.0.0rc5/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.0rc6/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/pandas/validation/errors.py` & `arize-7.0.0rc6/arize/pandas/validation/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,17 +518,17 @@
     def __init__(self, name: str, acceptable_range: str) -> None:
         self.name = name
         self.acceptable_range = acceptable_range
 
     def error_message(self) -> str:
         return (
             f"{self.name} is out of range. "
-            f"Only values within {self.acceptable_range} from the current time are accepted. "
-            "If this is your pre-production data, you could also just remove the timestamp column "
-            "from the Schema."
+            f"Predictions that are made more than {self.acceptable_range} in the future from the current "
+            "time are not accepted. If this is your pre-production data, you could also just remove the "
+            "timestamp column from the Schema."
         )
 
 
 class InvalidValueMissingValue(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Missing_Value"
 
@@ -690,7 +690,21 @@
             )
         elif self.reason == "scores_out_of_bounds":
             msg += (
                 "Found at least one confidence score out of bounds. "
                 "Confidence scores must be between 0 and 1"
             )
         return msg
+
+
+class InvalidAdditionalHeaders(ValidationError):
+    def __repr__(self) -> str:
+        return "Invalid_Additional_Headers"
+
+    def __init__(self, invalid_headers: Iterable) -> None:
+        self.invalid_header_names = invalid_headers
+
+    def error_message(self) -> str:
+        return (
+            "Found invalid additional header, cannot use reserved headers named: "
+            f"{', '.join(map(str, self.invalid_header_names))}."
+        )
```

### Comparing `arize-7.0.0rc5/arize/pandas/validation/validator.py` & `arize-7.0.0rc6/arize/pandas/validation/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import chain
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import arize.pandas.validation.errors as err
 import numpy as np
 import pandas as pd
 import pyarrow as pa
+from arize.utils.logging import logger
 from arize.utils.types import (
     CATEGORICAL_MODEL_TYPES,
     NUMERIC_MODEL_TYPES,
     EmbeddingColumnNames,
     Environments,
     Metrics,
     ModelTypes,
@@ -1193,49 +1194,49 @@
             # pandas min/max will fail due to type incompatibility. So we check for
             # missing value first.
             if dataframe[col].isnull().values.any():
                 return [err.InvalidValueMissingValue("Prediction timestamp", "missing")]
 
             now_t = datetime.datetime.now()
             lbound, ubound = (
-                (now_t - datetime.timedelta(days=365)).timestamp(),
+                (now_t - datetime.timedelta(days=730)).timestamp(),
                 (now_t + datetime.timedelta(days=365)).timestamp(),
             )
 
             # faster than pyarrow compute
             stats = dataframe[col].agg(["min", "max"])
 
             ta = pa.Table.from_pandas(stats.to_frame())
             type_ = ta.column(0).type
             min_, max_ = ta.column(0)
 
             # this part needs improvement: dealing with python types is hard :(
+            # Add warning when minimum timestamp is lower than lower bound
             if (
-                (
-                    type(type_) == pa.TimestampType
-                    and (stats["min"].timestamp() < lbound or stats["max"].timestamp() > ubound)
-                )
-                or (
-                    type_ in (pa.int64(), pa.float64())
-                    and (min_.as_py() < lbound or max_.as_py() > ubound)
-                )
+                (isinstance(type_, pa.TimestampType) and (stats["min"].timestamp() < lbound))
+                or (type_ in (pa.int64(), pa.float64()) and (min_.as_py() < lbound))
                 or (
                     type_ == pa.date32()
-                    and (
-                        int(min_.cast(pa.int32()).as_py() * 60 * 60 * 24) < lbound
-                        or int(max_.cast(pa.int32()).as_py() * 60 * 60 * 24) > ubound
-                    )
+                    and (int(min_.cast(pa.int32()).as_py() * 60 * 60 * 24) < lbound)
+                )
+                or (type_ == pa.date64() and (int(min_.cast(pa.int64()).as_py() // 1000) < lbound))
+            ):
+                logger.warning(
+                    "Predictions with timestamps older than 2 years will not be shown in the Arize platform."
                 )
+
+            # Check if max timestamp value exceeds 1 year limit
+            if (
+                (isinstance(type_, pa.TimestampType) and (stats["max"].timestamp() > ubound))
+                or (type_ in (pa.int64(), pa.float64()) and (max_.as_py() > ubound))
                 or (
-                    type_ == pa.date64()
-                    and (
-                        int(min_.cast(pa.int64()).as_py() // 1000) < lbound
-                        or int(max_.cast(pa.int64()).as_py() // 1000) > ubound
-                    )
+                    type_ == pa.date32()
+                    and (int(max_.cast(pa.int32()).as_py() * 60 * 60 * 24) > ubound)
                 )
+                or (type_ == pa.date64() and (int(max_.cast(pa.int64()).as_py() // 1000) > ubound))
             ):
                 return [
                     err.InvalidValueTimestamp("Prediction timestamp", acceptable_range="one year")
                 ]
 
         return []
```

### Comparing `arize-7.0.0rc5/arize/public_pb2.py` & `arize-7.0.0rc6/arize/public_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='public.proto',
   package='public',
   syntax='proto3',
   serialized_options=b'\n\022com.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/public',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0cpublic.proto\x12\x06public\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x01\n\nBulkRecord\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x1f\n\x07records\x18\x05 \x03(\x0b\x32\x0e.public.Record\x12\x11\n\tspace_key\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05R\ttimestamp\"\x99\x05\n\x06Record\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rprediction_id\x18\x03 \x01(\t\x12&\n\nprediction\x18\x08 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\t \x01(\x0b\x32\x0e.public.Actual\x12\x37\n\x13\x66\x65\x61ture_importances\x18\n \x01(\x0b\x32\x1a.public.FeatureImportances\x12:\n\x15prediction_and_actual\x18\x0b \x01(\x0b\x32\x1b.public.PredictionAndActual\x12\x11\n\tspace_key\x18\x0c \x01(\t\x12<\n\x12\x65nvironment_params\x18\r \x01(\x0b\x32 .public.Record.EnvironmentParams\x1a\xa1\x02\n\x11\x45nvironmentParams\x12=\n\x08training\x18\x01 \x01(\x0b\x32).public.Record.EnvironmentParams.TrainingH\x00\x12\x41\n\nvalidation\x18\x02 \x01(\x0b\x32+.public.Record.EnvironmentParams.ValidationH\x00\x12\x41\n\nproduction\x18\x03 \x01(\x0b\x32+.public.Record.EnvironmentParams.ProductionH\x00\x1a\n\n\x08Training\x1a\x1e\n\nValidation\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x1a\x0c\n\nProductionB\r\n\x0b\x65nvironmentJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xae\x02\n\x13PreProductionRecord\x12\x45\n\x0ftraining_record\x18\x01 \x01(\x0b\x32*.public.PreProductionRecord.TrainingRecordH\x00\x12I\n\x11validation_record\x18\x02 \x01(\x0b\x32,.public.PreProductionRecord.ValidationRecordH\x00\x1a\x44\n\x10ValidationRecord\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x1e\n\x06record\x18\x02 \x01(\x0b\x32\x0e.public.Record\x1a\x30\n\x0eTrainingRecord\x12\x1e\n\x06record\x18\x01 \x01(\x0b\x32\x0e.public.RecordB\r\n\x0brecord_type\"\xad\x02\n\x10ScoreCategorical\x12\x17\n\x0b\x63\x61tegorical\x18\x01 \x01(\tB\x02\x18\x01\x12\x11\n\x05score\x18\x02 \x01(\x01\x42\x02\x18\x01\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0b\x32!.public.ScoreCategorical.CategoryH\x00\x12@\n\x0escore_category\x18\x04 \x01(\x0b\x32&.public.ScoreCategorical.ScoreCategoryH\x00\x1a\x1c\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x1aN\n\rScoreCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1c\n\x10numeric_sequence\x18\x03 \x03(\x01\x42\x02\x18\x01\x42\x06\n\x04type\"\xb1\x01\n\x0fObjectDetection\x12;\n\x0e\x62ounding_boxes\x18\x01 \x03(\x0b\x32#.public.ObjectDetection.BoundingBox\x1a\x61\n\x0b\x42oundingBox\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12+\n\x05score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x85\x01\n\x11RankingPrediction\x12\x1b\n\x13prediction_group_id\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x02 \x01(\x03\x12\x36\n\x10prediction_score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\r\n\x05label\x18\x04 \x01(\t\"l\n\rRankingActual\x12$\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32\x12.public.MultiValue\x12\x35\n\x0frelevance_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x82\x01\n\x05Label\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x42\x06\n\x04\x64\x61ta\"\xef\x01\n\x0fPredictionLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12,\n\x07ranking\x18\x05 \x01(\x0b\x32\x19.public.RankingPredictionH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\xe7\x01\n\x0b\x41\x63tualLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12(\n\x07ranking\x18\x05 \x01(\x0b\x32\x15.public.RankingActualH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\x83\x03\n\nPrediction\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12 \n\x05label\x18\x03 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12\x32\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32 .public.Prediction.FeaturesEntry\x12*\n\x04tags\x18\x05 \x03(\x0b\x32\x1c.public.Prediction.TagsEntry\x12\x31\n\x10prediction_label\x18\x06 \x01(\x0b\x32\x17.public.PredictionLabel\x1a>\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\x95\x01\n\x05Value\x12\x10\n\x06string\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12)\n\x0bmulti_value\x18\x04 \x01(\x0b\x32\x12.public.MultiValueH\x00\x12&\n\tembedding\x18\x05 \x01(\x0b\x32\x11.public.EmbeddingH\x00\x42\x06\n\x04\x64\x61ta\"\x1c\n\nMultiValue\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xed\x01\n\tEmbedding\x12\x0e\n\x06vector\x18\x01 \x03(\x01\x12\x32\n\x0clink_to_data\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08raw_data\x18\x04 \x01(\x0b\x32\x19.public.Embedding.RawData\x1aK\n\x07RawData\x12\x32\n\ntokenArray\x18\x02 \x01(\x0b\x32\x1c.public.Embedding.TokenArrayH\x00\x42\x06\n\x04typeJ\x04\x08\x01\x10\x02\x1a\x1c\n\nTokenArray\x12\x0e\n\x06tokens\x18\x01 \x03(\tJ\x04\x08\x02\x10\x03\"\xe8\x01\n\x06\x41\x63tual\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x05label\x18\x02 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12&\n\x04tags\x18\x03 \x03(\x0b\x32\x18.public.Actual.TagsEntry\x12)\n\x0c\x61\x63tual_label\x18\x04 \x01(\x0b\x32\x13.public.ActualLabel\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xe6\x01\n\x12\x46\x65\x61tureImportances\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12O\n\x13\x66\x65\x61ture_importances\x18\x03 \x03(\x0b\x32\x32.public.FeatureImportances.FeatureImportancesEntry\x1a\x39\n\x17\x46\x65\x61tureImportancesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"]\n\x13PredictionAndActual\x12&\n\nprediction\x18\x01 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x0e.public.Actual\"\x8b\x01\n\nFileHeader\x12\x33\n\x0b\x65nvironment\x18\x01 \x01(\x0e\x32\x1e.public.FileHeader.Environment\"H\n\x0b\x45nvironment\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\xc3\'\n\x06Schema\x12+\n\tconstants\x18\x01 \x01(\x0b\x32\x18.public.Schema.Constants\x12<\n\x11\x61rize_conclusions\x18\x02 \x01(\x0b\x32\x1f.public.Schema.ArizeConclusionsH\x00\x12>\n\x12\x61rize_explanations\x18\x03 \x01(\x0b\x32 .public.Schema.ArizeExplanationsH\x00\x12\x32\n\x0c\x61rrow_schema\x18\x04 \x01(\x0b\x32\x1a.public.Schema.ArrowSchemaH\x00\x12\x36\n\x0egeneric_schema\x18\x05 \x01(\x0b\x32\x1c.public.Schema.GenericSchemaH\x00\x12K\n\x19\x61rize_conclusion_pointers\x18\x06 \x01(\x0b\x32&.public.Schema.ArizeConclusionPointersH\x00\x12M\n\x1a\x61rize_explanation_pointers\x18\x07 \x01(\x0b\x32\'.public.Schema.ArizeExplanationPointersH\x00\x1a\xa5\x01\n\tConstants\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\t\x12/\n\x0b\x65nvironment\x18\x04 \x01(\x0e\x32\x1a.public.Schema.Environment\x12,\n\nmodel_type\x18\x05 \x01(\x0e\x32\x18.public.Schema.ModelType\x1a\x12\n\x10\x41rizeConclusions\x1a\x13\n\x11\x41rizeExplanations\x1a\x19\n\x17\x41rizeConclusionPointers\x1a\x1a\n\x18\x41rizeExplanationPointers\x1a\xff\x08\n\x0b\x41rrowSchema\x12!\n\x19prediction_id_column_name\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_column_names\x18\x02 \x03(\t\x12\x1d\n\x15timestamp_column_name\x18\x03 \x01(\t\x12$\n\x1cprediction_label_column_name\x18\x04 \x01(\t\x12$\n\x1cprediction_score_column_name\x18\x05 \x01(\t\x12 \n\x18\x61\x63tual_label_column_name\x18\x06 \x01(\t\x12 \n\x18\x61\x63tual_score_column_name\x18\x07 \x01(\t\x12W\n\x18shap_values_column_names\x18\x08 \x03(\x0b\x32\x35.public.Schema.ArrowSchema.ShapValuesColumnNamesEntry\x12\x18\n\x10tag_column_names\x18\t \x03(\t\x12/\n#actual_numeric_sequence_column_name\x18\n \x01(\tB\x02\x18\x01\x12O\n\x1e\x65mbedding_feature_column_names\x18\x0b \x03(\x0b\x32#.public.Schema.EmbeddingColumnNamesB\x02\x18\x01\x12%\n\x1dmodel_environment_column_name\x18\x0c \x01(\t\x12!\n\x19model_version_column_name\x18\r \x01(\t\x12\x1c\n\x14\x62\x61tch_id_column_name\x18\x0e \x01(\t\x12\'\n\x1fprediction_group_id_column_name\x18\x0f \x01(\t\x12\x18\n\x10rank_column_name\x18\x10 \x01(\t\x12j\n\"embedding_feature_column_names_map\x18\x11 \x03(\x0b\x32>.public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry\x12\x66\n.prediction_object_detection_label_column_names\x18\x12 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12\x62\n*actual_object_detection_label_column_names\x18\x13 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x1a<\n\x1aShapValuesColumnNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aj\n#EmbeddingFeatureColumnNamesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames:\x02\x38\x01\x1a\x93\x01\n\x1fObjectDetectionLabelColumnNames\x12&\n\x1e\x62\x62oxes_coordinates_column_name\x18\x01 \x01(\t\x12%\n\x1d\x62\x62oxes_categories_column_name\x18\x02 \x01(\t\x12!\n\x19\x62\x62oxes_scores_column_name\x18\x03 \x01(\t\x1an\n\x14\x45mbeddingColumnNames\x12\x1a\n\x12vector_column_name\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61ta_column_name\x18\x02 \x01(\t\x12 \n\x18link_to_data_column_name\x18\x03 \x01(\t\x1a\x8c\x15\n\rGenericSchema\x12\x43\n\rprediction_id\x18\x01 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\ttimestamp\x18\x03 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_label\x18\x04 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_score\x18\x05 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_label\x18\x06 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_score\x18\x07 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x0bshap_values\x18\x08 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\x04tags\x18\t \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12G\n\x11model_environment\x18\n \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rmodel_version\x18\x0b \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12>\n\x08\x62\x61tch_id\x18\x0c \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12=\n\x07\x65xclude\x18\r \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12Q\n\x17\x61\x63tual_numeric_sequence\x18\x0e \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptorB\x02\x18\x01\x12Q\n\x12\x65mbedding_features\x18\x0f \x01(\x0b\x32\x35.public.Schema.GenericSchema.EmbeddingFieldDescriptor\x12I\n\x13prediction_group_id\x18\x10 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12:\n\x04rank\x18\x11 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12k\n!prediction_object_detection_label\x18\x12 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12g\n\x1d\x61\x63tual_object_detection_label\x18\x13 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12\x46\n\x10\x63hange_timestamp\x18\x14 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rfeatures_list\x18\x15 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12?\n\ttags_list\x18\x16 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x1a%\n\x0f\x46ieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x1a\x41\n\x14GroupFieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x12\x15\n\rcapture_group\x18\x02 \x01(\t\x1a\xba\x03\n\x18\x45mbeddingFieldDescriptor\x12Y\n\nproperties\x18\x01 \x03(\x0b\x32\x45.public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry\x1a\xc3\x01\n\x14\x45mbeddingPropertyMap\x12u\n\x0eproperties_map\x18\x01 \x03(\x0b\x32].public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a}\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0b\x32J.public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap:\x02\x38\x01\x1a\x89\x04\n#ObjectDetectionLabelFieldDescriptor\x12\x64\n\nproperties\x18\x01 \x03(\x0b\x32P.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry\x1a\xe5\x01\n\x1fObjectDetectionLabelPropertyMap\x12\x8b\x01\n\x0eproperties_map\x18\x01 \x03(\x0b\x32s.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x93\x01\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12o\n\x05value\x18\x02 \x01(\x0b\x32`.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap:\x02\x38\x01\"T\n\x0b\x45nvironment\x12\x17\n\x13UNKNOWN_ENVIRONMENT\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\x86\x01\n\tModelType\x12\x15\n\x11UNKNOWN_MODELTYPE\x10\x00\x12\n\n\x06\x42INARY\x10\x01\x12\x0b\n\x07NUMERIC\x10\x02\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x03\x12\x15\n\x11SCORE_CATEGORICAL\x10\x04\x12\x0b\n\x07RANKING\x10\x05\x12\x14\n\x10OBJECT_DETECTION\x10\x06\x42\x08\n\x06schema\"I\n\x17\x41rrowFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x1f\n\x17real_time_ingestion_uri\x18\x02 \x01(\t\":\n\x16UserFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x11\n\tfile_uuid\x18\x02 \x01(\tBO\n\x12\x63om.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/publicb\x06proto3'
+  serialized_pb=b'\n\x0cpublic.proto\x12\x06public\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x01\n\nBulkRecord\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x1f\n\x07records\x18\x05 \x03(\x0b\x32\x0e.public.Record\x12\x11\n\tspace_key\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05R\ttimestamp\"\x99\x05\n\x06Record\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rprediction_id\x18\x03 \x01(\t\x12&\n\nprediction\x18\x08 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\t \x01(\x0b\x32\x0e.public.Actual\x12\x37\n\x13\x66\x65\x61ture_importances\x18\n \x01(\x0b\x32\x1a.public.FeatureImportances\x12:\n\x15prediction_and_actual\x18\x0b \x01(\x0b\x32\x1b.public.PredictionAndActual\x12\x11\n\tspace_key\x18\x0c \x01(\t\x12<\n\x12\x65nvironment_params\x18\r \x01(\x0b\x32 .public.Record.EnvironmentParams\x1a\xa1\x02\n\x11\x45nvironmentParams\x12=\n\x08training\x18\x01 \x01(\x0b\x32).public.Record.EnvironmentParams.TrainingH\x00\x12\x41\n\nvalidation\x18\x02 \x01(\x0b\x32+.public.Record.EnvironmentParams.ValidationH\x00\x12\x41\n\nproduction\x18\x03 \x01(\x0b\x32+.public.Record.EnvironmentParams.ProductionH\x00\x1a\n\n\x08Training\x1a\x1e\n\nValidation\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x1a\x0c\n\nProductionB\r\n\x0b\x65nvironmentJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xae\x02\n\x13PreProductionRecord\x12\x45\n\x0ftraining_record\x18\x01 \x01(\x0b\x32*.public.PreProductionRecord.TrainingRecordH\x00\x12I\n\x11validation_record\x18\x02 \x01(\x0b\x32,.public.PreProductionRecord.ValidationRecordH\x00\x1a\x44\n\x10ValidationRecord\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x1e\n\x06record\x18\x02 \x01(\x0b\x32\x0e.public.Record\x1a\x30\n\x0eTrainingRecord\x12\x1e\n\x06record\x18\x01 \x01(\x0b\x32\x0e.public.RecordB\r\n\x0brecord_type\"\x86\x03\n\x10ScoreCategorical\x12\x17\n\x0b\x63\x61tegorical\x18\x01 \x01(\tB\x02\x18\x01\x12\x11\n\x05score\x18\x02 \x01(\x01\x42\x02\x18\x01\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0b\x32!.public.ScoreCategorical.CategoryH\x00\x12@\n\x0escore_category\x18\x04 \x01(\x0b\x32&.public.ScoreCategorical.ScoreCategoryH\x00\x12:\n\x0bscore_value\x18\x05 \x01(\x0b\x32#.public.ScoreCategorical.ScoreValueH\x00\x1a\x1c\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x1a\x1b\n\nScoreValue\x12\r\n\x05value\x18\x01 \x01(\x01\x1aN\n\rScoreCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1c\n\x10numeric_sequence\x18\x03 \x03(\x01\x42\x02\x18\x01\x42\x06\n\x04type\"\xb1\x01\n\x0fObjectDetection\x12;\n\x0e\x62ounding_boxes\x18\x01 \x03(\x0b\x32#.public.ObjectDetection.BoundingBox\x1a\x61\n\x0b\x42oundingBox\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12+\n\x05score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x85\x01\n\x11RankingPrediction\x12\x1b\n\x13prediction_group_id\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x02 \x01(\x03\x12\x36\n\x10prediction_score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\r\n\x05label\x18\x04 \x01(\t\"l\n\rRankingActual\x12$\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32\x12.public.MultiValue\x12\x35\n\x0frelevance_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x82\x01\n\x05Label\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x42\x06\n\x04\x64\x61ta\"\xef\x01\n\x0fPredictionLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12,\n\x07ranking\x18\x05 \x01(\x0b\x32\x19.public.RankingPredictionH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\xe7\x01\n\x0b\x41\x63tualLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12(\n\x07ranking\x18\x05 \x01(\x0b\x32\x15.public.RankingActualH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x42\x06\n\x04\x64\x61ta\"\x83\x03\n\nPrediction\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12 \n\x05label\x18\x03 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12\x32\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32 .public.Prediction.FeaturesEntry\x12*\n\x04tags\x18\x05 \x03(\x0b\x32\x1c.public.Prediction.TagsEntry\x12\x31\n\x10prediction_label\x18\x06 \x01(\x0b\x32\x17.public.PredictionLabel\x1a>\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\x95\x01\n\x05Value\x12\x10\n\x06string\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12)\n\x0bmulti_value\x18\x04 \x01(\x0b\x32\x12.public.MultiValueH\x00\x12&\n\tembedding\x18\x05 \x01(\x0b\x32\x11.public.EmbeddingH\x00\x42\x06\n\x04\x64\x61ta\"\x1c\n\nMultiValue\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xed\x01\n\tEmbedding\x12\x0e\n\x06vector\x18\x01 \x03(\x01\x12\x32\n\x0clink_to_data\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08raw_data\x18\x04 \x01(\x0b\x32\x19.public.Embedding.RawData\x1aK\n\x07RawData\x12\x32\n\ntokenArray\x18\x02 \x01(\x0b\x32\x1c.public.Embedding.TokenArrayH\x00\x42\x06\n\x04typeJ\x04\x08\x01\x10\x02\x1a\x1c\n\nTokenArray\x12\x0e\n\x06tokens\x18\x01 \x03(\tJ\x04\x08\x02\x10\x03\"\xe8\x01\n\x06\x41\x63tual\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x05label\x18\x02 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12&\n\x04tags\x18\x03 \x03(\x0b\x32\x18.public.Actual.TagsEntry\x12)\n\x0c\x61\x63tual_label\x18\x04 \x01(\x0b\x32\x13.public.ActualLabel\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xe6\x01\n\x12\x46\x65\x61tureImportances\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12O\n\x13\x66\x65\x61ture_importances\x18\x03 \x03(\x0b\x32\x32.public.FeatureImportances.FeatureImportancesEntry\x1a\x39\n\x17\x46\x65\x61tureImportancesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"]\n\x13PredictionAndActual\x12&\n\nprediction\x18\x01 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x0e.public.Actual\"\x8b\x01\n\nFileHeader\x12\x33\n\x0b\x65nvironment\x18\x01 \x01(\x0e\x32\x1e.public.FileHeader.Environment\"H\n\x0b\x45nvironment\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\xd7\'\n\x06Schema\x12+\n\tconstants\x18\x01 \x01(\x0b\x32\x18.public.Schema.Constants\x12<\n\x11\x61rize_conclusions\x18\x02 \x01(\x0b\x32\x1f.public.Schema.ArizeConclusionsH\x00\x12>\n\x12\x61rize_explanations\x18\x03 \x01(\x0b\x32 .public.Schema.ArizeExplanationsH\x00\x12\x32\n\x0c\x61rrow_schema\x18\x04 \x01(\x0b\x32\x1a.public.Schema.ArrowSchemaH\x00\x12\x36\n\x0egeneric_schema\x18\x05 \x01(\x0b\x32\x1c.public.Schema.GenericSchemaH\x00\x12K\n\x19\x61rize_conclusion_pointers\x18\x06 \x01(\x0b\x32&.public.Schema.ArizeConclusionPointersH\x00\x12M\n\x1a\x61rize_explanation_pointers\x18\x07 \x01(\x0b\x32\'.public.Schema.ArizeExplanationPointersH\x00\x1a\xa5\x01\n\tConstants\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\t\x12/\n\x0b\x65nvironment\x18\x04 \x01(\x0e\x32\x1a.public.Schema.Environment\x12,\n\nmodel_type\x18\x05 \x01(\x0e\x32\x18.public.Schema.ModelType\x1a\x12\n\x10\x41rizeConclusions\x1a\x13\n\x11\x41rizeExplanations\x1a\x19\n\x17\x41rizeConclusionPointers\x1a\x1a\n\x18\x41rizeExplanationPointers\x1a\xff\x08\n\x0b\x41rrowSchema\x12!\n\x19prediction_id_column_name\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_column_names\x18\x02 \x03(\t\x12\x1d\n\x15timestamp_column_name\x18\x03 \x01(\t\x12$\n\x1cprediction_label_column_name\x18\x04 \x01(\t\x12$\n\x1cprediction_score_column_name\x18\x05 \x01(\t\x12 \n\x18\x61\x63tual_label_column_name\x18\x06 \x01(\t\x12 \n\x18\x61\x63tual_score_column_name\x18\x07 \x01(\t\x12W\n\x18shap_values_column_names\x18\x08 \x03(\x0b\x32\x35.public.Schema.ArrowSchema.ShapValuesColumnNamesEntry\x12\x18\n\x10tag_column_names\x18\t \x03(\t\x12/\n#actual_numeric_sequence_column_name\x18\n \x01(\tB\x02\x18\x01\x12O\n\x1e\x65mbedding_feature_column_names\x18\x0b \x03(\x0b\x32#.public.Schema.EmbeddingColumnNamesB\x02\x18\x01\x12%\n\x1dmodel_environment_column_name\x18\x0c \x01(\t\x12!\n\x19model_version_column_name\x18\r \x01(\t\x12\x1c\n\x14\x62\x61tch_id_column_name\x18\x0e \x01(\t\x12\'\n\x1fprediction_group_id_column_name\x18\x0f \x01(\t\x12\x18\n\x10rank_column_name\x18\x10 \x01(\t\x12j\n\"embedding_feature_column_names_map\x18\x11 \x03(\x0b\x32>.public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry\x12\x66\n.prediction_object_detection_label_column_names\x18\x12 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12\x62\n*actual_object_detection_label_column_names\x18\x13 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x1a<\n\x1aShapValuesColumnNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aj\n#EmbeddingFeatureColumnNamesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames:\x02\x38\x01\x1a\x93\x01\n\x1fObjectDetectionLabelColumnNames\x12&\n\x1e\x62\x62oxes_coordinates_column_name\x18\x01 \x01(\t\x12%\n\x1d\x62\x62oxes_categories_column_name\x18\x02 \x01(\t\x12!\n\x19\x62\x62oxes_scores_column_name\x18\x03 \x01(\t\x1an\n\x14\x45mbeddingColumnNames\x12\x1a\n\x12vector_column_name\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61ta_column_name\x18\x02 \x01(\t\x12 \n\x18link_to_data_column_name\x18\x03 \x01(\t\x1a\x8c\x15\n\rGenericSchema\x12\x43\n\rprediction_id\x18\x01 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\ttimestamp\x18\x03 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_label\x18\x04 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_score\x18\x05 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_label\x18\x06 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_score\x18\x07 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x0bshap_values\x18\x08 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\x04tags\x18\t \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12G\n\x11model_environment\x18\n \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rmodel_version\x18\x0b \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12>\n\x08\x62\x61tch_id\x18\x0c \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12=\n\x07\x65xclude\x18\r \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12Q\n\x17\x61\x63tual_numeric_sequence\x18\x0e \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptorB\x02\x18\x01\x12Q\n\x12\x65mbedding_features\x18\x0f \x01(\x0b\x32\x35.public.Schema.GenericSchema.EmbeddingFieldDescriptor\x12I\n\x13prediction_group_id\x18\x10 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12:\n\x04rank\x18\x11 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12k\n!prediction_object_detection_label\x18\x12 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12g\n\x1d\x61\x63tual_object_detection_label\x18\x13 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12\x46\n\x10\x63hange_timestamp\x18\x14 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rfeatures_list\x18\x15 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12?\n\ttags_list\x18\x16 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x1a%\n\x0f\x46ieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x1a\x41\n\x14GroupFieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x12\x15\n\rcapture_group\x18\x02 \x01(\t\x1a\xba\x03\n\x18\x45mbeddingFieldDescriptor\x12Y\n\nproperties\x18\x01 \x03(\x0b\x32\x45.public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry\x1a\xc3\x01\n\x14\x45mbeddingPropertyMap\x12u\n\x0eproperties_map\x18\x01 \x03(\x0b\x32].public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a}\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0b\x32J.public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap:\x02\x38\x01\x1a\x89\x04\n#ObjectDetectionLabelFieldDescriptor\x12\x64\n\nproperties\x18\x01 \x03(\x0b\x32P.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry\x1a\xe5\x01\n\x1fObjectDetectionLabelPropertyMap\x12\x8b\x01\n\x0eproperties_map\x18\x01 \x03(\x0b\x32s.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x93\x01\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12o\n\x05value\x18\x02 \x01(\x0b\x32`.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap:\x02\x38\x01\"T\n\x0b\x45nvironment\x12\x17\n\x13UNKNOWN_ENVIRONMENT\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\"\x9a\x01\n\tModelType\x12\x15\n\x11UNKNOWN_MODELTYPE\x10\x00\x12\n\n\x06\x42INARY\x10\x01\x12\x0b\n\x07NUMERIC\x10\x02\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x03\x12\x15\n\x11SCORE_CATEGORICAL\x10\x04\x12\x0b\n\x07RANKING\x10\x05\x12\x14\n\x10OBJECT_DETECTION\x10\x06\x12\x12\n\x0eGENERATIVE_LLM\x10\x07\x42\x08\n\x06schema\"I\n\x17\x41rrowFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x1f\n\x17real_time_ingestion_uri\x18\x02 \x01(\t\":\n\x16UserFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x11\n\tfile_uuid\x18\x02 \x01(\tBO\n\x12\x63om.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/publicb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,])
 
 
 
 _FILEHEADER_ENVIRONMENT = _descriptor.EnumDescriptor(
   name='Environment',
@@ -135,19 +135,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='OBJECT_DETECTION', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='GENERATIVE_LLM', index=7, number=7,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=8989,
-  serialized_end=9123,
+  serialized_start=9078,
+  serialized_end=9232,
 )
 _sym_db.RegisterEnumDescriptor(_SCHEMA_MODELTYPE)
 
 
 _BULKRECORD = _descriptor.Descriptor(
   name='BulkRecord',
   full_name='public.BulkRecord',
@@ -2716,16 +2721,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='schema', full_name='public.Schema.schema',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=4074,
-  serialized_end=9133,
+  serialized_start=4163,
+  serialized_end=9242,
 )
 
 
 _ARROWFILEUPLOADRESPONSE = _descriptor.Descriptor(
   name='ArrowFileUploadResponse',
   full_name='public.ArrowFileUploadResponse',
   filename=None,
@@ -2755,16 +2760,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9135,
-  serialized_end=9208,
+  serialized_start=9244,
+  serialized_end=9317,
 )
 
 
 _USERFILEUPLOADRESPONSE = _descriptor.Descriptor(
   name='UserFileUploadResponse',
   full_name='public.UserFileUploadResponse',
   filename=None,
@@ -2794,16 +2799,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9210,
-  serialized_end=9268,
+  serialized_start=9319,
+  serialized_end=9377,
 )
 
 _BULKRECORD.fields_by_name['records'].message_type = _RECORD
 _RECORD_ENVIRONMENTPARAMS_TRAINING.containing_type = _RECORD_ENVIRONMENTPARAMS
 _RECORD_ENVIRONMENTPARAMS_VALIDATION.containing_type = _RECORD_ENVIRONMENTPARAMS
 _RECORD_ENVIRONMENTPARAMS_PRODUCTION.containing_type = _RECORD_ENVIRONMENTPARAMS
 _RECORD_ENVIRONMENTPARAMS.fields_by_name['training'].message_type = _RECORD_ENVIRONMENTPARAMS_TRAINING
```

### Comparing `arize-7.0.0rc5/arize/utils/logging.py` & `arize-7.0.0rc6/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/utils/model_mapping.json` & `arize-7.0.0rc6/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/utils/types.py` & `arize-7.0.0rc6/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize/utils/utils.py` & `arize-7.0.0rc6/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/arize.egg-info/PKG-INFO` & `arize-7.0.0rc6/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.0rc5
+Version: 7.0.0rc6
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
```

### Comparing `arize-7.0.0rc5/arize.egg-info/SOURCES.txt` & `arize-7.0.0rc6/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.0.0rc5/setup.cfg` & `arize-7.0.0rc6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 	Arize AI = https://www.arize.com
 author = Arize AI
 author_email = support@arize.com
 license = BSD
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Logging
```

### Comparing `arize-7.0.0rc5/tests/test_api.py` & `arize-7.0.0rc6/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from pathlib import Path
 
 import arize.public_pb2 as pb2
 import numpy as np
 import pandas as pd
 import pytest
 from arize.api import Client, Embedding
+from arize.pandas.validation.errors import InvalidAdditionalHeaders
 from arize.utils.types import (
     Environments,
     ModelTypes,
     ObjectDetectionLabel,
     RankingActualLabel,
     RankingPredictionLabel,
 )
+from arize.utils.utils import get_python_version
 from google.protobuf.wrappers_pb2 import DoubleValue, StringValue
 
 BOOL_VAL = True
 STR_VAL = "arize"
 INT_VAL = 5
 FLOAT_VAL = 20.20
 NP_FLOAT = float(1.2)
@@ -26,15 +28,14 @@
     "model_version": "v1.2.3.4",
     "model_type_numeric": ModelTypes.NUMERIC,
     "model_type_score_categorical": ModelTypes.SCORE_CATEGORICAL,
     "model_type_regression": ModelTypes.REGRESSION,
     "model_type_binary_classification": ModelTypes.BINARY_CLASSIFICATION,
     "model_type_object_detection": ModelTypes.OBJECT_DETECTION,
     "model_type_ranking": ModelTypes.RANKING,
-    "model_version": "v1.2.3.4",
     "environment_training": Environments.TRAINING,
     "environment_validation": Environments.VALIDATION,
     "environment_production": Environments.PRODUCTION,
     "batch_id": "batch_id",
     "batch": "batch1234",
     "api_key": "API_KEY",
     "prediction_id": "prediction_0",
@@ -327,16 +328,21 @@
         "tag_double": pb2.Value(double=FLOAT_VAL),
         "tag_int": pb2.Value(int=INT_VAL),
         "tag_bool": pb2.Value(string=str(BOOL_VAL)),
     }
     return pb2.Actual(tags=tags)
 
 
-def get_stubbed_client():
-    c = Client(space_key="test_space", api_key="API_KEY", uri="https://localhost:443")
+def get_stubbed_client(additional_headers=None):
+    c = Client(
+        space_key=inputs["space_key"],
+        api_key=inputs["api_key"],
+        uri="https://localhost:443",
+        additional_headers=additional_headers,
+    )
 
     def _post(record, uri, indexes):
         return record
 
     c._post = _post
     return c
 
@@ -1127,9 +1133,33 @@
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Bounding box confidence scores must be between 0 and 1, inclusive" in str(excinfo.value)
 
 
+def test_instantiating_client_duplicated_header():
+    with pytest.raises(InvalidAdditionalHeaders) as excinfo:
+        _ = get_stubbed_client({"authorization": "FAKE_VALUE"})
+    assert (
+        "Found invalid additional header, cannot use reserved headers named: authorization."
+        in str(excinfo.value)
+    )
+
+
+def test_instantiating_client_additional_header():
+    c = get_stubbed_client({"JWT": "FAKE_VALUE"})
+    import arize
+
+    expected = {
+        "authorization": inputs["api_key"],
+        "Grpc-Metadata-space": inputs["space_key"],
+        "Grpc-Metadata-sdk-version": arize.__version__,
+        "Grpc-Metadata-python-version": get_python_version(),
+        "Grpc-Metadata-sdk": "py",
+        "JWT": "FAKE_VALUE",
+    }
+    assert c._header == expected
+
+
 if __name__ == "__main__":
     raise SystemExit(pytest.main([__file__]))
```

### Comparing `arize-7.0.0rc5/tests/test_utils.py` & `arize-7.0.0rc6/tests/test_utils.py`

 * *Files identical despite different names*

