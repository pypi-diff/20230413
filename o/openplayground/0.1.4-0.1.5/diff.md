# Comparing `tmp/openplayground-0.1.4.tar.gz` & `tmp/openplayground-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplayground-0.1.4.tar", max compression
+gzip compressed data, was "openplayground-0.1.5.tar", max compression
```

## Comparing `openplayground-0.1.4.tar` & `openplayground-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,32 @@
--rw-r--r--   0        0        0     1074 2023-04-07 16:23:09.045621 openplayground-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     4527 2023-04-11 18:22:21.034872 openplayground-0.1.4/README.md
--rw-r--r--   0        0        0      948 2023-04-13 16:55:18.502927 openplayground-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 16:23:09.051828 openplayground-0.1.4/server/__init__.py
--rwxr-xr-x   0        0        0    15398 2023-04-13 16:52:49.106643 openplayground-0.1.4/server/app.py
--rw-r--r--   0        0        0        0 2023-04-07 16:23:09.052030 openplayground-0.1.4/server/lib/__init__.py
--rw-r--r--   0        0        0     4473 2023-04-07 16:23:09.052190 openplayground-0.1.4/server/lib/api/__init__.py
--rw-r--r--   0        0        0     4632 2023-04-13 16:52:49.107315 openplayground-0.1.4/server/lib/api/inference.py
--rw-r--r--   0        0        0     4538 2023-04-07 16:23:09.052376 openplayground-0.1.4/server/lib/api/provider.py
--rw-r--r--   0        0        0      273 2023-04-07 16:23:09.052444 openplayground-0.1.4/server/lib/api/response_utils.py
--rw-r--r--   0        0        0     5034 2023-04-07 16:23:09.052543 openplayground-0.1.4/server/lib/entities.py
--rw-r--r--   0        0        0     1636 2023-04-07 16:23:09.052628 openplayground-0.1.4/server/lib/event_emitter.py
--rw-r--r--   0        0        0    30494 2023-04-13 16:52:49.108251 openplayground-0.1.4/server/lib/inference/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:23:09.052945 openplayground-0.1.4/server/lib/inference/huggingface/__init__.py
--rw-r--r--   0        0        0     7943 2023-04-07 16:23:09.053086 openplayground-0.1.4/server/lib/inference/huggingface/generator.py
--rw-r--r--   0        0        0      363 2023-04-07 16:23:09.053160 openplayground-0.1.4/server/lib/inference/huggingface/helpers.py
--rwxr-xr-x   0        0        0     5505 2023-04-11 18:35:56.373509 openplayground-0.1.4/server/lib/inference/huggingface/hf.py
--rwxr-xr-x   0        0        0     6856 2023-04-11 19:08:01.155341 openplayground-0.1.4/server/lib/sse.py
--rw-r--r--   0        0        0     1864 2023-04-11 19:09:52.213288 openplayground-0.1.4/server/lib/sseserver.py
--rw-r--r--   0        0        0    10480 2023-04-07 16:23:09.053510 openplayground-0.1.4/server/lib/storage.py
--rw-r--r--   0        0        0    18738 2023-04-13 16:53:10.326323 openplayground-0.1.4/server/models.json
--rwxr-xr-x   0        0        0      284 2023-04-07 16:23:09.053689 openplayground-0.1.4/server/requirements.txt
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 openplayground-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-13 18:11:51.052289 openplayground-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0     4527 2023-04-13 18:11:51.052399 openplayground-0.1.5/README.md
+-rw-r--r--   0        0        0      977 2023-04-13 18:18:11.798285 openplayground-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 18:11:51.058972 openplayground-0.1.5/server/__init__.py
+-rwxr-xr-x   0        0        0    15398 2023-04-13 18:11:51.059172 openplayground-0.1.5/server/app.py
+-rw-r--r--   0        0        0        0 2023-04-13 18:11:51.059259 openplayground-0.1.5/server/lib/__init__.py
+-rw-r--r--   0        0        0     4473 2023-04-13 18:11:51.059428 openplayground-0.1.5/server/lib/api/__init__.py
+-rw-r--r--   0        0        0     4632 2023-04-13 18:11:51.059553 openplayground-0.1.5/server/lib/api/inference.py
+-rw-r--r--   0        0        0     4538 2023-04-13 18:11:51.059650 openplayground-0.1.5/server/lib/api/provider.py
+-rw-r--r--   0        0        0      273 2023-04-13 18:11:51.059723 openplayground-0.1.5/server/lib/api/response_utils.py
+-rw-r--r--   0        0        0     5034 2023-04-13 18:11:51.059822 openplayground-0.1.5/server/lib/entities.py
+-rw-r--r--   0        0        0     1636 2023-04-13 18:11:51.059907 openplayground-0.1.5/server/lib/event_emitter.py
+-rw-r--r--   0        0        0    30494 2023-04-13 18:11:51.060192 openplayground-0.1.5/server/lib/inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 18:11:51.060324 openplayground-0.1.5/server/lib/inference/huggingface/__init__.py
+-rw-r--r--   0        0        0     7943 2023-04-13 18:11:51.060493 openplayground-0.1.5/server/lib/inference/huggingface/generator.py
+-rw-r--r--   0        0        0      363 2023-04-13 18:11:51.060587 openplayground-0.1.5/server/lib/inference/huggingface/helpers.py
+-rwxr-xr-x   0        0        0     5505 2023-04-13 18:11:51.060701 openplayground-0.1.5/server/lib/inference/huggingface/hf.py
+-rwxr-xr-x   0        0        0     6856 2023-04-13 18:11:51.060831 openplayground-0.1.5/server/lib/sse.py
+-rw-r--r--   0        0        0     1864 2023-04-13 18:11:51.060925 openplayground-0.1.5/server/lib/sseserver.py
+-rw-r--r--   0        0        0    10480 2023-04-13 18:11:51.061069 openplayground-0.1.5/server/lib/storage.py
+-rw-r--r--   0        0        0    18738 2023-04-13 18:11:51.061203 openplayground-0.1.5/server/models.json
+-rwxr-xr-x   0        0        0      284 2023-04-13 18:11:51.061299 openplayground-0.1.5/server/requirements.txt
+-rw-r--r--   0        0        0   889501 2023-04-13 18:12:34.185806 openplayground-0.1.5/server/static/index.d826928d.js
+-rw-r--r--   0        0        0   226215 2023-04-13 18:12:35.279106 openplayground-0.1.5/server/static/index.d826928d.js.br
+-rw-r--r--   0        0        0   276090 2023-04-13 18:12:34.211010 openplayground-0.1.5/server/static/index.d826928d.js.gz
+-rw-r--r--   0        0        0    43787 2023-04-13 18:12:30.739741 openplayground-0.1.5/server/static/index.e96bf64d.css
+-rw-r--r--   0        0        0     7193 2023-04-13 18:12:30.779338 openplayground-0.1.5/server/static/index.e96bf64d.css.br
+-rw-r--r--   0        0        0     8343 2023-04-13 18:12:30.740006 openplayground-0.1.5/server/static/index.e96bf64d.css.gz
+-rw-r--r--   0        0        0      814 2023-04-13 18:12:34.185732 openplayground-0.1.5/server/static/index.html
+-rw-r--r--   0        0        0      284 2023-04-13 18:12:34.187517 openplayground-0.1.5/server/static/index.html.br
+-rw-r--r--   0        0        0      423 2023-04-13 18:12:34.185812 openplayground-0.1.5/server/static/index.html.gz
+-rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 openplayground-0.1.5/PKG-INFO
```

### Comparing `openplayground-0.1.4/LICENSE` & `openplayground-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/README.md` & `openplayground-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/pyproject.toml` & `openplayground-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "openplayground"
-version = "0.1.4"
+version = "0.1.5"
 description = "An LLM playground you can run on your laptop."
 authors = ["Nat Friedman <nat@nat.org>"]
 readme = "README.md"
 homepage = "https://nat.dev/"
 repository = "https://github.com/nat/openplayground"
 keywords = ["llm", "playground", "openplayground"]
 packages = [
   { include = "server", from = "" },
 ]
