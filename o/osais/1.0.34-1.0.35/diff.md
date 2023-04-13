# Comparing `tmp/osais-1.0.34.tar.gz` & `tmp/osais-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-qt1lhzrv\osais-1.0.34.tar", last modified: Thu Apr 13 18:55:33 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-or1g8c_1\osais-1.0.35.tar", last modified: Thu Apr 13 21:41:48 2023, max compression
```

## Comparing `osais-1.0.34.tar` & `osais-1.0.35.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:55:33.351486 osais-1.0.34/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.34/LICENSE
--rw-rw-rw-   0        0        0     1113 2023-04-13 18:55:33.350485 osais-1.0.34/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.34/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 18:55:33.346486 osais-1.0.34/osais/
--rw-rw-rw-   0        0        0      652 2023-04-13 18:54:40.000000 osais-1.0.34/osais/__init__.py
--rw-rw-rw-   0        0        0    41351 2023-04-13 18:54:47.000000 osais-1.0.34/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:55:33.349486 osais-1.0.34/osais.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-13 18:55:33.000000 osais-1.0.34/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-13 18:55:33.000000 osais-1.0.34/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:55:33.000000 osais-1.0.34/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-13 18:55:33.000000 osais-1.0.34/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 18:55:33.000000 osais-1.0.34/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.34/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 18:55:33.351486 osais-1.0.34/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-13 18:54:55.000000 osais-1.0.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:41:48.894348 osais-1.0.35/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.35/LICENSE
+-rw-rw-rw-   0        0        0     1113 2023-04-13 21:41:48.894348 osais-1.0.35/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.35/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 21:41:48.890349 osais-1.0.35/osais/
+-rw-rw-rw-   0        0        0      652 2023-04-13 21:41:22.000000 osais-1.0.35/osais/__init__.py
+-rw-rw-rw-   0        0        0    41405 2023-04-13 21:41:15.000000 osais-1.0.35/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-04-13 21:41:48.893350 osais-1.0.35/osais.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.35/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 21:41:48.894348 osais-1.0.35/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-04-13 21:41:28.000000 osais-1.0.35/setup.py
```

### Comparing `osais-1.0.34/LICENSE` & `osais-1.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.34/PKG-INFO` & `osais-1.0.35/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.34
+Version: 1.0.35
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.34/osais/__init__.py` & `osais-1.0.35/osais/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.34"
+__version__="1.0.35"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isLocal
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
```

### Comparing `osais-1.0.34/osais/osais.py` & `osais-1.0.35/osais/osais.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.34"
+__version__="1.0.35"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -1052,15 +1052,15 @@
             "token": CredParam["tokenAI"],
             "uid": str(MorphingParam["uid"]),
             "stage": str(StageParam["stage"]),
             "cycle": str(MorphingParam["cycle"]),
             "engine": CredParam["engine"],
             "username": CredParam["username"],
             "descr": StageParam["descr"],
-            "filename": _filename,
+            "filename": _filename
         }
     }
 
     if "cost" in StageParam:
         objParam["response"]["cost"]= str(StageParam["cost"])
     
     response = requests.post(api_url, headers=headers, data=json.dumps(objParam) )
@@ -1136,14 +1136,15 @@
 
     ## from env, load AI config
     gConfig=osais_loadConfig(gName)
     gPortAI = gConfig["port"]
     gVersion = gConfig["version"]
 
     print("\r\n===== Config =====")
+    print("engine: "+str(gName) + " v"+str(gVersion))
     print("is Local: "+str(gIsLocal))
     print("is Virtual: "+str(gIsVirtualAI))
     print("owned by client: "+str(gUsername))
     print("===== /Config =====\r\n")
 
     ## make sure we have a config file
     _loadConfig(gName)
```

### Comparing `osais-1.0.34/osais.egg-info/PKG-INFO` & `osais-1.0.35/osais.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.34
+Version: 1.0.35
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.34/setup.py` & `osais-1.0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.34',
+    version='1.0.35',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

