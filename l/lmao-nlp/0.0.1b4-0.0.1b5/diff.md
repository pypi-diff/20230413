# Comparing `tmp/lmao-nlp-0.0.1b4.tar.gz` & `tmp/lmao-nlp-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b4.tar", last modified: Sun Apr  9 16:12:34 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b5.tar", last modified: Thu Apr 13 01:57:31 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b4.tar` & `lmao-nlp-0.0.1b5.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.439471 lmao-nlp-0.0.1b4/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b4/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-09 16:12:34.439296 lmao-nlp-0.0.1b4/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-02 17:45:52.000000 lmao-nlp-0.0.1b4/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b4/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-09 16:12:34.439516 lmao-nlp-0.0.1b4/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1437 2023-04-09 16:12:30.000000 lmao-nlp-0.0.1b4/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.433156 lmao-nlp-0.0.1b4/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.434154 lmao-nlp-0.0.1b4/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      129 2023-04-09 16:12:30.000000 lmao-nlp-0.0.1b4/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.434814 lmao-nlp-0.0.1b4/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      110 2023-04-09 15:34:12.000000 lmao-nlp-0.0.1b4/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      846 2023-04-09 15:38:24.000000 lmao-nlp-0.0.1b4/src/lmao/adapters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2023 2023-04-09 15:44:23.000000 lmao-nlp-0.0.1b4/src/lmao/adapters/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.435443 lmao-nlp-0.0.1b4/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-08 21:16:32.000000 lmao-nlp-0.0.1b4/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.436236 lmao-nlp-0.0.1b4/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       27 2023-04-03 22:26:17.000000 lmao-nlp-0.0.1b4/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     3395 2023-04-09 15:39:17.000000 lmao-nlp-0.0.1b4/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2845 2023-04-09 15:38:24.000000 lmao-nlp-0.0.1b4/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.436985 lmao-nlp-0.0.1b4/src/lmao/lm/prompts/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      105 2023-04-08 18:47:45.000000 lmao-nlp-0.0.1b4/src/lmao/lm/prompts/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1080 2023-04-08 21:54:48.000000 lmao-nlp-0.0.1b4/src/lmao/lm/prompts/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1607 2023-04-09 15:19:32.000000 lmao-nlp-0.0.1b4/src/lmao/lm/prompts/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.437581 lmao-nlp-0.0.1b4/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-02 16:55:57.000000 lmao-nlp-0.0.1b4/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-09 15:35:32.000000 lmao-nlp-0.0.1b4/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-09 15:19:42.000000 lmao-nlp-0.0.1b4/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1976 2023-04-09 03:26:12.000000 lmao-nlp-0.0.1b4/src/lmao/lm/utils.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1756 2023-04-09 15:35:17.000000 lmao-nlp-0.0.1b4/src/lmao/loader.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.438306 lmao-nlp-0.0.1b4/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       93 2023-04-09 15:33:39.000000 lmao-nlp-0.0.1b4/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      177 2023-04-09 15:23:07.000000 lmao-nlp-0.0.1b4/src/lmao/orchestrators/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1131 2023-04-09 15:32:16.000000 lmao-nlp-0.0.1b4/src/lmao/orchestrators/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-09 16:12:34.439111 lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-09 16:12:34.000000 lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)      782 2023-04-09 16:12:34.000000 lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-09 16:12:34.000000 lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-09 16:12:34.000000 lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-09 16:12:34.000000 lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.182344 lmao-nlp-0.0.1b5/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b5/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-13 01:57:31.182181 lmao-nlp-0.0.1b5/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1853 2023-04-13 01:54:40.000000 lmao-nlp-0.0.1b5/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b5/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-13 01:57:31.182384 lmao-nlp-0.0.1b5/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1437 2023-04-13 01:57:28.000000 lmao-nlp-0.0.1b5/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.177026 lmao-nlp-0.0.1b5/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178029 lmao-nlp-0.0.1b5/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      232 2023-04-13 01:57:28.000000 lmao-nlp-0.0.1b5/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178323 lmao-nlp-0.0.1b5/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      151 2023-04-12 16:05:36.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      722 2023-04-12 16:15:07.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/chatbot.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178696 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       50 2023-04-12 14:54:23.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      878 2023-04-12 02:01:57.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2119 2023-04-13 01:32:11.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/classification.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178981 lmao-nlp-0.0.1b5/src/lmao/lm/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-08 21:16:32.000000 lmao-nlp-0.0.1b5/src/lmao/lm/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.179505 lmao-nlp-0.0.1b5/src/lmao/lm/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       67 2023-04-11 21:11:07.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2081 2023-04-12 02:42:12.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5003 2023-04-13 01:30:54.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2820 2023-04-13 01:37:43.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.179921 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      105 2023-04-08 18:47:45.000000 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1070 2023-04-09 17:21:49.000000 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1607 2023-04-09 15:19:32.000000 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/classification.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.180595 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-11 21:04:00.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-11 22:13:08.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-09 15:35:32.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-11 20:57:46.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1976 2023-04-09 03:26:12.000000 lmao-nlp-0.0.1b5/src/lmao/lm/utils.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2858 2023-04-12 16:08:12.000000 lmao-nlp-0.0.1b5/src/lmao/loader.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.181141 lmao-nlp-0.0.1b5/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       93 2023-04-09 15:33:39.000000 lmao-nlp-0.0.1b5/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      177 2023-04-09 15:23:07.000000 lmao-nlp-0.0.1b5/src/lmao/orchestrators/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1175 2023-04-12 02:01:57.000000 lmao-nlp-0.0.1b5/src/lmao/orchestrators/classification.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.182006 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      925 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b4/LICENSE` & `lmao-nlp-0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b4/PKG-INFO` & `lmao-nlp-0.0.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b4/pyproject.toml` & `lmao-nlp-0.0.1b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b4/setup.py` & `lmao-nlp-0.0.1b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.1-beta.4"
+__version__ = "0.0.1-beta.5"
 
 with open("requirements.txt", "r") as f:
     install_requires = [line.replace("==", ">=") for line in f.read().splitlines() if line != "" if line[0] != "#"]
 
 extras_require = {}
 
 with open("requirements-dev.txt", "r") as f:
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao/adapters/base.py` & `lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     CLIENT_ERROR: str
     PREDICTION_ERROR: str
 
 
 @dataclass
 class TaskAdapterResponse:
     prediction: str
