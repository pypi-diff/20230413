# Comparing `tmp/ExoPSI-1.0.0.tar.gz` & `tmp/ExoPSI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExoPSI-1.0.0.tar", last modified: Sat Apr  8 05:53:06 2023, max compression
+gzip compressed data, was "ExoPSI-1.0.1.tar", last modified: Thu Apr 13 17:37:49 2023, max compression
```

## Comparing `ExoPSI-1.0.0.tar` & `ExoPSI-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:06.581290 ExoPSI-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:06.565669 ExoPSI-1.0.0/ExoPSI/
--rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.0/ExoPSI/__init__.py
--rw-rw-rw-   0        0        0     7980 2023-03-06 03:18:59.000000 ExoPSI-1.0.0/ExoPSI/exopsi.py
--rw-rw-rw-   0        0        0     1872 2023-03-21 17:45:32.000000 ExoPSI-1.0.0/ExoPSI/subfunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-08 05:53:06.581290 ExoPSI-1.0.0/ExoPSI.egg-info/
--rw-rw-rw-   0        0        0      793 2023-04-08 05:53:06.000000 ExoPSI-1.0.0/ExoPSI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-08 05:53:06.000000 ExoPSI-1.0.0/ExoPSI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 05:53:06.000000 ExoPSI-1.0.0/ExoPSI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-08 05:53:06.000000 ExoPSI-1.0.0/ExoPSI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-08 05:53:06.000000 ExoPSI-1.0.0/ExoPSI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      793 2023-04-08 05:53:06.581290 ExoPSI-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-02-25 08:19:59.000000 ExoPSI-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 05:53:06.581290 ExoPSI-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1410 2023-04-08 05:52:14.000000 ExoPSI-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:37:49.348549 ExoPSI-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:37:49.317146 ExoPSI-1.0.1/ExoPSI/
+-rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.1/ExoPSI/__init__.py
+-rw-rw-rw-   0        0        0     7980 2023-03-06 03:18:59.000000 ExoPSI-1.0.1/ExoPSI/exopsi.py
+-rw-rw-rw-   0        0        0     1872 2023-03-21 17:45:32.000000 ExoPSI-1.0.1/ExoPSI/subfunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:37:49.337540 ExoPSI-1.0.1/ExoPSI.egg-info/
+-rw-rw-rw-   0        0        0     6734 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-13 17:37:49.000000 ExoPSI-1.0.1/ExoPSI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6734 2023-04-13 17:37:49.337540 ExoPSI-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:37:49.348549 ExoPSI-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1417 2023-04-13 17:28:56.000000 ExoPSI-1.0.1/setup.py
```

### Comparing `ExoPSI-1.0.0/ExoPSI/exopsi.py` & `ExoPSI-1.0.1/ExoPSI/exopsi.py`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.0/ExoPSI/subfunctions.py` & `ExoPSI-1.0.1/ExoPSI/subfunctions.py`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.0/LICENSE` & `ExoPSI-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.0/setup.py` & `ExoPSI-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ExoPSI",
-    version="1.0.0",
-    description="Library to calculate Similarity Indexes",
+    version="1.0.1",
+    description="Library to calculate Planet Similarity Indexes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ExoPSI/ExoPSI",
     author=["Aditya Rai","Vaibhav Garg"],
     author_email="rai.aditya01@gmail.com",
     license="GNU GPL v3.0", 
     classifiers=[
```

