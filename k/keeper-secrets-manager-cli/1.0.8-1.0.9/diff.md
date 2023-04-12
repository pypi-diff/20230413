# Comparing `tmp/keeper-secrets-manager-cli-1.0.8.tar.gz` & `tmp/keeper-secrets-manager-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-cli-1.0.8.tar", last modified: Fri Feb 25 17:21:20 2022, max compression
+gzip compressed data, was "keeper-secrets-manager-cli-1.0.9.tar", last modified: Sun Mar 27 19:55:51 2022, max compression
```

## Comparing `keeper-secrets-manager-cli-1.0.8.tar` & `keeper-secrets-manager-cli-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 17:21:20.061823 keeper-secrets-manager-cli-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-02-25 17:21:20.061823 keeper-secrets-manager-cli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 17:21:20.061823 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34797 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4327 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)    29699 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)     8188 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 17:21:20.061823 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-25 17:21:19.000000 keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-25 17:21:20.061823 keeper-secrets-manager-cli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-02-25 17:21:01.000000 keeper-secrets-manager-cli-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34797 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4327 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/exec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29699 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8188 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/table.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-03-27 19:55:50.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 19:55:50.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 19:55:50.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/setup.py
```

### Comparing `keeper-secrets-manager-cli-1.0.8/PKG-INFO` & `keeper-secrets-manager-cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command line tool for Keeper Secrets Manager
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: ops@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://app.gitbook.com/@keeper-security/s/secrets-manager/secrets-manager/secrets-manager-command-line-interface
```

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/__init__.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/__main__.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/common.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/common.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/export.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/export.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/init.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/init.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/profile.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/profile.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/secret.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/secret.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli/table.py` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/table.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/PKG-INFO` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command line tool for Keeper Secrets Manager
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: ops@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://app.gitbook.com/@keeper-security/s/secrets-manager/secrets-manager/secrets-manager-command-line-interface
```

### Comparing `keeper-secrets-manager-cli-1.0.8/keeper_secrets_manager_cli.egg-info/SOURCES.txt` & `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.0.8/setup.py` & `keeper-secrets-manager-cli-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'update-checker',
     'psutil'
 ]
 
 # Version set in the keeper_secrets_manager_cli.version file.
 setup(
     name="keeper-secrets-manager-cli",
-    version="1.0.8",
+    version="1.0.9",
     description="Command line tool for Keeper Secrets Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="ops@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

