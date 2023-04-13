# Comparing `tmp/cd2t-1.4.0.tar.gz` & `tmp/cd2t-1.5.0.tar.gz`

## Comparing `cd2t-1.4.0.tar` & `cd2t-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/DataParser.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/References.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/results.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/schema.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/utils.py
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/List.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/NoneDataType.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/any.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/base.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/bool.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/datatype.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/enum.py
--rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/float.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/idlist.py
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/integer.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/multitype.py
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/object.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/schema.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 cd2t-1.4.0/cd2t/types/string.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.4.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.4.0/LICENSE
--rw-r--r--   0        0        0    17038 2020-02-02 00:00:00.000000 cd2t-1.4.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 cd2t-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/DataParser.py
+-rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/References.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/__init__.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/results.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/schema.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/utils.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/List.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/NoneDataType.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/any.py
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/base.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/bool.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/datatype.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/enum.py
+-rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/float.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/idlist.py
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/integer.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/multitype.py
+-rw-r--r--   0        0        0    10718 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/object.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/schema.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 cd2t-1.5.0/cd2t/types/string.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.5.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.5.0/LICENSE
+-rw-r--r--   0        0        0    17429 2020-02-02 00:00:00.000000 cd2t-1.5.0/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18076 2020-02-02 00:00:00.000000 cd2t-1.5.0/PKG-INFO
```

### Comparing `cd2t-1.4.0/cd2t/DataParser.py` & `cd2t-1.5.0/cd2t/DataParser.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/References.py` & `cd2t-1.5.0/cd2t/References.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import enum
-from cd2t.results import ValidationFinding
+from cd2t.results import ValidationFinding, Finding
 
 class OPT(enum.IntFlag):
     NONE = 1
     UNIQUE = 2
     UNIQUE_GLOBAL = 4
     PRODUCER = 8
     PRODUCER_GLOBAL = 16
@@ -11,16 +11,35 @@
     CONSUMER_GLOBAL = 64
     ALLOW_ORPHAN_PRODUCER = 128
 
 
 INIT_OPTIONS = OPT.UNIQUE | OPT.UNIQUE_GLOBAL | OPT.PRODUCER | OPT.PRODUCER_GLOBAL
 
 
-class ReferenceFinding(ValidationFinding):
-    pass
+class ReferenceFinding(Finding):
+    def __init__(self, message: str, path='', reference=None) -> None:
+        super().__init__(message=message, path=path)
+        self.reference = reference
+    
+    def __str__(self):
+        ns_lookup = False
+        if self.reference and isinstance(self.reference, ConsumerElement) \
+                and self.reference.provider_namespace:
+            ns_lookup = True
+            namespace = self.reference.namespace + ' > '
+        elif self.reference.namespace:
+            namespace = self.reference.namespace + ' > '
+        elif self.namespace:
+            namespace = self.namespace + ' > '
+        else:
+            namespace = ''
+        path = self.path + ': ' if self.path else ''
+        message = f"{self.message} in '{self.reference.provider_namespace}'" \
+                     if ns_lookup else self.message
+        return namespace + path + message
     
 
 class ReferenceError(Exception):
     pass
 
 
 class ReferenceElement():
@@ -70,14 +89,20 @@
 
     def get_producers_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
         return self.references.get(ref_key, dict()).get('producers', list())
 
     def get_consumers_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
         return self.references.get(ref_key, dict()).get('consumers', list())
 
+    def get_unique_values_by_ref_key(self, ref_key :str) -> set:
+        unique_values = set()
+        for e in self.get_uniques_by_ref_key(ref_key):
+            unique_values.add(e.value)
+        return unique_values
+
     def _add_ref_key(self, ref_key :str):
         if ref_key in self.references.keys():
             return
         self.references[ref_key] = dict(
             uniques=list(),
             producers=list(),
             consumers=list()
@@ -121,20 +146,22 @@
     def get_producer_consumer_issues(self):
         results = list()
         for ref_key, ref_lists in self.references.items():
             for consumer in ref_lists['consumers']:
                 if len(consumer.consumes_from) == 0:
                     # No producer found during analysis!
                     results.append(ReferenceFinding(path=consumer.path,
-                                                    message="No provider found"))
+                                                    message="No producer found",
+                                                    reference=consumer))
             for producer in ref_lists['producers']:
                 if OPT.ALLOW_ORPHAN_PRODUCER not in producer.options and len(producer.provides_to) == 0:
                     # Producer has no consumer!
                     results.append(ReferenceFinding(path=producer.path,
-                                                    message="Producer has no consumer"))
+                                                    message="Producer has no consumer",
+                                                    reference=producer))
         return results
 
 
 class NameSpace(GlobalSpace):
     uOPT = OPT.UNIQUE
     pOPT = OPT.PRODUCER
     cOPT = OPT.CONSUMER
