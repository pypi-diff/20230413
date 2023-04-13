# Comparing `tmp/leaguecloser-1.0.1.tar.gz` & `tmp/leaguecloser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "leaguecloser-1.0.2.tar", last modified: Thu Apr 13 06:06:49 2023, max compression
```

## Comparing `leaguecloser-1.0.1.tar` & `leaguecloser-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/Dev Setup.ps1
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/Makefile
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/Auto League Closer.spec
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/InstallerSetupScript.iss
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/dev-requirements.txt
--rw-r--r--   0        0        0    83012 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/icon.ico
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/requirements.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/app.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/__init__.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/computer.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/league.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/sikuli.py
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/1681351869136.png
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/1681352088077.png
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/close_league.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/tests/test_sequence.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/LICENSE
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.838083 leaguecloser-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-13 01:51:56.000000 leaguecloser-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2422 2023-04-13 06:06:49.836082 leaguecloser-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1983 2023-04-13 05:48:02.000000 leaguecloser-1.0.2/README.md
+-rw-rw-rw-   0        0        0      660 2023-04-13 06:06:36.000000 leaguecloser-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:06:49.839083 leaguecloser-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.778023 leaguecloser-1.0.2/src/
+-rw-rw-rw-   0        0        0      373 2023-04-13 02:39:23.000000 leaguecloser-1.0.2/src/app.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.795328 leaguecloser-1.0.2/src/leaguecloser/
+-rw-rw-rw-   0        0        0      283 2023-04-13 03:02:26.000000 leaguecloser-1.0.2/src/leaguecloser/__init__.py
+-rw-rw-rw-   0        0        0    10786 2023-04-13 02:59:12.000000 leaguecloser-1.0.2/src/leaguecloser/computer.py
+-rw-rw-rw-   0        0        0     1169 2023-04-13 04:45:18.000000 leaguecloser-1.0.2/src/leaguecloser/league.py
+-rw-rw-rw-   0        0        0      564 2023-04-13 04:45:21.000000 leaguecloser-1.0.2/src/leaguecloser/sikuli.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.828349 leaguecloser-1.0.2/src/leaguecloser.egg-info/
+-rw-rw-rw-   0        0        0     2422 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.833083 leaguecloser-1.0.2/tests/
+-rw-rw-rw-   0        0        0      960 2023-04-13 03:13:42.000000 leaguecloser-1.0.2/tests/test_sequence.py
```

### Comparing `leaguecloser-1.0.1/src/leaguecloser/computer.py` & `leaguecloser-1.0.2/src/leaguecloser/computer.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.1/src/leaguecloser/league.py` & `leaguecloser-1.0.2/src/leaguecloser/league.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.1/src/leaguecloser/sikuli.py` & `leaguecloser-1.0.2/src/leaguecloser/sikuli.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.1/tests/test_sequence.py` & `leaguecloser-1.0.2/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.1/LICENSE` & `leaguecloser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.1/README.md` & `leaguecloser-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.1/pyproject.toml` & `leaguecloser-1.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "leaguecloser"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Giantpizzahead" },
 ]
 description = "Mock package that auto-closes the League client"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
 ]
+
 dependencies = [
   "psutil",
   "pyautogui",
   "pywin32",
 ]
 
 [project.urls]
