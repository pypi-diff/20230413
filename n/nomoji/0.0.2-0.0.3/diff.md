# Comparing `tmp/nomoji-0.0.2.tar.gz` & `tmp/nomoji-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomoji-0.0.2.tar", last modified: Thu Apr 13 13:55:06 2023, max compression
+gzip compressed data, was "nomoji-0.0.3.tar", last modified: Thu Apr 13 15:15:19 2023, max compression
```

## Comparing `nomoji-0.0.2.tar` & `nomoji-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.750388 nomoji-0.0.2/
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.2/.gitignore
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.2/LICENSE
--rw-r--r--   0 leriomaggio   (502) staff       (20)      959 2023-04-13 13:55:06.750209 nomoji-0.0.2/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      672 2023-04-13 13:52:33.000000 nomoji-0.0.2/README.md
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.748718 nomoji-0.0.2/nomoji/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      547 2023-04-13 13:52:15.000000 nomoji-0.0.2/nomoji/__init__.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.749754 nomoji-0.0.2/nomoji.egg-info/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      959 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      212 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/SOURCES.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/dependency_links.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/top_level.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.2/pyproject.toml
--rw-r--r--   0 leriomaggio   (502) staff       (20)       38 2023-04-13 13:55:06.750451 nomoji-0.0.2/setup.cfg
--rw-r--r--   0 leriomaggio   (502) staff       (20)      632 2023-04-13 13:54:15.000000 nomoji-0.0.2/setup.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.749967 nomoji-0.0.2/tests/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      707 2023-04-13 13:52:09.000000 nomoji-0.0.2/tests/test_nomoji.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 15:15:19.721333 nomoji-0.0.3/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.3/.gitignore
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.3/LICENSE
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1337 2023-04-13 15:15:19.721423 nomoji-0.0.3/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      799 2023-04-13 15:15:02.000000 nomoji-0.0.3/README.md
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 15:15:19.719758 nomoji-0.0.3/nomoji/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      547 2023-04-13 13:52:15.000000 nomoji-0.0.3/nomoji/__init__.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 15:15:19.720773 nomoji-0.0.3/nomoji.egg-info/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1337 2023-04-13 15:15:19.000000 nomoji-0.0.3/nomoji.egg-info/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      222 2023-04-13 15:15:19.000000 nomoji-0.0.3/nomoji.egg-info/SOURCES.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-13 15:15:19.000000 nomoji-0.0.3/nomoji.egg-info/dependency_links.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-13 15:15:19.000000 nomoji-0.0.3/nomoji.egg-info/top_level.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.3/pyproject.toml
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      312 2023-04-13 15:15:19.721706 nomoji-0.0.3/setup.cfg
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      632 2023-04-13 15:12:20.000000 nomoji-0.0.3/setup.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 15:15:19.720930 nomoji-0.0.3/tests/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      707 2023-04-13 13:52:09.000000 nomoji-0.0.3/tests/test_nomoji.py
```

### Comparing `nomoji-0.0.2/.gitignore` & `nomoji-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.2/LICENSE` & `nomoji-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.2/PKG-INFO` & `nomoji-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.2
+Version: 0.0.3
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # emoji-numbers
-Simple and silly Python package to print numbers using Emoji digits.
+Simple and silly Python package to print integer numbers using Emoji digits.
+
+Plus there is also a fancy `GAME_DIE` to use for apps like [`dnd-roller`](https://github.com/leriomaggio/dnd-roller).
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
 
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
 * [Mahe Iram Khan](https://us.pycon.org/2023/speaker/profile/166/)
```

### Comparing `nomoji-0.0.2/README.md` & `nomoji-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # emoji-numbers
-Simple and silly Python package to print numbers using Emoji digits.
+Simple and silly Python package to print integer numbers using Emoji digits.
+
+Plus there is also a fancy `GAME_DIE` to use for apps like [`dnd-roller`](https://github.com/leriomaggio/dnd-roller).
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
 
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
 * [Mahe Iram Khan](https://us.pycon.org/2023/speaker/profile/166/)
```

### Comparing `nomoji-0.0.2/nomoji/__init__.py` & `nomoji-0.0.3/nomoji/__init__.py`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.2/nomoji.egg-info/PKG-INFO` & `nomoji-0.0.3/nomoji.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.2
+Version: 0.0.3
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # emoji-numbers
-Simple and silly Python package to print numbers using Emoji digits.
+Simple and silly Python package to print integer numbers using Emoji digits.
+
+Plus there is also a fancy `GAME_DIE` to use for apps like [`dnd-roller`](https://github.com/leriomaggio/dnd-roller).
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
 
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
 * [Mahe Iram Khan](https://us.pycon.org/2023/speaker/profile/166/)
```

### Comparing `nomoji-0.0.2/setup.py` & `nomoji-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(os.path.join(CURRENT_FOLDER, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="nomoji",
     author="Valerio Maggio",
-    version="0.0.2",
+    version="0.0.3",
     author_email="vmaggio@anaconda.com",
     description="Silly Python Package to print digits using emojis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leriomaggio/emoji-numbers/",
     packages=find_packages(exclude=[]),
     include_package_data=True,
```

### Comparing `nomoji-0.0.2/tests/test_nomoji.py` & `nomoji-0.0.3/tests/test_nomoji.py`

 * *Files identical despite different names*

