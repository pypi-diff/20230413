# Comparing `tmp/rcsb.utils.targets-0.66.tar.gz` & `tmp/rcsb.utils.targets-0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.66.tar", last modified: Wed Mar 29 14:08:48 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.67.tar", last modified: Thu Apr 13 16:33:31 2023, max compression
```

## Comparing `rcsb.utils.targets-0.66.tar` & `rcsb.utils.targets-0.67.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-29 14:08:48.993529 rcsb.utils.targets-0.66/
--rw-r--r--   0 vsts      (1001) docker     (122)     5612 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-03-29 14:08:48.993529 rcsb.utils.targets-0.66/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-29 14:08:48.989529 rcsb.utils.targets-0.66/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-29 14:08:48.989529 rcsb.utils.targets-0.66/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-29 14:08:48.993529 rcsb.utils.targets-0.66/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7028 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-29 13:52:57.000000 rcsb.utils.targets-0.66/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-29 14:08:48.989529 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-03-29 14:08:48.000000 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-03-29 14:08:48.000000 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-29 14:08:48.000000 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-29 13:54:00.000000 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-03-29 14:08:48.000000 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-29 14:08:48.000000 rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-03-29 13:52:58.000000 rcsb.utils.targets-0.66/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-03-29 14:08:48.993529 rcsb.utils.targets-0.66/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-03-29 13:52:58.000000 rcsb.utils.targets-0.66/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5758 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      952 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.911996 rcsb.utils.targets-0.67/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.911996 rcsb.utils.targets-0.67/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8379 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8841 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-13 16:19:18.000000 rcsb.utils.targets-0.67/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 16:33:31.911996 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 16:20:13.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-13 16:33:31.000000 rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-13 16:19:19.000000 rcsb.utils.targets-0.67/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-04-13 16:33:31.915996 rcsb.utils.targets-0.67/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-04-13 16:19:19.000000 rcsb.utils.targets-0.67/setup.py
```

### Comparing `rcsb.utils.targets-0.66/HISTORY.txt` & `rcsb.utils.targets-0.67/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,7 +52,8 @@
    6-Jan-2023  - V0.60 Configuration changes to support tox 4
    9-Feb-2023  - V0.61 Find Highest_Clin_Trial column regardless of month in SAbDabTargetProvider(), Update baseVersion for ChEMBL
   27-Feb-2023  - V0.62 Fix PharosTargetProvider mysql loading issue
    3-Mar-2023  - V0.63 Fix typo and handle missing activityType in PharosTargetCofactorProvider()
   13-Mar-2023  - V0.64 Add CARDTargetAnnotationProvider (to replace CARDTargetFeatureProvider)
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
+  11-Apr-2023  - V0.67 Fix issue with lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
```

### Comparing `rcsb.utils.targets-0.66/LICENSE` & `rcsb.utils.targets-0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/PKG-INFO` & `rcsb.utils.targets-0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.66
+Version: 0.67
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.66/README.md` & `rcsb.utils.targets-0.67/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 #  File:           CARDTargetOntologyProvider.py
 #  Date:           14-Mar-2023 dwp
 #
 #  Updates:
-#
+#   11-Apr-2023 dwp  Fix issue with lineage tree building--handle cases with two parents at same depth;
+#                    Add treeNodeList building and exporting
 ##
 """
 Accessors for CARD ontologies.
 
 """
 
 import datetime
@@ -26,15 +27,15 @@
 
     def __init__(self, **kwargs):
         #
         self.__cachePath = kwargs.get("cachePath", ".")
         self.__dirPath = os.path.join(self.__cachePath, "CARD-ontology")
         #
         self.__mU = MarshalUtil(workPath=self.__dirPath)
-        self.__oD, self.__version = self.__reload(self.__dirPath, **kwargs)
+        self.__oD, self.__tnL, self.__version = self.__reload(self.__dirPath, **kwargs)
         #
 
     def testCache(self, minCount=500):
         if self.__oD and len(self.__oD) > minCount:
             return True
         else:
             return False
