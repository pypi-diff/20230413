# Comparing `tmp/rxn-onmt-utils-1.0.1.tar.gz` & `tmp/rxn-onmt-utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-onmt-utils-1.0.1.tar", last modified: Fri Mar 10 09:35:02 2023, max compression
+gzip compressed data, was "rxn-onmt-utils-1.0.2.tar", last modified: Thu Apr 13 15:36:39 2023, max compression
```

## Comparing `rxn-onmt-utils-1.0.1.tar` & `rxn-onmt-utils-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-10 09:35:02.574320 rxn-onmt-utils-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/internal_translation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/model_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/model_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/strip_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/train_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-10 09:34:53.000000 rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 09:35:02.570320 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-10 09:35:02.000000 rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.470267 rxn-onmt-utils-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.466266 rxn-onmt-utils-1.0.2/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.470267 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/internal_translation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.470267 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/strip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/train_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-13 15:36:29.000000 rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:36:39.474267 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 15:36:39.000000 rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/top_level.txt
```

### Comparing `rxn-onmt-utils-1.0.1/LICENSE` & `rxn-onmt-utils-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/PKG-INFO` & `rxn-onmt-utils-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-onmt-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities related to the use of OpenNMT
 Home-page: https://github.com/rxn4chemistry/rxn-onmt-utils
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-onmt-utils/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-onmt-utils
 Classifier: Operating System :: OS Independent
```

### Comparing `rxn-onmt-utils-1.0.1/README.md` & `rxn-onmt-utils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/internal_translation_utils.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/internal_translation_utils.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/model_introspection.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_introspection.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/model_resize.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/model_resize.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/extend_model_with_vocab.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     "-v",
     required=True,
     help="Vocab for finetuning (vocab.pt generated by ONMT).",
 )
 @click.option(
     "--output_path", "-o", required=True, help="Where to save the resized model."
 )
-def extend_model_vocab(model_path: str, vocab_path: str, output_path: str):
+def main(model_path: str, vocab_path: str, output_path: str):
     """Extend model vocab, resize and initialise additional weights."""
 
     resizer = ModelResizer(model_path)
 
     resizer.extend_vocab(vocab_path)
 
     resizer.save_checkpoint(output_path)
 
 
 if __name__ == "__main__":
-    extend_model_vocab()
+    main()
```

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/scripts/translate.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/scripts/translate.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/train_command.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/train_command.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/translate.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translate.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn/onmt_utils/translator.py` & `rxn-onmt-utils-1.0.2/src/rxn/onmt_utils/translator.py`

 * *Files identical despite different names*

### Comparing `rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/PKG-INFO` & `rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rxn-onmt-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities related to the use of OpenNMT
 Home-page: https://github.com/rxn4chemistry/rxn-onmt-utils
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-onmt-utils/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-onmt-utils
 Classifier: Operating System :: OS Independent
```

### Comparing `rxn-onmt-utils-1.0.1/src/rxn_onmt_utils.egg-info/SOURCES.txt` & `rxn-onmt-utils-1.0.2/src/rxn_onmt_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