-    llm_response: ClientResponse
+    lm_response: ClientResponse
     success: bool
 
 
 class TaskAdapter(ABC):
-    def __init__(self, lm: BaseClient, lm_method_name: str, prompter: Prompter):
-        self.lm = lm
+    def __init__(self, lm_client: BaseClient, client_method_name: str, prompter: Prompter):
+        self.lm_client = lm_client
         self.prompter = prompter
-        self.lm_method_name = lm_method_name
+        self.client_method_name = client_method_name
 
     @abstractmethod
     def predict(self, text: str) -> TaskAdapterResponse:
         pass
 
 
 adapter_errors = TaskAdapterErrors(CLIENT_ERROR="CLIENT ERROR", PREDICTION_ERROR="PREDICTION ERROR")
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao/adapters/classification.py` & `lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/classification.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from typing import List
 
-from lmao.adapters.base import TaskAdapter, TaskAdapterResponse, adapter_errors
+from lmao.adapters.tasks.base import TaskAdapter, TaskAdapterResponse, adapter_errors
 from lmao.lm.clients.base import SUCCESS_STATUS_CODE, BaseClient
 from lmao.lm.prompts.classification import ClassificationPrompter, SentimentAnalysisPrompter
 
 __all__ = ["TextClassificationAdapter", "SentimentAnalysisAdapter"]
 
 
 class TextClassificationAdapter(TaskAdapter):
-    def __init__(self, lm: BaseClient, lm_method_name: str, categories: List[str], lowercase: bool = True, **kwargs):
+    def __init__(
+        self, lm_client: BaseClient, client_method_name: str, categories: List[str], lowercase: bool = True, **kwargs
+    ):
         self.lowercase = lowercase
         self.categories = [c.lower() for c in categories] if lowercase else categories
         prompter = kwargs.pop("prompter", None) or ClassificationPrompter(categories=self.categories, **kwargs)
-        super().__init__(lm=lm, lm_method_name=lm_method_name, prompter=prompter)
+        super().__init__(lm_client=lm_client, client_method_name=client_method_name, prompter=prompter)
 
     def predict(self, text: str, **kwargs) -> TaskAdapterResponse:
