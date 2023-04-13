# Comparing `tmp/TraffiX-0.1.3a0.tar.gz` & `tmp/TraffiX-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TraffiX-0.1.3a0.tar", last modified: Thu Apr 13 17:00:24 2023, max compression
+gzip compressed data, was "TraffiX-0.1.4a0.tar", last modified: Thu Apr 13 17:36:42 2023, max compression
```

## Comparing `TraffiX-0.1.3a0.tar` & `TraffiX-0.1.4a0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:00:24.240562 TraffiX-0.1.3a0/
--rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.3a0/LICENSE
--rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 TraffiX-0.1.3a0/MANIFEST.in
--rw-r--r--   0 maman      (501) staff       (20)     2743 2023-04-13 17:00:24.239907 TraffiX-0.1.3a0/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 TraffiX-0.1.3a0/README.md
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:00:24.229366 TraffiX-0.1.3a0/TraffiX/
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/.___init__.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/.__api.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/.__version.py
--rw-r--r--   0 maman      (501) staff       (20)      519 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/OD.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:00:24.237082 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/
--rw-r--r--   0 maman      (501) staff       (20)     2743 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)      439 2023-04-13 17:00:24.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/SOURCES.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/dependency_links.txt
--rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/requires.txt
--rw-r--r--   0 maman      (501) staff       (20)       46 2023-04-13 17:00:23.000000 TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/top_level.txt
--rw-r--r--   0 maman      (501) staff       (20)       75 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/__init__.py
--rw-r--r--   0 maman      (501) staff       (20)      622 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/_api.py
--rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/_version.py
--rw-r--r--   0 maman      (501) staff       (20)     5245 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/add.py
--rw-r--r--   0 maman      (501) staff       (20)     1322 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/flow.py
--rw-r--r--   0 maman      (501) staff       (20)      670 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/lpr.py
--rw-r--r--   0 maman      (501) staff       (20)      228 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/me2.py
--rw-r--r--   0 maman      (501) staff       (20)     2123 2023-04-13 16:58:26.000000 TraffiX-0.1.3a0/TraffiX/ue.py
--rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 17:00:24.240702 TraffiX-0.1.3a0/setup.cfg
--rwxr-xr-x   0 maman      (501) staff       (20)     1181 2023-04-13 16:59:32.000000 TraffiX-0.1.3a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:36:42.756472 TraffiX-0.1.4a0/
+-rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.4a0/LICENSE
+-rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 TraffiX-0.1.4a0/MANIFEST.in
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 17:36:42.755790 TraffiX-0.1.4a0/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 TraffiX-0.1.4a0/README.md
+-rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 17:36:42.756669 TraffiX-0.1.4a0/setup.cfg
+-rwxr-xr-x   0 maman      (501) staff       (20)     1182 2023-04-13 17:26:03.000000 TraffiX-0.1.4a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:36:42.750972 TraffiX-0.1.4a0/traffix/
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/.___init__.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/.__api.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/.__version.py
+-rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 TraffiX-0.1.4a0/traffix/OD.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 17:36:42.754903 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)      424 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/SOURCES.txt
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/dependency_links.txt
+-rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/requires.txt
+-rw-r--r--   0 maman      (501) staff       (20)       42 2023-04-13 17:36:42.000000 TraffiX-0.1.4a0/traffix/TraffiX.egg-info/top_level.txt
+-rw-r--r--   0 maman      (501) staff       (20)       75 2023-04-13 16:58:26.000000 TraffiX-0.1.4a0/traffix/__init__.py
+-rw-r--r--   0 maman      (501) staff       (20)      567 2023-04-13 17:35:20.000000 TraffiX-0.1.4a0/traffix/_api.py
+-rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 17:25:45.000000 TraffiX-0.1.4a0/traffix/_version.py
+-rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 TraffiX-0.1.4a0/traffix/add.py
+-rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 TraffiX-0.1.4a0/traffix/flow.py
+-rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 TraffiX-0.1.4a0/traffix/lpr.py
+-rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 TraffiX-0.1.4a0/traffix/ue.py
```

### Comparing `TraffiX-0.1.3a0/LICENSE` & `TraffiX-0.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.3a0/PKG-INFO` & `TraffiX-0.1.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: TraffiX
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: A package for macroscopic transportation assignment.
-Home-page: https://github.com/Ultios/StraPy
+Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `TraffiX-0.1.3a0/README.md` & `TraffiX-0.1.4a0/README.md`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.3a0/TraffiX/.___init__.py` & `TraffiX-0.1.4a0/traffix/.___init__.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.3a0/TraffiX/.__api.py` & `TraffiX-0.1.4a0/traffix/.__api.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.3a0/TraffiX/.__version.py` & `TraffiX-0.1.4a0/traffix/.__version.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.3a0/TraffiX/TraffiX.egg-info/PKG-INFO` & `TraffiX-0.1.4a0/traffix/TraffiX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: TraffiX
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: A package for macroscopic transportation assignment.
-Home-page: https://github.com/Ultios/StraPy
+Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `TraffiX-0.1.3a0/TraffiX/_api.py` & `TraffiX-0.1.4a0/traffix/_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from .add import add_edge_capacity
 from .add import flatten_osmid
 from .add import add_edge_initial_travel_time
 from .flow import Flow_from_OD
 from .flow import link_flow
 from .lpr import update_travel_time_lpr
 from .lpr import lpr
-from .me2 import ME2
-from .me2 import isConvergenceME2
 from .OD import OD_nodes_list
 from .OD import OD_shortest_path
 from .ue import line_search
 from .ue import bisection
 from .ue import update
 from .ue import update_mainflow
 from .ue import CCA
```

