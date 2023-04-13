# Comparing `tmp/veevatools-0.0.94.tar.gz` & `tmp/veevatools-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veevatools-0.0.94.tar", last modified: Thu Mar  9 15:53:03 2023, max compression
+gzip compressed data, was "veevatools-0.0.95.tar", last modified: Thu Apr 13 20:49:57 2023, max compression
```

## Comparing `veevatools-0.0.94.tar` & `veevatools-0.0.95.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.467784 veevatools-0.0.94/
--rw-rw-rw-   0        0        0      658 2022-05-07 04:14:46.000000 veevatools-0.0.94/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2022-05-08 00:45:13.000000 veevatools-0.0.94/MANIFEST.in
--rw-rw-rw-   0        0        0     6648 2023-03-09 15:53:03.467784 veevatools-0.0.94/PKG-INFO
--rw-rw-rw-   0        0        0     6291 2022-06-29 21:08:45.000000 veevatools-0.0.94/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.451784 veevatools-0.0.94/salesforce/
--rw-rw-rw-   0        0        0       73 2022-05-19 04:32:15.000000 veevatools-0.0.94/salesforce/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.453784 veevatools-0.0.94/salesforce/custom_exceptions/
--rw-rw-rw-   0        0        0      142 2022-06-24 18:09:22.000000 veevatools-0.0.94/salesforce/custom_exceptions/__init__.py
--rw-rw-rw-   0        0        0     3416 2022-05-16 20:22:53.000000 veevatools-0.0.94/salesforce/custom_exceptions/salesforce_exceptions.py
--rw-rw-rw-   0        0        0      274 2022-05-19 04:43:58.000000 veevatools-0.0.94/salesforce/decorators.py
--rw-rw-rw-   0        0        0    94245 2023-02-14 20:47:49.000000 veevatools-0.0.94/salesforce/salesforce.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.456784 veevatools-0.0.94/salesforce/utilities/
--rw-rw-rw-   0        0        0      302 2022-09-01 00:09:33.000000 veevatools-0.0.94/salesforce/utilities/__init__.py
--rw-rw-rw-   0        0        0      704 2022-06-30 05:29:51.000000 veevatools-0.0.94/salesforce/utilities/async_utils.py
--rw-rw-rw-   0        0        0     3897 2022-06-28 03:58:32.000000 veevatools-0.0.94/salesforce/utilities/df_utils.py
--rw-rw-rw-   0        0        0     2112 2023-03-09 15:52:01.000000 veevatools-0.0.94/salesforce/utilities/sf_query_processors.py
--rw-rw-rw-   0        0        0      763 2023-03-09 15:53:03.468784 veevatools-0.0.94/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-05-07 03:46:02.000000 veevatools-0.0.94/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.460783 veevatools-0.0.94/veevanetwork/
--rw-rw-rw-   0        0        0       40 2022-06-08 00:43:06.000000 veevatools-0.0.94/veevanetwork/__init__.py
--rw-rw-rw-   0        0        0        0 2022-06-16 04:00:20.000000 veevatools-0.0.94/veevanetwork/api.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.462783 veevatools-0.0.94/veevanetwork/custom_exceptions/
--rw-rw-rw-   0        0        0      148 2022-06-23 17:12:46.000000 veevatools-0.0.94/veevanetwork/custom_exceptions/__init__.py
--rw-rw-rw-   0        0        0     3870 2022-06-20 23:49:28.000000 veevatools-0.0.94/veevanetwork/custom_exceptions/veevanetwork_exceptions.py
--rw-rw-rw-   0        0        0   122066 2022-06-16 02:54:23.000000 veevatools-0.0.94/veevanetwork/network_api_v25.json
--rw-rw-rw-   0        0        0    81646 2022-12-02 05:41:49.000000 veevatools-0.0.94/veevanetwork/veevanetwork.py
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.465784 veevatools-0.0.94/veevatools.egg-info/
--rw-rw-rw-   0        0        0     6648 2023-03-09 15:53:03.000000 veevatools-0.0.94/veevatools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-03-09 15:53:03.000000 veevatools-0.0.94/veevatools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 15:53:03.000000 veevatools-0.0.94/veevatools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-03-09 15:53:03.000000 veevatools-0.0.94/veevatools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-03-09 15:53:03.000000 veevatools-0.0.94/veevatools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 15:53:03.466784 veevatools-0.0.94/veevavault/
--rw-rw-rw-   0        0        0       36 2022-06-08 00:45:04.000000 veevatools-0.0.94/veevavault/__init__.py
--rw-rw-rw-   0        0        0     8963 2022-11-30 05:55:48.000000 veevatools-0.0.94/veevavault/veevavault.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.475044 veevatools-0.0.95/
+-rw-rw-rw-   0        0        0      658 2022-05-07 04:14:46.000000 veevatools-0.0.95/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2022-05-08 00:45:13.000000 veevatools-0.0.95/MANIFEST.in
+-rw-rw-rw-   0        0        0     6648 2023-04-13 20:49:57.475044 veevatools-0.0.95/PKG-INFO
+-rw-rw-rw-   0        0        0     6291 2022-06-29 21:08:45.000000 veevatools-0.0.95/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.459041 veevatools-0.0.95/salesforce/
+-rw-rw-rw-   0        0        0       73 2022-05-19 04:32:15.000000 veevatools-0.0.95/salesforce/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.461041 veevatools-0.0.95/salesforce/custom_exceptions/
+-rw-rw-rw-   0        0        0      142 2022-06-24 18:09:22.000000 veevatools-0.0.95/salesforce/custom_exceptions/__init__.py
+-rw-rw-rw-   0        0        0     3416 2022-05-16 20:22:53.000000 veevatools-0.0.95/salesforce/custom_exceptions/salesforce_exceptions.py
+-rw-rw-rw-   0        0        0      274 2022-05-19 04:43:58.000000 veevatools-0.0.95/salesforce/decorators.py
+-rw-rw-rw-   0        0        0    94293 2023-04-13 20:49:22.000000 veevatools-0.0.95/salesforce/salesforce.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.464041 veevatools-0.0.95/salesforce/utilities/
+-rw-rw-rw-   0        0        0      302 2022-09-01 00:09:33.000000 veevatools-0.0.95/salesforce/utilities/__init__.py
+-rw-rw-rw-   0        0        0      704 2022-06-30 05:29:51.000000 veevatools-0.0.95/salesforce/utilities/async_utils.py
+-rw-rw-rw-   0        0        0     3897 2022-06-28 03:58:32.000000 veevatools-0.0.95/salesforce/utilities/df_utils.py
+-rw-rw-rw-   0        0        0     2112 2023-03-09 15:52:01.000000 veevatools-0.0.95/salesforce/utilities/sf_query_processors.py
+-rw-rw-rw-   0        0        0      763 2023-04-13 20:49:57.476043 veevatools-0.0.95/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-05-07 03:46:02.000000 veevatools-0.0.95/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.468042 veevatools-0.0.95/veevanetwork/
+-rw-rw-rw-   0        0        0       40 2022-06-08 00:43:06.000000 veevatools-0.0.95/veevanetwork/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-06-16 04:00:20.000000 veevatools-0.0.95/veevanetwork/api.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.470042 veevatools-0.0.95/veevanetwork/custom_exceptions/
+-rw-rw-rw-   0        0        0      148 2022-06-23 17:12:46.000000 veevatools-0.0.95/veevanetwork/custom_exceptions/__init__.py
+-rw-rw-rw-   0        0        0     3870 2022-06-20 23:49:28.000000 veevatools-0.0.95/veevanetwork/custom_exceptions/veevanetwork_exceptions.py
+-rw-rw-rw-   0        0        0   122066 2022-06-16 02:54:23.000000 veevatools-0.0.95/veevanetwork/network_api_v25.json
+-rw-rw-rw-   0        0        0    81646 2022-12-02 05:41:49.000000 veevatools-0.0.95/veevanetwork/veevanetwork.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.473041 veevatools-0.0.95/veevatools.egg-info/
+-rw-rw-rw-   0        0        0     6648 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.475044 veevatools-0.0.95/veevavault/
+-rw-rw-rw-   0        0        0       36 2022-06-08 00:45:04.000000 veevatools-0.0.95/veevavault/__init__.py
+-rw-rw-rw-   0        0        0     9177 2023-03-15 17:03:59.000000 veevatools-0.0.95/veevavault/veevavault.py
```

### Comparing `veevatools-0.0.94/LICENSE.txt` & `veevatools-0.0.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/PKG-INFO` & `veevatools-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veevatools
-Version: 0.0.94
+Version: 0.0.95
 Summary: Veeva tools library for accelerating Veeva Systems Internal Tools development
 Home-page: https://github.com/michaelpay
 Author: Michael Pay
 Author-email: monickenish@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `veevatools-0.0.94/README.md` & `veevatools-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/salesforce/custom_exceptions/salesforce_exceptions.py` & `veevatools-0.0.95/salesforce/custom_exceptions/salesforce_exceptions.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/salesforce/salesforce.py` & `veevatools-0.0.95/salesforce/salesforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -1245,15 +1245,15 @@
             objectDescribe = getattr(self.sf, object).describe()
             objectPicklistValues = pd.DataFrame(index=range(0,max(len(field["picklistValues"]) for field in objectDescribe['fields'] if field['type'] == 'picklist')))
             for x in [pd.Series(data = [picklist['value'] for picklist in field['picklistValues']], name = object + "." + field["name"]) for field in objectDescribe['fields'] if field['type'] == 'picklist']:
                 objectPicklistValues.insert(0, str(x.name), x)
             referenceList.append(objectPicklistValues)
         return referenceList
 
-    def record_type_retrieval(self, objectAPIName, fieldAPINames = ["Id","Name",'SobjectType']):
+    def record_type_retrieval(self, objectAPIName, fieldAPINames = ["Id","Name",'SobjectType', 'IsActive']):
         """
         TODO:
         
         Description of what it does
         
         Description of arguments and data types
         
@@ -1265,15 +1265,16 @@
         """
         sfRTDF = pd.DataFrame(self.sf.query_all("SELECT "+ ",".join(fieldAPINames) + " from RecordType WHERE SobjectType = '" + objectAPIName + "'")['records'])
         
         # If only master RT exists
         if len(sfRTDF) == 0:
             master_rt = {
                 "Name": "Master",
-                "DeveloperName": "Master"
+                "DeveloperName": "Master",
+                "IsActive": True,
             }
 
             sfRTDF = pd.DataFrame(master_rt, index=[0])
         else:
             sfRTDF.drop(columns="attributes", inplace = True)
         return sfRTDF
```