-        response = getattr(self.lm, self.lm_method_name)(self.prompter.create_prompt(text), **kwargs)
+        response = getattr(self.lm_client, self.client_method_name)(self.prompter.create_prompt(text), **kwargs)
         success = True
         if response.status_code == SUCCESS_STATUS_CODE:
             prediction = response.text.strip().lower() if self.lowercase else response.text.strip()
             prediction = prediction.replace(".", "")
             if prediction not in self.categories:
                 prediction = adapter_errors.PREDICTION_ERROR
                 success = False
         else:
             prediction = adapter_errors.CLIENT_ERROR
             success = False
-        return TaskAdapterResponse(prediction=prediction, llm_response=response, success=success)
+        return TaskAdapterResponse(prediction=prediction, lm_response=response, success=success)
 
 
 class SentimentAnalysisAdapter(TextClassificationAdapter):
-    def __init__(self, lm: BaseClient, lm_method_name: str, include_neutral: bool = True, **kwargs):
+    def __init__(self, lm_client: BaseClient, client_method_name: str, include_neutral: bool = True, **kwargs):
         super().__init__(
-            lm=lm,
-            lm_method_name=lm_method_name,
+            lm_client=lm_client,
+            client_method_name=client_method_name,
             categories=["positive", "negative"] + (["neutral"] if include_neutral else []),
             lowercase=True,
             prompter=SentimentAnalysisPrompter(include_neutral=include_neutral, **kwargs),
         )
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b5/src/lmao/lm/clients/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,140 @@
 import os
 import re
-from abc import ABC, abstractmethod
+from abc import ABC, abstractmethod, abstractstaticmethod
 from collections import deque
-from dataclasses import dataclass
-from typing import Deque, List, Optional, Tuple
+from typing import Callable, Deque, List, NamedTuple, Optional, Tuple
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 __all__ = ["ClientResponse", "BaseClient", "ChatHistory", "SUCCESS_STATUS_CODE"]
+
+
+class APIHeader(NamedTuple):
+    key: str
+    value: Callable
+
+
 SUCCESS_STATUS_CODE = 200
+API_HEADER_FORMAT_DICT = {
+    "x-api-key": APIHeader(key="X-API-Key", value=lambda api_key: api_key),
+    "basic authentication": APIHeader(key="Authorization", value=lambda api_key: f"Basic {api_key}"),
+    "bearer authentication": APIHeader(key="Authorization", value=lambda api_key: f"Bearer {api_key}"),
+}
 
 
-@dataclass
-class ClientResponse:
+class ClientResponse(NamedTuple):
     text: Optional[str]
     raw_response: dict
     status_code: int
 
     def __repr__(self):
-        repr = "\n".join([f"{k}: {v}" for k, v in self.__dict__.items()])
+        repr = "\n".join([f"{k}: {v}" for k, v in self._asdict().items()])
         repr = re.sub(r"^", " " * 4, repr, 0, re.M)
         return f"{self.__class__.__name__}({{\n{repr}\n}})"
 
 
 class ChatHistory(ABC):
-    def __init__(self, length: int = 10):
-        self.length = length
-        self._messages: Deque = deque(maxlen=length)
+    human_role: str = "human"
+    assistant_role: str = "assistant"
 
-    @abstractmethod
-    def append(self, *args, **kwargs):
+    def __init__(self, max_length: int = 10):
+        self.max_length = max_length
+        self._messages: Deque = deque(maxlen=max_length)
+
+    @abstractstaticmethod
+    def check_message_format(message):
         pass
 
     @abstractmethod
-    def check_message_format(self, message):
+    def to_request_format(self):
         pass
 
+    def add_assistant_message(self, message: str):
+        self.append(role=self.assistant_role, content=message)
+
+    def add_human_message(self, message: str):
+        self.append(role=self.human_role, content=message)
+
+    def append(self, role: str, content: str):
+        self._messages.append(self.check_message_format({"role": role, "content": content}))
+
     def clear(self):
         self._messages.clear()
 
+    @property
+    def messages(self):
+        return list(self._messages)
+
+    @messages.setter
+    def messages(self, messages):
+        self._messages = [self.check_message_format(m) for m in messages]
+
     def __iter__(self):
         return iter(self._messages)
 
     def __len__(self):
         return len(self._messages)
 
     def __repr__(self):
