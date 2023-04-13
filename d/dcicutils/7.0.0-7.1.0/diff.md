# Comparing `tmp/dcicutils-7.0.0.tar.gz` & `tmp/dcicutils-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.0.0.tar", max compression
+gzip compressed data, was "dcicutils-7.1.0.tar", max compression
```

## Comparing `dcicutils-7.0.0.tar` & `dcicutils-7.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1166 2020-06-26 13:31:34.710949 dcicutils-7.0.0/README.rst
--rw-r--r--   0        0        0        0 2023-04-07 15:32:44.264637 dcicutils-7.0.0/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-07 15:32:44.269515 dcicutils-7.0.0/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2022-09-12 17:47:33.199849 dcicutils-7.0.0/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-02-03 18:43:26.004805 dcicutils-7.0.0/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2022-12-05 18:22:34.726889 dcicutils-7.0.0/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-07 15:32:44.270216 dcicutils-7.0.0/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-07 15:32:44.275435 dcicutils-7.0.0/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2022-09-12 17:47:33.201910 dcicutils-7.0.0/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2021-09-01 19:18:33.261747 dcicutils-7.0.0/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-07 15:32:44.281332 dcicutils-7.0.0/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2022-07-14 16:55:23.169003 dcicutils-7.0.0/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2022-07-14 16:55:23.169517 dcicutils-7.0.0/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2022-09-12 17:47:33.203186 dcicutils-7.0.0/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2022-09-12 17:47:33.203764 dcicutils-7.0.0/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2022-09-12 17:47:33.204441 dcicutils-7.0.0/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-07 15:32:44.281748 dcicutils-7.0.0/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2022-09-12 17:47:33.205392 dcicutils-7.0.0/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2022-09-12 17:47:33.205684 dcicutils-7.0.0/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46318 2023-04-07 15:32:44.287107 dcicutils-7.0.0/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2022-09-12 17:47:33.207369 dcicutils-7.0.0/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2022-12-05 18:22:34.728275 dcicutils-7.0.0/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9257 2022-09-12 17:47:33.208328 dcicutils-7.0.0/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-07 15:28:37.360372 dcicutils-7.0.0/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-07 15:32:44.287768 dcicutils-7.0.0/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2021-05-06 19:01:44.700749 dcicutils-7.0.0/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2020-05-15 15:45:42.789486 dcicutils-7.0.0/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2020-05-15 15:45:42.789652 dcicutils-7.0.0/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2022-11-30 15:39:36.604614 dcicutils-7.0.0/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2020-05-15 15:45:42.790150 dcicutils-7.0.0/dcicutils/log_utils.py
--rw-r--r--   0        0        0    86616 2023-04-07 15:32:44.288510 dcicutils-7.0.0/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5510 2023-01-20 17:23:34.654143 dcicutils-7.0.0/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2022-12-05 18:22:34.729161 dcicutils-7.0.0/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2022-10-06 15:32:13.272174 dcicutils-7.0.0/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   120626 2023-04-07 15:32:44.289245 dcicutils-7.0.0/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-07 15:32:44.294803 dcicutils-7.0.0/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-07 15:32:44.300746 dcicutils-7.0.0/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-07 15:32:44.306949 dcicutils-7.0.0/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    19745 2023-04-07 15:32:44.312682 dcicutils-7.0.0/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2022-09-12 17:47:33.217026 dcicutils-7.0.0/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     3654 2023-04-07 15:32:44.329792 dcicutils-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     2423 2023-04-07 15:33:00.136284 dcicutils-7.0.0/setup.py
--rw-r--r--   0        0        0     2718 2023-04-07 15:33:00.136571 dcicutils-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-13 15:16:36.923706 dcicutils-7.1.0/README.rst
+-rw-r--r--   0        0        0        0 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46318 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-13 15:16:36.923706 dcicutils-7.1.0/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9257 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87196 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   120743 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    19745 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-13 15:16:36.927705 dcicutils-7.1.0/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3654 2023-04-13 15:16:36.927705 dcicutils-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 dcicutils-7.1.0/PKG-INFO
```

### Comparing `dcicutils-7.0.0/README.rst` & `dcicutils-7.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/base.py` & `dcicutils-7.1.0/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/beanstalk_utils.py` & `dcicutils-7.1.0/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/cloudformation_utils.py` & `dcicutils-7.1.0/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/codebuild_utils.py` & `dcicutils-7.1.0/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/command_utils.py` & `dcicutils-7.1.0/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/common.py` & `dcicutils-7.1.0/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/creds_utils.py` & `dcicutils-7.1.0/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/data_utils.py` & `dcicutils-7.1.0/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/deployment_utils.py` & `dcicutils-7.1.0/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/diff_utils.py` & `dcicutils-7.1.0/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/docker_utils.py` & `dcicutils-7.1.0/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/ecr_scripts.py` & `dcicutils-7.1.0/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/ecr_utils.py` & `dcicutils-7.1.0/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/ecs_utils.py` & `dcicutils-7.1.0/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/env_base.py` & `dcicutils-7.1.0/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/env_manager.py` & `dcicutils-7.1.0/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/env_scripts.py` & `dcicutils-7.1.0/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/env_utils.py` & `dcicutils-7.1.0/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/env_utils_legacy.py` & `dcicutils-7.1.0/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/es_utils.py` & `dcicutils-7.1.0/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/exceptions.py` & `dcicutils-7.1.0/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/ff_mocks.py` & `dcicutils-7.1.0/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/ff_utils.py` & `dcicutils-7.1.0/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/jh_utils.py` & `dcicutils-7.1.0/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/kibana/dashboards.json` & `dcicutils-7.1.0/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/kibana/readme.md` & `dcicutils-7.1.0/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/lang_utils.py` & `dcicutils-7.1.0/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/log_utils.py` & `dcicutils-7.1.0/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/misc_utils.py` & `dcicutils-7.1.0/dcicutils/misc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1383,24 +1383,30 @@
         return str(self)
 
     def __str__(self):
         updater_name = self._update_function.__name__
         return f"CachedField(name={self.name!r},update_function={updater_name},timeout={self.timeout!r})"
 
 
