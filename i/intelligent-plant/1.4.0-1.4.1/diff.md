# Comparing `tmp/intelligent_plant-1.4.0.tar.gz` & `tmp/intelligent_plant-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelligent_plant-1.4.0.tar", last modified: Fri Jan 14 16:26:31 2022, max compression
+gzip compressed data, was "intelligent_plant-1.4.1.tar", last modified: Thu Apr 13 14:41:27 2023, max compression
```

## Comparing `intelligent_plant-1.4.0.tar` & `intelligent_plant-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-01-14 16:26:31.565263 intelligent_plant-1.4.0/
--rw-rw-rw-   0        0        0     1099 2019-08-01 10:38:26.000000 intelligent_plant-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     1380 2022-01-14 16:26:31.565263 intelligent_plant-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2020-07-13 13:18:00.000000 intelligent_plant-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-01-14 16:26:31.542272 intelligent_plant-1.4.0/intelligent_plant/
--rw-rw-rw-   0        0        0       79 2019-07-12 10:47:27.000000 intelligent_plant-1.4.0/intelligent_plant/__init__.py
--rw-rw-rw-   0        0        0    13114 2021-08-19 10:28:33.000000 intelligent_plant-1.4.0/intelligent_plant/app_store_client.py
--rw-rw-rw-   0        0        0     8328 2022-01-14 15:49:28.000000 intelligent_plant-1.4.0/intelligent_plant/data_core_client.py
--rw-rw-rw-   0        0        0     7023 2021-08-13 11:04:39.000000 intelligent_plant-1.4.0/intelligent_plant/http_client.py
--rw-rw-rw-   0        0        0     4082 2022-01-14 15:55:19.000000 intelligent_plant-1.4.0/intelligent_plant/utility.py
-drwxrwxrwx   0        0        0        0 2022-01-14 16:26:31.563265 intelligent_plant-1.4.0/intelligent_plant.egg-info/
--rw-rw-rw-   0        0        0     1380 2022-01-14 16:26:31.000000 intelligent_plant-1.4.0/intelligent_plant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2022-01-14 16:26:31.000000 intelligent_plant-1.4.0/intelligent_plant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-14 16:26:31.000000 intelligent_plant-1.4.0/intelligent_plant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-01-14 16:26:31.000000 intelligent_plant-1.4.0/intelligent_plant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-01-14 16:26:31.000000 intelligent_plant-1.4.0/intelligent_plant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-14 16:26:31.565263 intelligent_plant-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2022-01-14 16:26:19.000000 intelligent_plant-1.4.0/setup.py
+drwxrwxrwx   0 ross      (1000) ross      (1000)        0 2023-04-13 14:41:27.253095 intelligent_plant-1.4.1/
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     1099 2019-08-01 10:38:26.000000 intelligent_plant-1.4.1/LICENSE
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     1293 2023-04-13 14:41:27.237470 intelligent_plant-1.4.1/PKG-INFO
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     1023 2020-07-13 13:18:00.000000 intelligent_plant-1.4.1/README.md
+drwxrwxrwx   0 ross      (1000) ross      (1000)        0 2023-04-13 14:41:27.127698 intelligent_plant-1.4.1/intelligent_plant/
+-rwxrwxrwx   0 ross      (1000) ross      (1000)       79 2019-07-12 10:47:27.000000 intelligent_plant-1.4.1/intelligent_plant/__init__.py
+-rwxrwxrwx   0 ross      (1000) ross      (1000)    12977 2023-04-13 14:40:26.000000 intelligent_plant-1.4.1/intelligent_plant/app_store_client.py
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     8302 2023-04-13 14:35:14.000000 intelligent_plant-1.4.1/intelligent_plant/data_core_client.py
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     7023 2021-08-13 11:04:39.000000 intelligent_plant-1.4.1/intelligent_plant/http_client.py
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     4363 2023-04-12 16:03:22.000000 intelligent_plant-1.4.1/intelligent_plant/utility.py
+drwxrwxrwx   0 ross      (1000) ross      (1000)        0 2023-04-13 14:41:27.221846 intelligent_plant-1.4.1/intelligent_plant.egg-info/
+-rwxrwxrwx   0 ross      (1000) ross      (1000)     1293 2023-04-13 14:41:26.000000 intelligent_plant-1.4.1/intelligent_plant.egg-info/PKG-INFO
+-rwxrwxrwx   0 ross      (1000) ross      (1000)      398 2023-04-13 14:41:26.000000 intelligent_plant-1.4.1/intelligent_plant.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ross      (1000) ross      (1000)        1 2023-04-13 14:41:26.000000 intelligent_plant-1.4.1/intelligent_plant.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ross      (1000) ross      (1000)       30 2023-04-13 14:41:26.000000 intelligent_plant-1.4.1/intelligent_plant.egg-info/requires.txt
+-rwxrwxrwx   0 ross      (1000) ross      (1000)       18 2023-04-13 14:41:26.000000 intelligent_plant-1.4.1/intelligent_plant.egg-info/top_level.txt
+-rwxrwxrwx   0 ross      (1000) ross      (1000)       38 2023-04-13 14:41:27.253095 intelligent_plant-1.4.1/setup.cfg
+-rwxrwxrwx   0 ross      (1000) ross      (1000)      557 2023-04-13 14:31:24.000000 intelligent_plant-1.4.1/setup.py
```

### Comparing `intelligent_plant-1.4.0/LICENSE` & `intelligent_plant-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `intelligent_plant-1.4.0/PKG-INFO` & `intelligent_plant-1.4.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: intelligent_plant
-Version: 1.4.0
-Summary: A wrapper for the Intellinget Plant API
-Home-page: https://github.com/intelligentplant/py-app-store-api
-Author: Intelligent Plant
-Author-email: support@intelligentplant.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python App Store API Client
 A python implmentation of the Intelligent Plant industrial appstore API client
 
 See the example folder for example on how to use the library for authorization code and implicit OAuth grant flows.
 
 ## Getting started
 
@@ -43,9 +31,8 @@
 
 To run the authorization code grant flow (server) example run:
 
 `python example\authorization_code_grant_flow.py`
 
 To use this library as part of a Jupyter Notebook join the Jupyter Hub:
 
-https://appstore.intelligentplant.com/Home/AppProfile?appId=40d7a49722f84be4986318bb5cc98cf3
-
+https://appstore.intelligentplant.com/Home/AppProfile?appId=40d7a49722f84be4986318bb5cc98cf3
```