### Comparing `veevatools-0.0.94/salesforce/utilities/async_utils.py` & `veevatools-0.0.95/salesforce/utilities/async_utils.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/salesforce/utilities/df_utils.py` & `veevatools-0.0.95/salesforce/utilities/df_utils.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/salesforce/utilities/sf_query_processors.py` & `veevatools-0.0.95/salesforce/utilities/sf_query_processors.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/setup.cfg` & `veevatools-0.0.95/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6565 7661 746f 6f6c 730d 0a76   = veevatools..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 340d  ersion = 0.0.94.
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 350d  ersion = 0.0.95.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2056  .description = V
 00000040: 6565 7661 2074 6f6f 6c73 206c 6962 7261  eeva tools libra
 00000050: 7279 2066 6f72 2061 6363 656c 6572 6174  ry for accelerat
 00000060: 696e 6720 5665 6576 6120 5379 7374 656d  ing Veeva System
 00000070: 7320 496e 7465 726e 616c 2054 6f6f 6c73  s Internal Tools
 00000080: 2064 6576 656c 6f70 6d65 6e74 0d0a 6175   development..au
 00000090: 7468 6f72 203d 204d 6963 6861 656c 2050  thor = Michael P
```

### Comparing `veevatools-0.0.94/veevanetwork/custom_exceptions/veevanetwork_exceptions.py` & `veevatools-0.0.95/veevanetwork/custom_exceptions/veevanetwork_exceptions.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/veevanetwork/network_api_v25.json` & `veevatools-0.0.95/veevanetwork/network_api_v25.json`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/veevanetwork/veevanetwork.py` & `veevatools-0.0.95/veevanetwork/veevanetwork.py`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/veevatools.egg-info/PKG-INFO` & `veevatools-0.0.95/veevatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veevatools
-Version: 0.0.94
+Version: 0.0.95
 Summary: Veeva tools library for accelerating Veeva Systems Internal Tools development
 Home-page: https://github.com/michaelpay
 Author: Michael Pay
 Author-email: monickenish@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `veevatools-0.0.94/veevatools.egg-info/SOURCES.txt` & `veevatools-0.0.95/veevatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.94/veevavault/veevavault.py` & `veevatools-0.0.95/veevavault/veevavault.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,20 @@
             "Accept": "application/json",
             "Authorization": self.sessionId
         }
         params = {
         "q":query
         }
 
-        r = pd.DataFrame(requests.get(url, headers=h, params=params).json()['data'])
+        r = requests.get(url, headers=h, params=params).json()
+
+        if r['responseStatus'] == 'FAILURE':
+            raise Exception(r['errors'])
+        else:
+            r = pd.DataFrame(r['data'])
         
         return r
     
     def bulk_query(self, query):
         url = f"{self.vaultURL}/api/{self.LatestAPIversion}/query"
         
         h = {
@@ -139,14 +144,17 @@
             "Authorization": self.sessionId
         }
         params = {
         "q":query
         }
 
         r = requests.get(url, headers=h, params=params).json()
+
+        if r['responseStatus'] == 'FAILURE':
+            raise Exception(r['errors'])
         
         output = pd.DataFrame(r['data'])
         
         try:
             next_page_url = r['responseDetails']['next_page'][:-4]
             more_pages = True
             page_count = 1000
```

