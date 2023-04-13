# Comparing `tmp/fling_cli-0.1.1.tar.gz` & `tmp/fling_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_cli-0.1.1.tar", max compression
+gzip compressed data, was "fling_cli-0.1.2.tar", max compression
```

## Comparing `fling_cli-0.1.1.tar` & `fling_cli-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-04-07 22:10:44.399732 fling_cli-0.1.1/fling_cli/__init__.py
--rw-r--r--   0        0        0     2038 2023-04-12 19:54:28.740946 fling_cli-0.1.1/fling_cli/auth.py
--rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.1/fling_cli/bin/__init__.py
--rw-r--r--   0        0        0     6870 2023-04-12 19:37:24.854872 fling_cli-0.1.1/fling_cli/bin/fling.py
--rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.1/fling_cli/logo-hc.txt
--rw-r--r--   0        0        0      861 2023-04-12 23:36:41.323143 fling_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 fling_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2163 2023-04-05 23:25:42.977524 fling_cli-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-13 01:17:37.262832 fling_cli-0.1.2/fling_cli/__init__.py
+-rw-r--r--   0        0        0     2040 2023-04-13 01:15:50.829929 fling_cli-0.1.2/fling_cli/auth.py
+-rw-r--r--   0        0        0        0 2023-04-04 19:06:55.600802 fling_cli-0.1.2/fling_cli/bin/__init__.py
+-rw-r--r--   0        0        0     6870 2023-04-12 19:37:24.854872 fling_cli-0.1.2/fling_cli/bin/fling.py
+-rw-r--r--   0        0        0     3834 2023-04-08 02:13:26.640377 fling_cli-0.1.2/fling_cli/logo-hc.txt
+-rw-r--r--   0        0        0      861 2023-04-13 01:17:37.257680 fling_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 fling_cli-0.1.2/PKG-INFO
```

### Comparing `fling_cli-0.1.1/README.md` & `fling_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.1/fling_cli/auth.py` & `fling_cli-0.1.2/fling_cli/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     async def callback(state: str, token: str, username: str):
         # Die after this request finishes, no matter what
 
         if state != stored_state:
             raise Exception("State doesn't match, bad!")
         print(f"Saving token for `{username}` to keyring.")
         keyring.set_password("fling-github-token", username, token)
-        default_password = keyring.get_password("fling-github-token", "system-default")
-        if not default_password:
-            print(f"No default account, Saving token for `{username}` as default.")
-            keyring.set_password("fling-github-token", "system-default", token)
+        # default_password = keyring.get_password("fling-github-token", "system-default")
+        # if not default_password:
+        #     print(f"No default account, Saving token for `{username}` as default.")
+        keyring.set_password("fling-github-token", "system-default", token)
         return RedirectResponse('http://localhost:5817', status_code=302)
 
     @app.get("/")
     def app_index(background_tasks: BackgroundTasks):
         background_tasks.add_task(signal.raise_signal, signal.SIGINT)
         return HTMLResponse(
             "<html><h1>GitHub login succeeded. You may close this window.</h1></html>"
```

### Comparing `fling_cli-0.1.1/fling_cli/bin/fling.py` & `fling_cli-0.1.2/fling_cli/bin/fling.py`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.1/fling_cli/logo-hc.txt` & `fling_cli-0.1.2/fling_cli/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_cli-0.1.1/pyproject.toml` & `fling_cli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fling-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "Side Project Management from the command line"
 authors = ["Joshua McKenty <jmckenty@gmail.com>", "Anouk Ruhaak <anoukruhaak@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fling_cli"}]
 
 [tool.poetry.dependencies]
 click = "*"
```

### Comparing `fling_cli-0.1.1/PKG-INFO` & `fling_cli-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

