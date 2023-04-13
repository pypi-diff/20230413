# Comparing `tmp/flojoy-0.2.2.dev3.tar.gz` & `tmp/flojoy-0.2.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy-0.2.2.dev3.tar", last modified: Sat Apr  8 18:31:58 2023, max compression
+gzip compressed data, was "flojoy-0.2.2.dev4.tar", last modified: Thu Apr 13 00:20:29 2023, max compression
```

## Comparing `flojoy-0.2.2.dev3.tar` & `flojoy-0.2.2.dev4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev3/LICENSE.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev3/README.md
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-08 18:31:58.579559 flojoy-0.2.2.dev3/flojoy/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev3/flojoy/__init__.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev3/flojoy/flojoy_instruction.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    18958 2023-04-08 18:30:05.000000 flojoy-0.2.2.dev3/flojoy/flojoy_python.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2629 2023-04-04 17:08:12.000000 flojoy-0.2.2.dev3/flojoy/job_result_builder.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1774 2023-04-04 17:08:40.000000 flojoy-0.2.2.dev3/flojoy/job_result_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2114 2023-04-04 17:08:55.000000 flojoy-0.2.2.dev3/flojoy/plotly_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev3/flojoy/utils.py
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/flojoy.egg-info/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/SOURCES.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/dependency_links.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/requires.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/top_level.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/setup.cfg
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-08 18:31:00.000000 flojoy-0.2.2.dev3/setup.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev4/LICENSE.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev4/README.md
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/flojoy/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev4/flojoy/__init__.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev4/flojoy/flojoy_instruction.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    19528 2023-04-13 00:12:11.000000 flojoy-0.2.2.dev4/flojoy/flojoy_python.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     3024 2023-04-13 00:13:32.000000 flojoy-0.2.2.dev4/flojoy/job_result_builder.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2128 2023-04-13 00:09:10.000000 flojoy-0.2.2.dev4/flojoy/job_result_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2368 2023-04-13 00:14:51.000000 flojoy-0.2.2.dev4/flojoy/plotly_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev4/flojoy/utils.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/flojoy.egg-info/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/SOURCES.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/dependency_links.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/requires.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-13 00:20:29.000000 flojoy-0.2.2.dev4/flojoy.egg-info/top_level.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-13 00:20:29.369062 flojoy-0.2.2.dev4/setup.cfg
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-13 00:08:08.000000 flojoy-0.2.2.dev4/setup.py
```

### Comparing `flojoy-0.2.2.dev3/LICENSE.txt` & `flojoy-0.2.2.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev3/PKG-INFO` & `flojoy-0.2.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev3
+Version: 0.2.2.dev4
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev3/flojoy/flojoy_python.py` & `flojoy-0.2.2.dev4/flojoy/flojoy_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,29 @@
 
     v.x = np.linspace(1,20,0.1)
     v.y = np.sin(v.x)
     v.type = 'ordered_pair'
 
     '''
     allowed_types = ['grayscale', 'matrix', 'dataframe',
-                     'image', 'ordered_pair', 'ordered_triple', 'scalar']
+                     'image', 'ordered_pair', 'ordered_triple', 'scalar', 'plotly']
     allowed_keys = ['x', 'y', 'z', 't', 'm',
-                    'c', 'r', 'g', 'b', 'a']
+                    'c', 'r', 'g', 'b', 'a','f']
     combinations = {
         'x': ['y', 't', 'z'],
         'y': ['x', 't', 'z'],
         'z': ['x', 'y', 't'],
         'c': ['t'],
         'm': ['t'],
         't':  [value for value in allowed_keys if value not in ['t']],
         'r': ['g', 'b', 't', 'a'],
         'g': ['r', 'b', 't', 'a'],
         'b': ['r', 'g', 't', 'a'],
         'a': ['r', 'g', 'b', 't'],
+        'f': []
     }
 
     def _ndarrayify(self, value):
         s = str(type(value))
         v_type = s.split("'")[1]
 
         match v_type:
@@ -114,14 +115,20 @@
                     self['z'] = kwargs['z']
             case 'scalar':
                 if 'c' not in kwargs:
                     raise KeyError(
                         f'c key must be provided for type "{data_type}"')
                 else:
                     self['c'] = kwargs['c']
+            case 'plotly':
+                if 'f' not in kwargs:
+                    raise KeyError(
+                        f'f key must be provided for type "{data_type}"')
+                else:
+                    self['f'] = kwargs['f']
             case _:
                 if data_type.startswith('parametric_'):
                     if 't' not in kwargs:
                         raise KeyError(
                             f't key must be provided for "{data_type}"')
                     self['t'] = kwargs['t']
                     t = kwargs['t']
@@ -151,14 +158,17 @@
                     raise KeyError(self.build_error_text(key, data_type))
             case 'ordered_triple':
                 if key not in ['x', 'y', 'z']:
                     raise KeyError(self.build_error_text(key, data_type))
             case 'scalar':
                 if key not in ['c']:
                     raise KeyError(self.build_error_text(key, data_type))
+            case 'plotly':
+                if key not in ['f']:
+                    raise KeyError(self.build_error_text(key, data_type))
 
     def set_data(self, data_type: str, key: str, value, isType: bool):
         if data_type not in self.allowed_types and data_type.startswith('parametric_'):
             if 't' not in self:
                 if key != 't':
                     raise KeyError(
                         f't key must be provided for "{data_type}"')
@@ -185,15 +195,16 @@
 
                 super().__setitem__(key, array)
                 return
         elif data_type in self.allowed_types:
             self.validate_key(data_type, key)
             if isType:
                 return
-            super().__setitem__(key, self._ndarrayify(value))
+            formatted_value = self._ndarrayify(value) if data_type != 'plotly' else value
+            super().__setitem__(key, formatted_value)
         else:
             raise ValueError(
                 f'Invalid data type "{data_type}"')
 
     def __init__(self, **kwargs):
         if 'type' in kwargs:
             self['type'] = kwargs['type']
@@ -229,15 +240,16 @@
 
                     if key in self.combinations.keys():
                         self.check_combination(
                             key, has_keys, self.combinations[key])
                         super().__setitem__(key, value)
                         return
                 else:
-                    super().__setitem__(key, self._ndarrayify(value))
+                    formatted_value = self._ndarrayify(value) if key != 'f' else value
+                    super().__setitem__(key, formatted_value)
                     return
         else:
             has_any_key = False
             has_keys = []
             for i in self.allowed_keys:
                 if hasattr(self, i):
                     has_keys.append(i)
```

### Comparing `flojoy-0.2.2.dev3/flojoy/job_result_builder.py` & `flojoy-0.2.2.dev4/flojoy/job_result_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from flojoy import DataContainer
 import numpy as np
-
+from typing import TypedDict
 from flojoy.flojoy_instruction import FLOJOY_INSTRUCTION
-from flojoy.plotly_utils import data_container_to_plotly, get_plot_fig_by_type
+from flojoy.plotly_utils import data_container_to_plotly
+from plotly.graph_objects import Figure
 
 
 class JobResultBuilder:
 
+
     def __init__(self) -> None:
-        self.data = self.instructions = None
+        self.instructions = None
+        self.data = self.get_default_data()
 
     def _add_instructions(self, instruction):
         self.instructions = self.instructions if self.instructions is not None else {}
         self.instructions = {
             **self.instructions,
             **instruction,
         }
 
     def from_inputs(self, inputs: list[DataContainer]):
         # if no inputs were provided, construct fake output
         if len(inputs) == 0:
-            x = list()
-            for i in range(1000):
-                x.append(i)
-            y = np.full(1000, 1)
-
-            self.data = DataContainer(x=x, y=y)
+            self.data = self.get_default_data()
         else:
             self.data = inputs[0]
 
         return self
 
     def from_data(self, data):
         self.data = data
@@ -64,24 +62,34 @@
                 # instructions to job scheduler (watch.py)
                 **self.instructions,
                 # instruction to fetch_input method in flojoy.py
                 FLOJOY_INSTRUCTION.RESULT_FIELD: "data",
                 'data': result,
             }
         return result
-
-    def to_plot(self, plot_type: str, **kwargs):
+    class To_plot_args(TypedDict):
+        plot_type: str
+        fig: Figure
+        data_container_plotly: DataContainer
+        
+    def to_plot(self, args: To_plot_args):
         if not self.instructions:
             self.instructions = {}
-        if len(kwargs.items()) == 0:
-            output = data_container_to_plotly(self.data, plot_type=plot_type)
-        else:
-            fig = get_plot_fig_by_type(plot_type=plot_type, **kwargs)
+        if args.get('fig', None) is not None:
+            fig = args['fig'] # get_plot_fig_by_type(plot_type=plot_type, **kwargs)
             output = fig.to_dict()
+        elif args.get('data_container_plotly',None) is not None:
+            output = data_container_to_plotly(args['data_container_plotly'], None)
+        else:
+            output = data_container_to_plotly(self.data, plot_type=args['plot_type'])
 
         return {
             **self.instructions,
             FLOJOY_INSTRUCTION.DATACONTAINER_FIELD: 'result',
             'result': self.data,
             FLOJOY_INSTRUCTION.RESULT_FIELD: 'data',
             'data': output
         }
+    def get_default_data(self):
+        x = np.arange(0,1000,1)
+        y = np.ones_like(x)
+        return DataContainer(x=x, y=y)
```

### Comparing `flojoy-0.2.2.dev3/flojoy/utils.py` & `flojoy-0.2.2.dev4/flojoy/utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev3/flojoy.egg-info/PKG-INFO` & `flojoy-0.2.2.dev4/flojoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev3
+Version: 0.2.2.dev4
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev3/setup.py` & `flojoy-0.2.2.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='flojoy',
     packages=['flojoy'],
-    version='0.2.2.dev3',
+    version='0.2.2.dev4',
     license='MIT',
     description='Python client library for Flojoy.',
     author='flojoy',
     author_email='jack.parmer@proton.me',
     url='https://github.com/flojoy-io/flojoy-python',
     download_url='https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip',
     keywords=['data-acquisition', 'lab-automation', 'low-code', 'python', 'scheduler', 'topic'],
```