### Comparing `intelligent_plant-1.4.0/intelligent_plant/app_store_client.py` & `intelligent_plant-1.4.1/intelligent_plant/app_store_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,23 @@
         if expires_in is None:
             self.expiry_time = None
         else:
             self.expiry_time = time.time() + expires_in
 
         http_client.HttpClient.__init__(self, base_url, authorization_header ="Bearer " + self.access_token)
 
-    def get_data_core_client(self, data_core_url = None):
+    def get_data_core_client(self, *args, **kwargs):
         """
         Get the data core client with the same authorization details as this app store client.
-        :param data_core_url: The base URL for the data core API (optional, leaving it unspecified will determine the data core url relative to this client's base URL)
+        :param base_url: The base URL for the data core API. The default value is "https://api.intelligentplant.com/datacore/" (the app store data api)
 
         :return: The data core client with the same authorization as this app store client.
         """
-        data_core_url = urllib.parse.urljoin(self.base_url, "gestalt/datacore/") if data_core_url == None else data_core_url
-        return data_core_client.DataCoreClient(base_url = data_core_url, authorization_header ="Bearer " + self.access_token)
+        kwargs['authorization_header'] = "Bearer " + self.access_token
+        return data_core_client.DataCoreClient(*args, **kwargs)
 
     def get_user_info(self):
         """
         Get the authenticated user's user info from the app store.
 
         :return: The users infor as a parsed JSON object
         :raises: :class:`HTTPError`, if one occurred.
```

### Comparing `intelligent_plant-1.4.0/intelligent_plant/data_core_client.py` & `intelligent_plant-1.4.1/intelligent_plant/data_core_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
             tags[entry[0]] = [entry[1]]
 
     return tags
 
 class DataCoreClient(http_client.HttpClient):
     """Access the Intelligent Plant Data Core API"""
 
-    def __init__(self, base_url = "https://appstore.intelligentplant.com/gestalt/datacore/", **kwargs):
+    def __init__(self, base_url = "https://api.intelligentplant.com/datacore/", **kwargs):
         """
         Initialise a data core client with the specified authoriation haeder value and base URL.
         It is recommended that you use AppStoreClient.get_data_core_client(..) rather than calling this directly.
 
         :param authorization_header: The authorization header that will be used for all requests.
