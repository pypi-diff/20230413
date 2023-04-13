# Comparing `tmp/ensemble_gnn-1.0.2.tar.gz` & `tmp/ensemble_gnn-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_gnn-1.0.2.tar", last modified: Mon Feb 27 13:33:59 2023, max compression
+gzip compressed data, was "ensemble_gnn-1.0.3.tar", last modified: Thu Apr 13 09:11:25 2023, max compression
```

## Comparing `ensemble_gnn-1.0.2.tar` & `ensemble_gnn-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:33:59.076623 ensemble_gnn-1.0.2/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1072 2022-11-11 13:01:31.000000 ensemble_gnn-1.0.2/LICENSE
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    13815 2023-02-27 13:33:59.076623 ensemble_gnn-1.0.2/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    12601 2023-02-27 12:43:05.000000 ensemble_gnn-1.0.2/README.md
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:33:59.076623 ensemble_gnn-1.0.2/ensemble_gnn/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       43 2022-11-11 13:53:13.000000 ensemble_gnn-1.0.2/ensemble_gnn/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      259 2023-02-27 09:03:33.000000 ensemble_gnn-1.0.2/ensemble_gnn/core.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     6959 2023-02-27 12:58:30.000000 ensemble_gnn-1.0.2/ensemble_gnn/ensemble.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     4302 2023-02-27 09:02:43.000000 ensemble_gnn-1.0.2/ensemble_gnn/utils.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-02-27 13:33:59.076623 ensemble_gnn-1.0.2/ensemble_gnn.egg-info/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)    13815 2023-02-27 13:33:59.000000 ensemble_gnn-1.0.2/ensemble_gnn.egg-info/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      298 2023-02-27 13:33:59.000000 ensemble_gnn-1.0.2/ensemble_gnn.egg-info/SOURCES.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2023-02-27 13:33:59.000000 ensemble_gnn-1.0.2/ensemble_gnn.egg-info/dependency_links.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       57 2023-02-27 13:33:59.000000 ensemble_gnn-1.0.2/ensemble_gnn.egg-info/requires.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       13 2023-02-27 13:33:59.000000 ensemble_gnn-1.0.2/ensemble_gnn.egg-info/top_level.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       38 2023-02-27 13:33:59.076623 ensemble_gnn-1.0.2/setup.cfg
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1550 2023-02-27 13:33:20.000000 ensemble_gnn-1.0.2/setup.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:11:25.210214 ensemble_gnn-1.0.3/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1072 2022-11-11 13:01:31.000000 ensemble_gnn-1.0.3/LICENSE
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    13815 2023-04-13 09:11:25.210214 ensemble_gnn-1.0.3/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    12601 2023-02-28 09:56:47.000000 ensemble_gnn-1.0.3/README.md
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:11:25.210214 ensemble_gnn-1.0.3/ensemble_gnn/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       43 2022-11-11 13:53:13.000000 ensemble_gnn-1.0.3/ensemble_gnn/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      259 2023-02-27 09:03:33.000000 ensemble_gnn-1.0.3/ensemble_gnn/core.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    16201 2023-04-11 10:39:43.000000 ensemble_gnn-1.0.3/ensemble_gnn/ensemble.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     4302 2023-02-27 09:02:43.000000 ensemble_gnn-1.0.3/ensemble_gnn/utils.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-04-13 09:11:25.210214 ensemble_gnn-1.0.3/ensemble_gnn.egg-info/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)    13815 2023-04-13 09:11:25.000000 ensemble_gnn-1.0.3/ensemble_gnn.egg-info/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      298 2023-04-13 09:11:25.000000 ensemble_gnn-1.0.3/ensemble_gnn.egg-info/SOURCES.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2023-04-13 09:11:25.000000 ensemble_gnn-1.0.3/ensemble_gnn.egg-info/dependency_links.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       57 2023-04-13 09:11:25.000000 ensemble_gnn-1.0.3/ensemble_gnn.egg-info/requires.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       13 2023-04-13 09:11:25.000000 ensemble_gnn-1.0.3/ensemble_gnn.egg-info/top_level.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       38 2023-04-13 09:11:25.210214 ensemble_gnn-1.0.3/setup.cfg
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1550 2023-04-13 09:11:05.000000 ensemble_gnn-1.0.3/setup.py
```

### Comparing `ensemble_gnn-1.0.2/LICENSE` & `ensemble_gnn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemble_gnn-1.0.2/PKG-INFO` & `ensemble_gnn-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemble_gnn
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ensemble learning with graph neural networks
 Home-page: https://github.com/pievos101/Ensemble-GNN
 Author: Bastian Pfeifer
 Author-email: bastian.pfeifer@medunigraz.at
 License: MIT
 Keywords: graph neural networks,ensemble learning
 Platform: UNKNOWN