-        repr = "\n".join([str(m) for m in self._messages])
-        repr = "\n" + re.sub(r"^", " " * 4, repr, 0, re.M) + "\n" if len(self._messages) > 0 else ""
+        max_length = f"max_length: {self.max_length}"
+        if len(self._messages) == 0:
+            repr = max_length
+        else:
+            repr = "\n".join([str(m) for m in self._messages]) + f"\n{max_length}"
+            repr = f"\n{re.sub(r'^', ' ' * 4, repr, 0, re.M)}\n"
         return f"{self.__class__.__name__}([{repr}])"
 
 
 class LM(ABC):
     @abstractmethod
     def complete(self, prompt: str, **kwargs) -> ClientResponse:
         pass
 
 
 class BaseClient(LM, ABC):
     base_url: str = "none"
     api_env_name: str = "none"
+    api_header_format: str = "none"
 
     #  If the backoff_factor is 0.1, then sleep() will sleep for [0.0s, 0.2s, 0.4s, …] between retries.
     RETRY_BACKOFF_FACTOR: float = 0.1
     RETRY_STATUS_CODES: List[int] = [429, 500, 502, 503, 504]
 
     def __init__(self, api_key: Optional[str] = None, max_retries: int = 5):
         self.max_retries = max_retries
         self.__api_key = api_key or os.environ.get(self.api_env_name)
         if self.__api_key is None:
             raise ValueError("You must provide an API key or set api_env_name to initialize an LM Client.")
         if self.base_url == "none":
-            raise ValueError("All Client subclasses must define a base URL attribute.")
+            raise ValueError("Client subclasses must define a base URL attribute.")
+        if self.api_header_format not in API_HEADER_FORMAT_DICT:
+            raise ValueError(f"Client subclasses must have api_header_format in {list(API_HEADER_FORMAT_DICT.keys())}")
+        self._api_header = API_HEADER_FORMAT_DICT[self.api_header_format]
 
-    def _post_request(self, api_path: str, request: dict, **extra_header_kwargs) -> Tuple[int, dict]:
+    def _post_request(self, api_path: str, request: dict, extra_headers: Optional[dict] = None) -> Tuple[int, dict]:
         with requests.Session() as session:
             retries = Retry(
                 total=self.max_retries,
                 backoff_factor=self.RETRY_BACKOFF_FACTOR,
                 status_forcelist=self.RETRY_STATUS_CODES,
             )
             session.mount("https://", HTTPAdapter(max_retries=retries))
             session.mount("http://", HTTPAdapter(max_retries=retries))
             headers = {
                 "accept": "application/json",
                 "content-type": "application/json",
-                "Authorization": f"Bearer {self.__api_key}",
+                self._api_header.key: self._api_header.value(self.__api_key),
             }
-            headers.update(extra_header_kwargs)
+            headers.update(extra_headers or {})
+            if self.__api_key not in headers.values():
+                headers["Authorization"] = f"Bearer {self.__api_key}"
+
         response = requests.post(url=f"{self.base_url}/{api_path}", json=request, headers=headers)
         status_code = response.status_code
         try:
             response_dict = response.json()
         except requests.exceptions.JSONDecodeError:
             response_dict = {}
             status_code = 500 if status_code != SUCCESS_STATUS_CODE else status_code
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao/lm/prompts/base.py` & `lmao-nlp-0.0.1b5/src/lmao/lm/prompts/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import ABC, abstractmethod
 from typing import Optional
 
 __all__ = ["default_templates", "Prompter"]
 
 default_templates = {
     "classification": (
-        "Classify the following input text into one of the following {num_categories} categories: [{categories}]. "
+        "Classify the input text into one of the following {num_categories} categories: [{categories}]. "
         "Respond with the answer only, without punctuation.\n\n"
         "{examples}"
         "Input: {input_text}\nCategory:"
     ),
     "sentiment_analysis": (
-        "Classify the sentiment of the following input one of the following "
+        "Classify the sentiment of the input text into one of the following "
         "{num_categories} categories: [{categories}]. Respond with the answer only, without punctuation.\n\n"
         "{examples}"
         "Input: {input_text}\nSentiment:"
     ),
 }
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao/lm/prompts/classification.py` & `lmao-nlp-0.0.1b5/src/lmao/lm/prompts/classification.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b4/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b5/src/lmao/lm/schemas/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import Dict, List, Optional, Union
 
 from pydantic import Extra, Field, validator
 
 from lmao.lm.schemas.base import API_DEFAULTS, BaseSchema
 
