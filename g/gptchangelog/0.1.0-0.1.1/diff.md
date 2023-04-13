# Comparing `tmp/gptchangelog-0.1.0.tar.gz` & `tmp/gptchangelog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptchangelog-0.1.0.tar", last modified: Thu Apr 13 15:49:28 2023, max compression
+gzip compressed data, was "gptchangelog-0.1.1.tar", last modified: Thu Apr 13 16:27:09 2023, max compression
```

## Comparing `gptchangelog-0.1.0.tar` & `gptchangelog-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 15:49:28.773314 gptchangelog-0.1.0/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1089 2023-04-13 15:28:44.000000 gptchangelog-0.1.0/LICENSE
--rw-r--r--   0 xjodoin    (501) staff       (20)     1858 2023-04-13 15:49:28.773071 gptchangelog-0.1.0/PKG-INFO
--rw-r--r--   0 xjodoin    (501) staff       (20)     1085 2023-04-13 15:48:08.000000 gptchangelog-0.1.0/README.md
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 15:49:28.772739 gptchangelog-0.1.0/gptchangelog.egg-info/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1858 2023-04-13 15:49:28.000000 gptchangelog-0.1.0/gptchangelog.egg-info/PKG-INFO
--rw-r--r--   0 xjodoin    (501) staff       (20)      244 2023-04-13 15:49:28.000000 gptchangelog-0.1.0/gptchangelog.egg-info/SOURCES.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)        1 2023-04-13 15:49:28.000000 gptchangelog-0.1.0/gptchangelog.egg-info/dependency_links.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       52 2023-04-13 15:49:28.000000 gptchangelog-0.1.0/gptchangelog.egg-info/entry_points.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       30 2023-04-13 15:49:28.000000 gptchangelog-0.1.0/gptchangelog.egg-info/requires.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)        1 2023-04-13 15:49:28.000000 gptchangelog-0.1.0/gptchangelog.egg-info/top_level.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       38 2023-04-13 15:49:28.773402 gptchangelog-0.1.0/setup.cfg
--rw-r--r--   0 xjodoin    (501) staff       (20)     1173 2023-04-13 15:26:33.000000 gptchangelog-0.1.0/setup.py
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 16:27:09.701250 gptchangelog-0.1.1/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1089 2023-04-13 15:28:44.000000 gptchangelog-0.1.1/LICENSE
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1861 2023-04-13 16:27:09.700988 gptchangelog-0.1.1/PKG-INFO
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1088 2023-04-13 15:56:57.000000 gptchangelog-0.1.1/README.md
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 16:27:09.698595 gptchangelog-0.1.1/gptchangelog/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     2939 2023-04-13 16:23:08.000000 gptchangelog-0.1.1/gptchangelog/__init__.py
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 16:27:09.700601 gptchangelog-0.1.1/gptchangelog.egg-info/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1861 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/PKG-INFO
+-rw-r--r--   0 xjodoin    (501) staff       (20)      269 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/SOURCES.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)        1 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/dependency_links.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       52 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/entry_points.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       30 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/requires.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       13 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/top_level.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       38 2023-04-13 16:27:09.701347 gptchangelog-0.1.1/setup.cfg
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1173 2023-04-13 16:25:44.000000 gptchangelog-0.1.1/setup.py
```

### Comparing `gptchangelog-0.1.0/LICENSE` & `gptchangelog-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gptchangelog-0.1.0/PKG-INFO` & `gptchangelog-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptchangelog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically generate a changelog using GPT-3
 Home-page: https://github.com/xjodoin/gptchangelog
 Author: Xavier Jodoin
 Author-email: xavier@jodoin.me
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -34,21 +34,21 @@
 
 Before using GPT Changelog, you need to create a configuration file named config.ini in the $HOME/.config/gptchangelog directory.
 
     [openai]
     api_key = your_openai_api_key_here
 
 Replace your_openai_api_key_here with your actual OpenAI API key.
-Usage
+
+## Usage
 
 To generate a changelog and prepend it to the CHANGELOG.md file, navigate to your Git repository directory and run the following command:
 
     gptchangelog
 
-
 The script will fetch commit messages since the most recent tag, determine the next version based on semantic versioning, generate a changelog using OpenAI's GPT-3, and prepend the changelog to the CHANGELOG.md file. If the CHANGELOG.md file does not exist, the script will create it.
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `gptchangelog-0.1.0/README.md` & `gptchangelog-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 Before using GPT Changelog, you need to create a configuration file named config.ini in the $HOME/.config/gptchangelog directory.
 
     [openai]
     api_key = your_openai_api_key_here
 
 Replace your_openai_api_key_here with your actual OpenAI API key.
-Usage
+
+## Usage
 
 To generate a changelog and prepend it to the CHANGELOG.md file, navigate to your Git repository directory and run the following command:
 
     gptchangelog
 
-
 The script will fetch commit messages since the most recent tag, determine the next version based on semantic versioning, generate a changelog using OpenAI's GPT-3, and prepend the changelog to the CHANGELOG.md file. If the CHANGELOG.md file does not exist, the script will create it.
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `gptchangelog-0.1.0/gptchangelog.egg-info/PKG-INFO` & `gptchangelog-0.1.1/gptchangelog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptchangelog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically generate a changelog using GPT-3
 Home-page: https://github.com/xjodoin/gptchangelog
 Author: Xavier Jodoin
 Author-email: xavier@jodoin.me
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -34,21 +34,21 @@
 
 Before using GPT Changelog, you need to create a configuration file named config.ini in the $HOME/.config/gptchangelog directory.
 
     [openai]
     api_key = your_openai_api_key_here
 
 Replace your_openai_api_key_here with your actual OpenAI API key.
-Usage
+
+## Usage
 
 To generate a changelog and prepend it to the CHANGELOG.md file, navigate to your Git repository directory and run the following command:
 
     gptchangelog
 
-
 The script will fetch commit messages since the most recent tag, determine the next version based on semantic versioning, generate a changelog using OpenAI's GPT-3, and prepend the changelog to the CHANGELOG.md file. If the CHANGELOG.md file does not exist, the script will create it.
 
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `gptchangelog-0.1.0/setup.py` & `gptchangelog-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gptchangelog",
-    version="0.1.0",
+    version="0.1.1",
     author="Xavier Jodoin",
     author_email="xavier@jodoin.me",
     description="Automatically generate a changelog using GPT-3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xjodoin/gptchangelog",
     packages=find_packages(),
```

