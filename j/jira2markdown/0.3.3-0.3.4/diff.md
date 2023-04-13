# Comparing `tmp/jira2markdown-0.3.3.tar.gz` & `tmp/jira2markdown-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira2markdown-0.3.3.tar", max compression
+gzip compressed data, was "jira2markdown-0.3.4.tar", max compression
```

## Comparing `jira2markdown-0.3.3.tar` & `jira2markdown-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     6011 2023-04-06 17:32:37.179554 jira2markdown-0.3.3/README.md
--rw-r--r--   0        0        0       36 2021-01-31 16:47:22.204367 jira2markdown-0.3.3/jira2markdown/__init__.py
--rw-r--r--   0        0        0     2328 2022-01-12 19:03:05.207863 jira2markdown-0.3.3/jira2markdown/elements.py
--rw-r--r--   0        0        0        0 2021-01-31 17:11:54.757777 jira2markdown-0.3.3/jira2markdown/markup/__init__.py
--rw-r--r--   0        0        0     2207 2022-12-06 15:24:24.761173 jira2markdown-0.3.3/jira2markdown/markup/advanced.py
--rw-r--r--   0        0        0      477 2022-11-24 18:33:27.195584 jira2markdown-0.3.3/jira2markdown/markup/base.py
--rw-r--r--   0        0        0      762 2022-12-06 15:24:24.761173 jira2markdown-0.3.3/jira2markdown/markup/headings.py
--rw-r--r--   0        0        0     1555 2023-04-06 17:32:37.179554 jira2markdown-0.3.3/jira2markdown/markup/images.py
--rw-r--r--   0        0        0     3076 2023-02-03 14:53:07.283223 jira2markdown-0.3.3/jira2markdown/markup/links.py
--rw-r--r--   0        0        0     4074 2022-12-10 09:48:27.736671 jira2markdown-0.3.3/jira2markdown/markup/lists.py
--rw-r--r--   0        0        0     2213 2022-12-06 15:24:24.762173 jira2markdown-0.3.3/jira2markdown/markup/tables.py
--rw-r--r--   0        0        0     1230 2022-12-06 15:24:24.762173 jira2markdown-0.3.3/jira2markdown/markup/text_breaks.py
--rw-r--r--   0        0        0     5456 2023-04-06 17:36:37.060726 jira2markdown-0.3.3/jira2markdown/markup/text_effects.py
--rw-r--r--   0        0        0      646 2022-12-06 15:24:24.762173 jira2markdown-0.3.3/jira2markdown/parser.py
--rw-r--r--   0        0        0     1044 2023-04-06 17:38:34.547160 jira2markdown-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 jira2markdown-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-13 06:40:47.028860 jira2markdown-0.3.4/LICENSE
+-rw-r--r--   0        0        0     6011 2023-04-06 17:32:37.179554 jira2markdown-0.3.4/README.md
+-rw-r--r--   0        0        0       36 2021-01-31 16:47:22.204367 jira2markdown-0.3.4/jira2markdown/__init__.py
+-rw-r--r--   0        0        0     2328 2022-01-12 19:03:05.207863 jira2markdown-0.3.4/jira2markdown/elements.py
+-rw-r--r--   0        0        0        0 2021-01-31 17:11:54.757777 jira2markdown-0.3.4/jira2markdown/markup/__init__.py
+-rw-r--r--   0        0        0     2207 2022-12-06 15:24:24.761173 jira2markdown-0.3.4/jira2markdown/markup/advanced.py
+-rw-r--r--   0        0        0      477 2022-11-24 18:33:27.195584 jira2markdown-0.3.4/jira2markdown/markup/base.py
+-rw-r--r--   0        0        0      762 2022-12-06 15:24:24.761173 jira2markdown-0.3.4/jira2markdown/markup/headings.py
+-rw-r--r--   0        0        0     1555 2023-04-06 17:32:37.179554 jira2markdown-0.3.4/jira2markdown/markup/images.py
+-rw-r--r--   0        0        0     3076 2023-02-03 14:53:07.283223 jira2markdown-0.3.4/jira2markdown/markup/links.py
+-rw-r--r--   0        0        0     4074 2022-12-10 09:48:27.736671 jira2markdown-0.3.4/jira2markdown/markup/lists.py
+-rw-r--r--   0        0        0     2213 2022-12-06 15:24:24.762173 jira2markdown-0.3.4/jira2markdown/markup/tables.py
+-rw-r--r--   0        0        0     1230 2022-12-06 15:24:24.762173 jira2markdown-0.3.4/jira2markdown/markup/text_breaks.py
+-rw-r--r--   0        0        0     5456 2023-04-06 17:36:37.060726 jira2markdown-0.3.4/jira2markdown/markup/text_effects.py
+-rw-r--r--   0        0        0      646 2022-12-06 15:24:24.762173 jira2markdown-0.3.4/jira2markdown/parser.py
+-rw-r--r--   0        0        0     1106 2023-04-13 06:40:47.028860 jira2markdown-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     7073 1970-01-01 00:00:00.000000 jira2markdown-0.3.4/PKG-INFO
```

### Comparing `jira2markdown-0.3.3/README.md` & `jira2markdown-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/elements.py` & `jira2markdown-0.3.4/jira2markdown/elements.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/advanced.py` & `jira2markdown-0.3.4/jira2markdown/markup/advanced.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/headings.py` & `jira2markdown-0.3.4/jira2markdown/markup/headings.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/images.py` & `jira2markdown-0.3.4/jira2markdown/markup/images.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/links.py` & `jira2markdown-0.3.4/jira2markdown/markup/links.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/lists.py` & `jira2markdown-0.3.4/jira2markdown/markup/lists.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/tables.py` & `jira2markdown-0.3.4/jira2markdown/markup/tables.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/text_breaks.py` & `jira2markdown-0.3.4/jira2markdown/markup/text_breaks.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/markup/text_effects.py` & `jira2markdown-0.3.4/jira2markdown/markup/text_effects.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/jira2markdown/parser.py` & `jira2markdown-0.3.4/jira2markdown/parser.py`

 * *Files identical despite different names*

### Comparing `jira2markdown-0.3.3/pyproject.toml` & `jira2markdown-0.3.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "jira2markdown"
-version = "0.3.3"
+version = "0.3.4"
 description = "Convert text from JIRA markup to Markdown using parsing expression grammars"
+license = "MIT"
 authors = ["Evgeniy Krysanov <evgeniy.krysanov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/catcombo/jira2markdown"
 packages = [
     { include = "jira2markdown" },
 ]
 keywords = ["jira", "markdown"]
 classifiers = [
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: Markdown",
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyparsing = "^3"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `jira2markdown-0.3.3/PKG-INFO` & `jira2markdown-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: jira2markdown
-Version: 0.3.3
+Version: 0.3.4
 Summary: Convert text from JIRA markup to Markdown using parsing expression grammars
 Home-page: https://github.com/catcombo/jira2markdown
+License: MIT
 Keywords: jira,markdown
 Author: Evgeniy Krysanov
 Author-email: evgeniy.krysanov@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
```