-__all__ = ["OpenAIChatSchema", "OpenAIGenerateSchema", "openai_model_regex"]
+__all__ = ["OpenAIChatSchema", "OpenAICompleteSchema", "openai_model_regex"]
 
 
 model_versions = r"(?:3\.5-turbo|4)"
 date_label_pattern = r"(?:0[1-9]|1[012])(?:0[1-9]|[12][0-9]|3[01])$"
 openai_model_regex = dict(
     chat=re.compile(rf"gpt-(?:{model_versions}(?:(?!-)\b|-{date_label_pattern}))"),
     complete=re.compile(r"text-davinci-\d\d\d"),
@@ -35,15 +35,15 @@
     @validator("model", pre=True, always=True)
     def validate_model(cls, v):
         if not openai_model_regex["chat"].search(v):
             raise ValueError(f"{v} is an invalid model format.")
         return v
 
 
-class OpenAIGenerateSchema(BaseSchema):
+class OpenAICompleteSchema(BaseSchema):
     """API Reference: https://platform.openai.com/docs/api-reference/completions/create"""
 
     class Config:
         extra = Extra.forbid
 
     model: str = Field(default="text-davinci-003", description="Must be of the form `text-davinci-[model_version]`.")
     prompt: Optional[str] = Field(default=None)
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b5/src/lmao/lm/utils.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b4/src/lmao/orchestrators/classification.py` & `lmao-nlp-0.0.1b5/src/lmao/orchestrators/classification.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from lmao.lm.clients.base import BaseClient
 from lmao.orchestrators.base import BaseOrchestrator
 
 __all__ = ["SentimentAnalysisOrchestrator"]
 
 
 class SentimentAnalysisOrchestrator(BaseOrchestrator):
-    def __init__(self, lm: BaseClient, lm_method_name: str, include_neutral: bool = True):
-        self.lm_method_name = lm_method_name
-        self.adapter = SentimentAnalysisAdapter(lm, lm_method_name, include_neutral=include_neutral)
+    def __init__(self, lm_client: BaseClient, client_method_name: str, include_neutral: bool = True):
+        self.client_method_name = client_method_name
+        self.adapter = SentimentAnalysisAdapter(lm_client, client_method_name, include_neutral=include_neutral)
         self.categories = ["positive", "negative"] + (["neutral"] if include_neutral else [])
         super().__init__()
 
     def run_pipeline(self, data: Union[Iterable, str], **kwargs) -> List[str]:
         temperature = kwargs.pop("temperature", 0)
         data = [data] if isinstance(data, str) else data
         predictions = []
         for text in data:
             predictions.append(self.adapter.predict(text, temperature=temperature, **kwargs).prediction)
-            if hasattr(self.adapter.lm, "chat_history"):
-                self.adapter.lm.chat_history.clear()
+            if hasattr(self.adapter.lm_client, "chat_history"):
+                self.adapter.lm_client.chat_history.clear()
         return predictions
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b4/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/lmao/__init__.py
 src/lmao/loader.py
 src/lmao/adapters/__init__.py
-src/lmao/adapters/base.py
-src/lmao/adapters/classification.py
+src/lmao/adapters/chatbot.py
+src/lmao/adapters/tasks/__init__.py
+src/lmao/adapters/tasks/base.py
+src/lmao/adapters/tasks/classification.py
 src/lmao/lm/__init__.py
 src/lmao/lm/utils.py
 src/lmao/lm/clients/__init__.py
+src/lmao/lm/clients/anthropic.py
 src/lmao/lm/clients/base.py
 src/lmao/lm/clients/openai.py
 src/lmao/lm/prompts/__init__.py
 src/lmao/lm/prompts/base.py
 src/lmao/lm/prompts/classification.py
 src/lmao/lm/schemas/__init__.py
+src/lmao/lm/schemas/anthropic.py
 src/lmao/lm/schemas/base.py
 src/lmao/lm/schemas/openai.py
 src/lmao/orchestrators/__init__.py
 src/lmao/orchestrators/base.py
 src/lmao/orchestrators/classification.py
 src/lmao_nlp.egg-info/PKG-INFO
 src/lmao_nlp.egg-info/SOURCES.txt
```

