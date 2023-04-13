# Comparing `tmp/qaoalib-0.1.7.tar.gz` & `tmp/qaoalib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaoalib-0.1.7.tar", last modified: Wed Jan 25 03:56:39 2023, max compression
+gzip compressed data, was "qaoalib-0.1.8.tar", last modified: Thu Apr 13 12:44:37 2023, max compression
```

## Comparing `qaoalib-0.1.7.tar` & `qaoalib-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 03:56:39.080522 qaoalib-0.1.7/
--rw-rw-rw-   0        0        0     1088 2021-05-03 05:04:16.000000 qaoalib-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1443 2023-01-25 03:56:39.080522 qaoalib-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-01-25 03:47:52.000000 qaoalib-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-25 03:56:38.938883 qaoalib-0.1.7/qaoalib/
--rw-rw-rw-   0        0        0       53 2022-04-28 07:47:51.000000 qaoalib-0.1.7/qaoalib/__init__.py
--rw-rw-rw-   0        0        0      519 2021-05-11 09:10:13.000000 qaoalib-0.1.7/qaoalib/json.py
--rw-rw-rw-   0        0        0     1593 2021-05-26 01:13:30.000000 qaoalib-0.1.7/qaoalib/math.py
-drwxrwxrwx   0        0        0        0 2023-01-25 03:56:39.049280 qaoalib-0.1.7/qaoalib/qaoa/
--rw-rw-rw-   0        0        0       91 2022-06-20 06:27:33.000000 qaoalib-0.1.7/qaoalib/qaoa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-25 03:56:39.080522 qaoalib-0.1.7/qaoalib/qaoa/landscape/
--rw-rw-rw-   0        0        0      114 2021-05-11 09:10:51.000000 qaoalib-0.1.7/qaoalib/qaoa/landscape/__init__.py
--rw-rw-rw-   0        0        0     3255 2022-05-11 08:16:21.000000 qaoalib-0.1.7/qaoalib/qaoa/landscape/base.py
--rw-rw-rw-   0        0        0     2476 2022-05-11 06:23:38.000000 qaoalib-0.1.7/qaoalib/qaoa/landscape/direct_numpy.py
--rw-rw-rw-   0        0        0     1426 2022-05-11 06:25:22.000000 qaoalib-0.1.7/qaoalib/qaoa/landscape/hadamard_test.py
--rw-rw-rw-   0        0        0     1680 2022-05-11 06:24:39.000000 qaoalib-0.1.7/qaoalib/qaoa/landscape/hybrid_fast.py
--rw-rw-rw-   0        0        0     5996 2021-12-08 04:26:09.000000 qaoalib-0.1.7/qaoalib/qaoa/layerwise.py
--rw-rw-rw-   0        0        0     1686 2022-06-15 08:52:35.000000 qaoalib-0.1.7/qaoalib/qaoa/qis.py
--rw-rw-rw-   0        0        0     1783 2022-06-28 05:52:47.000000 qaoalib-0.1.7/qaoalib/qaoa/qmc.py
--rw-rw-rw-   0        0        0     3661 2022-06-15 08:52:24.000000 qaoalib-0.1.7/qaoalib/qaoa/utils.py
--rw-rw-rw-   0        0        0     7944 2023-01-25 03:49:57.000000 qaoalib-0.1.7/qaoalib/utils.py
--rw-rw-rw-   0        0        0       21 2023-01-25 03:54:49.000000 qaoalib-0.1.7/qaoalib/version.py
-drwxrwxrwx   0        0        0        0 2023-01-25 03:56:38.954545 qaoalib-0.1.7/qaoalib.egg-info/
--rw-rw-rw-   0        0        0     1443 2023-01-25 03:56:38.000000 qaoalib-0.1.7/qaoalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-01-25 03:56:38.000000 qaoalib-0.1.7/qaoalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 03:56:38.000000 qaoalib-0.1.7/qaoalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-01-25 03:56:38.000000 qaoalib-0.1.7/qaoalib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-25 03:56:38.000000 qaoalib-0.1.7/qaoalib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-25 03:56:39.080522 qaoalib-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      922 2022-04-28 07:56:26.000000 qaoalib-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-25 03:56:39.080522 qaoalib-0.1.7/test/
--rw-rw-rw-   0        0        0       87 2021-12-08 04:31:51.000000 qaoalib-0.1.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.631838 qaoalib-0.1.8/
+-rw-rw-rw-   0        0        0     1088 2021-05-03 05:04:16.000000 qaoalib-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1443 2023-04-13 12:44:37.631838 qaoalib-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-01-25 03:47:52.000000 qaoalib-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.425228 qaoalib-0.1.8/qaoalib/
+-rw-rw-rw-   0        0        0       53 2022-04-28 07:47:51.000000 qaoalib-0.1.8/qaoalib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.465470 qaoalib-0.1.8/qaoalib/data/
+-rw-rw-rw-   0        0        0        0 2023-04-04 00:41:47.000000 qaoalib-0.1.8/qaoalib/data/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-02-09 02:39:10.000000 qaoalib-0.1.8/qaoalib/data/graph.py
+-rw-rw-rw-   0        0        0      737 2023-02-09 03:35:51.000000 qaoalib-0.1.8/qaoalib/data/result.py
+-rw-rw-rw-   0        0        0      519 2021-05-11 09:10:13.000000 qaoalib-0.1.8/qaoalib/json.py
+-rw-rw-rw-   0        0        0     1593 2021-05-26 01:13:30.000000 qaoalib-0.1.8/qaoalib/math.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.573816 qaoalib-0.1.8/qaoalib/qaoa/
+-rw-rw-rw-   0        0        0       91 2022-06-20 06:27:33.000000 qaoalib-0.1.8/qaoalib/qaoa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.625829 qaoalib-0.1.8/qaoalib/qaoa/landscape/
+-rw-rw-rw-   0        0        0      114 2021-05-11 09:10:51.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/__init__.py
+-rw-rw-rw-   0        0        0     3255 2022-05-11 08:16:21.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/base.py
+-rw-rw-rw-   0        0        0     2476 2022-05-11 06:23:38.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/direct_numpy.py
+-rw-rw-rw-   0        0        0     1426 2022-05-11 06:25:22.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/hadamard_test.py
+-rw-rw-rw-   0        0        0     1680 2022-05-11 06:24:39.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/hybrid_fast.py
+-rw-rw-rw-   0        0        0     5996 2021-12-08 04:26:09.000000 qaoalib-0.1.8/qaoalib/qaoa/layerwise.py
+-rw-rw-rw-   0        0        0     1686 2022-06-15 08:52:35.000000 qaoalib-0.1.8/qaoalib/qaoa/qis.py
+-rw-rw-rw-   0        0        0     1787 2023-01-30 05:54:20.000000 qaoalib-0.1.8/qaoalib/qaoa/qmc.py
+-rw-rw-rw-   0        0        0     1965 2023-04-04 00:01:17.000000 qaoalib-0.1.8/qaoalib/qaoa/strategy.py
+-rw-rw-rw-   0        0        0     3661 2022-06-15 08:52:24.000000 qaoalib-0.1.8/qaoalib/qaoa/utils.py
+-rw-rw-rw-   0        0        0     9013 2023-02-09 03:36:01.000000 qaoalib-0.1.8/qaoalib/utils.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 12:42:27.000000 qaoalib-0.1.8/qaoalib/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.438228 qaoalib-0.1.8/qaoalib.egg-info/
+-rw-rw-rw-   0        0        0     1443 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 12:44:37.631838 qaoalib-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      922 2022-04-28 07:56:26.000000 qaoalib-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.629879 qaoalib-0.1.8/test/
+-rw-rw-rw-   0        0        0       87 2021-12-08 04:31:51.000000 qaoalib-0.1.8/test/test.py
```

### Comparing `qaoalib-0.1.7/LICENSE` & `qaoalib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/PKG-INFO` & `qaoalib-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaoalib
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for QAOA Maxcut calculations
 Home-page: https://github.com/xenoicwyce/qaoalib
 Author: Xinwei Lee
 Author-email: xenoicwyce@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qaoalib-0.1.7/README.md` & `qaoalib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/json.py` & `qaoalib-0.1.8/qaoalib/json.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/math.py` & `qaoalib-0.1.8/qaoalib/math.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/landscape/base.py` & `qaoalib-0.1.8/qaoalib/qaoa/landscape/base.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/landscape/direct_numpy.py` & `qaoalib-0.1.8/qaoalib/qaoa/landscape/direct_numpy.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/landscape/hadamard_test.py` & `qaoalib-0.1.8/qaoalib/qaoa/landscape/hadamard_test.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/landscape/hybrid_fast.py` & `qaoalib-0.1.8/qaoalib/qaoa/landscape/hybrid_fast.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/layerwise.py` & `qaoalib-0.1.8/qaoalib/qaoa/layerwise.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/qis.py` & `qaoalib-0.1.8/qaoalib/qaoa/qis.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/qmc.py` & `qaoalib-0.1.8/qaoalib/qaoa/qmc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from qiskit import Aer, execute
 
 from .qis import qaoa_circuit, sv_backend
 from .utils import expectation, I, Z
 from ..math import fast_kron
 
