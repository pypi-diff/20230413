# Comparing `tmp/maxdmg_back-0.0.4.tar.gz` & `tmp/maxdmg_back-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxdmg_back-0.0.4.tar", last modified: Thu Mar 30 18:35:04 2023, max compression
+gzip compressed data, was "maxdmg_back-0.0.5.tar", last modified: Thu Apr 13 12:06:14 2023, max compression
```

## Comparing `maxdmg_back-0.0.4.tar` & `maxdmg_back-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.599902 maxdmg_back-0.0.4/
--rw-r--r--   0 at        (1000) at        (1000)      332 2023-03-30 18:35:04.599902 maxdmg_back-0.0.4/PKG-INFO
--rw-r--r--   0 at        (1000) at        (1000)        0 2023-03-21 18:15:24.000000 maxdmg_back-0.0.4/README.md
--rw-r--r--   0 at        (1000) at        (1000)      458 2023-03-30 18:34:26.000000 maxdmg_back-0.0.4/pyproject.toml
--rw-r--r--   0 at        (1000) at        (1000)       38 2023-03-30 18:35:04.599902 maxdmg_back-0.0.4/setup.cfg
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.549902 maxdmg_back-0.0.4/src/
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.549902 maxdmg_back-0.0.4/src/maxdmg_back/
--rw-r--r--   0 at        (1000) at        (1000)      124 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/__init__.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.586569 maxdmg_back-0.0.4/src/maxdmg_back/app/
--rw-r--r--   0 at        (1000) at        (1000)      268 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/API.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.586569 maxdmg_back-0.0.4/src/maxdmg_back/app/APIs/
--rw-r--r--   0 at        (1000) at        (1000)     1058 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/APIs/Messages.py
--rw-r--r--   0 at        (1000) at        (1000)     2496 2023-03-30 18:34:10.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/APIs/MonoAPI.py
--rw-r--r--   0 at        (1000) at        (1000)       36 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/APIs/__init__.py
--rw-r--r--   0 at        (1000) at        (1000)     1511 2023-03-21 18:24:14.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Assembly.py
--rw-r--r--   0 at        (1000) at        (1000)     2930 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Exceptions.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.589902 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/
--rw-r--r--   0 at        (1000) at        (1000)      632 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/APIFactory.py
--rw-r--r--   0 at        (1000) at        (1000)      383 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/ActiveUsersFactory.py
--rw-r--r--   0 at        (1000) at        (1000)     1281 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/FormElemFactory.py
--rw-r--r--   0 at        (1000) at        (1000)     2531 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/FormFactory.py
--rw-r--r--   0 at        (1000) at        (1000)     2527 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/StorageFactory.py
--rw-r--r--   0 at        (1000) at        (1000)      258 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/__init__.py
--rw-r--r--   0 at        (1000) at        (1000)     3659 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Form.py
--rw-r--r--   0 at        (1000) at        (1000)     5256 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/FormElems.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.593236 maxdmg_back-0.0.4/src/maxdmg_back/app/Interface/
--rw-r--r--   0 at        (1000) at        (1000)      199 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Interface/Form.py
--rw-r--r--   0 at        (1000) at        (1000)     2156 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Interface/FormElem.py
--rw-r--r--   0 at        (1000) at        (1000)       33 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Interface/__init__.py
--rw-r--r--   0 at        (1000) at        (1000)     2644 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/StateHistory.py
--rw-r--r--   0 at        (1000) at        (1000)     1697 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/StateMachine.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.596569 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/
--rw-r--r--   0 at        (1000) at        (1000)     1282 2023-03-30 12:30:07.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/ActiveUsers.py
--rw-r--r--   0 at        (1000) at        (1000)     1759 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/Context.py
--rw-r--r--   0 at        (1000) at        (1000)     1282 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/Models.py
--rw-r--r--   0 at        (1000) at        (1000)     3605 2023-03-30 12:30:07.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/Storage.py
--rw-r--r--   0 at        (1000) at        (1000)      539 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/StorageInterface.py
--rw-r--r--   0 at        (1000) at        (1000)      208 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/__init__.py
--rw-r--r--   0 at        (1000) at        (1000)     1076 2023-03-21 18:15:41.000000 maxdmg_back-0.0.4/src/maxdmg_back/app/Types.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-30 18:35:04.566569 maxdmg_back-0.0.4/src/maxdmg_back.egg-info/
--rw-r--r--   0 at        (1000) at        (1000)      332 2023-03-30 18:35:04.000000 maxdmg_back-0.0.4/src/maxdmg_back.egg-info/PKG-INFO
--rw-r--r--   0 at        (1000) at        (1000)     1222 2023-03-30 18:35:04.000000 maxdmg_back-0.0.4/src/maxdmg_back.egg-info/SOURCES.txt
--rw-r--r--   0 at        (1000) at        (1000)        1 2023-03-30 18:35:04.000000 maxdmg_back-0.0.4/src/maxdmg_back.egg-info/dependency_links.txt
--rw-r--r--   0 at        (1000) at        (1000)       12 2023-03-30 18:35:04.000000 maxdmg_back-0.0.4/src/maxdmg_back.egg-info/top_level.txt
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.825223 maxdmg_back-0.0.5/
+-rw-r--r--   0 at        (1000) at        (1000)      332 2023-04-13 12:06:14.825223 maxdmg_back-0.0.5/PKG-INFO
+-rw-r--r--   0 at        (1000) at        (1000)        0 2023-03-21 18:15:24.000000 maxdmg_back-0.0.5/README.md
+-rw-r--r--   0 at        (1000) at        (1000)      458 2023-04-13 12:05:09.000000 maxdmg_back-0.0.5/pyproject.toml
+-rw-r--r--   0 at        (1000) at        (1000)       38 2023-04-13 12:06:14.825223 maxdmg_back-0.0.5/setup.cfg
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.755223 maxdmg_back-0.0.5/src/
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.755223 maxdmg_back-0.0.5/src/maxdmg_back/
+-rw-r--r--   0 at        (1000) at        (1000)      306 2023-04-13 12:05:56.000000 maxdmg_back-0.0.5/src/maxdmg_back/__init__.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.805223 maxdmg_back-0.0.5/src/maxdmg_back/app/
+-rw-r--r--   0 at        (1000) at        (1000)      268 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/API.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.808556 maxdmg_back-0.0.5/src/maxdmg_back/app/APIs/
+-rw-r--r--   0 at        (1000) at        (1000)     1058 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/APIs/Messages.py
+-rw-r--r--   0 at        (1000) at        (1000)     2496 2023-03-30 18:34:10.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/APIs/MonoAPI.py
+-rw-r--r--   0 at        (1000) at        (1000)       36 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/APIs/__init__.py
+-rw-r--r--   0 at        (1000) at        (1000)     1511 2023-03-21 18:24:14.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Assembly.py
+-rw-r--r--   0 at        (1000) at        (1000)     3413 2023-04-13 12:05:56.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Errors.py
+-rw-r--r--   0 at        (1000) at        (1000)     3319 2023-04-13 12:05:56.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Exceptions.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.811890 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/
+-rw-r--r--   0 at        (1000) at        (1000)      632 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/APIFactory.py
+-rw-r--r--   0 at        (1000) at        (1000)      383 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/ActiveUsersFactory.py
+-rw-r--r--   0 at        (1000) at        (1000)     1281 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/FormElemFactory.py
+-rw-r--r--   0 at        (1000) at        (1000)     2531 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/FormFactory.py
+-rw-r--r--   0 at        (1000) at        (1000)     2527 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/StorageFactory.py
+-rw-r--r--   0 at        (1000) at        (1000)      258 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/__init__.py
+-rw-r--r--   0 at        (1000) at        (1000)     3659 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Form.py
+-rw-r--r--   0 at        (1000) at        (1000)     5256 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/FormElems.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.815223 maxdmg_back-0.0.5/src/maxdmg_back/app/Interface/
+-rw-r--r--   0 at        (1000) at        (1000)      199 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Interface/Form.py
+-rw-r--r--   0 at        (1000) at        (1000)     2156 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Interface/FormElem.py
+-rw-r--r--   0 at        (1000) at        (1000)       33 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Interface/__init__.py
+-rw-r--r--   0 at        (1000) at        (1000)     2644 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/StateHistory.py
+-rw-r--r--   0 at        (1000) at        (1000)     1697 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/StateMachine.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.821889 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/
+-rw-r--r--   0 at        (1000) at        (1000)     1282 2023-03-30 12:30:07.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/ActiveUsers.py
+-rw-r--r--   0 at        (1000) at        (1000)     1759 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/Context.py
+-rw-r--r--   0 at        (1000) at        (1000)     1282 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/Models.py
+-rw-r--r--   0 at        (1000) at        (1000)     3605 2023-03-30 12:30:07.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/Storage.py
+-rw-r--r--   0 at        (1000) at        (1000)      539 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/StorageInterface.py
+-rw-r--r--   0 at        (1000) at        (1000)      208 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/__init__.py
+-rw-r--r--   0 at        (1000) at        (1000)     1076 2023-03-21 18:15:41.000000 maxdmg_back-0.0.5/src/maxdmg_back/app/Types.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 12:06:14.758556 maxdmg_back-0.0.5/src/maxdmg_back.egg-info/
+-rw-r--r--   0 at        (1000) at        (1000)      332 2023-04-13 12:06:14.000000 maxdmg_back-0.0.5/src/maxdmg_back.egg-info/PKG-INFO
+-rw-r--r--   0 at        (1000) at        (1000)     1252 2023-04-13 12:06:14.000000 maxdmg_back-0.0.5/src/maxdmg_back.egg-info/SOURCES.txt
+-rw-r--r--   0 at        (1000) at        (1000)        1 2023-04-13 12:06:14.000000 maxdmg_back-0.0.5/src/maxdmg_back.egg-info/dependency_links.txt
+-rw-r--r--   0 at        (1000) at        (1000)       12 2023-04-13 12:06:14.000000 maxdmg_back-0.0.5/src/maxdmg_back.egg-info/top_level.txt
```

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/APIs/Messages.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/APIs/Messages.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/APIs/MonoAPI.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/APIs/MonoAPI.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Assembly.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Assembly.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Exceptions.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,7 +103,21 @@
         return (FormElemSwitchedHistory, (self.message, self.name))
 
 
 # ==== Messaging Exceptions
 class UserDone(Exception):
     pass
 
+
+# ==== maxdmg-resource Exceptions
+
+class MaxDmgResourceErrors(Exception):
+    def __init__(self, errors):
+        self.message = 'Errors occured in maxdmg-resource: '
+        self.errors  = errors
+
+        super(MaxDmgResourceErrors, self).__init__( 
+            (self.message, self.errors) )
+
+    def __reduce__(self):
+        return (MaxDmgResourceErrors, (self.message, self.errors))
+
```

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/APIFactory.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/APIFactory.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/FormElemFactory.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/FormElemFactory.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/FormFactory.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/FormFactory.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Factories/StorageFactory.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Factories/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Form.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Form.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/FormElems.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/FormElems.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Interface/FormElem.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Interface/FormElem.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/StateHistory.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/StateHistory.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/StateMachine.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/StateMachine.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/ActiveUsers.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/ActiveUsers.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/Context.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/Context.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/Models.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/Models.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/Storage.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/Storage.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Storage/StorageInterface.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back/app/Types.py` & `maxdmg_back-0.0.5/src/maxdmg_back/app/Types.py`

 * *Files identical despite different names*

### Comparing `maxdmg_back-0.0.4/src/maxdmg_back.egg-info/SOURCES.txt` & `maxdmg_back-0.0.5/src/maxdmg_back.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/maxdmg_back/__init__.py
 src/maxdmg_back.egg-info/PKG-INFO
 src/maxdmg_back.egg-info/SOURCES.txt
 src/maxdmg_back.egg-info/dependency_links.txt
 src/maxdmg_back.egg-info/top_level.txt
 src/maxdmg_back/app/API.py
 src/maxdmg_back/app/Assembly.py
+src/maxdmg_back/app/Errors.py
 src/maxdmg_back/app/Exceptions.py
 src/maxdmg_back/app/Form.py
 src/maxdmg_back/app/FormElems.py
 src/maxdmg_back/app/StateHistory.py
 src/maxdmg_back/app/StateMachine.py
 src/maxdmg_back/app/Types.py
 src/maxdmg_back/app/APIs/Messages.py
```

