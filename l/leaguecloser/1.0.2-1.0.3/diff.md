# Comparing `tmp/leaguecloser-1.0.2.tar.gz` & `tmp/leaguecloser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaguecloser-1.0.2.tar", last modified: Thu Apr 13 06:06:49 2023, max compression
+gzip compressed data, was "leaguecloser-1.0.3.tar", last modified: Thu Apr 13 06:42:18 2023, max compression
```

## Comparing `leaguecloser-1.0.2.tar` & `leaguecloser-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.838083 leaguecloser-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-04-13 01:51:56.000000 leaguecloser-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2422 2023-04-13 06:06:49.836082 leaguecloser-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1983 2023-04-13 05:48:02.000000 leaguecloser-1.0.2/README.md
--rw-rw-rw-   0        0        0      660 2023-04-13 06:06:36.000000 leaguecloser-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 06:06:49.839083 leaguecloser-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.778023 leaguecloser-1.0.2/src/
--rw-rw-rw-   0        0        0      373 2023-04-13 02:39:23.000000 leaguecloser-1.0.2/src/app.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.795328 leaguecloser-1.0.2/src/leaguecloser/
--rw-rw-rw-   0        0        0      283 2023-04-13 03:02:26.000000 leaguecloser-1.0.2/src/leaguecloser/__init__.py
--rw-rw-rw-   0        0        0    10786 2023-04-13 02:59:12.000000 leaguecloser-1.0.2/src/leaguecloser/computer.py
--rw-rw-rw-   0        0        0     1169 2023-04-13 04:45:18.000000 leaguecloser-1.0.2/src/leaguecloser/league.py
--rw-rw-rw-   0        0        0      564 2023-04-13 04:45:21.000000 leaguecloser-1.0.2/src/leaguecloser/sikuli.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.828349 leaguecloser-1.0.2/src/leaguecloser.egg-info/
--rw-rw-rw-   0        0        0     2422 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 06:06:49.000000 leaguecloser-1.0.2/src/leaguecloser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 06:06:49.833083 leaguecloser-1.0.2/tests/
--rw-rw-rw-   0        0        0      960 2023-04-13 03:13:42.000000 leaguecloser-1.0.2/tests/test_sequence.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.850026 leaguecloser-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-04-13 01:51:56.000000 leaguecloser-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-04-13 06:27:50.000000 leaguecloser-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2427 2023-04-13 06:42:18.850026 leaguecloser-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1988 2023-04-13 06:31:14.000000 leaguecloser-1.0.3/README.md
+-rw-rw-rw-   0        0        0      712 2023-04-13 06:41:09.000000 leaguecloser-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:42:18.851027 leaguecloser-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.781971 leaguecloser-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.803308 leaguecloser-1.0.3/src/leaguecloser/
+-rw-rw-rw-   0        0        0      283 2023-04-13 03:02:26.000000 leaguecloser-1.0.3/src/leaguecloser/__init__.py
+-rw-rw-rw-   0        0        0    10786 2023-04-13 02:59:12.000000 leaguecloser-1.0.3/src/leaguecloser/computer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.782480 leaguecloser-1.0.3/src/leaguecloser/data/
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.841710 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/
+-rw-rw-rw-   0        0        0    10142 2023-04-13 02:12:05.000000 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/1681351869136.png
+-rw-rw-rw-   0        0        0     9375 2023-04-13 02:14:48.000000 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/1681352088077.png
+-rw-rw-rw-   0        0        0      115 2023-04-13 02:36:50.000000 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/close_league.py
+-rw-rw-rw-   0        0        0     1169 2023-04-13 04:45:18.000000 leaguecloser-1.0.3/src/leaguecloser/league.py
+-rw-rw-rw-   0        0        0     1067 2023-04-13 06:30:17.000000 leaguecloser-1.0.3/src/leaguecloser/sikuli.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.831585 leaguecloser-1.0.3/src/leaguecloser.egg-info/
+-rw-rw-rw-   0        0        0     2427 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.845746 leaguecloser-1.0.3/tests/
+-rw-rw-rw-   0        0        0      960 2023-04-13 03:13:42.000000 leaguecloser-1.0.3/tests/test_sequence.py
```

### Comparing `leaguecloser-1.0.2/LICENSE` & `leaguecloser-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.2/PKG-INFO` & `leaguecloser-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaguecloser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Mock package that auto-closes the League client
 Author: Giantpizzahead
 Project-URL: Homepage, https://github.com/Giantpizzahead/auto-league-closer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -65,9 +65,9 @@
 ```
 
 ## Development Setup
 
 First, setup a [virtual environment](https://kylefu.me/cheat_python/envanddeps.html). Then run:
 
 ```powershell