+
 class Qmc:
     def __init__(self, G, params):
         self.graph = G
         self.params = params
         self.circuit = qaoa_circuit(self.graph, self.params)
         self.result = None
         self.expectation = None
@@ -24,14 +25,15 @@
         if backend_name == 'qasm_simulator':
             self.result = result.get_counts()
         elif backend_name == 'statevector_simulator':
             self.result = np.asarray(result.get_statevector())
 
         self.expectation = expectation(self.graph, self.result)
 
+
 class QmcFastKron(Qmc):
     def __init__(self, G, params):
         super().__init__(G, params)
 
     def _fast_kron_exp(self, sv):
         sum_ = 0
         for u, v, d in self.graph.edges(data=True):
```

### Comparing `qaoalib-0.1.7/qaoalib/qaoa/utils.py` & `qaoalib-0.1.8/qaoalib/qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.7/qaoalib/utils.py` & `qaoalib-0.1.8/qaoalib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import Union, Literal, Optional
 import warnings
 import numpy as np
 import networkx as nx
 
+from .data.graph import RegGraphData, GnpGraphData
+
 
 def get_info(filename, indicator, mode='get-numeric'):
     try:
         pos = filename.index(indicator)
     except ValueError:
         return None
 
@@ -257,7 +260,47 @@
             expectations = -(np.asarray(arr) + data['shift'])
             data['expectations'][p] = expectations
             data['alpha'][p] = expectations / data['true_obj']
     else:
         for p, arr in data['expectations'].items():
             data['energies'][p] = -(np.asarray(arr) + data['shift'])
             data['alpha'][p] = np.asarray(arr) / data['true_obj']
