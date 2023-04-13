# Comparing `tmp/python-eigen-ingenuity-0.4.4.tar.gz` & `tmp/python-eigen-ingenuity-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.4.tar", last modified: Thu Apr  6 15:04:00 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.5.tar", last modified: Thu Apr 13 16:19:21 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.4.tar` & `python-eigen-ingenuity-0.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-06 15:04:00.766403 python-eigen-ingenuity-0.4.4/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.4/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.4/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-04-06 15:04:00.766157 python-eigen-ingenuity-0.4.4/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.4/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-06 15:04:00.763942 python-eigen-ingenuity-0.4.4/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    15868 2023-04-05 14:48:43.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-06 15:04:00.764702 python-eigen-ingenuity-0.4.4/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6133 2023-04-05 13:42:19.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3040 2023-04-06 10:18:06.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36189 2023-04-06 11:02:05.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2829 2023-03-08 14:18:40.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4067 2022-12-01 09:50:12.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    11778 2022-12-15 11:39:53.000000 python-eigen-ingenuity-0.4.4/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.4/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-06 15:04:00.765822 python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-04-06 15:04:00.000000 python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-04-06 15:04:00.000000 python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-04-06 15:04:00.000000 python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       24 2023-04-06 15:04:00.000000 python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-04-06 15:04:00.000000 python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-04-06 15:04:00.766459 python-eigen-ingenuity-0.4.4/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      689 2023-04-04 15:23:03.000000 python-eigen-ingenuity-0.4.4/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-13 16:19:21.774478 python-eigen-ingenuity-0.4.5/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.5/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.5/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-04-13 16:19:21.773876 python-eigen-ingenuity-0.4.5/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.5/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-13 16:19:21.771775 python-eigen-ingenuity-0.4.5/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    15868 2023-04-05 14:48:43.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-13 16:19:21.772574 python-eigen-ingenuity-0.4.5/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6236 2023-04-06 15:19:51.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3040 2023-04-06 15:18:26.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36189 2023-04-06 11:02:05.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2829 2023-03-08 14:18:40.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4067 2022-12-01 09:50:12.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    11778 2022-12-15 11:39:53.000000 python-eigen-ingenuity-0.4.5/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.5/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-04-13 16:19:21.773589 python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-04-13 16:19:21.000000 python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      551 2023-04-13 16:19:21.000000 python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-04-13 16:19:21.000000 python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       24 2023-04-13 16:19:21.000000 python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-04-13 16:19:21.000000 python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-04-13 16:19:21.774568 python-eigen-ingenuity-0.4.5/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      689 2023-04-13 16:18:55.000000 python-eigen-ingenuity-0.4.5/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.4/LICENSE` & `python-eigen-ingenuity-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/PKG-INFO` & `python-eigen-ingenuity-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.4
+Version: 0.4.5
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.4/README.md` & `python-eigen-ingenuity-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/assetmodel.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/core/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/elastic.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,23 @@
   for node in nodes:
       code = node.code
       print(code)  
 """
 
 from eigeningenuity import EigenServer
 from urllib.parse import quote as urlquote
-from eigeningenuity.historian import get_historian
 from eigeningenuity.util import is_list,force_list,_do_eigen_json_request,EigenException
 from eigeningenuity.core import get_default_server
 import pandas as pd
 import datetime as dt
 import json
 import requests
 from requests.exceptions import ConnectionError
 from urllib.error import URLError
+from typing import Union
 
 from urllib3.exceptions import InsecureRequestWarning
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
 class ElasticConnection (object):
     """An elasticsearch instance which talks the Eigen elastic endpoint.
     """
@@ -45,15 +45,15 @@
         """Preflight Request to verify connection to ingenuity"""
         try:
             status = requests.get(self.baseurl + "?cmd=DODIRECTSEARCH&clientname=" + instance + "&index=" + index + "&search=%7B%7D").status_code
             if status != 200:
                 raise ConnectionError(
                     "Invalid API Response from " + self.baseurl + "?cmd=DODIRECTSEARCH&clientname" + instance + ". Please check the base url is correct, the instance is running and has an elasticsearch database.")
         except (URLError, ConnectionError):
-            raise ConnectionError ("Failed to connect to ingenuity instance at " + self.baseurl + "?cmd=DODIRECTSEARCH" + ". Please check the url is correct and the instance is up.")
+            raise ConnectionError ("Failed to connect to ingenuity instance at " + self.baseurl + "?cmd=DODIRECTSEARCH&clientname=" + instance + "&index=" + index + ". Please check the url is correct and the instance is up.")
         
         return status
     
     def listIndices(self,instance:str):
         """Lists all indices in Elastic Database.
 
         Args:
@@ -97,15 +97,15 @@
                 return True
             else:
                 return False
 
         return result
 
 
-    def executeRawQuery(self,index:str, query:str, instance:str = "elasticsearch-int", output:str = "json", filepath:str = None):
+    def executeRawQuery(self,index:str, query:Union[str,dict], instance:str = "elasticsearch-int", output:str = "json", filepath:str = None):
         """Executes a raw cypher query against Elastic.
 
         Args:
             index: The elasticsearch index to query
             query: The body of the query
             instance: (Optional) The instance of elasticsearch to query. Defaults to elasticsearch-int
             output: (Optional) The format in which to return the data. Accepts one of: "raw" - The raw json returned by the API; "json" - A processed version of the json response; "df" - A formatted pandas dataframe object; "file" - Writes the response to a .json file in the local directory. Defaults to "json"
@@ -114,14 +114,18 @@
         Returns:
             Elasticsearch API response to the query, the format is dependent on the output parameter
         """
         self._testConnection(instance,index)
         validOutputTypes = ["raw", "json", "df", "file"]
         if output not in validOutputTypes:
             raise ValueError("output must be one of %r." % validOutputTypes)
+
+        if type(query) is dict:
+            query = json.dumps(query)
+
         args = {}
         args["clientname"] = instance
         args["index"] = index
         args["search"] = query
 
         response = self._doJsonRequest("DODIRECTSEARCH", args)
 
@@ -136,14 +140,16 @@
             return pd.json_normalize(response['results'])
         elif output == "file":
             if filepath is None:
                 filepath = "eigenElasticResponse-" + index + "-" + str(dt.datetime.now().strftime("%Y-%m-%dT%H:%M:%S"))
             with open(filepath + ".json", "w") as f:
                 f.write(json.dumps(response, indent=4))
 
+
+
 def get_elastic(eigenserver:EigenServer = None):
     """Instantiate an elasticsearch connection for the given EigenServer.
 
     Args:
         eigenserver: (Optional) An EigenServer Object linked to the ingenuity url containing the elasticsearch. Can be omitted if environmental variable "EIGENSERVER" exists and is equal to the Ingenuity base url
 
     Returns:
```

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/historian.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.5/eigeningenuity/util.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.4
+Version: 0.4.5
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.4/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.5/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.4/setup.py` & `python-eigen-ingenuity-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.4',
+    version='0.4.5',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
```

