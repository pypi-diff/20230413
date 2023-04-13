# Comparing `tmp/leaguecloser-1.0.0.tar.gz` & `tmp/leaguecloser-1.0.1.tar.gz`

## Comparing `leaguecloser-1.0.0.tar` & `leaguecloser-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/InitVenv.ps1
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/dev-requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/requirements.txt
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/app.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/__init__.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/computer.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/league.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/sikuli.py
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/close_league.sikuli/1681351869136.png
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/close_league.sikuli/1681352088077.png
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/src/leaguecloser/close_league.sikuli/close_league.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/tests/test_sequence.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/LICENSE
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 leaguecloser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/Dev Setup.ps1
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/Makefile
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/Auto League Closer.spec
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/InstallerSetupScript.iss
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/dev-requirements.txt
+-rw-r--r--   0        0        0    83012 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/icon.ico
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/misc/requirements.txt
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/app.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/__init__.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/computer.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/league.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/sikuli.py
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/1681351869136.png
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/1681352088077.png
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/close_league.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/tests/test_sequence.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 leaguecloser-1.0.1/PKG-INFO
```

### Comparing `leaguecloser-1.0.0/src/leaguecloser/computer.py` & `leaguecloser-1.0.1/src/leaguecloser/computer.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.0/src/leaguecloser/league.py` & `leaguecloser-1.0.1/src/leaguecloser/league.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     try:
         computer.focus_window("League of Legends")
     except Exception as e:
         print("Unable to focus the League window... just wait until it opens :)")
         print(e)
         return False
     # Run the SikuliX script
-    script_path = os.path.join(os.path.dirname(__file__), "close_league.sikuli")
+    script_path = os.path.join(os.path.dirname(__file__), "data", "close_league.sikuli")
     exit_code = sikuli.run_sikuli_script(script_path)
     if exit_code != 0:
         print("SikuliX script failed to run... good luck queuing though :)")
         return False
     return True
```

### Comparing `leaguecloser-1.0.0/src/leaguecloser/sikuli.py` & `leaguecloser-1.0.1/src/leaguecloser/sikuli.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.0/src/leaguecloser/close_league.sikuli/1681351869136.png` & `leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/1681351869136.png`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.0/src/leaguecloser/close_league.sikuli/1681352088077.png` & `leaguecloser-1.0.1/src/leaguecloser/data/close_league.sikuli/1681352088077.png`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.0/tests/test_sequence.py` & `leaguecloser-1.0.1/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.0/.gitignore` & `leaguecloser-1.0.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Source: https://github.com/github/gitignore/blob/main/Python.gitignore
 
+.vscode/
+
 # Mac
 .DS_Store
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `leaguecloser-1.0.0/LICENSE` & `leaguecloser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.0/pyproject.toml` & `leaguecloser-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "leaguecloser"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Giantpizzahead" },
 ]
 description = "Mock package that auto-closes the League client"
 readme = "README.md"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: Microsoft :: Windows",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: Microsoft :: Windows",
+]
+dependencies = [
+  "psutil",
+  "pyautogui",
+  "pywin32",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Giantpizzahead/auto-league-closer"
 
 [tool.pytest.ini_options]
 addopts = [
-    "--import-mode=importlib",
+  "--import-mode=importlib",
 ]
```