@@ -167,22 +194,27 @@
         else:
             linked_elements += self.namespace_obj.add_element(reference)
         return linked_elements
     
     def get_producer_consumer_issues(self):
         results = list()
         for namespace, ns_obj in self.ns_obj_store.items():
-            _results = ns_obj.get_producer_consumer_issues()
-            for r in _results:
-                r.path = namespace+" > "+r.path
-                results.append(r)
+            results += ns_obj.get_producer_consumer_issues()
+            # for r in _results:
+            #     r.path = namespace+" > "+r.path
+            #     results.append(r)
         return results
         
     def same_unique(self, reference :str) -> list[ReferenceElement]:
         others = self.namespace_obj.get_uniques_by_value(
             reference.value, reference.reference)
         if OPT.UNIQUE_GLOBAL in reference.options:
             others += self.globalspace_obj.get_uniques_by_value(
                 reference.value, reference.reference)
         if others:
             return others[0]
         return None
+
+    def get_unique_values_by_ref_key(self, ref_key :str) -> set:
+        ns_uniques = set(self.namespace_obj.get_unique_values_by_ref_key(ref_key))
+        global_unique = set(self.globalspace_obj.get_unique_values_by_ref_key(ref_key))
+        return ns_uniques.union(global_unique)
```

### Comparing `cd2t-1.4.0/cd2t/results.py` & `cd2t-1.5.0/cd2t/results.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,37 +24,27 @@
     def __lt__(self, other):
         return str(self) < str(other)
     
 
 class ValidationFinding(Finding):
     pass
 
-
-class ReferenceFinding(ValidationFinding):
-    def __init__(self, message: str, path='', reference=None) -> None:
-        super().__init__(message=message, path=path)
-        self.reference = reference
-
-
-class UniqueErrorFinding(ReferenceFinding):
-    pass
-
-
-class MissingReferenceFinding(ReferenceFinding):
-    pass
-
     
 class DataTypeMismatch(ValidationFinding):
     pass
     
 
 class WrongValueFinding(ValidationFinding):
     pass
 
 
+class UniqueErrorFinding(ValidationFinding):
+    pass
+
+
 class FindingsList(list):
     def __str__(self):
         __str_list = list()
         for finding in self:
             __str_list.append(str(finding))
         return '\n'.join( __str_list )
```

### Comparing `cd2t-1.4.0/cd2t/schema.py` & `cd2t-1.5.0/cd2t/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/utils.py` & `cd2t-1.5.0/cd2t/utils.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/types/List.py` & `cd2t-1.5.0/cd2t/types/List.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         self.elements = dict()
         self.element_data_type = None
     
     def build_schema(self, schema :dict, path :str,
                      data_types :dict, subschemas :dict,
                      subpath :list):
         self.__init__()
-        self.path = path
+        path = path + '[]'
         self.load_schema_options(schema, path)
         if len(self.elements) == 0:
             self.element_data_type = AnyDataType()
             return
         if not 'type' in self.elements.keys():
-            raise SchemaError("'elements' need to have a key 'type'", self.path)
+            raise SchemaError("'elements' need to have a key 'type'", path)
         element_data_type_name = self.elements['type']
         if element_data_type_name not in data_types.keys():
             raise SchemaError("'elements' data type '%s' not found" % 
-                              (element_data_type_name), self.path)
+                              (element_data_type_name), path)
         self.element_data_type = data_types[element_data_type_name]()
         # Save recursively detected data type (i.e. from 'schema' --> subschema)
         self.element_data_type = self.element_data_type.build_schema(
-            schema=self.elements, path=path+"[.]", data_types=data_types,
+            schema=self.elements, path=path, data_types=data_types,
             subschemas=subschemas, subpath=subpath)
         return self
     
     def build_sub_references(self, data :any, path :str, references :References):
         i = 0
         for element in data:
             self.element_data_type.build_references(element, "%s[%d]" % (path, i), references)
