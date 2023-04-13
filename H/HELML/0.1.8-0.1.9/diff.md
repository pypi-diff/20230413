# Comparing `tmp/HELML-0.1.8.tar.gz` & `tmp/HELML-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HELML-0.1.8.tar", last modified: Sun Apr  9 11:39:30 2023, max compression
+gzip compressed data, was "HELML-0.1.9.tar", last modified: Thu Apr 13 07:06:03 2023, max compression
```

## Comparing `HELML-0.1.8.tar` & `HELML-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 11:39:30.855459 HELML-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-04-09 11:39:30.850459 HELML-0.1.8/HELML/
--rw-rw-rw-   0        0        0      274 2023-03-15 13:42:07.000000 HELML-0.1.8/HELML/__init__.py
--rw-rw-rw-   0        0        0    16401 2023-04-09 11:29:37.000000 HELML-0.1.8/HELML/_helml.py
--rw-rw-rw-   0        0        0      122 2023-04-09 11:38:27.000000 HELML-0.1.8/HELML/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:39:30.853459 HELML-0.1.8/HELML.egg-info/
--rw-rw-rw-   0        0        0     2472 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-03-15 16:11:37.000000 HELML-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2472 2023-04-09 11:39:30.854459 HELML-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1747 2023-04-04 15:46:14.000000 HELML-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 11:39:30.855459 HELML-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-04-09 11:39:04.000000 HELML-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:06:03.650311 HELML-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-04-13 07:06:03.646311 HELML-0.1.9/HELML/
+-rw-rw-rw-   0        0        0      274 2023-03-15 13:42:07.000000 HELML-0.1.9/HELML/__init__.py
+-rw-rw-rw-   0        0        0    16638 2023-04-13 06:29:30.000000 HELML-0.1.9/HELML/_helml.py
+-rw-rw-rw-   0        0        0      122 2023-04-13 07:03:40.000000 HELML-0.1.9/HELML/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:06:03.649311 HELML-0.1.9/HELML.egg-info/
+-rw-rw-rw-   0        0        0     2471 2023-04-13 07:06:03.000000 HELML-0.1.9/HELML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-04-13 07:06:03.000000 HELML-0.1.9/HELML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 07:06:03.000000 HELML-0.1.9/HELML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 07:06:03.000000 HELML-0.1.9/HELML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-03-15 16:11:37.000000 HELML-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2471 2023-04-13 07:06:03.649311 HELML-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1746 2023-04-13 07:04:58.000000 HELML-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 07:06:03.650311 HELML-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-04-13 07:04:02.000000 HELML-0.1.9/setup.py
```

### Comparing `HELML-0.1.8/HELML/_helml.py` & `HELML-0.1.9/HELML/_helml.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,28 +95,28 @@
             # add the appropriate number of colons to the left of the key, based on the current level
             ident = lvl_ch * level
 
              # add space-ident to the left of the key (if need)
             if HELML.ENABLE_SPC_IDENT and spc_ch == ' ':
                 ident = spc_ch * (level * HELML.ENABLE_SPC_IDENT) + ident
 
-            is_arr = isinstance(value, (list, tuple, set))
+            is_numkeys = isinstance(value, (list, tuple, set))
 
-            if is_arr or isinstance(value, dict):
+            if is_numkeys or isinstance(value, dict):
                 # Add empty line before create-key
                 if HELML.ENABLE_KEY_UPLINES and spc_ch == ' ':
                     results_arr.append('')
-                
+
                 # add ":" after key for lists
-                if is_arr:
+                if not is_numkeys:
                     key += lvl_ch
 
                 results_arr.append(ident + key)
 
-                HELML._encode(value, results_arr, level + 1, lvl_ch, spc_ch, is_arr)
+                HELML._encode(value, results_arr, level + 1, lvl_ch, spc_ch, is_numkeys)
 
                 if HELML.ENABLE_KEY_UPLINES and spc_ch == ' ':
                     results_arr.append(spc_ch * level + '#')
             else:
                 # use selected value encoder function
                 value = value_enco_fun(value, spc_ch)
 
@@ -125,27 +125,21 @@
 
     @staticmethod
     def decode(
         src_rows: str,
         get_layers: Union[int, str, Set[Union[str, int]], List[Union[str, int]]] = [0]
     ) -> Dict:
 