### Comparing `TraffiX-0.1.3a0/TraffiX/add.py` & `TraffiX-0.1.4a0/traffix/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import osmnx as ox
+import pandas as pd
+import networkx as nx
 
 
 
 
 def add_edge_lanes(G, lanes_min=1):
     """
     Add default lanes towards NaN lanes value in edge attributes.
@@ -72,15 +75,14 @@
     #Impute missing values with width value.
     width = (
         edges[["highway", "width"]].set_index("highway").iloc[:, 0].fillna(width_min)
     )
     #Change lanes column into numeric
     edges["width"]=pd.to_numeric(edges["width"])
     edges["width"] = width.values
-    display(edges["width"])
     nx.set_edge_attributes(G, values=edges["width"], name="width")
     
     return G
 
 def add_edge_capacity(G, base_capacity=None, fallback=1650):
     """
     Add edge capacity to graph as new "capacity" edge attributes.
```

### Comparing `TraffiX-0.1.3a0/TraffiX/flow.py` & `TraffiX-0.1.4a0/traffix/flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import networkx as nx
 
 
 
 def Flow_from_OD(OD):
     OD.index += 1
     OD.columns = list(range(1,len(OD.index)+1))
     if not len(OD.index) == len(OD.columns):
```

### Comparing `TraffiX-0.1.3a0/TraffiX/lpr.py` & `TraffiX-0.1.4a0/traffix/lpr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import networkx as nx
+import numpy as np
+
 def update_travel_time_lpr(G, alpha=0.15, beta=4):
     df = nx.to_pandas_edgelist(G, edge_key='ekey').set_index(["source","target","ekey"])
     df['travel_time'] = df.apply(lambda x: lpr(x, alpha, beta), axis=1).values
     nx.set_edge_attributes(G, df['travel_time'], name='travel_time')
     return G
 
 #This is a link performance function derived from Indonesia's Highway Manual (MKJI 1997).
```

### Comparing `TraffiX-0.1.3a0/TraffiX/ue.py` & `TraffiX-0.1.4a0/traffix/ue.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-
+import networkx as nx
+import pandas as pd
+import numpy as np
 
 def line_search(row, a, alpha, beta):
     t=row['initial_travel_time']
     x=row['flow']
     y=row['auxflow']
     c=row['capacity']
     return -t*(x-y)*(alpha*(((x+a*(y-x))/c)**beta)+1)
```

### Comparing `TraffiX-0.1.3a0/setup.py` & `TraffiX-0.1.4a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 
 from setuptools import setup
 
 
 setup(
     name="TraffiX", 
-    version = "0.1.3-alpha",
+    version = "0.1.4-alpha",
     description = "A package for macroscopic transportation assignment.",
-    package_dir = {"":"TraffiX"},
+    package_dir = {"":"traffix"},
     author = "Aulia Rahman",
     author_email = "rahmancs02@gmail.com",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
-    url="https://github.com/Ultios/StraPy",
+    url="https://github.com/Ultios/traffix",
     include_package_data=True,
     classifiers  = [
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