-> & '.\Dev Setup.ps1'
+> & '.\misc\Dev Setup.ps1'
 ```
```

### Comparing `leaguecloser-1.0.2/README.md` & `leaguecloser-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,9 +53,9 @@
 ```
 
 ## Development Setup
 
 First, setup a [virtual environment](https://kylefu.me/cheat_python/envanddeps.html). Then run:
 
 ```powershell
-> & '.\Dev Setup.ps1'
+> & '.\misc\Dev Setup.ps1'
 ```
```

### Comparing `leaguecloser-1.0.2/pyproject.toml` & `leaguecloser-1.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "leaguecloser"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Giantpizzahead" },
 ]
 description = "Mock package that auto-closes the League client"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -21,11 +21,14 @@
   "pyautogui",
   "pywin32",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Giantpizzahead/auto-league-closer"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.pytest.ini_options]
 addopts = [
   "--import-mode=importlib",
 ]
```

### Comparing `leaguecloser-1.0.2/src/leaguecloser/computer.py` & `leaguecloser-1.0.3/src/leaguecloser/computer.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.2/src/leaguecloser/league.py` & `leaguecloser-1.0.3/src/leaguecloser/league.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.2/src/leaguecloser/sikuli.py` & `leaguecloser-1.0.3/src/leaguecloser/sikuli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 """
 Runs SikuliX scripts from Python.
 """
 
 import os
+import requests
 import subprocess
 
 
 def run_sikuli_script(script_path):
     """Runs a SikuliX script from Python.
 
     Args:
         script_path (str): The path to the script to run.
 
     Returns:
         int: The exit code of the SikuliX script.
     """
+    # Check if Sikuli is installed
     sikuli_jar = os.path.join(os.path.dirname(__file__), "lib", "sikulixide-2.0.5.jar")
+    if not os.path.isfile(sikuli_jar):
+        # Create lib directory and download Sikuli
+        print("(First time running, downloading SikuliX... you better not queue...)")
+        os.makedirs(os.path.dirname(sikuli_jar), exist_ok=True)
+        url = "https://launchpad.net/sikuli/sikulix/2.0.5/+download/sikulixide-2.0.5.jar"
+        with open(sikuli_jar, "wb") as f:
+            f.write(requests.get(url).content)
+    
+    # Run Sikuli
     return subprocess.call(
         ["java", "-jar", sikuli_jar, "-r", script_path],
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
```

### Comparing `leaguecloser-1.0.2/src/leaguecloser.egg-info/PKG-INFO` & `leaguecloser-1.0.3/src/leaguecloser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaguecloser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Mock package that auto-closes the League client
 Author: Giantpizzahead
 Project-URL: Homepage, https://github.com/Giantpizzahead/auto-league-closer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -65,9 +65,9 @@
 ```
 
 ## Development Setup
 
 First, setup a [virtual environment](https://kylefu.me/cheat_python/envanddeps.html). Then run:
 
 ```powershell
-> & '.\Dev Setup.ps1'
+> & '.\misc\Dev Setup.ps1'
 ```
```

### Comparing `leaguecloser-1.0.2/tests/test_sequence.py` & `leaguecloser-1.0.3/tests/test_sequence.py`

 * *Files identical despite different names*

