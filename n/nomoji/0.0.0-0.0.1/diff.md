# Comparing `tmp/nomoji-0.0.0.tar.gz` & `tmp/nomoji-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomoji-0.0.0.tar", last modified: Thu Apr 13 13:45:48 2023, max compression
+gzip compressed data, was "nomoji-0.0.1.tar", last modified: Thu Apr 13 13:46:24 2023, max compression
```

## Comparing `nomoji-0.0.0.tar` & `nomoji-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:45:48.911985 nomoji-0.0.0/
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.0/.gitignore
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.0/LICENSE
--rw-r--r--   0 leriomaggio   (502) staff       (20)      918 2023-04-13 13:45:48.911821 nomoji-0.0.0/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      671 2023-04-13 13:20:40.000000 nomoji-0.0.0/README.md
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:45:48.910016 nomoji-0.0.0/nomoji/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      543 2023-04-13 13:38:22.000000 nomoji-0.0.0/nomoji/__init__.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:45:48.911135 nomoji-0.0.0/nomoji.egg-info/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      918 2023-04-13 13:45:48.000000 nomoji-0.0.0/nomoji.egg-info/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      212 2023-04-13 13:45:48.000000 nomoji-0.0.0/nomoji.egg-info/SOURCES.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-13 13:45:48.000000 nomoji-0.0.0/nomoji.egg-info/dependency_links.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-13 13:45:48.000000 nomoji-0.0.0/nomoji.egg-info/top_level.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.0/pyproject.toml
--rw-r--r--   0 leriomaggio   (502) staff       (20)       38 2023-04-13 13:45:48.912038 nomoji-0.0.0/setup.cfg
--rw-r--r--   0 leriomaggio   (502) staff       (20)      565 2023-04-13 13:41:02.000000 nomoji-0.0.0/setup.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:45:48.911324 nomoji-0.0.0/tests/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      705 2023-04-13 13:39:02.000000 nomoji-0.0.0/tests/test_nomoji.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.465727 nomoji-0.0.1/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.1/.gitignore
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.1/LICENSE
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      918 2023-04-13 13:46:24.465558 nomoji-0.0.1/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      671 2023-04-13 13:20:40.000000 nomoji-0.0.1/README.md
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.463977 nomoji-0.0.1/nomoji/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      543 2023-04-13 13:38:22.000000 nomoji-0.0.1/nomoji/__init__.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.465008 nomoji-0.0.1/nomoji.egg-info/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      918 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      212 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/SOURCES.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/dependency_links.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/top_level.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.1/pyproject.toml
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       38 2023-04-13 13:46:24.465793 nomoji-0.0.1/setup.cfg
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      588 2023-04-13 13:46:18.000000 nomoji-0.0.1/setup.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.465232 nomoji-0.0.1/tests/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      705 2023-04-13 13:39:02.000000 nomoji-0.0.1/tests/test_nomoji.py
```

### Comparing `nomoji-0.0.0/.gitignore` & `nomoji-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.0/LICENSE` & `nomoji-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.0/PKG-INFO` & `nomoji-0.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: nomoji
-Version: 0.0.0
-Summary: Silly Python Package to print digits using emojis
-Home-page: https://github.com/leriomaggio/emoji-numbers/
-Author: Valerio Maggio
-Author-email: vmaggio@anaconda.com
-License-File: LICENSE
-
 # emoji-numbers
 Simple and silly Python package to print numbers using Emoji digits.
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
```

### Comparing `nomoji-0.0.0/README.md` & `nomoji-0.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: nomoji
+Version: 0.0.1
+Summary: Silly Python Package to print digits using emojis
+Home-page: https://github.com/leriomaggio/emoji-numbers/
+Author: Valerio Maggio
+Author-email: vmaggio@anaconda.com
+License-File: LICENSE
+
 # emoji-numbers
 Simple and silly Python package to print numbers using Emoji digits.
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
```

### Comparing `nomoji-0.0.0/nomoji/__init__.py` & `nomoji-0.0.1/nomoji/__init__.py`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.0/nomoji.egg-info/PKG-INFO` & `nomoji-0.0.1/nomoji.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.0
+Version: 0.0.1
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
 License-File: LICENSE
 
 # emoji-numbers
```

### Comparing `nomoji-0.0.0/setup.py` & `nomoji-0.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 CURRENT_FOLDER = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(CURRENT_FOLDER, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name="nomoji",
       author="Valerio Maggio",
+      version="0.0.1",
       author_email="vmaggio@anaconda.com",
       description="Silly Python Package to print digits using emojis",
       long_description=long_description,
       url="https://github.com/leriomaggio/emoji-numbers/",
       packages=find_packages(exclude=[]),
       nclude_package_data=True)
```

### Comparing `nomoji-0.0.0/tests/test_nomoji.py` & `nomoji-0.0.1/tests/test_nomoji.py`

 * *Files identical despite different names*