@@ -70,15 +70,15 @@
         FL = FindingsList()
         if self.minimum and len(data) < self.minimum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Length of list is lower than %d' % self.minimum))
         elif self.maximum and len(data) > self.maximum:
             FL.append(WrongValueFinding(
-                        path=self.path,
+                        path=path,
                         message='Length of list is greater than %d' % self.maximum))
         i = 0
         for element in data:
             FL += self.element_data_type.validate_data(
                 element, "%s[%d]" % (path, i), references)
             i += 1
```

### Comparing `cd2t-1.4.0/cd2t/types/base.py` & `cd2t-1.5.0/cd2t/types/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,12 +141,13 @@
             other = references.same_unique(ref_element)
             if other is not None:
                 if other.namespace != references.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
                 FL.append(ReferenceFinding(
-                    path=path,message="Unique value already used at '%s'" % _path))
+                    path=path,message="Unique value already used at '%s'" % _path,
+                    reference=ref_element))
                 return FL
         # If unique or just for producer/consumer mapping, add element to references
         references.add_element(ref_element)
         return FL
```

### Comparing `cd2t-1.4.0/cd2t/types/bool.py` & `cd2t-1.5.0/cd2t/types/bool.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/types/enum.py` & `cd2t-1.5.0/cd2t/types/enum.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/types/float.py` & `cd2t-1.5.0/cd2t/types/float.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/types/idlist.py` & `cd2t-1.5.0/cd2t/types/idlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self.allowed_ids = None
         self.not_allowed_ids = list()
     
     def build_schema(self, schema :dict, path :str,
                      data_types :dict, subschemas :dict,
                      subpath :list):
         self.__init__()
+        path = path + '{id}'
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
         if self.id_type not in ['string', 'integer']:
             raise SchemaError("id_type '%s' is not valid" % self.id_type, path)
         if 'type' in self.elements.keys():
             element_type_name = self.elements['type']
             if element_type_name not in data_types:
@@ -49,123 +50,125 @@
             self.element_type = data_types[element_type_name]()
         elif self.elements:
             raise SchemaError("'type' not found in elements schema", path)
         else:
             self.element_type = AnyDataType()
         # Save recursively detected data type (i.e. from 'schema' --> subschema)
         self.element_type = self.element_type.build_schema(
-            schema=self.elements, path=path+'<.>',
+            schema=self.elements, path=path,
             data_types=data_types, subschemas=subschemas, subpath=subpath)
         return self
     
     def build_sub_references(self, data :any, path :str, references :References):
         for id, element in data.items():
-            new_path = str(id) if not path else "%s.%s" % (path, str(id))
             self.element_type.build_references(data=element,
-                                            path=new_path,
+                                            path=path + '{id}',
                                             references=references)
     
     def autogenerate_data(self, data :any, path :str, references :References):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
         new_dict = dict()
         for id, element in data.items():
-            new_path = str(id) if not path else "%s.%s" % (path, str(id))
+            new_path = path + '{}' + str(id)
             _data, _FL = self.element_type.autogenerate_data(data=element,
                                                             path=new_path,
                                                             references=references)
             new_dict[id] = _data
             FL += _FL
         return new_dict, FL
 
     def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
         FL = FindingsList()
+        path = path + '{}'
         if self.minimum and len(data) < self.minimum:
             FL.append(WrongValueFinding(
                         path=path,
-                        message='Attribute (ID) count is lower than minimum %d' % self.minimum))
+                        message='Attribute count is lower than minimum %d' % self.minimum))
         elif self.maximum is not None and len(data) > self.maximum:
             FL.append(WrongValueFinding(
                         path=path,
-                        message='Attribute (ID) count is greater than maximum %d' % self.maximum))
+                        message='Attribute count is greater than maximum %d' % self.maximum))
 
         for id, element in data.items():
             _FL = FindingsList()