+
+def convert_graph(
+    G: nx.Graph,
+    graph_type: Literal['reg', 'gnp'],
+    prob: Optional[float] = None,
+    solve_brute: bool = True,
+) -> Union[RegGraphData, GnpGraphData]:
+
+    if solve_brute:
+        true_obj, _ = maxcut_brute(G)
+    else:
+        true_obj = 0
+
+    n_nodes = len(G.nodes)
+    edges = list(G.edges)
+    n_edges = len(G.edges)
+    shift = -n_edges / 2.0
+
+    if graph_type == 'reg':
+        deg = len(list(G.neighbors(0)))
+        return RegGraphData(
+            deg=deg,
+            n_nodes=n_nodes,
+            edges=edges,
+            n_edges=n_edges,
+            shift=shift,
+            true_obj=true_obj,
+        )
+
+    elif graph_type == 'gnp':
+        if prob is None:
+            raise ValueError('`prob` must be passed for Gnp graphs.')
+        return GnpGraphData(
+            prob=prob,
+            n_nodes=n_nodes,
+            edges=edges,
+            n_edges=n_edges,
+            shift=shift,
+            true_obj=true_obj,
+        )
```

### Comparing `qaoalib-0.1.7/qaoalib.egg-info/PKG-INFO` & `qaoalib-0.1.8/qaoalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaoalib
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for QAOA Maxcut calculations
 Home-page: https://github.com/xenoicwyce/qaoalib
 Author: Xinwei Lee
 Author-email: xenoicwyce@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `qaoalib-0.1.7/qaoalib.egg-info/SOURCES.txt` & `qaoalib-0.1.8/qaoalib.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,22 @@
 qaoalib/utils.py
 qaoalib/version.py
 qaoalib.egg-info/PKG-INFO
 qaoalib.egg-info/SOURCES.txt
 qaoalib.egg-info/dependency_links.txt
 qaoalib.egg-info/requires.txt
 qaoalib.egg-info/top_level.txt
+qaoalib/data/__init__.py
+qaoalib/data/graph.py
+qaoalib/data/result.py
 qaoalib/qaoa/__init__.py
 qaoalib/qaoa/layerwise.py
 qaoalib/qaoa/qis.py
 qaoalib/qaoa/qmc.py
+qaoalib/qaoa/strategy.py
 qaoalib/qaoa/utils.py
 qaoalib/qaoa/landscape/__init__.py
 qaoalib/qaoa/landscape/base.py
 qaoalib/qaoa/landscape/direct_numpy.py
 qaoalib/qaoa/landscape/hadamard_test.py
 qaoalib/qaoa/landscape/hybrid_fast.py
 test/test.py
```

### Comparing `qaoalib-0.1.7/setup.py` & `qaoalib-0.1.8/setup.py`

 * *Files identical despite different names*

