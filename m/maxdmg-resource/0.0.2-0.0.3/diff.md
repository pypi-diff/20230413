# Comparing `tmp/maxdmg_resource-0.0.2.tar.gz` & `tmp/maxdmg_resource-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxdmg_resource-0.0.2.tar", last modified: Tue Mar 21 18:38:53 2023, max compression
+gzip compressed data, was "maxdmg_resource-0.0.3.tar", last modified: Thu Apr 13 11:07:28 2023, max compression
```

## Comparing `maxdmg_resource-0.0.2.tar` & `maxdmg_resource-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.810571 maxdmg_resource-0.0.2/
--rw-r--r--   0 at        (1000) at        (1000)      344 2023-03-21 18:38:53.810571 maxdmg_resource-0.0.2/PKG-INFO
--rw-r--r--   0 at        (1000) at        (1000)        0 2023-03-21 18:01:10.000000 maxdmg_resource-0.0.2/README.md
--rw-r--r--   0 at        (1000) at        (1000)      523 2023-03-21 18:38:38.000000 maxdmg_resource-0.0.2/pyproject.toml
--rw-r--r--   0 at        (1000) at        (1000)       38 2023-03-21 18:38:53.810571 maxdmg_resource-0.0.2/setup.cfg
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.803904 maxdmg_resource-0.0.2/src/
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.807237 maxdmg_resource-0.0.2/src/maxdmg_resource/
--rw-r--r--   0 at        (1000) at        (1000)     1322 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/__init__.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.810571 maxdmg_resource-0.0.2/src/maxdmg_resource/app/
--rw-r--r--   0 at        (1000) at        (1000)      851 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/API.py
--rwxr-xr-x   0 at        (1000) at        (1000)     1247 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Config.py
--rwxr-xr-x   0 at        (1000) at        (1000)     2622 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Exceptions.py
--rwxr-xr-x   0 at        (1000) at        (1000)     3199 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Graph.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.810571 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Loader/
--rwxr-xr-x   0 at        (1000) at        (1000)     9684 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Loader/Loader.py
--rw-r--r--   0 at        (1000) at        (1000)     1315 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Loader/Models.py
--rw-r--r--   0 at        (1000) at        (1000)      227 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Loader/__init__.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.810571 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/
--rw-r--r--   0 at        (1000) at        (1000)      383 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/Doc.py
--rw-r--r--   0 at        (1000) at        (1000)     1072 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/Form.py
--rwxr-xr-x   0 at        (1000) at        (1000)     1497 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/State.py
--rwxr-xr-x   0 at        (1000) at        (1000)      799 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/Transition.py
--rw-r--r--   0 at        (1000) at        (1000)       15 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/Typedefs.py
--rw-r--r--   0 at        (1000) at        (1000)      223 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/__init__.py
-drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-03-21 18:38:53.807237 maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/
--rw-r--r--   0 at        (1000) at        (1000)      344 2023-03-21 18:38:53.000000 maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/PKG-INFO
--rw-r--r--   0 at        (1000) at        (1000)      773 2023-03-21 18:38:53.000000 maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/SOURCES.txt
--rw-r--r--   0 at        (1000) at        (1000)        1 2023-03-21 18:38:53.000000 maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/dependency_links.txt
--rw-r--r--   0 at        (1000) at        (1000)       39 2023-03-21 18:38:53.000000 maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/requires.txt
--rw-r--r--   0 at        (1000) at        (1000)       16 2023-03-21 18:38:53.000000 maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/top_level.txt
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.864324 maxdmg_resource-0.0.3/
+-rw-r--r--   0 at        (1000) at        (1000)      344 2023-04-13 11:07:28.864324 maxdmg_resource-0.0.3/PKG-INFO
+-rw-r--r--   0 at        (1000) at        (1000)        0 2023-03-21 18:01:10.000000 maxdmg_resource-0.0.3/README.md
+-rw-r--r--   0 at        (1000) at        (1000)      523 2023-04-13 10:53:51.000000 maxdmg_resource-0.0.3/pyproject.toml
+-rw-r--r--   0 at        (1000) at        (1000)       38 2023-04-13 11:07:28.864324 maxdmg_resource-0.0.3/setup.cfg
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.857658 maxdmg_resource-0.0.3/src/
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.857658 maxdmg_resource-0.0.3/src/maxdmg_resource/
+-rw-r--r--   0 at        (1000) at        (1000)     1368 2023-04-13 10:53:03.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/__init__.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.860991 maxdmg_resource-0.0.3/src/maxdmg_resource/app/
+-rw-r--r--   0 at        (1000) at        (1000)      897 2023-04-13 10:53:03.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/API.py
+-rwxr-xr-x   0 at        (1000) at        (1000)     1247 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Config.py
+-rwxr-xr-x   0 at        (1000) at        (1000)     2622 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Exceptions.py
+-rwxr-xr-x   0 at        (1000) at        (1000)     4147 2023-04-13 10:53:03.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Graph.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.864324 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/
+-rw-r--r--   0 at        (1000) at        (1000)      553 2023-04-13 10:53:03.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/Errors.py
+-rwxr-xr-x   0 at        (1000) at        (1000)    10377 2023-04-13 10:53:03.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/Loader.py
+-rw-r--r--   0 at        (1000) at        (1000)     1315 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/Models.py
+-rw-r--r--   0 at        (1000) at        (1000)      227 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/__init__.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.864324 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/
+-rw-r--r--   0 at        (1000) at        (1000)      383 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/Doc.py
+-rw-r--r--   0 at        (1000) at        (1000)     1072 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/Form.py
+-rwxr-xr-x   0 at        (1000) at        (1000)     1497 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/State.py
+-rwxr-xr-x   0 at        (1000) at        (1000)      799 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/Transition.py
+-rw-r--r--   0 at        (1000) at        (1000)       15 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/Typedefs.py
+-rw-r--r--   0 at        (1000) at        (1000)      223 2023-03-21 18:00:43.000000 maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/__init__.py
+drwxr-xr-x   0 at        (1000) at        (1000)        0 2023-04-13 11:07:28.860991 maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/
+-rw-r--r--   0 at        (1000) at        (1000)      344 2023-04-13 11:07:28.000000 maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/PKG-INFO
+-rw-r--r--   0 at        (1000) at        (1000)      814 2023-04-13 11:07:28.000000 maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 at        (1000) at        (1000)        1 2023-04-13 11:07:28.000000 maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 at        (1000) at        (1000)       39 2023-04-13 11:07:28.000000 maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/requires.txt
+-rw-r--r--   0 at        (1000) at        (1000)       16 2023-04-13 11:07:28.000000 maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/top_level.txt
```

### Comparing `maxdmg_resource-0.0.2/pyproject.toml` & `maxdmg_resource-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0", 
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name    = "maxdmg_resource"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="tonotonokon" },
 ]
 dependencies = [
     "python-dotenv==1.0.0",
     "pyairtable==1.4.0",
 ]