+            id_path = path + str(id)
             if self.id_type == 'string':
                 if not isinstance(id, str):
                     _FL.append(WrongValueFinding(
-                        path=path, message="Attribute (ID) '%s' is not a string" % str(id)))
+                        path=id_path, message="Attribute is not a string"))
                 elif self.id_minimum and len(id) < self.id_minimum:
                     _FL.append(WrongValueFinding(
-                        path=path,
-                        message="String length of attribute (ID) '%s' is lower than minimum %d" %
-                                (id, self.id_minimum)))
+                        path=id_path,
+                        message="String length of attribute is lower than minimum %d" %
+                                self.id_minimum))
                 elif self.id_maximum is not None and len(id) > self.id_maximum:
                     _FL.append(WrongValueFinding(
-                        path=path,
-                        message="String length of attribute (ID) '%s' is greater than maximum %d" %
-                                (id, self.id_maximum)))
+                        path=id_path,
+                        message="String length of attribute is greater than maximum %d" %
+                                self.id_maximum))
                 else:
                     not_allowed = False
                     for regex in self.not_allowed_ids:
                         if re.match(regex, id):
                             _FL.append(WrongValueFinding(
-                                path=path,
-                                message="Attribute '%s' is not allowed" % id))
+                                path=id_path,
+                                message="Attribute is not allowed"))
                             not_allowed = True
                     if not not_allowed and self.allowed_ids:
                         allowed = False
                         for regex in self.allowed_ids:
                             if re.match(regex, id):
                                 allowed = True
                                 break
                         if not allowed:
                             _FL.append(WrongValueFinding(
-                                    path=path,
-                                    message="Attribute '%s' does not match any allowed value" % id))
+                                    path=id_path,
+                                    message="Attribute does not match any allowed value"))
                     
             else: # id_type == 'integer'
                 if not isinstance(id, int):
                     _FL.append(WrongValueFinding(
-                        path=path, message="Attribute (ID) '%s' is not a integer" % str(id)))
+                        path=id_path, message="Attribute is not a integer"))
                 elif self.id_minimum and id < self.id_minimum:
                     _FL.append(WrongValueFinding(
-                        path=path,
-                        message="Attribute (ID) '%d' is lower than minimum %d" % (id, self.id_minimum)))
+                        path=id_path,
+                        message="Attribute is lower than minimum %d" % self.id_minimum))
                 elif self.id_maximum is not None and id > self.id_maximum:
                     _FL.append(WrongValueFinding(
-                        path=path,
-                        message="Attribute (ID) '%d' is greater than maximum %d" % (id, self.id_maximum)))
+                        path=id_path,
+                        message="Attribute is greater than maximum %d" % self.id_maximum))
                 elif id in self.not_allowed_ids:
                     _FL.append(WrongValueFinding(
-                        path=path,
-                        message="Attribute (ID) '%d' is not allowed" % id, ))
+                        path=id_path,
+                        message="Attribute is not allowed"))
                 elif self.allowed_ids and id not in self.allowed_ids:
                     _FL.append(WrongValueFinding(
-                        path=path,
-                        message="Attribute (ID) '%d' is not an allowed value" % id, ))
+                        path=id_path,
+                        message="Attribute is not an allowed value"))
 
             if not _FL:
-                new_path = str(id) if not path else "%s.%s" % (path, str(id))
                 FL += (self.element_type.validate_data(
-                    data=element, path=new_path, references=references))
+                    data=element, path=id_path, references=references))
             else:
                 FL += _FL
         return FL
 
     def verify_reference(self, data :any, path :str, references=References()) -> FindingsList:
         if not self.data_matches_type(data) or OPT.NONE in self.ref_OPT:
             return []
         results = list()
         for id in data.keys():
-            element = ReferenceElement(self.ref_key, path, id, self.ref_OPT)
+            id_path = path + '{}' + id
+            element = ReferenceElement(self.ref_key, id_path, id, self.ref_OPT)
             other = references.same_unique(element)
             if other is not None:
                 if references.namespace != other.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
