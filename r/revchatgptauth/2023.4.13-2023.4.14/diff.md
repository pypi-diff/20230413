# Comparing `tmp/revchatgptauth-2023.4.13.tar.gz` & `tmp/revchatgptauth-2023.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revchatgptauth-2023.4.13.tar", max compression
+gzip compressed data, was "revchatgptauth-2023.4.14.tar", max compression
```

## Comparing `revchatgptauth-2023.4.13.tar` & `revchatgptauth-2023.4.14.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1208 2023-04-12 06:37:29.470110 revchatgptauth-2023.4.13/README.md
--rw-r--r--   0        0        0     1250 2023-04-12 06:37:52.942179 revchatgptauth-2023.4.13/pyproject.toml
--rw-r--r--   0        0        0      247 2023-04-12 06:37:29.474110 revchatgptauth-2023.4.13/revchatgptauth/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-12 06:37:29.474110 revchatgptauth-2023.4.13/revchatgptauth/chatgpt_access_token_parser.py
--rw-r--r--   0        0        0     1561 2023-04-12 06:37:29.474110 revchatgptauth-2023.4.13/revchatgptauth/openai_cookie_parser.py
--rw-r--r--   0        0        0        0 2023-04-12 06:37:29.474110 revchatgptauth-2023.4.13/revchatgptauth/py.typed
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 revchatgptauth-2023.4.13/PKG-INFO
+-rw-r--r--   0        0        0     1208 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/README.md
+-rw-r--r--   0        0        0     1326 2023-04-13 06:25:54.753340 revchatgptauth-2023.4.14/pyproject.toml
+-rw-r--r--   0        0        0      247 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/__init__.py
+-rw-r--r--   0        0        0     1056 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/chatgpt_access_token_parser.py
+-rw-r--r--   0        0        0     1561 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/openai_cookie_parser.py
+-rw-r--r--   0        0        0        0 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/test/__init__.py
+-rw-r--r--   0        0        0     1989 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/test/test_chatgpt_access_token_parser.py
+-rw-r--r--   0        0        0     3124 2023-04-13 06:25:32.560910 revchatgptauth-2023.4.14/revChatGPTAuth/test/test_openai_cookie_parser.py
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 revchatgptauth-2023.4.14/PKG-INFO
```

### Comparing `revchatgptauth-2023.4.13/README.md` & `revchatgptauth-2023.4.14/README.md`

 * *Files identical despite different names*

### Comparing `revchatgptauth-2023.4.13/pyproject.toml` & `revchatgptauth-2023.4.14/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-name = "revchatgptauth"
-version = "2023.04.13"
+name = "revChatGPTAuth"
+version = "2023.04.14"
 description = ""
 authors = []
 readme = "README.md"
+[[tool.poetry.packages]]
+include = "revChatGPTAuth"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonPlatform = "All"
 venvPath = "./.venv"
 stubPath = "./.type_stubs"
 include = [ "./*",]
@@ -53,7 +55,8 @@
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 invoke = "^2.0.0"
 ruff = "^0.0.261"
 types-invoke = "^2.0.0.6"
 types-toml = "^0.10.8.6"
 pyright = "^1.1.302"
+pytest-sugar = "^0.9.7"
```

### Comparing `revchatgptauth-2023.4.13/revchatgptauth/chatgpt_access_token_parser.py` & `revchatgptauth-2023.4.14/revChatGPTAuth/chatgpt_access_token_parser.py`

 * *Files identical despite different names*

### Comparing `revchatgptauth-2023.4.13/revchatgptauth/openai_cookie_parser.py` & `revchatgptauth-2023.4.14/revChatGPTAuth/openai_cookie_parser.py`

 * *Files identical despite different names*

### Comparing `revchatgptauth-2023.4.13/PKG-INFO` & `revchatgptauth-2023.4.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revchatgptauth
-Version: 2023.4.13
+Version: 2023.4.14
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
```