-        :param base_url: The base URL to make requests from. The default value is "https://appstore.intelligentplant.com/gestalt/datacore/" (the app store data api)
+        :param base_url: The base URL to make requests from. The default value is "https://api.intelligentplant.com/datacore/" (the app store data api)
         """
         super().__init__(base_url, **kwargs)
     
     def get_data_sources(self):
         """
         Get the list of available data sources
```

### Comparing `intelligent_plant-1.4.0/intelligent_plant/http_client.py` & `intelligent_plant-1.4.1/intelligent_plant/http_client.py`

 * *Files identical despite different names*

### Comparing `intelligent_plant-1.4.0/intelligent_plant/utility.py` & `intelligent_plant-1.4.1/intelligent_plant/utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,42 +4,40 @@
 
 import math
 from functools import reduce
 import datetime
 
 import pandas as pd
 
-def query_result_to_data_frame(result, include_dsn=False):
+def query_result_to_data_frame(result, include_dsn=False, force_numeric=False, force_string=False):
     """Convert the result of a data query into a data frame
        warn: this assumes that the timestamps for eachtag match (i.e. this won't work properly for raw queries)
-
        :param result: The parsed JSON result object. seealso: data_core_clinet.DataCoreClient.get_data(..)
        :param include_dsn: Whether or not to include the sata source name in the column name, defaul false.
-
+       :param force_numeric: Force numeric values to be taken over string values. Default: False
+       :param force_string: Force string values to be taken over numeric values. Default: False
        :return: A data frame with the queried tags as column headers and a row for each data point returned.
     """
     frame_data = {}
     
+
+    assert not (bool(force_numeric) and bool(force_string)), f'At most one of force_numeric or force_string can be set. Numeric: {force_numeric}, String: {force_string}' 
+    
     for dsn in result:
         #put the data data each tag into the data frame
-        for tag in result[dsn].items():
-            tag = tag[1]
+        for (tag_name, tag_data) in result[dsn].items():
             if (include_dsn):
-                name = dsn + " " + tag["TagName"]
+                name = dsn + "." + tag_name
             else:
-                name = tag["TagName"]
+                name = tag_name
             
             if (not "TimeStamp" in frame_data):
-                frame_data["TimeStamp"] = list(map(lambda x: pd.Timestamp(x["UtcSampleTime"]), tag["Values"]))
-
-            is_numeric = reduce(lambda x, y: x and y["IsNumeric"], tag["Values"], True)
-            if (is_numeric):
-                values = list(map(lambda x: x["NumericValue"], tag["Values"]))
-            else:
-                values = list(map(lambda x: x["TextValue"], tag["Values"]))
+                frame_data["TimeStamp"] = list(map(lambda x: pd.Timestamp(x["UtcSampleTime"]), tag_data["Values"]))
+            
+            values = list(map(lambda x: float(x["NumericValue"]) if (force_numeric or x["IsNumeric"]) and (not force_string) else x["TextValue"], tag_data["Values"]))
 
             frame_data[name] = values
     
     
     return pd.DataFrame(frame_data)
 
 def construct_tag_value(tag_name, utc_sample_time = None, numeric_value = None, text_value = None, status = 'Good', unit = '', notes = None, error = None, properties = {}):