-                results.append(UniqueErrorFinding(path=path, message="ID '%s' already used at '%s'" % (str(id), _path)))
+                results.append(UniqueErrorFinding(
+                    path=id_path, message="ID '%s' already used at '%s'" % (str(id), _path)))
             else:
                 references.add_element(element)
         return results
```

### Comparing `cd2t-1.4.0/cd2t/types/multitype.py` & `cd2t-1.5.0/cd2t/types/multitype.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/types/object.py` & `cd2t-1.5.0/cd2t/types/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.autogenerate = True
         return
     
     def build_schema(self, schema :dict, path :str,
                      data_types :dict, subschemas :dict,
                      subpath :list):
         self.__init__()
+        path = path + '{}'
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
         if self.attributes is None:
             # No other options should be set:
             for option, required, cls, init_value in self.options:
                 if exec("self." + option + " != init_value"):
                     raise SchemaError("Option 'attribute' is omitted, no other option is expected.")
@@ -65,68 +66,67 @@
                     raise SchemaError("Required attribute '%s' " % req_attr +\
                                       "for dependency '%s' not in attributes" % dep_attr, path)
             for ex_attr in dep_info.get('excludes', []):
                 if not self._attribute_in_list(ex_attr, list(self.attributes.keys()), self.allow_regex_attributes):
                     raise SchemaError("Excluded attribute '%s' " % ex_attr +\
                                       "for dependency '%s' not in attributes" % dep_attr, path)
         #
-        if path:
-            path = path + '.'
         for a_name, a_schema in self.attributes.items():
+            a_path = path + a_name
             if not isinstance(a_schema, dict):
-                raise SchemaError("Attribute '%s' schema is not a dictionary" % a_name, path)
+                raise SchemaError("Schema is not a dictionary", a_path)
             if 'type' in a_schema.keys():
                 type_name = a_schema['type']
                 if type_name not in data_types.keys():
-                    raise SchemaError("Attribute '%s' data type '%s' not found" % (a_name, type_name), path)
+                    raise SchemaError("Data type '%s' not found" % type_name, a_path)
                 data_type = data_types[type_name]()
             else:
                 data_type = AnyDataType()
             # Save recursively detected data type (i.e. from 'schema' --> subschema)
             _data_type = data_type.build_schema(a_schema, path + a_name, data_types, subschemas, subpath)
             self.attributes_objects[a_name] = _data_type
         return self
     
     def build_references(self, data :any, path :str, references :References):
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 continue
-            new_path = a_name if not path else "%s.%s" % (path, a_name)
-            data_type.build_references(a_data, new_path, references)
+            a_path = path + '{}' + a_name
+            data_type.build_references(a_data, a_path, references)
     
     def autogenerate_data(self, data :any, path :str, references :References):
         FL = FindingsList()
         if data is None or not self.data_matches_type(data):
             return data, FL
         new_data = dict()
         processed_attributes = list()
         if not self.allow_regex_attributes and self.autogenerate:
             for a_name, data_type in self.attributes_objects.items():
                 processed_attributes.append(a_name)
-                new_path = a_name if not path else "%s.%s" % (path, a_name)
+                a_path = path + '{}' + a_name
                 _FL = FindingsList()
                 if a_name not in data.keys():
                     _data, _FL = data_type.autogenerate_data(
-                        data=None, path=new_path, references=references)
+                        data=None, path=a_path, references=references)
                     if _FL:
                         new_data[a_name] = _data
                 else:
-                    _data, _FL = data_type.autogenerate_data(data[a_name], new_path, references)
+                    _data, _FL = data_type.autogenerate_data(data[a_name], a_path, references)
                     new_data[a_name] = _data
                 FL += _FL
         for a_name, a_data in data.items():
             if a_name in processed_attributes:
                 continue
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 new_data[a_name] = a_data
                 continue
-            new_path = a_name if not path else "%s.%s" % (path, a_name)
-            _data, _FL = data_type.autogenerate_data(a_data, new_path, references)
+            a_path = path + '{}' + a_name
+            _data, _FL = data_type.autogenerate_data(a_data, a_path, references)
             new_data[a_name] = _data
             FL += _FL
         return new_data, FL
     
     @staticmethod
     def _attribute_in_list(attribute :str, attributes :list, regex_allowed=False) -> bool:
         if regex_allowed:
