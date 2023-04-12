# Comparing `tmp/rasaio.integrations-0.0.8.tar.gz` & `tmp/rasaio.integrations-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rasaio.integrations-0.0.8.tar", last modified: Fri May 10 14:02:38 2019, max compression
+gzip compressed data, was "dist/rasaio.integrations-0.0.9.tar", last modified: Thu May 23 17:51:23 2019, max compression
```

## Comparing `rasaio.integrations-0.0.8.tar` & `rasaio.integrations-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      141 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)       87 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)        1 2019-05-10 14:02:37.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2019-05-10 14:02:37.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      627 2019-05-10 14:02:37.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2019-05-10 14:02:37.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       61 2019-05-10 14:02:37.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      479 2019-05-10 14:02:37.000000 rasaio.integrations-0.0.8/rasaio.integrations.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      854 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/rasaio/
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/rasaio/integrations/
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/rasaio/integrations/test/
--rw-rw-rw-   0 root         (0) root         (0)     1300 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/test/test_salesforce.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/rasaio/integrations/salesforce/
--rw-rw-rw-   0 root         (0) root         (0)     4335 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/salesforce/salesforce.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/salesforce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14893 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/rasaio/integrations/utilties/
--rw-rw-rw-   0 root         (0) root         (0)     2104 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/utilties/helper.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/utilties/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/integrations/constants.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/rasaio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2019-05-10 14:02:27.000000 rasaio.integrations-0.0.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      479 2019-05-10 14:02:38.000000 rasaio.integrations-0.0.8/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/LICENSE.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio/
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio/integrations/
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio/integrations/utilties/
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/utilties/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/utilties/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio/integrations/salesforce/
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/salesforce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4335 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/salesforce/salesforce.py
+-rw-rw-rw-   0 root         (0) root         (0)    14735 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio/integrations/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/test/test_salesforce.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/integrations/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/rasaio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      854 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2019-05-23 17:51:12.000000 rasaio.integrations-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      479 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)        1 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      627 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      479 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/rasaio.integrations.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       38 2019-05-23 17:51:23.000000 rasaio.integrations-0.0.9/setup.cfg
```

### Comparing `rasaio.integrations-0.0.8/rasaio.integrations.egg-info/SOURCES.txt` & `rasaio.integrations-0.0.9/rasaio.integrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rasaio.integrations-0.0.8/setup.py` & `rasaio.integrations-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_reqs = parse_requirements('requires.txt', session=False)
 
 README="""Python class to integrate rasa.io and another customer database"""
 
 setup(
   name='rasaio.integrations',
-  version='0.0.8',
+  version='0.0.9',
   description=README,
   long_description=README,
   long_description_content_type='text/x-rst',
   classifiers=[
     "Programming Language :: Python :: 3.6"
   ],
   author="rasa.io",
```

### Comparing `rasaio.integrations-0.0.8/rasaio/integrations/test/test_salesforce.py` & `rasaio.integrations-0.0.9/rasaio/integrations/test/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `rasaio.integrations-0.0.8/rasaio/integrations/salesforce/salesforce.py` & `rasaio.integrations-0.0.9/rasaio/integrations/salesforce/salesforce.py`

 * *Files identical despite different names*

### Comparing `rasaio.integrations-0.0.8/rasaio/integrations/salesforce/__init__.py` & `rasaio.integrations-0.0.9/rasaio/integrations/salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `rasaio.integrations-0.0.8/rasaio/integrations/__init__.py` & `rasaio.integrations-0.0.9/rasaio/integrations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,28 +46,28 @@
   email: str
   external_id: str = None # unique identifier field in customer database which doesn't change e.g. id
   first_name: str = None
   last_name: str = None
   is_active: str = None
   is_subscribed: str = None
   updated: str= None
+  # exta fields can be supported by calling setattr on FieldMapping object
 
 class IntegrationBase(abc.ABC):
   def __init__(self, rasa_api_attrs: RasaApiAttributes, field_mapping: FieldMapping, log_func):
     """
       rasa_api_attrs: rasa api attributes
       field_mapping: field mappings
       log_func: partial function with takes 2 parameter (message, message_type)
     """
     self.rasa_api_attrs = rasa_api_attrs
-    self.field_mapping = field_mapping
     self.log_func = log_func
 
     self.updated_since : datetime = None if self.rasa_api_attrs.sync_type == SyncType.FULL else self.rasa_api_attrs.last_run_date
-    self.field_mapping_json = json.loads(self.field_mapping.to_json()) # pylint: disable=E1101
+    self.field_mapping_json = field_mapping.__dict__
     self.rasa_sync_on_fieldname = self.rasa_api_attrs.sync_on_fieldname
     self.customer_sync_on_fieldname = self.field_mapping_json[self.rasa_sync_on_fieldname]
 
     self.rasa_api_token = self.__get_rasa_api_token()
     self.rasa_active_persons = []
     self.rasa_inactive_persons = []
     self.__rasa_persons_by_email = {}
@@ -275,34 +275,32 @@
   def __unsubscribe_rasa_persons_for_oneway_sync(self):
     for rasa_person in self.rasa_active_persons:
       if not self.rasa_active_person_by_id.get(rasa_person[ID]):
         self.__unsubscribe_rasa_person(rasa_person)
 
   def map_customer_persons_to_rasa_persons(self, customer_persons):
     mapped_persons = []
-    field_mapping_json = json.loads(self.field_mapping.to_json()) # pylint: disable=E1101
     for customer_person in customer_persons:
-      mapped_person = {k : customer_person[v] for k, v in field_mapping_json.items() if v and customer_person.get(v) is not None}
+      mapped_person = {k : customer_person[v] for k, v in self.field_mapping_json.items() if v and customer_person.get(v) is not None}
       if mapped_person.get(UPDATED):
         mapped_person[UPDATED] = parse_date_from(mapped_person[UPDATED])
       mapped_persons.append(mapped_person)
     return mapped_persons
 
   def map_rasa_persons_to_customer_persons(self, rasa_persons):
     mapped_persons = []
-    field_mapping_json = json.loads(self.field_mapping.to_json()) # pylint: disable=E1101
     for rasa_person in rasa_persons:
       if self.rasa_api_attrs.is_person_attribute_supported:
         rasa_person = self.__get_rasa_person_with_attributes(rasa_person[ID])
         if not rasa_person:
           continue
 
-      mapped_person = {v : rasa_person[k] for k, v in field_mapping_json.items() if v and rasa_person.get(k) is not None}
-      if field_mapping_json.get(UPDATED) and mapped_person.get(field_mapping_json[UPDATED]):
-        mapped_person[field_mapping_json[UPDATED]] = parse_date_from(mapped_person[field_mapping_json[UPDATED]])
+      mapped_person = {v : rasa_person[k] for k, v in self.field_mapping_json.items() if v and rasa_person.get(k) is not None}
+      if self.field_mapping_json.get(UPDATED) and mapped_person.get(self.field_mapping_json[UPDATED]):
+        mapped_person[self.field_mapping_json[UPDATED]] = parse_date_from(mapped_person[self.field_mapping_json[UPDATED]])
       mapped_persons.append(mapped_person)
 
     return mapped_persons
 
   def __get_rasa_id_from_create_response(self, response):
     results = response.json()[RESULTS]
     return results[0].get(ID)
```

### Comparing `rasaio.integrations-0.0.8/rasaio/integrations/utilties/helper.py` & `rasaio.integrations-0.0.9/rasaio/integrations/utilties/helper.py`

 * *Files identical despite different names*

### Comparing `rasaio.integrations-0.0.8/LICENSE.txt` & `rasaio.integrations-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