@@ -49,14 +50,17 @@
             aroId (str): ARO ID in the form of "ARO:3001059"
 
         Returns:
             list: list of dictionaries containing the "id" and "name" of each parent
         """
         return self.__oD.get(aroId, [])
 
+    def getTreeNodeList(self):
+        return self.__tnL
+
     def __reload(self, dirPath, **kwargs):
         oD = None
         version = None
         startTime = time.time()
         useCache = kwargs.get("useCache", True)
         #
         ok = False
@@ -80,35 +84,35 @@
         else:
             logger.info("Fetching url %s path %s", ontologyDumpUrl, ontologyDumpPath)
             ok = fU.get(ontologyDumpUrl, ontologyDumpPath)
             fU.mkdir(ontologyDumpDirPath)
             fU.uncompress(ontologyDumpPath, outputDir=ontologyDumpDirPath)
             fU.unbundleTarfile(os.path.join(ontologyDumpDirPath, ontologyDumpFileName[:-4]), dirPath=ontologyDumpDirPath)
             logger.info("Completed fetch (%r) at %s (%.4f seconds)", ok, time.strftime("%Y %m %d %H:%M:%S", time.localtime()), time.time() - startTime)
-            oD, version = self.__parseOntologyData(os.path.join(ontologyDumpDirPath, "aro.obo"))
+            oD, tnL, version = self.__parseOntologyData(os.path.join(ontologyDumpDirPath, "aro.obo"))
             #
             tS = datetime.datetime.now().isoformat()
             qD = {"version": version, "created": tS, "data": oD}
             oD = qD["data"]
             ok = self.__mU.doExport(ontologyDataPath, qD, fmt="json", indent=3)
             logger.info("Export CARD ontology data (%d) status %r", len(oD), ok)
 
-        return oD, version
+        return oD, tnL, version
 
     def __parseOntologyData(self, filePath):
         """Parse CARD ontology data
 
         Args:
             filePath (str): card ontology data file (aro.obo)
 
         Returns:
             (dict, string): dictionary of all ARO IDs and their ancestor lineages, ontology version string
         """
         try:
-            cpD = None
+            cpD, tnL = None, None
             version = None
             parentChildList = []
             idNameD = {}
 
             with open(filePath, "r", encoding="utf-8") as f:
                 data = f.read()
 
@@ -131,54 +135,75 @@
                     if childName and childId not in idNameD:
                         idNameD[childId] = childName
                     if item.startswith("[Typedef]"):
                         break
 
             logger.info("Ontology parent-child pair count (%d)", len(parentChildList))
 
-            cpD = self.__buildLineageTree(parentChildList, idNameD)
+            cpD, tnL = self.__buildLineageTree(parentChildList, idNameD)
 
         except Exception as e:
             logger.exception("Failing with %s", str(e))
-        return cpD, version
+        return cpD, tnL, version
 
     def __buildLineageTree(self, parentChildTupleList, idNameMapD):
-        """Build a lineage tree containing all children as keys and a
-        list of all possible parents as the values.
+        """Build a lineage tree containing all children as keys and a list of all possible parents as the values.
 
         Args:
             parentChildTupleList (list): list of (parent, child) tuples (e.g., [('ARO:1000003', 'ARO:0000000'), ('ARO:1000003', 'ARO:0000001')])
             idNameMapD (dict): dictionary mapping of ARO IDs to their corresponding name
 
         Returns:
             dict: dictionary containing all children as keys and all possible parents as values
                   (including the child itself, but excluding the top-level parent 'ARO:1000001')
         """
         # create a dictionary to store the parents of each child
-        parents = {}
+        childToParentD = {}
         for parent, child in parentChildTupleList:
-            if child not in parents:
-                parents[child] = []
-            parents[child].append(parent)
+            if child not in childToParentD:
+                childToParentD[child] = []
+            childToParentD[child].append(parent)
+
+        treeNodeL = self.__exportTreeNodeList(childToParentD, idNameMapD)
 
         # create a dictionary to store the ancestors of each child
         lineageD = {}
-        for child in parents.keys():
-            lineageD[child] = []
+        for child in childToParentD.keys():
+            lineageD[child] = [{"id": child, "name": idNameMapD[child], "depth": 0}]  # Add the child to its own ancestry list
             stack = [child]
+            depth = -1
             while stack:
                 node = stack.pop()
-                if node in parents:
-                    for parent in parents[node]:
-                        lineageD[child].append(parent)
-                        stack.append(parent)
-
-        # Go through the lineage dict and add the child to its own list and remove the top-level "ARO:1000001"
-        # Also, update the list to contain both the parent ARO IDs and their associated names.
-        for child, pL in lineageD.items():
-            if child not in pL:
-                npL = [child] + [p for p in pL if p != "ARO:1000001"]
-                npL.reverse()  # List oldest/broadest ancestor first (depth=1), youngest/most-specific child last (depth=n)
-                npL = [{"id": id, "name": idNameMapD[id], "depth": ii + 1} for ii, id in enumerate(npL)]
-                lineageD[child] = npL
+                if node in childToParentD:
+                    for parent in childToParentD[node]:
+                        if parent != "ARO:1000001":  # Exclude the top-level "ARO:1000001"
+                            if parent not in [d["id"] for d in lineageD[child]]:
+                                lineageD[child].append({"id": parent, "name": idNameMapD[parent], "depth": depth})
+                                stack.append(parent)
+                    depthLevels = set(i["depth"] for i in lineageD[child])
+                    depth = min(depthLevels) - 1
+            numDepthLevels = len(set(i["depth"] for i in lineageD[child]))
+            #
+            # Flip the depth numbering so that oldest ancestor has depth=1 and youngest/most-specific child has depth=n
+            nL = []
+            for aD in lineageD[child]:
+                aD["depth"] += numDepthLevels
+                nL.append(aD)
+            snL = sorted(nL, key=lambda x: x["depth"])  # List oldest/broadest ancestor first (depth=1), youngest/most-specific child last (depth=n)
+            lineageD[child] = snL
+
+        return lineageD, treeNodeL
+
+    def __exportTreeNodeList(self, childToParentD, idNameMapD):
+        """Create tree node list in the format of:
+
+        {'id': 'ARO:1000003', 'name': 'antibiotic molecule'}
+        {'id': 'ARO:0000041', 'name': 'bacitracin', 'parents': ['ARO:3000053', 'ARO:3000707']}
+        {'id': 'ARO:0000039', 'name': 'spectinomycin', 'parents': ['ARO:0000016']}
+        """
+        #
+        dL = []
+        for child, parentL in childToParentD.items():
+            tD = {"id": child, "name": idNameMapD[child], "parents": parentL}
+            dL.append(tD)
 
-        return lineageD
+        return dL
```

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.67/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.66
+Version: 0.67
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.66/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.67/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.66/setup.py` & `rcsb.utils.targets-0.67/setup.py`

 * *Files identical despite different names*