@@ -48,15 +46,15 @@
        :param tag_name: The pname of the tag to write to.
        :param utc_sample_time: The UTC sample time that should be recored with the timestamp. Default value: the current system time.
        :param numeric_value: The numeric value that should be written. Optional, for text values leave unspecified or None.
        :param text_value: The text value that should be written. Optional, for numeric values leave unspecified or None.
        :param status: The status of this tag value. Must be 'Good', 'Bad' or 'Uncertain'. Default: 'Good'
        :param unit: The unit value that should be written. Default: the empty string.
        :param notes: Any notes that should be written. Default: None.
-       "param properties: Dictionary of generic properties to be written. Default {}
+       :param properties: Dictionary of generic properties to be written. Default {}
 
        :return: A tag value dictionary which can be used to write values to historians using data core.
     """
     
     assert numeric_value is not None or text_value is not None, 'Either numeric or text value must be specified'
     
     # set sample time to now if unspecified
```

### Comparing `intelligent_plant-1.4.0/intelligent_plant.egg-info/PKG-INFO` & `intelligent_plant-1.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-Metadata-Version: 2.1
-Name: intelligent-plant
-Version: 1.4.0
-Summary: A wrapper for the Intellinget Plant API
-Home-page: https://github.com/intelligentplant/py-app-store-api
-Author: Intelligent Plant
-Author-email: support@intelligentplant.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python App Store API Client
-A python implmentation of the Intelligent Plant industrial appstore API client
-
-See the example folder for example on how to use the library for authorization code and implicit OAuth grant flows.
-
-## Getting started
-
-### Installing using pip
-
-`pip install intelligent-plant`
-
-### Installing from Source
-
-Using pip:
-
-`pip install git+https://github.com/intelligentplant/py-app-store-api`
-
-Alternatively clone the Git repo:
-
-`git clone https://github.com/intelligentplant/py-app-store-api.git`
-
-To install necessary dependancies run:
-
-`pip install -r requirements.txt`
-
-## Examples
-
-To run the implicit grant flow (client) example run:
-
-`python example\implicit_grant_flow.py`
-
-To run the authorization code grant flow (server) example run:
-
-`python example\authorization_code_grant_flow.py`
-
-To use this library as part of a Jupyter Notebook join the Jupyter Hub:
-
-https://appstore.intelligentplant.com/Home/AppProfile?appId=40d7a49722f84be4986318bb5cc98cf3
-
+Metadata-Version: 2.1
+Name: intelligent_plant
+Version: 1.4.1
+Summary: A wrapper for the Intellinget Plant API
+Home-page: https://github.com/intelligentplant/py-app-store-api
+Author: Intelligent Plant
+Author-email: support@intelligentplant.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python App Store API Client
+A python implmentation of the Intelligent Plant industrial appstore API client
+
+See the example folder for example on how to use the library for authorization code and implicit OAuth grant flows.
+
+## Getting started
+
+### Installing using pip
+
+`pip install intelligent-plant`
+
+### Installing from Source
+
+Using pip:
+
+`pip install git+https://github.com/intelligentplant/py-app-store-api`
+
+Alternatively clone the Git repo:
+
+`git clone https://github.com/intelligentplant/py-app-store-api.git`
+
+To install necessary dependancies run:
+
+`pip install -r requirements.txt`
+
+## Examples
+
+To run the implicit grant flow (client) example run:
+
+`python example\implicit_grant_flow.py`
+
+To run the authorization code grant flow (server) example run:
+
+`python example\authorization_code_grant_flow.py`
+
+To use this library as part of a Jupyter Notebook join the Jupyter Hub:
+
+https://appstore.intelligentplant.com/Home/AppProfile?appId=40d7a49722f84be4986318bb5cc98cf3
```

### Comparing `intelligent_plant-1.4.0/setup.py` & `intelligent_plant-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
    name='intelligent_plant',
    url="https://github.com/intelligentplant/py-app-store-api",
-   version='1.4.0',
+   version='1.4.1',
    description='A wrapper for the Intellinget Plant API',
    long_description=long_description,
    long_description_content_type="text/markdown",
    author='Intelligent Plant',
    author_email="support@intelligentplant.com",
    packages=['intelligent_plant'],
    install_requires=['requests', 'requests_ntlm', 'pandas']
```