+class StorageCell:
+
+    def __init__(self, initial_value=None):
+        self.value = initial_value
+
+
 def make_counter(start=0, step=1):
     """
     Creates a counter that generates values counting from a given start (default 0) by a given step (default 1).
     """
-    storage = [start]
+    storage = StorageCell(start)
 
     def counter():
-        value = storage[0]
-        storage[0] += step
-        return value
+        old_value = storage.value
+        storage.value += step
+        return old_value
 
     return counter
 
 
 def copy_json(obj):
     """ This function is taken and renamed from ENCODE's snovault quick_deepcopy
 
@@ -2159,7 +2165,19 @@
         cycle is detected, :exc:`CycleError` will be raised.
         """
         self.prepare()
         while self.is_active():
             node_group = self.get_ready()
             yield from node_group
             self.done(*node_group)
+
+
+def deduplicate_list(lst):
+    """ De-duplicates the given list by converting it to a set then back to a list.
+    NOTES:
+    * The list must contain 'hashable' type elements that can be used in sets.
+    * The result list might not be ordered the same as the input list.
+    * This will also take tuples as input, though the result will be a list.
+    :param lst: list to de-duplicate
+    :return: de-duplicated list
+    """
+    return list(set(lst))
```

### Comparing `dcicutils-7.0.0/dcicutils/obfuscation_utils.py` & `dcicutils-7.1.0/dcicutils/obfuscation_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Some utilities related to obfuscating sensitive data (dmichaels/2022-07-20).
 
 import copy
 import re
 
-from dcicutils.misc_utils import check_true
-from typing import Optional
+from .common import AnyJsonData
+from .misc_utils import check_true, StorageCell
+from typing import Optional, Any, Union
 
 
 # The _SENSITIVE_KEY_NAMES_REGEX regex defines key names representing sensitive values, case-insensitive.
 # Note the below 'crypt(?!_key_id$)' regex matches any thing with 'crypt' except for 'crypt_key_id'.
 _SENSITIVE_KEY_NAMES_REGEX = re.compile(
     r"""
     .*(
@@ -20,27 +21,28 @@
         session.*token |
         session.*id    |
         crypt(?!_key_id$)
     ).*
     """, re.VERBOSE | re.IGNORECASE)
 
 
