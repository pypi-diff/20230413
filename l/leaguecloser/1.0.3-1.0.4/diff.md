# Comparing `tmp/leaguecloser-1.0.3.tar.gz` & `tmp/leaguecloser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaguecloser-1.0.3.tar", last modified: Thu Apr 13 06:42:18 2023, max compression
+gzip compressed data, was "leaguecloser-1.0.4.tar", last modified: Thu Apr 13 07:02:30 2023, max compression
```

## Comparing `leaguecloser-1.0.3.tar` & `leaguecloser-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.850026 leaguecloser-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-04-13 01:51:56.000000 leaguecloser-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       53 2023-04-13 06:27:50.000000 leaguecloser-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2427 2023-04-13 06:42:18.850026 leaguecloser-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1988 2023-04-13 06:31:14.000000 leaguecloser-1.0.3/README.md
--rw-rw-rw-   0        0        0      712 2023-04-13 06:41:09.000000 leaguecloser-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 06:42:18.851027 leaguecloser-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.781971 leaguecloser-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.803308 leaguecloser-1.0.3/src/leaguecloser/
--rw-rw-rw-   0        0        0      283 2023-04-13 03:02:26.000000 leaguecloser-1.0.3/src/leaguecloser/__init__.py
--rw-rw-rw-   0        0        0    10786 2023-04-13 02:59:12.000000 leaguecloser-1.0.3/src/leaguecloser/computer.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.782480 leaguecloser-1.0.3/src/leaguecloser/data/
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.841710 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/
--rw-rw-rw-   0        0        0    10142 2023-04-13 02:12:05.000000 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/1681351869136.png
--rw-rw-rw-   0        0        0     9375 2023-04-13 02:14:48.000000 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/1681352088077.png
--rw-rw-rw-   0        0        0      115 2023-04-13 02:36:50.000000 leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/close_league.py
--rw-rw-rw-   0        0        0     1169 2023-04-13 04:45:18.000000 leaguecloser-1.0.3/src/leaguecloser/league.py
--rw-rw-rw-   0        0        0     1067 2023-04-13 06:30:17.000000 leaguecloser-1.0.3/src/leaguecloser/sikuli.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.831585 leaguecloser-1.0.3/src/leaguecloser.egg-info/
--rw-rw-rw-   0        0        0     2427 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 06:42:18.000000 leaguecloser-1.0.3/src/leaguecloser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 06:42:18.845746 leaguecloser-1.0.3/tests/
--rw-rw-rw-   0        0        0      960 2023-04-13 03:13:42.000000 leaguecloser-1.0.3/tests/test_sequence.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.418236 leaguecloser-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-13 01:51:56.000000 leaguecloser-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-04-13 06:27:50.000000 leaguecloser-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2427 2023-04-13 07:02:30.417233 leaguecloser-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1988 2023-04-13 06:31:14.000000 leaguecloser-1.0.4/README.md
+-rw-rw-rw-   0        0        0      727 2023-04-13 06:57:30.000000 leaguecloser-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 07:02:30.418236 leaguecloser-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.341591 leaguecloser-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.367406 leaguecloser-1.0.4/src/leaguecloser/
+-rw-rw-rw-   0        0        0      283 2023-04-13 03:02:26.000000 leaguecloser-1.0.4/src/leaguecloser/__init__.py
+-rw-rw-rw-   0        0        0    10786 2023-04-13 02:59:12.000000 leaguecloser-1.0.4/src/leaguecloser/computer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.342592 leaguecloser-1.0.4/src/leaguecloser/data/
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.409445 leaguecloser-1.0.4/src/leaguecloser/data/close_league.sikuli/
+-rw-rw-rw-   0        0        0    10142 2023-04-13 02:12:05.000000 leaguecloser-1.0.4/src/leaguecloser/data/close_league.sikuli/1681351869136.png
+-rw-rw-rw-   0        0        0     9375 2023-04-13 02:14:48.000000 leaguecloser-1.0.4/src/leaguecloser/data/close_league.sikuli/1681352088077.png
+-rw-rw-rw-   0        0        0      115 2023-04-13 02:36:50.000000 leaguecloser-1.0.4/src/leaguecloser/data/close_league.sikuli/close_league.py
+-rw-rw-rw-   0        0        0     1151 2023-04-13 07:01:27.000000 leaguecloser-1.0.4/src/leaguecloser/league.py
+-rw-rw-rw-   0        0        0     1301 2023-04-13 07:00:26.000000 leaguecloser-1.0.4/src/leaguecloser/sikuli.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.398299 leaguecloser-1.0.4/src/leaguecloser.egg-info/
+-rw-rw-rw-   0        0        0     2427 2023-04-13 07:02:30.000000 leaguecloser-1.0.4/src/leaguecloser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-04-13 07:02:30.000000 leaguecloser-1.0.4/src/leaguecloser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 07:02:30.000000 leaguecloser-1.0.4/src/leaguecloser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-13 07:02:30.000000 leaguecloser-1.0.4/src/leaguecloser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 07:02:30.000000 leaguecloser-1.0.4/src/leaguecloser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 07:02:30.414240 leaguecloser-1.0.4/tests/
+-rw-rw-rw-   0        0        0      960 2023-04-13 03:13:42.000000 leaguecloser-1.0.4/tests/test_sequence.py
```

### Comparing `leaguecloser-1.0.3/LICENSE` & `leaguecloser-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.3/PKG-INFO` & `leaguecloser-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaguecloser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Mock package that auto-closes the League client
 Author: Giantpizzahead
 Project-URL: Homepage, https://github.com/Giantpizzahead/auto-league-closer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `leaguecloser-1.0.3/README.md` & `leaguecloser-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.3/pyproject.toml` & `leaguecloser-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "leaguecloser"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Giantpizzahead" },
 ]
 description = "Mock package that auto-closes the League client"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -16,14 +16,15 @@
   "Operating System :: Microsoft :: Windows",
 ]
 
 dependencies = [
   "psutil",
   "pyautogui",
   "pywin32",
+  "requests",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Giantpizzahead/auto-league-closer"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `leaguecloser-1.0.3/src/leaguecloser/computer.py` & `leaguecloser-1.0.4/src/leaguecloser/computer.py`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/1681351869136.png` & `leaguecloser-1.0.4/src/leaguecloser/data/close_league.sikuli/1681351869136.png`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.3/src/leaguecloser/data/close_league.sikuli/1681352088077.png` & `leaguecloser-1.0.4/src/leaguecloser/data/close_league.sikuli/1681352088077.png`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.3/src/leaguecloser/league.py` & `leaguecloser-1.0.4/src/leaguecloser/league.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         bool: Whether the League client was closed.
     """
     # Try to focus the League window
     try:
         computer.focus_window("League of Legends")
     except Exception as e:
         print("Unable to focus the League window... just wait until it opens :)")
-        print(e)
         return False
     # Run the SikuliX script
     script_path = os.path.join(os.path.dirname(__file__), "data", "close_league.sikuli")
     exit_code = sikuli.run_sikuli_script(script_path)
     if exit_code != 0:
         print("SikuliX script failed to run... good luck queuing though :)")
         return False
```

### Comparing `leaguecloser-1.0.3/src/leaguecloser/sikuli.py` & `leaguecloser-1.0.4/src/leaguecloser/sikuli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 """
 Runs SikuliX scripts from Python.
 """
 
 import os
 import requests
 import subprocess
+import sys
+
+# Get SikuliX jar path depending on if we're frozen or not (PyInstaller)
+if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
+    SIKULI_JAR = os.path.join(os.getenv("PROGRAMDATA"), "Auto League Closer", "sikulixide-2.0.5.jar")
+else:
+    SIKULI_JAR = os.path.join(os.path.dirname(__file__), "lib", "sikulixide-2.0.5.jar")
+
+# Install SikuliX if needed
+if not os.path.isfile(SIKULI_JAR):
+    print("(First time setup, downloading SikuliX... you better not queue...)")
+    # Create directories if missing
+    os.makedirs(os.path.dirname(SIKULI_JAR), exist_ok=True)
+    # Download SikuliX
+    url = "https://launchpad.net/sikuli/sikulix/2.0.5/+download/sikulixide-2.0.5.jar"
+    with open(SIKULI_JAR, "wb") as f:
+        f.write(requests.get(url).content)
 
 
 def run_sikuli_script(script_path):
     """Runs a SikuliX script from Python.
 
     Args:
         script_path (str): The path to the script to run.
 
     Returns:
         int: The exit code of the SikuliX script.
     """
-    # Check if Sikuli is installed
-    sikuli_jar = os.path.join(os.path.dirname(__file__), "lib", "sikulixide-2.0.5.jar")
-    if not os.path.isfile(sikuli_jar):
-        # Create lib directory and download Sikuli
-        print("(First time running, downloading SikuliX... you better not queue...)")
-        os.makedirs(os.path.dirname(sikuli_jar), exist_ok=True)
-        url = "https://launchpad.net/sikuli/sikulix/2.0.5/+download/sikulixide-2.0.5.jar"
-        with open(sikuli_jar, "wb") as f:
-            f.write(requests.get(url).content)
-    
     # Run Sikuli
     return subprocess.call(
-        ["java", "-jar", sikuli_jar, "-r", script_path],
+        ["java", "-jar", SIKULI_JAR, "-r", script_path],
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
```

### Comparing `leaguecloser-1.0.3/src/leaguecloser.egg-info/PKG-INFO` & `leaguecloser-1.0.4/src/leaguecloser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaguecloser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Mock package that auto-closes the League client
 Author: Giantpizzahead
 Project-URL: Homepage, https://github.com/Giantpizzahead/auto-league-closer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `leaguecloser-1.0.3/src/leaguecloser.egg-info/SOURCES.txt` & `leaguecloser-1.0.4/src/leaguecloser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leaguecloser-1.0.3/tests/test_sequence.py` & `leaguecloser-1.0.4/tests/test_sequence.py`

 * *Files identical despite different names*

