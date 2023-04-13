# Comparing `tmp/nomoji-0.0.1.tar.gz` & `tmp/nomoji-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomoji-0.0.1.tar", last modified: Thu Apr 13 13:46:24 2023, max compression
+gzip compressed data, was "nomoji-0.0.2.tar", last modified: Thu Apr 13 13:55:06 2023, max compression
```

## Comparing `nomoji-0.0.1.tar` & `nomoji-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.465727 nomoji-0.0.1/
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.1/.gitignore
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.1/LICENSE
--rw-r--r--   0 leriomaggio   (502) staff       (20)      918 2023-04-13 13:46:24.465558 nomoji-0.0.1/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      671 2023-04-13 13:20:40.000000 nomoji-0.0.1/README.md
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.463977 nomoji-0.0.1/nomoji/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      543 2023-04-13 13:38:22.000000 nomoji-0.0.1/nomoji/__init__.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.465008 nomoji-0.0.1/nomoji.egg-info/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      918 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      212 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/SOURCES.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/dependency_links.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-13 13:46:24.000000 nomoji-0.0.1/nomoji.egg-info/top_level.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.1/pyproject.toml
--rw-r--r--   0 leriomaggio   (502) staff       (20)       38 2023-04-13 13:46:24.465793 nomoji-0.0.1/setup.cfg
--rw-r--r--   0 leriomaggio   (502) staff       (20)      588 2023-04-13 13:46:18.000000 nomoji-0.0.1/setup.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:46:24.465232 nomoji-0.0.1/tests/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      705 2023-04-13 13:39:02.000000 nomoji-0.0.1/tests/test_nomoji.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.750388 nomoji-0.0.2/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.2/.gitignore
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.2/LICENSE
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      959 2023-04-13 13:55:06.750209 nomoji-0.0.2/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      672 2023-04-13 13:52:33.000000 nomoji-0.0.2/README.md
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.748718 nomoji-0.0.2/nomoji/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      547 2023-04-13 13:52:15.000000 nomoji-0.0.2/nomoji/__init__.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.749754 nomoji-0.0.2/nomoji.egg-info/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      959 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      212 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/SOURCES.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/dependency_links.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-13 13:55:06.000000 nomoji-0.0.2/nomoji.egg-info/top_level.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.2/pyproject.toml
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       38 2023-04-13 13:55:06.750451 nomoji-0.0.2/setup.cfg
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      632 2023-04-13 13:54:15.000000 nomoji-0.0.2/setup.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-13 13:55:06.749967 nomoji-0.0.2/tests/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      707 2023-04-13 13:52:09.000000 nomoji-0.0.2/tests/test_nomoji.py
```

### Comparing `nomoji-0.0.1/.gitignore` & `nomoji-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.1/LICENSE` & `nomoji-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.1/PKG-INFO` & `nomoji-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.1
+Version: 0.0.2
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # emoji-numbers
 Simple and silly Python package to print numbers using Emoji digits.
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
+
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
 * [Mahe Iram Khan](https://us.pycon.org/2023/speaker/profile/166/)
 * [Valerio Maggio](https://us.pycon.org/2023/speaker/profile/109/)
 
 This package will be published on PyPi and it will be used solely
 to demonstrate how to add `pip` dependecies to a `conda` package.
```

### Comparing `nomoji-0.0.1/README.md` & `nomoji-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # emoji-numbers
 Simple and silly Python package to print numbers using Emoji digits.
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
+
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
 * [Mahe Iram Khan](https://us.pycon.org/2023/speaker/profile/166/)
 * [Valerio Maggio](https://us.pycon.org/2023/speaker/profile/109/)
 
 This package will be published on PyPi and it will be used solely
 to demonstrate how to add `pip` dependecies to a `conda` package.
```

### Comparing `nomoji-0.0.1/nomoji/__init__.py` & `nomoji-0.0.2/nomoji/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 __version__ = "0.0.1"
 
-KEYCAPS_DIGIT ="%d\uFE0F\u20E3"
+KEYCAPS_DIGIT = "%d\uFE0F\u20E3"
 KEYCAPS_TEN = "\u1F51F"
 GAME_DIE = "🎲"
 
 DIGITS = {n: (KEYCAPS_DIGIT % n) for n in range(10)}
 DIGITS[10] = KEYCAPS_TEN
 
+
 def emojize(number: int) -> str:
     """Convert any integer number into emoji digits"""
 
     try:
         number = abs(int(number))
     except ValueError as e:
         raise ValueError("Only integer numbers could be emojized")
     else:
-        if number in range(0,9):
+        if number in range(0, 9):
             return DIGITS[number]
-        return " ".join([DIGITS[int(d)] for d in str(number)])
+        return " ".join([DIGITS[int(d)] for d in str(number)])
```

### Comparing `nomoji-0.0.1/nomoji.egg-info/PKG-INFO` & `nomoji-0.0.2/nomoji.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.1
+Version: 0.0.2
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # emoji-numbers
 Simple and silly Python package to print numbers using Emoji digits.
 
 This project is used as part of the PyConUS tutorial **Publishing your Python project, the conda way** 
 presented at [PyConUS](https://us.pycon.org/2023/schedule/presentation/94/) by:
+
 * [Dave Clements](https://us.pycon.org/2023/speaker/profile/108/)
 * [Bianca Henderson](https://us.pycon.org/2023/speaker/profile/75/)
 * [Mahe Iram Khan](https://us.pycon.org/2023/speaker/profile/166/)
 * [Valerio Maggio](https://us.pycon.org/2023/speaker/profile/109/)
 
 This package will be published on PyPi and it will be used solely
 to demonstrate how to add `pip` dependecies to a `conda` package.
```

### Comparing `nomoji-0.0.1/setup.py` & `nomoji-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 from setuptools import find_packages, setup
 
 CURRENT_FOLDER = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(CURRENT_FOLDER, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-setup(name="nomoji",
-      author="Valerio Maggio",
-      version="0.0.1",
-      author_email="vmaggio@anaconda.com",
-      description="Silly Python Package to print digits using emojis",
-      long_description=long_description,
-      url="https://github.com/leriomaggio/emoji-numbers/",
-      packages=find_packages(exclude=[]),
-      nclude_package_data=True)
+setup(
+    name="nomoji",
+    author="Valerio Maggio",
+    version="0.0.2",
+    author_email="vmaggio@anaconda.com",
+    description="Silly Python Package to print digits using emojis",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/leriomaggio/emoji-numbers/",
+    packages=find_packages(exclude=[]),
+    include_package_data=True,
+)
```

### Comparing `nomoji-0.0.1/tests/test_nomoji.py` & `nomoji-0.0.2/tests/test_nomoji.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 from nomoji import DIGITS, GAME_DIE
 from nomoji import emojize
 
+
 def test_game_die():
     assert GAME_DIE == "🎲"
 
 
 def test_all_digits():
     assert len(DIGITS) == 11, "Not all numbers in Digits"
     assert all(k in range(0, 11) for k in DIGITS)
@@ -23,8 +24,8 @@
 
 
 def test_emojize_on_float_numbers():
     assert emojize(1.3) == DIGITS[1]
 
 
 def test_emojize_on_negative_ints():
-    assert emojize(-9) == DIGITS[9]
+    assert emojize(-9) == DIGITS[9]
```

