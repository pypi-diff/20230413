# Comparing `tmp/pyoomysql-0.2.3.tar.gz` & `tmp/pyoomysql-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoomysql-0.2.3.tar", last modified: Tue Oct 25 15:34:14 2022, max compression
+gzip compressed data, was "pyoomysql-0.2.4.tar", last modified: Thu Apr 13 17:07:49 2023, max compression
```

## Comparing `pyoomysql-0.2.3.tar` & `pyoomysql-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:34:14.027040 pyoomysql-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-10-25 15:34:14.027040 pyoomysql-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6092 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:34:14.023040 pyoomysql-0.2.3/pyoomysql/
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/Column.py
--rw-r--r--   0 runner    (1001) docker     (121)    14181 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/Database.py
--rw-r--r--   0 runner    (1001) docker     (121)    12405 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/Schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    24810 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/Table.py
--rw-r--r--   0 runner    (1001) docker     (121)    18668 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/User.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:34:14.023040 pyoomysql-0.2.3/pyoomysql/util/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/util/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/pyoomysql/util/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:34:14.023040 pyoomysql-0.2.3/pyoomysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-10-25 15:34:13.000000 pyoomysql-0.2.3/pyoomysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-10-25 15:34:13.000000 pyoomysql-0.2.3/pyoomysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 15:34:13.000000 pyoomysql-0.2.3/pyoomysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-25 15:34:13.000000 pyoomysql-0.2.3/pyoomysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-25 15:34:13.000000 pyoomysql-0.2.3/pyoomysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 15:34:14.027040 pyoomysql-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 15:34:14.027040 pyoomysql-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-10-25 15:34:06.000000 pyoomysql-0.2.3/tests/simple_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:07:49.981826 pyoomysql-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6355 2023-04-13 17:07:49.980826 pyoomysql-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6092 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:07:49.977825 pyoomysql-0.2.4/pyoomysql/
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)    14329 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/Database.py
+-rw-rw-rw-   0 root         (0) root         (0)    12405 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    24810 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/Table.py
+-rw-rw-rw-   0 root         (0) root         (0)    18668 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/User.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:07:49.979826 pyoomysql-0.2.4/pyoomysql/util/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/util/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/pyoomysql/util/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:07:49.978826 pyoomysql-0.2.4/pyoomysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6355 2023-04-13 17:07:49.000000 pyoomysql-0.2.4/pyoomysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      424 2023-04-13 17:07:49.000000 pyoomysql-0.2.4/pyoomysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 17:07:49.000000 pyoomysql-0.2.4/pyoomysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 17:07:49.000000 pyoomysql-0.2.4/pyoomysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-13 17:07:49.000000 pyoomysql-0.2.4/pyoomysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 17:07:49.981826 pyoomysql-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:07:49.980826 pyoomysql-0.2.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-13 17:07:27.000000 pyoomysql-0.2.4/tests/simple_script.py
```

### Comparing `pyoomysql-0.2.3/LICENSE` & `pyoomysql-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/PKG-INFO` & `pyoomysql-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyoomysql
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Object-Orinted MySQL interface
-Home-page: https://github.com/Silvarion/pyoomysql
+Home-page: https://gitlab.com/jsanchezd/pyoomysql
 Author: Jesus Alejandro Sanchez Davila
 Author-email: jsanchez.consultant@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -247,7 +249,9 @@
         name = "some_nice_username",
         host = "% or host to connect from",
         password = "very_long_and_strong_password"
     )
 
     # Create the user in the database
     myuser.create()
+
+
```

### Comparing `pyoomysql-0.2.3/README.md` & `pyoomysql-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/pyoomysql/Column.py` & `pyoomysql-0.2.4/pyoomysql/Column.py`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/pyoomysql/Database.py` & `pyoomysql-0.2.4/pyoomysql/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 # Database class
 class Database:
     # Attributes
     connection = None
 
     # Creator
     def __init__(self, hostname, port=3306, schema='information_schema'):
-        self.hostname = hostname
-        self.port = port
-        self.schema = schema
-        self.auth_plugin = None
+        self.auth_plugin    = None
+        self.connection     = None
+        self.hostname       = hostname
+        self.port           = port
+        self.schema         = schema
+        self.version        = None
         logger.setLevel(logging.INFO)
 
     # Python Object overrides
     def __str__(self):
         return json.dumps({
             "hostname": self.hostname,
             "port": self.port,
@@ -295,16 +297,17 @@
         self.execute(command=f"SET GLOBAL SQL_SLAVE_SKIP_COUNTER = {amount}")
         logger.info("Starting replication process again...")
         self.start_replica()
         logger.info("All done.")
 
     # Check if there's an active connection to the database
     def is_connected(self):
-        if self.connection.is_connected():
-            return True
+        if self.connection is not None:
+            if self.connection.is_connected():
+                return True
         else:
             return False
 
     # Global Variables
     def get_global_variable(self, variable_name):
         return self.execute(command=f"SELECT variable_name, variable_value FROM information_schema.global_variables WHERE variable_name = '{variable_name}'")["rows"][0]
```

### Comparing `pyoomysql-0.2.3/pyoomysql/Schema.py` & `pyoomysql-0.2.4/pyoomysql/Schema.py`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/pyoomysql/Table.py` & `pyoomysql-0.2.4/pyoomysql/Table.py`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/pyoomysql/User.py` & `pyoomysql-0.2.4/pyoomysql/User.py`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/pyoomysql/util/sql.py` & `pyoomysql-0.2.4/pyoomysql/util/sql.py`

 * *Files identical despite different names*

### Comparing `pyoomysql-0.2.3/pyoomysql.egg-info/PKG-INFO` & `pyoomysql-0.2.4/pyoomysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pyoomysql
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Object-Orinted MySQL interface
-Home-page: https://github.com/Silvarion/pyoomysql
+Home-page: https://gitlab.com/jsanchezd/pyoomysql
 Author: Jesus Alejandro Sanchez Davila
 Author-email: jsanchez.consultant@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -247,7 +249,9 @@
         name = "some_nice_username",
         host = "% or host to connect from",
         password = "very_long_and_strong_password"
     )
 
     # Create the user in the database
     myuser.create()
+
+
```

### Comparing `pyoomysql-0.2.3/setup.py` & `pyoomysql-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyoomysql",
-    version="0.2.3",
+    version="0.2.4",
     author="Jesus Alejandro Sanchez Davila",
     author_email="jsanchez.consultant@gmail.com",
     description="Python Object-Orinted MySQL interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Silvarion/pyoomysql",
+    url="https://gitlab.com/jsanchezd/pyoomysql",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

### Comparing `pyoomysql-0.2.3/tests/simple_script.py` & `pyoomysql-0.2.4/tests/simple_script.py`

 * *Files identical despite different names*