@@ -147,17 +147,17 @@
 import ensemble_gnn as egnn
 
 # location of the files
 loc   = "/home/bastian/GitHub/GNN-SubNet/TCGA"
 # PPI network
 ppi   = f'{loc}/KIDNEY_RANDOM_PPI.txt'
 # single-omic features
-#feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt']
+feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt']
 # multi-omic features
-feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt', f'{loc}/KIDNEY_RANDOM_Methy_FEATURES.txt']
+#feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt', f'{loc}/KIDNEY_RANDOM_Methy_FEATURES.txt']
 # outcome class
 targ  = f'{loc}/KIDNEY_RANDOM_TARGET.txt'
 
 # Load the multi-omics data
 g = gnn.GNNSubNet(loc, ppi, feats, targ)
 
 # Get some general information about the data dimension
```

### Comparing `ensemble_gnn-1.0.2/README.md` & `ensemble_gnn-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -116,17 +116,17 @@
 import ensemble_gnn as egnn
 
 # location of the files
 loc   = "/home/bastian/GitHub/GNN-SubNet/TCGA"
 # PPI network
 ppi   = f'{loc}/KIDNEY_RANDOM_PPI.txt'
 # single-omic features
-#feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt']
+feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt']
 # multi-omic features
-feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt', f'{loc}/KIDNEY_RANDOM_Methy_FEATURES.txt']
+#feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt', f'{loc}/KIDNEY_RANDOM_Methy_FEATURES.txt']
 # outcome class
 targ  = f'{loc}/KIDNEY_RANDOM_TARGET.txt'
 
 # Load the multi-omics data
 g = gnn.GNNSubNet(loc, ppi, feats, targ)
 
 # Get some general information about the data dimension
```

### Comparing `ensemble_gnn-1.0.2/ensemble_gnn/utils.py` & `ensemble_gnn-1.0.3/ensemble_gnn/utils.py`

 * *Files identical despite different names*

### Comparing `ensemble_gnn-1.0.2/ensemble_gnn.egg-info/PKG-INFO` & `ensemble_gnn-1.0.3/ensemble_gnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemble-gnn
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ensemble learning with graph neural networks
 Home-page: https://github.com/pievos101/Ensemble-GNN
 Author: Bastian Pfeifer
 Author-email: bastian.pfeifer@medunigraz.at
 License: MIT
 Keywords: graph neural networks,ensemble learning
 Platform: UNKNOWN
@@ -147,17 +147,17 @@
 import ensemble_gnn as egnn
 
 # location of the files
 loc   = "/home/bastian/GitHub/GNN-SubNet/TCGA"
 # PPI network
 ppi   = f'{loc}/KIDNEY_RANDOM_PPI.txt'
 # single-omic features
-#feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt']
+feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt']
 # multi-omic features
-feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt', f'{loc}/KIDNEY_RANDOM_Methy_FEATURES.txt']
+#feats = [f'{loc}/KIDNEY_RANDOM_mRNA_FEATURES.txt', f'{loc}/KIDNEY_RANDOM_Methy_FEATURES.txt']
 # outcome class
 targ  = f'{loc}/KIDNEY_RANDOM_TARGET.txt'
 
 # Load the multi-omics data
 g = gnn.GNNSubNet(loc, ppi, feats, targ)
 
 # Get some general information about the data dimension
```

### Comparing `ensemble_gnn-1.0.2/setup.py` & `ensemble_gnn-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='ensemble_gnn',
-    version='1.0.2',
+    version='1.0.3',
     author='Bastian Pfeifer',
     license='MIT',
     author_email='bastian.pfeifer@medunigraz.at',
     description='Ensemble learning with graph neural networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pievos101/Ensemble-GNN',
```