@@ -142,72 +142,74 @@
                                                    full_match=True)
         return self.attributes_objects.get(name, None)
 
     def verify_data(self, data :any, path :str, references=References()) -> FindingsList:
         FL = FindingsList()
         if self.attributes is None:
             return FL
+        path = path + '{}'
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 if self.ignore_undefined_attributes:
                     continue
                 FL.append(ValidationFinding(path=path, message="Invalid attribute '%s'" % a_name))
                 continue
-            new_path = a_name if not path else "%s.%s" % (path, a_name)
-            FL += data_type.validate_data(data=a_data, path=new_path, references=references)
+            a_path = path + a_name
+            FL += data_type.validate_data(data=a_data, path=a_path, references=references)
         for req_attr in self.required_attributes:
             found_in_data_keys = False
             if self.allow_regex_attributes:
                 if regex_matches_in_string_list(
                                                         regex=req_attr,
                                                         strings=list(data.keys()),
                                                         full_match=True):
                     found_in_data_keys = True
             elif req_attr in data.keys():
                 found_in_data_keys = True
             if not found_in_data_keys:
                 FL.append(ValidationFinding(
-                    path = path,
-                    message = "Required attribute '%s' missing" % req_attr))
+                    path = path + req_attr,
+                    message = "Required attribute missing"))
         for attr_name, dep_info in self.dependencies.items():
             if not attr_name in data.keys():
                 continue
+            a_path = path + attr_name
             for req_attr in dep_info.get('requires', list()):
                 if self.allow_regex_attributes:
                     if not regex_matches_in_string_list(
                                                             regex=req_attr,
                                                             strings=list(data.keys()),
                                                             full_match=True):
                         FL.append(ValidationFinding(
-                            path = path,
-                            message = "No attribute matches regex requirement '%s' for attribute '%s'" % (req_attr, attr_name)))
+                            path = a_path,
+                            message = "No attribute matches regex requirements"))
                 elif req_attr not in data.keys():
                     FL.append(ValidationFinding(
-                        path = path,
-                        message = "Required attribute '%s' for attribute '%s' missing" % (req_attr, attr_name)))
+                        path = a_path,
+                        message = "Required attribute '%s' missing" % req_attr))
             for ex_attr in dep_info.get('excludes', list()):
                 match = None
                 if self.allow_regex_attributes:
                     match = regex_matches_in_string_list(
                                                             regex=ex_attr,
                                                             strings=list(data.keys()),
                                                             full_match=True)
                     if match:
                         found_in_data_keys = True
                 elif ex_attr in data.keys():
                     match = ex_attr
                 if match:
                     FL.append(ValidationFinding(
-                        path = path,
-                        message = "Excluded attribute '%s' for attribute '%s' found" % (match, attr_name)))
+                        path = a_path,
+                        message = "Excluded attribute '%s' found" % match))
         return FL
     
     def get_reference_data(self, data: any, path :str) -> any:
         ref_data = list()
         results = list()
         for ref_attr in self.reference_attributes:
             if ref_attr not in data.keys():
