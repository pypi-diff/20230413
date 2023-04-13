# Comparing `tmp/dorsa_logging-1.0.2.tar.gz` & `tmp/dorsa_logging-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorsa_logging-1.0.2.tar", last modified: Thu Apr 13 11:14:18 2023, max compression
+gzip compressed data, was "dorsa_logging-1.0.3.tar", last modified: Thu Apr 13 11:17:53 2023, max compression
```

## Comparing `dorsa_logging-1.0.2.tar` & `dorsa_logging-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_logging-1.0.2/LICENSE.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1084 2023-04-13 08:42:14.000000 dorsa_logging-1.0.2/README.md
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/dorsa_logging/
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)      584 2023-04-13 08:37:42.000000 dorsa_logging-1.0.2/dorsa_logging/__init__.py
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)     7223 2023-04-13 08:43:26.000000 dorsa_logging-1.0.2/dorsa_logging/logging_funcs.py
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/dorsa_logging.egg-info/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      281 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/requires.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       14 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/top_level.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/setup.cfg
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1723 2023-04-13 11:13:14.000000 dorsa_logging-1.0.2/setup.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_logging-1.0.3/LICENSE.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1084 2023-04-13 08:42:14.000000 dorsa_logging-1.0.3/README.md
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/dorsa_logging/
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)       39 2023-04-13 11:16:22.000000 dorsa_logging-1.0.3/dorsa_logging/__init__.py
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)     7223 2023-04-13 08:43:26.000000 dorsa_logging-1.0.3/dorsa_logging/logging_funcs.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/dorsa_logging.egg-info/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      281 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/requires.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       14 2023-04-13 11:17:53.000000 dorsa_logging-1.0.3/dorsa_logging.egg-info/top_level.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-13 11:17:53.451786 dorsa_logging-1.0.3/setup.cfg
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1723 2023-04-13 11:17:30.000000 dorsa_logging-1.0.3/setup.py
```

### Comparing `dorsa_logging-1.0.2/LICENSE.txt` & `dorsa_logging-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.2/PKG-INFO` & `dorsa_logging-1.0.3/dorsa_logging.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dorsa_logging
-Version: 1.0.2
+Name: dorsa-logging
+Version: 1.0.3
 Summary: Log application happenings
 Home-page: https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues
 Keywords: pypi,dorsa_logging
```

### Comparing `dorsa_logging-1.0.2/README.md` & `dorsa_logging-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.2/dorsa_logging/logging_funcs.py` & `dorsa_logging-1.0.3/dorsa_logging/logging_funcs.py`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.2/dorsa_logging.egg-info/PKG-INFO` & `dorsa_logging-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dorsa-logging
-Version: 1.0.2
+Name: dorsa_logging
+Version: 1.0.3
 Summary: Log application happenings
 Home-page: https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues
 Keywords: pypi,dorsa_logging
```

### Comparing `dorsa_logging-1.0.2/setup.py` & `dorsa_logging-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dorsa_logging',                           # should match the package folder
     packages=['dorsa_logging'],                     # should match the package folder
-    version='1.0.2',                                # important for updates
+    version='1.0.3',                                # important for updates
     license='Apache License 2.0',                                  # should match your chosen license
     description='Log application happenings',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Dorsa-co',
     author_email='info@dorsa-co.ir',
     url='https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging',
```