-def should_obfuscate(key: str) -> bool:
+def should_obfuscate(key: str, value: Any = None) -> bool:
     """
     Returns True if the given key looks as if it represents a sensitive value.
     Just sees if it contains "secret" or "password" or "crypt" some obvious variants,
     case-insensitive; i.e. whatever is in the _SENSITIVE_KEY_NAMES_REGEX list
     containing regular expressions; add more to if/when needed.
 
     :param key: Key name of some property which may or may not need to be obfuscated.
+    :param value: (optional) value of item to be obfuscated, just in case it already is obfuscated
     :return: True if the given key name looks as if it represents a sensitive value.
     """
-    if not key or not isinstance(key, str):
-        return False
-    return _SENSITIVE_KEY_NAMES_REGEX.match(key) is not None
+    obfuscate_because_of_key = isinstance(key, str) and bool(_SENSITIVE_KEY_NAMES_REGEX.match(key))
+    not_obfuscated_already = not isinstance(value, str) or not is_obfuscated(value)
+    return obfuscate_because_of_key and not_obfuscated_already
 
 
 def obfuscate(value: str, show: bool = False, obfuscated: Optional[str] = None) -> str:
     """
     Obfuscates and returns the given string value.
     If the given value is not a string, is None, or is empty then just returns the given value.
     If the show argument is True then does not actually obfuscate and simply returns the given string.
@@ -71,50 +73,60 @@
 
     NOTE: This is heuristic. Your password MIGHT be *** or <my-password>, but we're hoping not.
     """
 
     return isinstance(value, str) and bool(OBFUSCATED_VALUE.match(value))
 
 
-def obfuscate_dict(dictionary: dict, inplace: bool = False, show: bool = False,
-                   obfuscated: Optional[str] = None) -> dict:
+def obfuscate_json(item: Union[AnyJsonData, tuple], inplace: bool = False, show: bool = False,
+                   obfuscated: Optional[str] = None) -> Union[AnyJsonData, tuple]:
     """
     Obfuscates all STRING values within the given dictionary, RECURSIVELY, for all key names which look
     as if they represent sensitive values (based on the should_obfuscate function). By default, if the
     inplace argument is False, a COPY of the dictionary is returned, but ONLY if it actually needs to
     be modified (i.e. has values to obfuscate, based on key name, and which are not already obfuscated);
     i.e. the given dictionary is NOT modified if there are no values to obfuscate or if such values are
     already abfuscated. If the inplace argument is True, then any changes (value obfuscations) are made to
     the given dictionary itself in place (NOT a copy). In either case the resultant dictionary is returned.
     If the show argument is True then does not actually obfuscate and simply returns the given dictionary.
 
-    :param dictionary: Given dictionary whose senstive values obfuscate.
+    :param item: Any JSON object that might be or contain a dictionary whose senstive values are to be obfuscated.
     :param inplace: If True obfuscate the given dictionary in place; else a COPY is returned, if modified.
     :param show: If True does not actually obfuscate and simply returns the given dictionary.
+    :param obfuscated: The obfuscation string to use if one is not to be generated dynamically.
     :return: Resultant dictionary.
     """
 
     check_true(not obfuscated or is_obfuscated(obfuscated),
                message=f"If obfuscated= is supplied, it must be {OBFUSCATED_VALUE_DESCRIPTION}.")
 
