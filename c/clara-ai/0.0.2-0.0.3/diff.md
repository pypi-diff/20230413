# Comparing `tmp/clara_ai-0.0.2.tar.gz` & `tmp/clara_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clara_ai-0.0.2.tar", max compression
+gzip compressed data, was "clara_ai-0.0.3.tar", max compression
```

## Comparing `clara_ai-0.0.2.tar` & `clara_ai-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1534 2023-04-12 20:56:15.471438 clara_ai-0.0.2/LICENSE
--rw-r--r--   0        0        0     1888 2023-04-12 20:56:15.471438 clara_ai-0.0.2/README.md
--rw-r--r--   0        0        0     2558 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/cli.py
--rw-r--r--   0        0        0       54 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/console.py
--rw-r--r--   0        0        0     1682 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/consts.py
--rw-r--r--   0        0        0     3269 2023-04-12 20:56:15.471438 clara_ai-0.0.2/clara/index.py
--rw-r--r--   0        0        0      545 2023-04-12 20:56:15.471438 clara_ai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 clara_ai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1534 2023-04-13 17:48:10.642821 clara_ai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2148 2023-04-13 17:48:10.642821 clara_ai-0.0.3/README.md
+-rw-r--r--   0        0        0     4458 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/cli.py
+-rw-r--r--   0        0        0       54 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/console.py
+-rw-r--r--   0        0        0     2660 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/consts.py
+-rw-r--r--   0        0        0     5248 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/index.py
+-rw-r--r--   0        0        0      665 2023-04-13 17:48:10.646821 clara_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 clara_ai-0.0.3/PKG-INFO
```

### Comparing `clara_ai-0.0.2/LICENSE` & `clara_ai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.2/README.md` & `clara_ai-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ![Features](https://github.com/SeednapseAI/clara/raw/master/images/screenshot.png)
 
 ***This project is currently in its early stages of development and is considered a work in progress. You may encounter some issues, or incomplete features. We appreciate your understanding and patience as we continue to refine and enhance the project. Your feedback will help us improve and shape this project.***
 
 ## Introduction
 
-Clara is an AI-powered tool designed to assist developers in navigating unfamiliar code repositories, making it highly valuable during the on-boarding process for new projects, or when deciphering legacy code..
+Clara is an AI-powered tool designed to assist developers in navigating unfamiliar code repositories, making it highly valuable during the on-boarding process for new projects, or when deciphering legacy code.
 
 In the future, Clara will also provide support for tasks such as documentation, auditing, and developing new features, among others.
 
 ## Usage
 
 Install:
 
@@ -60,11 +60,26 @@
      clean
        Delete vector DB for a given path.
 
      config
        Get config for a given path.
 ```
 
+## Chat commands
+
+During chat you can also use this commands:
+
+```
+/context -- show the context for the last answer
+
+/edit    -- open editor to edit the message
+
+/quit
+/exit    -- exit (you can use also CTRL-C or CTRL-D)
+
+/help    -- show this message
+```
+
 ## Roadmap
 
-[ ] Improve chat: short-term history, context, personality,...
-[ ] Tools: document code, audit, refactoring, test creation,...
+- [ ] Improve chat: short-term history, context, personality,...
+- [ ] Tools: document code, audit, refactoring, test creation,...
```

### Comparing `clara_ai-0.0.2/pyproject.toml` & `clara_ai-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [tool.poetry]
 name = "clara-ai"
-version = "0.0.2"
+version = "0.0.3"
 description = "CLARA: Code Language Assistant & Repository Analyzer"
 authors = ["Cristóbal Carnero Liñán <cristobal@seednapse.ai>"]
 readme = "README.md"
 packages = [{include = "clara"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 langchain = {extras = ["llms"], version = "^0.0.136"}
 fire = "^0.5.0"
 chromadb = "^0.3.21"
 rich = "^13.3.3"
 tiktoken = "^0.3.3"
+prompt-toolkit = "^3.0.38"
+click = "^8.1.3"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.0"
+icecream = "^2.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 clara = "clara.cli:main"
```

### Comparing `clara_ai-0.0.2/PKG-INFO` & `clara_ai-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: clara-ai
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLARA: Code Language Assistant & Repository Analyzer
 Author: Cristóbal Carnero Liñán
 Author-email: cristobal@seednapse.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.21,<0.4.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: langchain[llms] (>=0.0.136,<0.0.137)
+Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
 CLARA: Code Language Assistant & Repository Analyzer 📜🔍🤖
 ========================================================
 
@@ -25,15 +27,15 @@
 
 ![Features](https://github.com/SeednapseAI/clara/raw/master/images/screenshot.png)
 
 ***This project is currently in its early stages of development and is considered a work in progress. You may encounter some issues, or incomplete features. We appreciate your understanding and patience as we continue to refine and enhance the project. Your feedback will help us improve and shape this project.***
 
 ## Introduction
 
-Clara is an AI-powered tool designed to assist developers in navigating unfamiliar code repositories, making it highly valuable during the on-boarding process for new projects, or when deciphering legacy code..
+Clara is an AI-powered tool designed to assist developers in navigating unfamiliar code repositories, making it highly valuable during the on-boarding process for new projects, or when deciphering legacy code.
 
 In the future, Clara will also provide support for tasks such as documentation, auditing, and developing new features, among others.
 
 ## Usage
 
 Install:
 
@@ -77,12 +79,27 @@
      clean
        Delete vector DB for a given path.
 
      config
        Get config for a given path.
 ```
 
+## Chat commands
+
+During chat you can also use this commands:
+
+```
+/context -- show the context for the last answer
+
+/edit    -- open editor to edit the message
+
+/quit
+/exit    -- exit (you can use also CTRL-C or CTRL-D)
+
+/help    -- show this message
+```
+
 ## Roadmap
 
-[ ] Improve chat: short-term history, context, personality,...
-[ ] Tools: document code, audit, refactoring, test creation,...
+- [ ] Improve chat: short-term history, context, personality,...
+- [ ] Tools: document code, audit, refactoring, test creation,...
```

