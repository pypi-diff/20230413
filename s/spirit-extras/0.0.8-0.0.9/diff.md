# Comparing `tmp/spirit-extras-0.0.8.tar.gz` & `tmp/spirit-extras-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spirit-extras-0.0.8.tar", last modified: Wed Mar  9 18:47:19 2022, max compression
+gzip compressed data, was "spirit-extras-0.0.9.tar", last modified: Thu Mar 10 09:48:46 2022, max compression
```

## Comparing `spirit-extras-0.0.8.tar` & `spirit-extras-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:47:19.779578 spirit-extras-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-03-09 18:47:19.779578 spirit-extras-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-03-09 18:47:19.779578 spirit-extras-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:47:19.775578 spirit-extras-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:47:19.779578 spirit-extras-0.0.8/src/spirit_extras/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/chain_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/configurations.py
--rw-r--r--   0 runner    (1001) docker     (121)     7588 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    34138 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/gneb_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/import_spirit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5605 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     7881 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/pyvista_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-03-09 18:47:00.000000 spirit-extras-0.0.8/src/spirit_extras/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-09 18:47:19.779578 spirit-extras-0.0.8/src/spirit_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-03-09 18:47:19.000000 spirit-extras-0.0.8/src/spirit_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-03-09 18:47:19.000000 spirit-extras-0.0.8/src/spirit_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-09 18:47:19.000000 spirit-extras-0.0.8/src/spirit_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-09 18:47:19.000000 spirit-extras-0.0.8/src/spirit_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-09 18:47:19.000000 spirit-extras-0.0.8/src/spirit_extras.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 09:48:46.271125 spirit-extras-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-03-10 09:48:46.271125 spirit-extras-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-03-10 09:48:46.271125 spirit-extras-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 09:48:46.267125 spirit-extras-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 09:48:46.271125 spirit-extras-0.0.9/src/spirit_extras/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/chain_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7588 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34245 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/gneb_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/import_spirit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5605 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7881 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/pyvista_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-03-10 09:48:24.000000 spirit-extras-0.0.9/src/spirit_extras/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 09:48:46.271125 spirit-extras-0.0.9/src/spirit_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-03-10 09:48:45.000000 spirit-extras-0.0.9/src/spirit_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-03-10 09:48:46.000000 spirit-extras-0.0.9/src/spirit_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-10 09:48:45.000000 spirit-extras-0.0.9/src/spirit_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-10 09:48:46.000000 spirit-extras-0.0.9/src/spirit_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-10 09:48:46.000000 spirit-extras-0.0.9/src/spirit_extras.egg-info/top_level.txt
```

### Comparing `spirit-extras-0.0.8/LICENSE` & `spirit-extras-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/PKG-INFO` & `spirit-extras-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spirit-extras
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to be used with the magnetism simulation tool spirit
 Home-page: https://github.com/msallermann/spirit_extras
 Author: Moritz Sallermann
 Author-email: m.sallermann@fz-juelich.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spirit-extras-0.0.8/setup.cfg` & `spirit-extras-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spirit-extras
-version = 0.0.8
+version = 0.0.9
 author = Moritz Sallermann
 author_email = m.sallermann@fz-juelich.de
 description = Package to be used with the magnetism simulation tool spirit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/msallermann/spirit_extras
 classifiers =
```

### Comparing `spirit-extras-0.0.8/src/spirit_extras/chain_io.py` & `spirit-extras-0.0.9/src/spirit_extras/chain_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 def chain_write_between(p_state, filename, idx_start, idx_stop, fileformat=None):
     """Writes the chain between idx_start and idx_stop to a file. Includes the endpoints!"""
     from spirit import io, chain
 
-    if not fileformat:
+    if fileformat is None:
         fileformat = io.FILEFORMAT_OVF_TEXT
 
     noi = chain.get_noi(p_state)
 
     if(idx_start > idx_stop or idx_start < 0 or idx_stop>= noi):
         raise Exception("Error in idx_start and/or idx_stop")
 
@@ -15,15 +15,15 @@
         io.image_append(p_state, filename, idx_image = i, fileformat = fileformat)
 
 
 def chain_write_split_at(p_state, filename_list, idx_list, fileformat=None):
     """Writes a chain split at each index in idx_list"""
     from spirit import io, chain
 
-    if not fileformat:
+    if fileformat is None:
         fileformat = io.FILEFORMAT_OVF_TEXT
 
     if(len(filename_list) != len(idx_list)-1):
         raise Exception("Length of filename list ({}) and length of idx_list ({}) not compatible".format(len(filename_list), len(idx_list)))
 
     for i in range(1,len(idx_list)):
         if(idx_list[i-i] > idx_list[i]):
```

### Comparing `spirit-extras-0.0.8/src/spirit_extras/configurations.py` & `spirit-extras-0.0.9/src/spirit_extras/configurations.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/data.py` & `spirit-extras-0.0.9/src/spirit_extras/data.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/gneb_workflow.py` & `spirit-extras-0.0.9/src/spirit_extras/gneb_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,14 +244,17 @@
 
         with open(json_file, "w") as f:
             f.write(json.dumps(node_dict, indent=4))
 
         for c in self.children:
             c.to_json()
 
+    def history_to_file(self, path):
+        np.savetxt(path, self.history, header="iteration, max. torque" )
+
     @staticmethod
     def from_json(json_file, parent=None, children=None):
 
         with open(json_file, "r") as f:
             data = json.load(f)
 
         name                            = data["name"]
@@ -640,15 +643,15 @@
 
             noi = chain.get_noi(p_state)
 
             if idx_mid < 0:
                 E = chain.get_energy(p_state)
                 idx_mid = np.argmax(E)
 
-            self.log("    idx_mid = {}".format(idx_mid))
+            self.log("idx_mid = {}".format(idx_mid))
 
             if(idx_mid >= 1 and idx_mid < noi-1):
                 for i in range(idx_mid-1):
                     chain.delete_image(p_state, idx_image=0)
                 for i in range(noi - idx_mid - 2):
                     chain.pop_back(p_state)
```

### Comparing `spirit-extras-0.0.8/src/spirit_extras/import_spirit.py` & `spirit-extras-0.0.9/src/spirit_extras/import_spirit.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/memory_monitor.py` & `spirit-extras-0.0.9/src/spirit_extras/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/plotting.py` & `spirit-extras-0.0.9/src/spirit_extras/plotting.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/post_processing.py` & `spirit-extras-0.0.9/src/spirit_extras/post_processing.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/pyvista_plotting.py` & `spirit-extras-0.0.9/src/spirit_extras/pyvista_plotting.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras/util.py` & `spirit-extras-0.0.9/src/spirit_extras/util.py`

 * *Files identical despite different names*

### Comparing `spirit-extras-0.0.8/src/spirit_extras.egg-info/PKG-INFO` & `spirit-extras-0.0.9/src/spirit_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spirit-extras
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to be used with the magnetism simulation tool spirit
 Home-page: https://github.com/msallermann/spirit_extras
 Author: Moritz Sallermann
 Author-email: m.sallermann@fz-juelich.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spirit-extras-0.0.8/src/spirit_extras.egg-info/SOURCES.txt` & `spirit-extras-0.0.9/src/spirit_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