-                results.append(ValidationFinding(path = path,
+                results.append(ValidationFinding(path = path+'{}',
                                            message = "Reference attribute '%s' missing" % ref_attr))
             ref_data.append(data[ref_attr])
         return ref_data, results
```

### Comparing `cd2t-1.4.0/cd2t/types/schema.py` & `cd2t-1.5.0/cd2t/types/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/cd2t/types/string.py` & `cd2t-1.5.0/cd2t/types/string.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/LICENSE` & `cd2t-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cd2t-1.4.0/README.md` & `cd2t-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.5.0**:
+- *New*: Integer Data Type - Autogenerate random value
+- *New*: Integer Data Type - Autogenerate default value
+- *New*: Improved Reference Findings
+- *Changed*: All Data Types - Schema and data path adjustment
+
 **Version 1.4.0**:
 - *New*: None Data Type added
 - *Fix*: Consumer namespace space lookup/linking failed, if producer was processed later.
 
 **Version 1.3.1**:
 - *Fix*: Schema Data Type - Validation failed
 
@@ -268,27 +274,31 @@
 - < int >
 # List of integers which values mustn't match.
 
 autogenerate: < bool | default -> false >
 # Requires 'reference.key' to be defined and not ''.
 # If no unique value could be generated, autogeneration fails.
 
+autogenerate_default: < int >
+# Generate this integer value if value is None. Ignores all other 'autogen' options
+
 autogenerate_maximum: < int >
 # Autogenerated integer must be lower or equals to this.
 # If omitted, 'maximum' key is upper limit
 
 autogenerate_minimum: < int >
 # Autogenerated integer must be greater or equals to this.
 # If omitted, 'minimum' key is lower limit
 
-autogenerate_find: < 'next_higher' | 'next_lower' | default -> 'next_higher' >
-# Tells autogenerate to try first available integer
-# starting at 'minimum' and increasing ('next_higher') or
-# starting at 'maximum' and decreasing ('next_lower').
-# If 'maximum' or 'minimum' is not specified, autogeneration starts at 1.
+autogenerate_find: < 'next_higher' | 'next_lower' | 'random' | default -> 'next_higher' >
+# Ignored, if 'autogenerate_default' is set.
+# Tells autogenerate to try first available integer value
+# starting at 'minimum' and increasing ('next_higher'),
+# starting at 'maximum' and decreasing ('next_lower') or
+# picking a random number within 'minimum' and 'maximum'.
 ```
 
 ### List Data Type
 **Description**  
 This data type represents a list of same data types.  
 If different data types are allowed in the list,
 use data type 'multitype' as elements.
```

### Comparing `cd2t-1.4.0/pyproject.toml` & `cd2t-1.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/cd2t",
 ]
 
 [project]
 name = "cd2t"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "cd2t validates data structure, data types and values with templates"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cd2t-1.4.0/PKG-INFO` & `cd2t-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cd2t
-Version: 1.4.0
+Version: 1.5.0
 Summary: cd2t validates data structure, data types and values with templates
 Project-URL: Homepage, https://gitlab.com/ko.no/cd2t
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/cd2t/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,20 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.5.0**:
+- *New*: Integer Data Type - Autogenerate random value
+- *New*: Integer Data Type - Autogenerate default value
+- *New*: Improved Reference Findings
+- *Changed*: All Data Types - Schema and data path adjustment
+
 **Version 1.4.0**:
 - *New*: None Data Type added
 - *Fix*: Consumer namespace space lookup/linking failed, if producer was processed later.
 
 **Version 1.3.1**:
 - *Fix*: Schema Data Type - Validation failed
 
@@ -284,27 +290,31 @@
 - < int >
 # List of integers which values mustn't match.
 
 autogenerate: < bool | default -> false >
 # Requires 'reference.key' to be defined and not ''.
 # If no unique value could be generated, autogeneration fails.
 
+autogenerate_default: < int >
+# Generate this integer value if value is None. Ignores all other 'autogen' options
+
 autogenerate_maximum: < int >
 # Autogenerated integer must be lower or equals to this.
 # If omitted, 'maximum' key is upper limit
 
 autogenerate_minimum: < int >
 # Autogenerated integer must be greater or equals to this.
 # If omitted, 'minimum' key is lower limit
 
-autogenerate_find: < 'next_higher' | 'next_lower' | default -> 'next_higher' >
-# Tells autogenerate to try first available integer
-# starting at 'minimum' and increasing ('next_higher') or
-# starting at 'maximum' and decreasing ('next_lower').
-# If 'maximum' or 'minimum' is not specified, autogeneration starts at 1.
+autogenerate_find: < 'next_higher' | 'next_lower' | 'random' | default -> 'next_higher' >
+# Ignored, if 'autogenerate_default' is set.
+# Tells autogenerate to try first available integer value
+# starting at 'minimum' and increasing ('next_higher'),
+# starting at 'maximum' and decreasing ('next_lower') or
+# picking a random number within 'minimum' and 'maximum'.
 ```
 
 ### List Data Type
 **Description**  
 This data type represents a list of same data types.  
 If different data types are allowed in the list,
 use data type 'multitype' as elements.
```

