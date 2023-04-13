# Comparing `tmp/Codelock-2.1.0.tar.gz` & `tmp/Codelock-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Codelock-2.1.0.tar", last modified: Thu Mar 30 17:48:19 2023, max compression
+gzip compressed data, was "Codelock-2.1.1.tar", last modified: Thu Apr 13 14:31:28 2023, max compression
```

## Comparing `Codelock-2.1.0.tar` & `Codelock-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 17:48:19.099053 Codelock-2.1.0/
--rw-rw-rw-   0        0        0       29 2023-03-30 17:30:11.000000 Codelock-2.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      658 2023-03-30 17:48:19.099053 Codelock-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-03-30 17:30:11.000000 Codelock-2.1.0/README.md
--rw-rw-rw-   0        0        0      157 2023-03-30 17:48:19.101055 Codelock-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-03-30 17:48:13.000000 Codelock-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 17:48:19.080052 Codelock-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-30 17:48:19.096055 Codelock-2.1.0/src/Codelock.egg-info/
--rw-rw-rw-   0        0        0      658 2023-03-30 17:48:19.000000 Codelock-2.1.0/src/Codelock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-03-30 17:48:19.000000 Codelock-2.1.0/src/Codelock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 17:48:19.000000 Codelock-2.1.0/src/Codelock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-03-30 17:48:19.000000 Codelock-2.1.0/src/Codelock.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2023-03-30 17:48:19.000000 Codelock-2.1.0/src/Codelock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-30 17:48:19.000000 Codelock-2.1.0/src/Codelock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 17:48:19.098054 Codelock-2.1.0/src/codelock/
--rw-rw-rw-   0        0        0       43 2023-03-30 17:30:11.000000 Codelock-2.1.0/src/codelock/__init__.py
--rw-rw-rw-   0        0        0    14286 2023-03-30 17:47:51.000000 Codelock-2.1.0/src/codelock/cdcli.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:28.109900 Codelock-2.1.1/
+-rw-rw-rw-   0        0        0       29 2023-04-13 14:19:38.000000 Codelock-2.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      571 2023-04-13 14:31:28.109900 Codelock-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-13 14:19:38.000000 Codelock-2.1.1/README.md
+-rw-rw-rw-   0        0        0      157 2023-04-13 14:31:28.113904 Codelock-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2973 2023-04-13 14:31:00.000000 Codelock-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:28.079873 Codelock-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:28.106897 Codelock-2.1.1/src/Codelock.egg-info/
+-rw-rw-rw-   0        0        0      571 2023-04-13 14:31:27.000000 Codelock-2.1.1/src/Codelock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-04-13 14:31:27.000000 Codelock-2.1.1/src/Codelock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:31:27.000000 Codelock-2.1.1/src/Codelock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:31:27.000000 Codelock-2.1.1/src/Codelock.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       46 2023-04-13 14:31:27.000000 Codelock-2.1.1/src/Codelock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 14:31:27.000000 Codelock-2.1.1/src/Codelock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 14:31:28.108899 Codelock-2.1.1/src/codelock/
+-rw-rw-rw-   0        0        0       43 2023-04-13 14:19:38.000000 Codelock-2.1.1/src/codelock/__init__.py
+-rw-rw-rw-   0        0        0    14294 2023-04-13 14:27:45.000000 Codelock-2.1.1/src/codelock/cdcli.py
```

### Comparing `Codelock-2.1.0/PKG-INFO` & `Codelock-2.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: Codelock
-Version: 2.1.0
-Summary: CodeLock Official CLI for the development environment
-Home-page: UNKNOWN
+Version: 2.1.1
+Summary: A cli for codelock
 Author: Codelock
 License: MIT
 Keywords: codelock,cli
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `Codelock-2.1.0/setup.py` & `Codelock-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     #     packagesToInstall.append("python3-tk")
 
 if os.name == "nt":
     packagesToInstall.append("tk")
 
 setup(
     name="Codelock",
-    version="2.1.0",
-    description="CodeLock Official CLI for the development environment",
+    version="2.1.1",
+    description="A cli for codelock",
     author="Codelock",
     license="MIT",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
```

### Comparing `Codelock-2.1.0/src/Codelock.egg-info/PKG-INFO` & `Codelock-2.1.1/src/Codelock.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: Codelock
-Version: 2.1.0
-Summary: CodeLock Official CLI for the development environment
-Home-page: UNKNOWN
+Version: 2.1.1
+Summary: A cli for codelock
 Author: Codelock
 License: MIT
 Keywords: codelock,cli
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `Codelock-2.1.0/src/codelock/cdcli.py` & `Codelock-2.1.1/src/codelock/cdcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
                     option = int(input("Select the repo: "))
 
                 commitMsg = input("Please enter commit message: ")
                 # print("Selected option: ",
                 #       repos[option]["listener_branch"], repos[option]["_id"])
                 # print("Commit message: ", commitMsg)
 
-                exculde_array = ["*.zip", "code_zip"]
+                exculde_array = ["*.zip", "code_zip", ".git"]
                 if os.path.exists(".gitignore"):
                     for line in open(".gitignore"):
                         li = line.strip()
                         if not li.startswith("#"):
                             exline = self.splitme(line.strip())
                             if exline != "":
                                 exculde_array.append(exline)
```

