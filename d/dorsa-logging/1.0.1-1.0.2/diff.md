# Comparing `tmp/dorsa_logging-1.0.1.tar.gz` & `tmp/dorsa_logging-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorsa_logging-1.0.1.tar", last modified: Thu Apr 13 10:58:44 2023, max compression
+gzip compressed data, was "dorsa_logging-1.0.2.tar", last modified: Thu Apr 13 11:14:18 2023, max compression
```

## Comparing `dorsa_logging-1.0.1.tar` & `dorsa_logging-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 10:58:44.483307 dorsa_logging-1.0.1/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_logging-1.0.1/LICENSE.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 10:58:44.483307 dorsa_logging-1.0.1/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1084 2023-04-13 08:42:14.000000 dorsa_logging-1.0.1/README.md
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 10:58:44.483307 dorsa_logging-1.0.1/dorsa_logging/
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)      584 2023-04-13 08:37:42.000000 dorsa_logging-1.0.1/dorsa_logging/__init__.py
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)     7223 2023-04-13 08:43:26.000000 dorsa_logging-1.0.1/dorsa_logging/logging_funcs.py
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 10:58:44.483307 dorsa_logging-1.0.1/dorsa_logging.egg-info/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 10:58:44.000000 dorsa_logging-1.0.1/dorsa_logging.egg-info/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      281 2023-04-13 10:58:44.000000 dorsa_logging-1.0.1/dorsa_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-13 10:58:44.000000 dorsa_logging-1.0.1/dorsa_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       23 2023-04-13 10:58:44.000000 dorsa_logging-1.0.1/dorsa_logging.egg-info/requires.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       14 2023-04-13 10:58:44.000000 dorsa_logging-1.0.1/dorsa_logging.egg-info/top_level.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-13 10:58:44.483307 dorsa_logging-1.0.1/setup.cfg
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1734 2023-04-13 10:55:36.000000 dorsa_logging-1.0.1/setup.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_logging-1.0.2/LICENSE.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1084 2023-04-13 08:42:14.000000 dorsa_logging-1.0.2/README.md
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/dorsa_logging/
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)      584 2023-04-13 08:37:42.000000 dorsa_logging-1.0.2/dorsa_logging/__init__.py
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)     7223 2023-04-13 08:43:26.000000 dorsa_logging-1.0.2/dorsa_logging/logging_funcs.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/dorsa_logging.egg-info/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1928 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      281 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/requires.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       14 2023-04-13 11:14:18.000000 dorsa_logging-1.0.2/dorsa_logging.egg-info/top_level.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-13 11:14:18.381307 dorsa_logging-1.0.2/setup.cfg
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1723 2023-04-13 11:13:14.000000 dorsa_logging-1.0.2/setup.py
```

### Comparing `dorsa_logging-1.0.1/LICENSE.txt` & `dorsa_logging-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.1/PKG-INFO` & `dorsa_logging-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorsa_logging
-Version: 1.0.1
+Version: 1.0.2
 Summary: Log application happenings
 Home-page: https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues
 Keywords: pypi,dorsa_logging
```

### Comparing `dorsa_logging-1.0.1/README.md` & `dorsa_logging-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.1/dorsa_logging/__init__.py` & `dorsa_logging-1.0.2/dorsa_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.1/dorsa_logging/logging_funcs.py` & `dorsa_logging-1.0.2/dorsa_logging/logging_funcs.py`

 * *Files identical despite different names*

### Comparing `dorsa_logging-1.0.1/dorsa_logging.egg-info/PKG-INFO` & `dorsa_logging-1.0.2/dorsa_logging.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorsa-logging
-Version: 1.0.1
+Version: 1.0.2
 Summary: Log application happenings
 Home-page: https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues
 Keywords: pypi,dorsa_logging
```

### Comparing `dorsa_logging-1.0.1/setup.py` & `dorsa_logging-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dorsa_logging',                           # should match the package folder
     packages=['dorsa_logging'],                     # should match the package folder
-    version='1.0.1',                                # important for updates
+    version='1.0.2',                                # important for updates
     license='Apache License 2.0',                                  # should match your chosen license
     description='Log application happenings',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Dorsa-co',
     author_email='info@dorsa-co.ir',
     url='https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging', 
     project_urls = {                                # Optional
         "Bug Tracker": "https://github.com/DORSA-co/modules/tree/main/Dorsa_Logging/issues"
     },
-    install_requires=['logging', 'dorsa_datetime'],                  # list all packages that your package uses
+    install_requires=['dorsa_datetime'],                  # list all packages that your package uses
     keywords=["pypi", "dorsa_logging"], # descriptive meta-data
     classifiers=[                                   # https://pypi.org/classifiers
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

