# Comparing `tmp/knowledge_mapper-0.0.8.tar.gz` & `tmp/knowledge_mapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge_mapper-0.0.8.tar", last modified: Thu Feb 10 15:43:47 2022, max compression
+gzip compressed data, was "knowledge_mapper-0.0.9.tar", last modified: Tue Mar  1 15:24:32 2022, max compression
```

## Comparing `knowledge_mapper-0.0.8.tar` & `knowledge_mapper-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-02-10 15:43:47.210612 knowledge_mapper-0.0.8/
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-01-06 16:16:06.000000 knowledge_mapper-0.0.8/MANIFEST.in
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      141 2022-02-10 15:43:47.210612 knowledge_mapper-0.0.8/PKG-INFO
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     7356 2022-02-10 14:32:43.000000 knowledge_mapper-0.0.8/README.md
-drwxrwxr-x   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-02-10 15:43:47.206612 knowledge_mapper-0.0.8/knowledge_mapper/
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       22 2022-02-10 15:30:30.000000 knowledge_mapper-0.0.8/knowledge_mapper/__init__.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     3335 2022-01-31 14:57:14.000000 knowledge_mapper-0.0.8/knowledge_mapper/__main__.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      367 2022-01-17 10:50:24.000000 knowledge_mapper-0.0.8/knowledge_mapper/data_source.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     5880 2022-02-10 15:29:33.000000 knowledge_mapper-0.0.8/knowledge_mapper/knowledge_base.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     4549 2022-01-17 10:50:24.000000 knowledge_mapper-0.0.8/knowledge_mapper/knowledge_interaction.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     3478 2022-01-17 16:31:07.000000 knowledge_mapper-0.0.8/knowledge_mapper/knowledge_mapper.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     5895 2022-01-06 16:19:13.000000 knowledge_mapper-0.0.8/knowledge_mapper/sparql_source.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     5157 2022-01-31 14:57:14.000000 knowledge_mapper-0.0.8/knowledge_mapper/sql_source.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     2812 2022-01-24 15:38:58.000000 knowledge_mapper-0.0.8/knowledge_mapper/tke_client.py
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      260 2022-01-17 10:50:24.000000 knowledge_mapper-0.0.8/knowledge_mapper/tke_exceptions.py
-drwxrwxr-x   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-02-10 15:43:47.210612 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      141 2022-02-10 15:43:47.000000 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      607 2022-02-10 15:43:47.000000 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)        1 2022-02-10 15:43:47.000000 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       69 2022-02-10 15:43:47.000000 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/entry_points.txt
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       40 2022-02-10 15:43:47.000000 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/requires.txt
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       17 2022-02-10 15:43:47.000000 knowledge_mapper-0.0.8/knowledge_mapper.egg-info/top_level.txt
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       38 2022-02-10 15:43:47.210612 knowledge_mapper-0.0.8/setup.cfg
--rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      323 2022-02-10 15:30:35.000000 knowledge_mapper-0.0.8/setup.py
+drwxrwxr-x   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-03-01 15:24:32.385242 knowledge_mapper-0.0.9/
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-01-06 16:16:06.000000 knowledge_mapper-0.0.9/MANIFEST.in
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      141 2022-03-01 15:24:32.385242 knowledge_mapper-0.0.9/PKG-INFO
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     7356 2022-02-10 14:32:43.000000 knowledge_mapper-0.0.9/README.md
+drwxrwxr-x   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-03-01 15:24:32.381242 knowledge_mapper-0.0.9/knowledge_mapper/
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       22 2022-03-01 15:24:23.000000 knowledge_mapper-0.0.9/knowledge_mapper/__init__.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     3595 2022-03-01 15:23:03.000000 knowledge_mapper-0.0.9/knowledge_mapper/__main__.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      367 2022-01-17 10:50:24.000000 knowledge_mapper-0.0.9/knowledge_mapper/data_source.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     6039 2022-03-01 15:23:03.000000 knowledge_mapper-0.0.9/knowledge_mapper/knowledge_base.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     4549 2022-01-17 10:50:24.000000 knowledge_mapper-0.0.9/knowledge_mapper/knowledge_interaction.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     3478 2022-03-01 12:50:41.000000 knowledge_mapper-0.0.9/knowledge_mapper/knowledge_mapper.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     5895 2022-01-06 16:19:13.000000 knowledge_mapper-0.0.9/knowledge_mapper/sparql_source.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     5157 2022-01-31 14:57:14.000000 knowledge_mapper-0.0.9/knowledge_mapper/sql_source.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)     2812 2022-01-24 15:38:58.000000 knowledge_mapper-0.0.9/knowledge_mapper/tke_client.py
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      260 2022-01-17 10:50:24.000000 knowledge_mapper-0.0.9/knowledge_mapper/tke_exceptions.py
+drwxrwxr-x   0 kruigerjf  (1000) kruigerjf  (1000)        0 2022-03-01 15:24:32.385242 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      141 2022-03-01 15:24:32.000000 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      607 2022-03-01 15:24:32.000000 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)        1 2022-03-01 15:24:32.000000 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       69 2022-03-01 15:24:32.000000 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/entry_points.txt
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       40 2022-03-01 15:24:32.000000 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/requires.txt
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       17 2022-03-01 15:24:32.000000 knowledge_mapper-0.0.9/knowledge_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)       38 2022-03-01 15:24:32.385242 knowledge_mapper-0.0.9/setup.cfg
+-rw-rw-r--   0 kruigerjf  (1000) kruigerjf  (1000)      323 2022-03-01 15:24:12.000000 knowledge_mapper-0.0.9/setup.py
```

### Comparing `knowledge_mapper-0.0.8/README.md` & `knowledge_mapper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/__main__.py` & `knowledge_mapper-0.0.9/knowledge_mapper/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import argparse
 import logging as log
 import pyjson5
 import sys
 import importlib
 import time