```

### Comparing `leaguecloser-1.0.1/PKG-INFO` & `leaguecloser-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-Metadata-Version: 2.1
-Name: leaguecloser
-Version: 1.0.1
-Summary: Mock package that auto-closes the League client
-Project-URL: Homepage, https://github.com/Giantpizzahead/auto-league-closer
-Author: Giantpizzahead
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: psutil
-Requires-Dist: pyautogui
-Requires-Dist: pywin32
-Description-Content-Type: text/markdown
-
-# Auto League Closer
-
-Tired of procrastinating on homework all day while still being hardstuck Bronze? Suffering from a bad case of League withdrawal?
-
-Well, I've got a solution for you! Install the **Auto League Closer**!
-
-This handy program will **automatically close the League of Legends client whenever it's running**, so you can get back to binging YouTube videos - uh, I mean doing homework :)
-
-*This is a mock application to demonstrate a clean project structure, along with steps to distribute Python modules and end user application installers.*
-
-## Installation
-
-Run the installer [here](https://github.com/Giantpizzahead/auto-league-closer/releases/download/v1.0.0/AutoLeagueCloserSetup.exe).
-
-## How It Works
-
-1. Repeatedly checks if League is open using [psutil](https://pypi.org/project/psutil/).
-2. Closes League in a \~fancy\~ way using [SikuliX](http://sikulix.com/).
-
-## Using the Python Module
-
-```bash
-$ pip install leaguecloser
-```
-
-View the [PyPi page](https://pypi.org/project/leaguecloser/1.0.0/).
-
-Example usage (also what the installable app does):
-
-```python
-import leaguecloser
-import time
-
-print("Searching for League...")
-while True:
-    if leaguecloser.is_league_running():
-        print("\nNO LEAGUE ALLOWED!")
-        if leaguecloser.close_league():
-            print("\nThat's right... now get back to work!")
-    time.sleep(3)
-```
-
-## Packaging and Building Methods
-
-The Makefile contains good practice methods for the common tasks below:
-
-```bash
-$ make run  # Runs the file
-$ make test  # Runs all tests
-$ make package_create  # Creates (or updates) the leaguecloser package
-$ make package_upload  # Uploads the leaguecloser package to PyPi
-$ make build_app  # Builds the app into a standalone folder with an executable
-```
-
-## Development Setup
-
-First, setup a [virtual environment](https://kylefu.me/cheat_python/envanddeps.html). Then run:
-
-```powershell
-> & '.\Dev Setup.ps1'
-```
+Metadata-Version: 2.1
+Name: leaguecloser
+Version: 1.0.2
+Summary: Mock package that auto-closes the League client
+Author: Giantpizzahead
+Project-URL: Homepage, https://github.com/Giantpizzahead/auto-league-closer
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Auto League Closer
+
+Tired of procrastinating on homework all day while still being hardstuck Bronze? Suffering from a bad case of League withdrawal?
+
+Well, I've got a solution for you! Install the **Auto League Closer**!
+
+This handy program will **automatically close the League of Legends client whenever it's running**, so you can get back to binging YouTube videos - uh, I mean doing homework :)
+
+*This is a mock application to demonstrate a clean project structure, along with steps to distribute Python modules and end user application installers.*
+
+## Installation
+
+Run the installer [here](https://github.com/Giantpizzahead/auto-league-closer/releases/download/v1.0.0/AutoLeagueCloserSetup.exe).
+
+## How It Works
+
+1. Repeatedly checks if League is open using [psutil](https://pypi.org/project/psutil/).
+2. Closes League in a \~fancy\~ way using [SikuliX](http://sikulix.com/).
+
+## Using the Python Module
+
+```bash
+$ pip install leaguecloser
+```
+
+View the [PyPi page](https://pypi.org/project/leaguecloser/1.0.0/).
+
+Example usage (also what the installable app does):
+
+```python
+import leaguecloser
+import time
+
+print("Searching for League...")
+while True:
+    if leaguecloser.is_league_running():
+        print("\nNO LEAGUE ALLOWED!")
+        if leaguecloser.close_league():
+            print("\nThat's right... now get back to work!")
+    time.sleep(3)
+```
+
+## Packaging and Building Methods
+
+The Makefile contains good practice methods for the common tasks below:
+
+```bash
+$ make run  # Runs the file
+$ make test  # Runs all tests
+$ make package_create  # Creates (or updates) the leaguecloser package
+$ make package_upload  # Uploads the leaguecloser package to PyPi
+$ make build_app  # Builds the app into a standalone folder with an executable
+```
+
+## Development Setup
+
+First, setup a [virtual environment](https://kylefu.me/cheat_python/envanddeps.html). Then run:
+
+```powershell
+> & '.\Dev Setup.ps1'
+```
```