-        # select value decoder function custom or internal default
-        value_deco_fun = HELML.CUSTOM_VALUE_DECODER if HELML.CUSTOM_VALUE_DECODER is not None else HELML.valueDecoder
-
         lvl_ch: str = ":"
         spc_ch: str = " "
-        layer_init: str = '0'
-        layer_curr:str = layer_init
-        all_layers = set([layer_init])
 
         # Prepare layers_set from get_layers
         # 1. Modify get_layers if needed: convert single T to array [0, T]
         if isinstance(get_layers, (int, str)):
-            get_layers = [layer_init, get_layers]
+            get_layers = ['0', get_layers]
         # 2. Create layers_set and set all values from get_layers (str)
         layers_set = set()
         for i in get_layers:
             if not isinstance(i, str):
                 i = str(i)
             layers_set.add(i)
 
@@ -155,14 +149,30 @@
             if exploder_ch in src_rows:
                 if "~" == exploder_ch and src_rows[-1] == "~":
                     lvl_ch = "."
                     spc_ch = "_"
                 break
 
         str_arr = src_rows.split(exploder_ch)
+        return HELML._decode(str_arr, layers_set, lvl_ch, spc_ch)
+
+    def _decode(
+        str_arr: list,
+        layers_set: set,
+        lvl_ch: str,
+        spc_ch: str
+    ) -> Dict:
+        
+        # layer values prepare
+        layer_init: str = '0'
+        layer_curr:str = layer_init
+        all_layers = set([layer_init])
+
+        # select value decoder function custom or internal default
+        value_deco_fun = HELML.CUSTOM_VALUE_DECODER if HELML.CUSTOM_VALUE_DECODER is not None else HELML.valueDecoder
 
         # Initialize result array and stack for keeping track of current array nesting
         result = {}
         stack = []
 
         # array of stack stamps for delayed conversion dict to list
         tolist = []
@@ -236,15 +246,15 @@
                         key = decoded_key
 
             # If the value is null, start a new dictionary and add it to the parent dictionary
             if value is None or value == '':
                 layer_curr = layer_init
                 parent[key] = {}
                 stack.append(key)
-                if value == '':
+                if value is None:
                     tolist.append(stack.copy())
             elif layer_curr in layers_set:
                 # Decode the value by selected value-decoder-function
                 value = value_deco_fun(value, spc_ch)
                 # Add the key-value pair to the current dictionary
                 parent[key] = value
```

### Comparing `HELML-0.1.8/HELML.egg-info/PKG-INFO` & `HELML-0.1.9/HELML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HELML
-Version: 0.1.8
+Version: 0.1.9
 Summary: Encoding-decoding HELML format
 Home-page: https://github.com/dynoser/HELML/tree/master/Python
 Author: AlexanderJer
 Author-email: alexierusalim@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -55,15 +55,15 @@
 # Decode the HELML string back into a data structure
 decoded_data = HELML.decode(encoded_data)
 ```
 encoded_data:
 ```console
 key1: value1
 
-key2:
+key2
  :--:  1
  :--:  2
  :--:  3
 
 key3
  :nested_key: nested_value
```

### Comparing `HELML-0.1.8/LICENSE` & `HELML-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `HELML-0.1.8/PKG-INFO` & `HELML-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HELML
-Version: 0.1.8
+Version: 0.1.9
 Summary: Encoding-decoding HELML format
 Home-page: https://github.com/dynoser/HELML/tree/master/Python
 Author: AlexanderJer
 Author-email: alexierusalim@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -55,15 +55,15 @@
 # Decode the HELML string back into a data structure
 decoded_data = HELML.decode(encoded_data)
 ```
 encoded_data:
 ```console
 key1: value1
 
-key2:
+key2
  :--:  1
  :--:  2
  :--:  3
 
 key3
  :nested_key: nested_value
```

### Comparing `HELML-0.1.8/README.md` & `HELML-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # Decode the HELML string back into a data structure
 decoded_data = HELML.decode(encoded_data)
 ```
 encoded_data:
 ```console
 key1: value1
 
-key2:
+key2
  :--:  1
  :--:  2
  :--:  3
 
 key3
  :nested_key: nested_value
```

### Comparing `HELML-0.1.8/setup.py` & `HELML-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HELML',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=[
     ],
     author='AlexanderJer',
     author_email='alexierusalim@gmail.com',
     description='Encoding-decoding HELML format',
     long_description=open('README.md').read(),
```