```

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/__init__.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,13 +30,14 @@
              AIRTABLE_CONFIG_TABLE_ID,
              AIRTABLE_CONFIG_TABLE_VIEW_ID
         ) 
 
         return {
             'graph'         : loader.graph,
             'forms'         : loader.forms,
-            'docs'          : loader.docs
+            'docs'          : loader.docs,
+            'errors'        : loader.errors,
         }
 
     def LoadFromConfig(self, config):
         return self.Load(**(vars(config)))
```

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/API.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/API.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,10 +20,11 @@
             config.AIRTABLE_CONFIG_TABLE_ID,
             config.AIRTABLE_CONFIG_TABLE_MAIN_VIEW_ID
         )
 
         return {
             'graph'         : loader.graph,
             'forms'         : loader.forms,
-            'docs'          : loader.docs
+            'docs'          : loader.docs,
+            'errors'        : loader.errors,
         }
```

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Config.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Config.py`

 * *Files identical despite different names*

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Exceptions.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Exceptions.py`

 * *Files identical despite different names*

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Loader/Loader.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/Loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,55 @@
 from pyairtable  import Table
-from typing      import Dict, Tuple
-
-from ..Types     import (State, StateType, StateBehavior, 
-                         Transition, TransitionType, 
-                         Form, FormType, Doc,
-                         ID_TYPE)
-from ..Graph     import Graph
-from ..Exceptions import UnknownFormType, TableIsEmpty
-from .Models     import (StateFieldsConsts, StateBehaviorConsts, 
-                         TransitionFieldConsts, TransitionTypesConsts, 
-                         FormFieldConsts, DocFieldConsts)
+from typing      import (
+    Dict, 
+    Tuple,
+    Optional,
+)
+from ..Types     import (
+    State, 
+    StateType, 
+    StateBehavior, 
+    Transition, 
+    TransitionType, 
+    Form, 
+    FormType, 
+    Doc, 
+    ID_TYPE
+)
+from ..Graph     import (
+    Graph,
+)
+from ..Exceptions import (
+    UnknownFormType, 
+    TableIsEmpty,
+)
+from .Models     import (
+    StateFieldsConsts, 
+    StateBehaviorConsts, 
+    TransitionFieldConsts, 
+    TransitionTypesConsts, 
+    FormFieldConsts, 
+    DocFieldConsts
+)
+from .Errors    import (
+    Errors,
+)
 
 
 class Loader():
     def __init__(self):
         self.states_records         = list()
         self.transitions_records    = list()
         self.forms_records          = list()
         self.config_records         = list()
         self.states_external        = list()
 
         self.forms : Dict[ID_TYPE, Form] = dict()
         self.docs  : Dict[ID_TYPE, Doc]  = dict()
+        self.errors: List[Tuple[str, Optional]] = list()
 
         self.graph                  = Graph()
 
     def load(self,
              AIRTABLE_API_KEY, 
              AIRTABLE_BASE_ID,
              AIRTABLE_STATES_TABLE_ID,
@@ -61,14 +85,18 @@
             ext_data = ext['external_table_data']
             loader = Loader()
             loader.load(AIRTABLE_API_KEY, *ext_data.splitlines())
 
             self.graph.AttachAnotherGraph(loader.graph, ext)
             self.forms.update(loader.forms)
             self.docs.update(loader.docs)
+            self.errors.extend(loader.errors)
+
+        self.errors.extend(self.graph.errors)
+        
     
     def load_tables(
             self,
             AIRTABLE_API_KEY, 
             AIRTABLE_BASE_ID,
             AIRTABLE_STATES_TABLE_ID,
             AIRTABLE_STATES_TABLE_MAIN_VIEW_ID,
@@ -80,41 +108,45 @@
             AIRTABLE_CONFIG_TABLE_MAIN_VIEW_ID):
         states_table        = Table(AIRTABLE_API_KEY, 
                                     AIRTABLE_BASE_ID,
                                     AIRTABLE_STATES_TABLE_ID)
         self.states_records = states_table.all( 
             view=AIRTABLE_STATES_TABLE_MAIN_VIEW_ID)
         if len(self.states_records) == 0:
-            raise TableIsEmpty('States')
+            self.errors.append((Errors.STATES_TABLE_EMPTY, ))
+            #raise TableIsEmpty('States')
 
         transitions_table   = Table(AIRTABLE_API_KEY, 
                                     AIRTABLE_BASE_ID,
                                     AIRTABLE_TRANSITIONS_TABLE_ID)
         self.transitions_records = transitions_table.all( 
             view=AIRTABLE_TRANSITION_TABLE_MAIN_VIEW_ID)
         if len(self.transitions_records) == 0:
-            raise TableIsEmpty('Transitions')
+            self.errors.append((Errors.TRANSITIONS_TABLE_EMPTY, ))
+            #raise TableIsEmpty('Transitions')
 
         forms_table         = Table(AIRTABLE_API_KEY, 
                                     AIRTABLE_BASE_ID,
                                     AIRTABLE_FORMS_TABLE_ID,
                                 )
         self.forms_records  = forms_table.all(
             view=AIRTABLE_FORMS_TABLE_MAIN_VIEW_ID)
         if len(self.forms_records) == 0:
-            raise TableIsEmpty('Forms')
+            self.errors.append((Errors.FORMS_TABLE_EMPTY, ))
+            #raise TableIsEmpty('Forms')
     
         config_table        = Table(AIRTABLE_API_KEY, 
                                     AIRTABLE_BASE_ID,
                                     AIRTABLE_CONFIG_TABLE_ID,
                                 )
         self.config_records = config_table.all(
             view=AIRTABLE_CONFIG_TABLE_MAIN_VIEW_ID)
         if len(self.config_records) == 0:
-            raise TableIsEmpty('Config')
+            self.errors.append((Errors.CONFIG_TABLE_EMPTY, ))
+            #raise TableIsEmpty('Config')
 
     def process_states_records(self):
         for record in self.states_records:
             fields = record['fields']
             state : State = {
                 'id'        : record['id'],
                 'name'      : fields.get(
@@ -151,16 +183,16 @@
                     state['behavior']=StateBehavior.FORM
                 case StateBehaviorConsts.INPUT_CHECK:
                     state['behavior']=StateBehavior.INPUT_CHECK
                 case StateBehaviorConsts.EXTERNAL:
                     state['behavior']=StateBehavior.EXTERNAL
                     self.states_external.append(state)
                 case _:
-                    raise RuntimeError(
-                        f"State {state['name']} does not have a behavior set")
+                    self.errors.append( (Errors.STATE_NO_BEHAVIOR, state['name']) )
+                    #raise RuntimeError(f"State {state['name']} does not have a behavior set")
            
             self.graph.AddState(state)
         return self.graph.states
 
 
     def process_transitions_records(self):
         transitions : Dict[ID_TYPE, Transition] = dict()
@@ -169,59 +201,61 @@
 
             transition : Transition = {
                     'id' : record['id'],
                     'name' : fields.get(
                         TransitionFieldConsts.NAME, 'NO NAME'),
                     'type': TransitionType.UNKNOWN,
                     'source_id' : fields.get(
-                        TransitionFieldConsts.SOURCE, None)[0],
+                        TransitionFieldConsts.SOURCE, [None,])[0],
                     'target_id' : fields.get(
-                        TransitionFieldConsts.TARGET, None)[0],
+                        TransitionFieldConsts.TARGET, [None,])[0],
                     'form_elem_ids' : fields.get(
                         TransitionFieldConsts.FORM_CONDITIONS, list()),
             }
 
             cond = fields.get(
                 TransitionFieldConsts.TRANSITION_CONDITION)
             match cond:
                 case TransitionTypesConsts.CONDITIONAL:
                     transition['type']=TransitionType.CONDITIONAL
                 case TransitionTypesConsts.UNCONDITIONAL:
                     transition['type']=TransitionType.UNCONDITIONAL
                 case TransitionTypesConsts.STRICT:
                     transition['type']=TransitionType.STRICT
                 case _:
-                    raise RuntimeError(
-                      f"Transition {transition['name']} does not have a condition set")
+                    self.errors.append( (Errors.TRANSITION_NO_BEHAVIOR, transition['name']) )
+                    #raise RuntimeError(f"Transition {transition['name']} does not have a condition set")
 
             self.graph.AddTransition(transition)
         return self.graph.transitions
 
 
     def process_forms_records(self):
         for record in self.forms_records:
             fields = record['fields']
             form : Form = {
                 'id'        : record['id'],
-                'name'      : fields[FormFieldConsts.NAME],
+                'name'      : fields.get(
+                    FormFieldConsts.NAME, "NO NAME"),
                 'type'      : FormType.UNKNOWN,
-                'text'      : fields[FormFieldConsts.TEXT],
+                'text'      : fields.get(
+                    FormFieldConsts.TEXT, "NO TEXT"),
                 'state_id'  : fields.get(
                     FormFieldConsts.STATE_ID, None),
                 'tags'      : fields.get(
                     FormFieldConsts.TAGS, ''),
             }
 
             t = record['fields'].get(FormFieldConsts.TYPE, None)
             for ft in FormType:
                 if ft.value == t:
                     form['type'] = ft
                     break
             if form['type'] == FormType.UNKNOWN:
-                raise UnknownFormType(form['name'])
+                    self.errors.append( (Errors.FORM_TYPE_UNKNOWN, form['name']) )
 
             if form['state_id']:
                 form['state_id'] = form['state_id'][0]
 
             self.forms[form['id']] = form
         return self.forms
```

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Loader/Models.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Loader/Models.py`

 * *Files identical despite different names*

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/Form.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/Form.py`

 * *Files identical despite different names*

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/State.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/State.py`

 * *Files identical despite different names*

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource/app/Types/Transition.py` & `maxdmg_resource-0.0.3/src/maxdmg_resource/app/Types/Transition.py`

 * *Files identical despite different names*

### Comparing `maxdmg_resource-0.0.2/src/maxdmg_resource.egg-info/SOURCES.txt` & `maxdmg_resource-0.0.3/src/maxdmg_resource.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/maxdmg_resource.egg-info/dependency_links.txt
 src/maxdmg_resource.egg-info/requires.txt
 src/maxdmg_resource.egg-info/top_level.txt
 src/maxdmg_resource/app/API.py
 src/maxdmg_resource/app/Config.py
 src/maxdmg_resource/app/Exceptions.py
 src/maxdmg_resource/app/Graph.py
+src/maxdmg_resource/app/Loader/Errors.py
 src/maxdmg_resource/app/Loader/Loader.py
 src/maxdmg_resource/app/Loader/Models.py
 src/maxdmg_resource/app/Loader/__init__.py
 src/maxdmg_resource/app/Types/Doc.py
 src/maxdmg_resource/app/Types/Form.py
 src/maxdmg_resource/app/Types/State.py
 src/maxdmg_resource/app/Types/Transition.py
```

