# Comparing `tmp/melkit-0.1.4.tar.gz` & `tmp/melkit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melkit-0.1.4.tar", last modified: Mon Apr 10 10:57:54 2023, max compression
+gzip compressed data, was "melkit-0.1.6.tar", last modified: Thu Apr 13 16:24:56 2023, max compression
```

## Comparing `melkit-0.1.4.tar` & `melkit-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:57:54.370715 melkit-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 10:57:53.000000 melkit-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 10:57:53.000000 melkit-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:57:54.370715 melkit-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-10 10:57:53.000000 melkit-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:57:54.366715 melkit-0.1.4/melkit/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22679 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 10:57:53.000000 melkit-0.1.4/melkit/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:57:54.370715 melkit-0.1.4/melkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 10:57:54.000000 melkit-0.1.4/melkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 10:57:53.000000 melkit-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:57:54.370715 melkit-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-10 10:57:53.000000 melkit-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:24:56.990030 melkit-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 16:24:56.000000 melkit-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 16:24:56.000000 melkit-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 16:24:56.990030 melkit-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 16:24:56.000000 melkit-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:24:56.990030 melkit-0.1.6/melkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:24:56.990030 melkit-0.1.6/melkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 16:24:56.000000 melkit-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:24:56.990030 melkit-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 16:24:56.000000 melkit-0.1.6/setup.py
```

### Comparing `melkit-0.1.4/LICENSE` & `melkit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `melkit-0.1.4/README.md` & `melkit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `melkit-0.1.4/melkit/inputs.py` & `melkit-0.1.6/melkit/inputs.py`

 * *Files identical despite different names*

### Comparing `melkit-0.1.4/melkit/toolkit.py` & `melkit-0.1.6/melkit/toolkit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 MELGEN/MELCOR file manipulation tools.
 '''
 
 from pandas import DataFrame, read_csv
 
-from os import remove
+from os import remove, rename
 from re import search, match, findall
 from json import dumps
 
 from typing import List, Union
 
 from .exceptions import ParseException
 from .inputs import Object, CV, FL, CF
@@ -23,15 +23,15 @@
     def __init__(self, filename: str):
         self._filename = filename
 
         self._cv_list = self._read_cvs()
         self._fl_list = self._read_fls()
         self._cf_list = self._read_cfs()
 
-#------------------------ OBJECT MANIPULATION TOOLS -----------------------#
+# ------------------------ OBJECT MANIPULATION TOOLS -----------------------#
 
     def _read_object(self, id_regex: str) -> List[Object]:
         '''
         Looks for objects in the input file according to a given ID regex
         '''
         ids, objs = [], []
         with open(self._filename, 'r') as file:
@@ -53,15 +53,15 @@
         return self._read_object(r'\bCV\d{3}00\b')
 
     def _read_fls(self) -> List[FL]:
         '''
         Looks for FLs in the input file and returns them as a list of FL objects.
         '''
         return self._read_object(r'\bFL\d{3}00\b')
-    
+
     def _read_cfs(self) -> List[CF]:
         '''
         Looks for CFs in the input file and returns them as a list of CF objects.
         '''
         return self._read_object(r'\bCF\d{3,8}00\b')
 
     def get_cv(self, cv_id: str) -> CV:
@@ -194,15 +194,15 @@
         return FL(fl_data)
 
     def get_cf(self, cf_id: str) -> CF:
         '''
         Searches for a CF in the input file and returns it as a CF object.
         '''
         cf_data = {}
-        
+
         arg_c = 0   # arg counter
 
         with open(self._filename, 'r') as file:
             for line in file:
                 if line.startswith(cf_id):
                     record = line.split()
                     record_id = record[0]
@@ -212,28 +212,29 @@
 
                     try:
                         if termination == '00':
                             record_data['CFNAME'] = record[1]
                             record_data['CFTYPE'] = record[2]
                             record_data['NCFARG'] = record[3]
                             record_data['CFSCAL'] = record[4]
-                            record_data['CFADCN'] = record[5] if len(record) > 5 else 0.0
+                            record_data['CFADCN'] = record[5] if len(
+                                record) > 5 else 0.0
                         elif termination == '01':
                             if record[1] in ['.TRUE.', '.FALSE.']:
                                 record_data['LCFVAL'] = record[1]
                             else:
-                                record_data['CFVALR'] = record[1] 
+                                record_data['CFVALR'] = record[1]
                         elif termination == '02':
                             record_data['ICFLIM'] = record[1]
                             if int(record[1]) in [1, 2, 3]:
                                 record_data['CFLIML'] = record[2]
                             if int(record[1]) in [2, 3]:
                                 record_data['CFLIMU'] = record[3]
                         elif match(r'0[3-4]', termination):
-                            record_data['FIELDS'] = record[1] # Fixable
+                            record_data['FIELDS'] = record[1]  # Fixable
                         elif termination == '05':
                             record_data['CLASS'] = record[1]
                         elif termination == '06':
                             record_data['MSGFIL'] = record[1]
                             if int(record[1]) in [1, 2]:
                                 record_data['SWTMSG'] = record[2]
                         elif match(r'[10-99]', termination):
@@ -258,129 +259,86 @@
         return self._cv_list
 
     def get_fl_list(self) -> List[FL]:
         '''
         Return the list of CVs in parsed file.
         '''
         return self._fl_list
-    
+
     def get_cf_list(self) -> List[CF]:
         '''
         Return the list of CFs in parsed file.
         '''
         return self._cf_list
 
-    def remove_object(self, obj_id: str, src_file: str = None, new_file: str = None) -> None:
+    def remove_object(self, obj_id: str, overwrite: bool = False, new_file: str = None) -> None:
         '''
         Deletes an object from the input file.
         '''
 
-        src_file = src_file or self._filename
-        new_file = new_file or self._filename + '_NEW'
+        src_file = self._filename
+        new_file = new_file or src_file + '_NEW'
 
         with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
             for line in f1:
                 if not line.startswith(obj_id):
                     f2.write(line)
 
-    def remove_objects(self, obj_ids: List[str], src_file: str = None, new_file: str = None) -> None:
-        '''
-        Deletes a list of objects from the input file.
-        '''
-
-        src_file = src_file or self._filename
-        new_file = new_file or self._filename + '_NEW'
+        if overwrite:
+            remove(src_file)
+            rename(new_file, src_file)
 
-        with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
-            for line in f1:
-                if line[:5] not in obj_ids:
-                    f2.write(line)
-
-    def write_object(self, obj: Object, src_file: str = None, new_file: str = None) -> None:
+    def write_object(self, obj: Object, overwrite: bool = False, new_file: str = None) -> None:
         '''
         Writes a new object in the input file.
         '''
 
-        src_file = src_file or self._filename
-        new_file = new_file or self._filename + '_NEW'
+        src_file = self._filename
+        new_file = new_file or src_file + '_NEW'
 
         with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
             written = False
             for line in f1:
                 if line.startswith('.') and not written:
                     f2.write('*\n' + str(obj) + '*\n' + line)
                     written = True
                 else:
                     f2.write(line)
 
-    def write_objects(self, obj_list: List[Object], src_file: str = None, new_file: str = None) -> None:
-        '''
-        Writes a new object in the input file.
-        '''
-
-        src_file = src_file or self._filename
-        new_file = new_file or self._filename + '_NEW'
-
-        with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
-            written = False
-            for line in f1:
-                if line.startswith('.') and not written:
-                    for obj in obj_list:
-                        f2.write('*\n' + str(obj) + '*\n')
-                    f2.write(line)
-                    written = True
-                else:
-                    f2.write(line)
+        if overwrite:
+            remove(src_file)
+            rename(new_file, src_file)
 
-    def update_object(self, obj: Object, src_file: str = None, new_file: str = None) -> None:
+    def update_object(self, obj: Object, overwrite: bool = False, new_file: str = None) -> None:
         '''
         Updates object input information.
         '''
 
-        src_file = src_file or self._filename
-        tmp_file = self._filename + '_TMP'
-        new_file = new_file or self._filename + '_NEW'
+        src_file = self._filename
+        new_file = new_file or src_file + '_NEW'
 
         obj_id = obj.get_id()
 
-        self.remove_object(obj_id, new_file=tmp_file)
-        self.write_object(obj, src_file=tmp_file, new_file=new_file)
-
-        remove(self._filename + '_TMP')
-
-    def update_objects(self, obj_list: Object, src_file: str = None, new_file: str = None) -> None:
-        '''
-        Updates objects input information.
-        '''
-
-        src_file = src_file or self._filename
-        tmp_file = self._filename + '_TMP'
-        new_file = new_file or self._filename + '_NEW'
-
-        obj_ids = [obj.get_id() for obj in obj_list]
-
-        self.remove_objects(obj_ids, new_file=tmp_file)
-        self.write_objects(obj_list, src_file=tmp_file, new_file=new_file)
-
-        remove(self._filename + '_TMP')
-
-    def clear_objects(self, src_file: str = None, new_file: str = None) -> None:
-        '''
-        Removes every CV or FL in the input file.
-        '''
+        if overwrite:
+            self.remove_object(obj_id, overwrite=True)
+            self.write_object(obj, overwrite=True)
+        else:
+            tmp_file = src_file + '_TMP'
+            self.remove_object(obj_id, new_file=tmp_file)
+            with open(tmp_file, 'r') as f1, open(new_file, 'w') as f2:
+                written = False
+                for line in f1:
+                    if line.startswith('.') and not written:
+                        f2.write('*\n' + str(obj) + '*\n' + line)
+                        written = True
+                    else:
+                        f2.write(line)
+            remove(tmp_file)
 
-        src_file = src_file or self._filename
-        new_file = new_file or self._filename + '_NEW'
-
-        with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
-            for line in f1:
-                if line[:2] not in ['CV', 'FL', 'CF', 'TF']:
-                    f2.write(line)
-
-#-------------------------------- EDF TOOLS -------------------------------#
+# -------------------------------- EDF TOOLS -------------------------------#
 
     def get_edf_vars(self) -> List[str]:
         '''
         Returns a list of variable names based on EDF records in file.
         '''
         keys = ['TIME']
         with open(self._filename, 'r') as file:
@@ -420,15 +378,15 @@
         '''
         Plot an EDF variable value along time.
         '''
         import matplotlib.pyplot as plt
         self.as_dataframe(datafile).plot(x='TIME', y=y_var)
         plt.show()
 
-#----------------------------- CONNECTION TOOLS ---------------------------#
+# ----------------------------- CONNECTION TOOLS ---------------------------#
 
     def get_fl_connections(self, cv_id: str) -> List[FL]:
         '''
         Get those FLs connected to a given CV
         '''
         fl_connected = []
         for fl in self._fl_list:
@@ -446,15 +404,14 @@
             if cv_id[2:] == fl.get_field('KCVFM'):
                 cv_connected.append(self.id_search(
                     self._cv_list, 'CV' + fl.get_field('KCVTO')))
             elif cv_id[2:] == fl.get_field('KCVTO'):
                 cv_connected.append(self.id_search(
                     self._cv_list, 'CV' + fl.get_field('KCVFM')))
         return cv_connected
-    
 
     def get_connected_cfs(self, obj_id: str) -> List[CF]:
         '''
         Get those CFs directly or indirectly connected to a given Object.
         - If the Object is an FL, the CF associated with the CFnnnTk record is returned and, recursively, all CFs on which this CF depends are added.
         - If the object is a CF, that CF and its dependencies are returned.
         '''
@@ -469,23 +426,22 @@
                     cf_connected.append(self.get_cf(cf_id))
                     # Recursion for interdependent CFs
                     cf_connected += self.get_connected_cfs(cf_id)
         # Get those CFs related to a given CF
         elif obj_id.startswith('CF'):
             cf = self.get_cf(obj_id)
             cf_values = findall(r'\bCFVALU\.\d+\b', dumps(cf.records))
-            for value in cf_values: 
+            for value in cf_values:
                 dot_pos = value.find('.')
                 cf_id = 'CF' + value[dot_pos + 1:]
                 cf_connected.append(self.get_cf(cf_id))
                 cf_connected += self.get_connected_cfs(cf_id)
 
         return cf_connected
 
-
     def create_submodel(self, cv_id: str, new_file: str = None) -> Union[List[CV], List[FL]]:
         '''
         Creates a submodel related to a given CV. Those neighbour CVs are made time-independent.
         '''
 
         new_file = new_file or self._filename + '_SUB'
         tmp_file = self._filename + '_TMP'
@@ -502,15 +458,15 @@
         self.write_objects(sub_cvs + sub_fls,
                            src_file=tmp_file, new_file=new_file)
 
         remove(self._filename + '_TMP')
 
         return sub_cvs, sub_fls
 
-#------------------------------- AUX TOOLS --------------------------------#
+# ------------------------------- AUX TOOLS --------------------------------#
 
     def get_used_ids(self, obj_list: List[Object]) -> List[str]:
         '''
         Returns a sorted list of used IDs from a list of objects.
         '''
         used_ids = []
         for obj in obj_list:
@@ -537,15 +493,15 @@
         Returns a single-column used IDs DataFrame from an object list. Also exports it as a CSV file.
         '''
         ids = self.get_used_ids(obj_list)
         df = DataFrame(ids, columns=['IDs'])
         df.to_csv(title, index=False)
 
         return df
-    
+
     def available_to_csv(self, obj_list: List[Object], title='./available.csv') -> DataFrame:
         '''
         Returns a single-column available IDs DataFrame from an object list. Also exports it as a CSV file.
         '''
         ids = self.get_available_ids(obj_list)
         df = DataFrame(ids, columns=['IDs'])
         df.to_csv(title, index=False)
```

### Comparing `melkit-0.1.4/setup.py` & `melkit-0.1.6/setup.py`

 * *Files identical despite different names*