+include = ["server/static/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aleph_alpha_client="^2.16.1"
 anthropic = "^0.2.3"
 cachetools="^5.3.0"
 click="^8.1.3"
@@ -35,11 +36,10 @@
 [[tool.poetry.source]]
 name = 'pypi-public'
 url = "https://pypi.org/simple/"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
 exclude = [
   ".env",
 ]
```

### Comparing `openplayground-0.1.4/server/app.py` & `openplayground-0.1.5/server/app.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/api/__init__.py` & `openplayground-0.1.5/server/lib/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/api/inference.py` & `openplayground-0.1.5/server/lib/api/inference.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/api/provider.py` & `openplayground-0.1.5/server/lib/api/provider.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/entities.py` & `openplayground-0.1.5/server/lib/entities.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/event_emitter.py` & `openplayground-0.1.5/server/lib/event_emitter.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/inference/__init__.py` & `openplayground-0.1.5/server/lib/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/inference/huggingface/generator.py` & `openplayground-0.1.5/server/lib/inference/huggingface/generator.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/inference/huggingface/hf.py` & `openplayground-0.1.5/server/lib/inference/huggingface/hf.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/sse.py` & `openplayground-0.1.5/server/lib/sse.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/sseserver.py` & `openplayground-0.1.5/server/lib/sseserver.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/lib/storage.py` & `openplayground-0.1.5/server/lib/storage.py`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/server/models.json` & `openplayground-0.1.5/server/models.json`

 * *Files identical despite different names*

### Comparing `openplayground-0.1.4/PKG-INFO` & `openplayground-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplayground
-Version: 0.1.4
+Version: 0.1.5
 Summary: An LLM playground you can run on your laptop.
 Home-page: https://nat.dev/
 Keywords: llm,playground,openplayground
 Author: Nat Friedman
 Author-email: nat@nat.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