+import signal
 
 from knowledge_mapper.knowledge_mapper import KnowledgeMapper
 
 from knowledge_mapper.data_source import DataSource
 from knowledge_mapper.sparql_source import SparqlSource
 from knowledge_mapper.sql_source import SqlSource
 
 log.basicConfig(level=log.INFO)
 
+# This function is called when a SIGTERM signal is received. This makes it so
+# that the knowledge mapper can be gracefully killed by Docker.
+def handle_sigterm(*args):
+    raise KeyboardInterrupt()
+
+signal.signal(signal.SIGTERM, handle_sigterm)
 
 DATA_SOURCE_MAX_CONNECTION_ATTEMPTS = 5
 DATA_SOURCE_WAIT_BEFORE_RETRY = 2
 
 def test_data_source(data_source: DataSource):
     success = False
     attempts = 0
```

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/knowledge_base.py` & `knowledge_mapper-0.0.9/knowledge_mapper/knowledge_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
     def register_knowledge_interaction(self, ki: knowledge_interaction.KnowledgeInteractionRegistrationRequest, name=None) -> knowledge_interaction.KnowledgeInteraction:
         body = {
             'knowledgeInteractionType': ki.type,
             'prefixes': ki.prefixes
         }
 
+        if name is not None:
+            body['knowledgeInteractionName'] = name
+
         if isinstance(ki, knowledge_interaction.AskKnowledgeInteractionRegistrationRequest | knowledge_interaction.AnswerKnowledgeInteractionRegistrationRequest):
             body['graphPattern'] = ki.pattern
         elif isinstance(ki, knowledge_interaction.PostKnowledgeInteractionRegistrationRequest | knowledge_interaction.ReactKnowledgeInteractionRegistrationRequest):
             body['argumentGraphPattern'] = ki.argument_pattern
             body['resultGraphPattern'] = ki.result_pattern
         else:
             raise Exception('`ki` must be a concrete knowledge interaction object')
@@ -69,14 +72,16 @@
         )
 
         if not response.ok:
             raise UnexpectedHttpResponseError(response)
         
         ki_id = response.json()['knowledgeInteractionId']
 
+        log.info(f'Successfully registered knowledge interaction {ki_id}.')
+
         registered_ki = knowledge_interaction.KnowledgeInteraction.from_req(ki, ki_id, self)
         self.kis[ki_id] = registered_ki
 
         if name is not None:
             self.kis_by_name[name] = registered_ki
 
         return registered_ki
```

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/knowledge_interaction.py` & `knowledge_mapper-0.0.9/knowledge_mapper/knowledge_interaction.py`

 * *Files identical despite different names*

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/knowledge_mapper.py` & `knowledge_mapper-0.0.9/knowledge_mapper/knowledge_mapper.py`

 * *Files identical despite different names*

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/sparql_source.py` & `knowledge_mapper-0.0.9/knowledge_mapper/sparql_source.py`

 * *Files identical despite different names*

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/sql_source.py` & `knowledge_mapper-0.0.9/knowledge_mapper/sql_source.py`

 * *Files identical despite different names*

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper/tke_client.py` & `knowledge_mapper-0.0.9/knowledge_mapper/tke_client.py`

 * *Files identical despite different names*

### Comparing `knowledge_mapper-0.0.8/knowledge_mapper.egg-info/SOURCES.txt` & `knowledge_mapper-0.0.9/knowledge_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

