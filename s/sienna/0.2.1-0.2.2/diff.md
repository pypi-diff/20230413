# Comparing `tmp/sienna-0.2.1.tar.gz` & `tmp/sienna-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sienna-0.2.1.tar", max compression
+gzip compressed data, was "sienna-0.2.2.tar", max compression
```

## Comparing `sienna-0.2.1.tar` & `sienna-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      380 2023-04-13 10:50:11.093087 sienna-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1378 2023-04-13 10:49:17.864625 sienna-0.2.1/sienna/.null-ls_875572_core.py
--rw-r--r--   0        0        0       62 2023-04-13 10:11:35.652403 sienna-0.2.1/sienna/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-13 10:50:11.093305 sienna-0.2.1/sienna/core.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 sienna-0.2.1/setup.py
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 sienna-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      380 2023-04-13 11:00:01.889446 sienna-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-04-13 10:11:35.652403 sienna-0.2.2/sienna/__init__.py
+-rw-r--r--   0        0        0     1521 2023-04-13 11:00:01.889623 sienna-0.2.2/sienna/core.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 sienna-0.2.2/setup.py
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 sienna-0.2.2/PKG-INFO
```

### Comparing `sienna-0.2.1/sienna/.null-ls_875572_core.py` & `sienna-0.2.2/sienna/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import os
 from typing import Dict, List, Union
 
 
 def __get_file_type(fpath: str) -> str:
     if fpath.endswith(".jsonl"):
         return "jsonl"
     elif fpath.endswith(".json"):
@@ -35,14 +36,24 @@
             json.dump(data, f)
     else:
         with open(fpath, "w") as f:
             f.write("\n".join(data))
 
 
 def add(data: Dict, fpath: str):
-    assert isinstance(data, dict), "Currently, only adding dict data to jsonl file is supported."
-    assert fpath.endswith(".jsonl"), "Currently, only adding dict data to jsonl file is supported."
+    assert isinstance(
+        data, dict
+    ), "Currently, only adding dict data to jsonl file is supported."
+    assert fpath.endswith(
+        ".jsonl"
+    ), "Currently, only adding dict data to jsonl file is supported."
+
+    exists = os.path.exists(fpath)
 
     with open(fpath, "a") as f:
-        f.write("\n")
+
+        if exists:
+            f.write("\n")
+        else:
+            print(f"Creating {fpath}")
+
         f.write(json.dumps(data))
-    pass
```