-    def has_values_to_obfuscate(dictionary: dict) -> bool:
-        for key, value in dictionary.items():
-            if isinstance(value, dict):
-                if has_values_to_obfuscate(value):
-                    return True
-            elif isinstance(value, str) and should_obfuscate(key) and not is_obfuscated(value):
-                return True
-        return False
-
-    if dictionary is None or not isinstance(dictionary, dict):
-        return {}
-    if isinstance(show, bool) and show:
-        return dictionary
-    if not isinstance(inplace, bool) or not inplace:
-        if has_values_to_obfuscate(dictionary):
-            dictionary = copy.deepcopy(dictionary)
-    for key, value in dictionary.items():
-        if isinstance(value, dict):
-            dictionary[key] = obfuscate_dict(value, show=False, inplace=False, obfuscated=obfuscated)
-        elif isinstance(value, str) and should_obfuscate(key) and not is_obfuscated(value):
-            dictionary[key] = obfuscate(value, show=False, obfuscated=obfuscated)
-    return dictionary
+    if show:
+        return item
+
+    orig_item = item
+
+    changed = StorageCell(False)
+
+    if not inplace:
+        item = copy.deepcopy(item)
+
+    def process_recursively(item: Union[AnyJsonData, tuple]):
+        # We only need to process non-atomic items recursively, since they are the only things
+        # that might conceivably be or contain a dictionary in need of obfuscation.
+        if isinstance(item, dict):
+            for key, value in item.items():
+                if should_obfuscate(key, value):
+                    changed.value = True
+                    item[key] = obfuscate(value, obfuscated=obfuscated)
+                else:
+                    process_recursively(value)
+        elif isinstance(item, list) or isinstance(item, tuple):
+            for element in item:
+                process_recursively(element)
+
+    process_recursively(item)
+
+    return item if changed.value else orig_item
+
+
+# The function obfuscate_dict is deprecated and will go away in a future major release.
+obfuscate_dict = obfuscate_json
```

### Comparing `dcicutils-7.0.0/dcicutils/opensearch_utils.py` & `dcicutils-7.1.0/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/qa_checkers.py` & `dcicutils-7.1.0/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/qa_utils.py` & `dcicutils-7.1.0/dcicutils/qa_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from unittest import mock
 from .env_utils import short_env_name
 from .exceptions import ExpectedErrorNotSeen, WrongErrorSeen, UnexpectedErrorAfterFix, WrongErrorSeenAfterFix
 from .lang_utils import there_are
 from .misc_utils import (
     PRINT, ignored, Retry, remove_prefix, REF_TZ,
     environ_bool, exported, override_environ, override_dict, local_attrs, full_class_name,
-    find_associations, get_error_message,
+    find_associations, get_error_message, remove_suffix,
 )
 from .qa_checkers import QA_EXCEPTION_PATTERN, find_uses, confirm_no_uses, VersionChecker, ChangeLogChecker
 
 
 # Using these names via qa_utils is deprecated. Their proper, supported home is now in qa_checkers.
 # Please rewrite imports to get them from qa_checkers, not qa_utils. -kmp 21-Sep-2022
 exported(QA_EXCEPTION_PATTERN, find_uses, confirm_no_uses, VersionChecker, ChangeLogChecker)
@@ -604,29 +604,31 @@
         For all cases, even stdout, .file_lines[fp] and .lines[fp] contain it.
         Notes:
             * If None is the fp value, sys.stdout is used instead. so that None and the current
               value of sys.stdout are synonyms.
             * This mock ignores 'end=' and will treat all calls to PRINT as if they were separate lines.
         """
         text = " ".join(map(str, args))
+        texts = remove_suffix('\n', text).split('\n')
+        last_text = texts[-1]
         print(text, **kwargs)  # noQA - This call to print is low-level implementation
         # This only captures non-file output output.
         file = kwargs.get('file')
         if file is None:
             file = sys.stdout
         if file is sys.stdout:
             # Easy access to stdout
-            self.lines.append(text)
-            self.last = text
+            self.lines.extend(texts)
+            self.last = last_text
             # Every output to stdout is implicitly like output to no file (None)
-            self.file_lines[None].append(text)
-            self.file_last[None] = text
+            self.file_lines[None].extend(texts)
+            self.file_last[None] = last_text
         # All accesses of any file/fp, including stdout, get associated with that destination
-        self.file_lines[file].append(text)
-        self.file_last[file] = text
+        self.file_lines[file].extend(texts)
+        self.file_last[file] = last_text
 
     def reset(self):
         self.lines = []
         self.last = None
         self.file_lines = self._file_lines_dict()
         self.file_last = self._file_last_dict()
```

### Comparing `dcicutils-7.0.0/dcicutils/redis_tools.py` & `dcicutils-7.1.0/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/redis_utils.py` & `dcicutils-7.1.0/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/s3_utils.py` & `dcicutils-7.1.0/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/secrets_utils.py` & `dcicutils-7.1.0/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/dcicutils/snapshot_utils.py` & `dcicutils-7.1.0/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.0.0/pyproject.toml` & `dcicutils-7.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.0.0"
+version = "7.1.0"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.0.0/PKG-INFO` & `dcicutils-7.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.0.0
+Version: 7.1.0
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: PyYAML (>=5.1,<5.5)
 Requires-Dist: aws-requests-auth (>=0.4.2,<1)
 Requires-Dist: boto3 (>=1.17.39,<2.0.0)
 Requires-Dist: botocore (>=1.20.39,<2.0.0)
 Requires-Dist: docker (>=4.4.4,<5.0.0)
```

