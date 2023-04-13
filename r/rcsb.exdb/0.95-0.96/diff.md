# Comparing `tmp/rcsb.exdb-0.95.tar.gz` & `tmp/rcsb.exdb-0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.exdb-0.95.tar", last modified: Wed Mar 15 17:25:13 2023, max compression
+gzip compressed data, was "rcsb.exdb-0.96.tar", last modified: Thu Apr 13 21:42:14 2023, max compression
```

## Comparing `rcsb.exdb-0.95.tar` & `rcsb.exdb-0.96.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/
--rw-r--r--   0 vsts      (1001) docker     (122)     7187 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4716 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.748362 rcsb.exdb-0.95/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb/exdb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb/exdb/branch/
--rw-r--r--   0 vsts      (1001) docker     (122)     2645 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/branch/BranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/branch/GlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4507 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/branch/GlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/branch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb/exdb/chemref/
--rw-r--r--   0 vsts      (1001) docker     (122)     4602 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/ChemRefEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2538 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/ChemRefExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5180 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/ChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15479 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/PubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11699 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/PubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    29079 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb/exdb/citation/
--rw-r--r--   0 vsts      (1001) docker     (122)     3501 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/citation/CitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7574 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/citation/CitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/citation/CitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb/exdb/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     9878 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/cli/ExDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb/exdb/entry/
--rw-r--r--   0 vsts      (1001) docker     (122)     5095 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/entry/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/entry/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.756362 rcsb.exdb-0.95/rcsb/exdb/seq/
--rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/AnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3423 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/LigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/PolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28751 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25935 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18181 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18008 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2315 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/TaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7477 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/UniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/UniProtExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/seq/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/rcsb/exdb/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3999 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9677 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/fixturePdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testAnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2936 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testBranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3696 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testChemRefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3353 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3625 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testCitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3141 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testCitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3064 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testCitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3360 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testEntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5268 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testGlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3201 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testGlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1953 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testGlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3040 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14144 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2944 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3537 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testPolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4679 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5187 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6511 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4947 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4186 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4897 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5005 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3469 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testTaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3557 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testTreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3403 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tests/testUniProtExtractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/rcsb/exdb/tree/
--rw-r--r--   0 vsts      (1001) docker     (122)    11284 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tree/TreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/tree/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/rcsb/exdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      466 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/utils/ObjectAdapterBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11057 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/utils/ObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/utils/ObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5089 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/utils/ObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6954 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/utils/ObjectValidator.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/rcsb/exdb/wf/
--rw-r--r--   0 vsts      (1001) docker     (122)     2486 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10714 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/wf/ExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2736 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/wf/GlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10388 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/wf/PubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/rcsb/exdb/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-15 17:25:13.752362 rcsb.exdb-0.95/rcsb.exdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-03-15 17:25:13.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-03-15 17:25:13.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-15 17:25:13.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-03-15 17:25:13.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-15 17:06:47.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-03-15 17:25:13.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-15 17:25:13.000000 rcsb.exdb-0.95/rcsb.exdb.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      443 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-15 17:25:13.760362 rcsb.exdb-0.95/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2184 2023-03-15 17:03:12.000000 rcsb.exdb-0.95/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/
+-rw-r--r--   0 vsts      (1001) docker     (122)     7244 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4716 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb/exdb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb/exdb/branch/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2645 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/BranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4000 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/GlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4507 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/GlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/branch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4602 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2538 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5180 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15479 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11699 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29079 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/citation/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3501 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/CitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7574 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/CitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/CitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9878 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/cli/ExDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.503020 rcsb.exdb-0.96/rcsb/exdb/entry/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5095 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/entry/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/entry/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.507021 rcsb.exdb-0.96/rcsb/exdb/seq/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/AnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3423 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3654 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/PolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28751 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25935 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18181 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18008 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2315 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/TaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7477 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/UniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2695 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/UniProtExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/seq/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3999 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9677 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/fixturePdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2657 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testAnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2936 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testBranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3696 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3353 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3625 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testCitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3141 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testCitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3064 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testCitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3360 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5268 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2295 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3201 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1953 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3040 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14144 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2944 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3537 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4679 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5187 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6511 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4947 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4186 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4897 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5005 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3469 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2536 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testTaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3557 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testTreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3403 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2604 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtExtractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/tree/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11987 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tree/TreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/tree/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      466 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11057 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5089 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6954 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/ObjectValidator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/rcsb/exdb/wf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2486 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10714 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/ExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2736 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/GlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10388 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/PubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/rcsb/exdb/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-13 21:42:14.499020 rcsb.exdb-0.96/rcsb.exdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5397 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-13 21:14:08.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      399 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-13 21:42:14.000000 rcsb.exdb-0.96/rcsb.exdb.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      443 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-13 21:42:14.515022 rcsb.exdb-0.96/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2184 2023-04-13 21:08:38.000000 rcsb.exdb-0.96/setup.py
```

### Comparing `rcsb.exdb-0.95/HISTORY.txt` & `rcsb.exdb-0.96/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -84,8 +84,9 @@
                   Add computed-models to tests & workflow;
                   Fix test case in testObjectExtractor;
                   Switch fixturePdbxLoader to use remote HTTP loading for Azure tests instead of local mock/sandbox paths
 25-May-2022 V0.92 Add error checking for SIFTS data loading in ReferenceSequenceAnnotationProvider and ReferenceSequenceAssignmentProvider
  9-Jan-2023 V0.93 Configuration changes to support tox 4
  9-Mar-2023 V0.94 Update ExDbWorkflow to make use of multiple processors for 'upd_ref_seq' operation;
                   Lower refChunkSize to 10 for requests to UniProt API
-13-Mar-2023 V0.95 Updates to PubChem workflow to use multiprocess count, disable git stash testing, remove obsolete entries from test data
+13-Mar-2023 V0.95 Updates to PubChem workflow to use multiprocess count, disable git stash testing, remove obsolete entries from test data
+12-Apr-2023 V0.96 Add CARD ontology data to tree builder
```

### Comparing `rcsb.exdb-0.95/LICENSE` & `rcsb.exdb-0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/PKG-INFO` & `rcsb.exdb-0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 0.95
+Version: 0.96
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.exdb-0.95/README.md` & `rcsb.exdb-0.96/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/branch/BranchedEntityExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/branch/BranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/branch/GlycanProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/branch/GlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/branch/GlycanUtils.py` & `rcsb.exdb-0.96/rcsb/exdb/branch/GlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/chemref/ChemRefEtlWorker.py` & `rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/chemref/ChemRefExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/chemref/ChemRefMappingProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/chemref/ChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/chemref/PubChemDataCacheProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/chemref/PubChemEtlWrapper.py` & `rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/chemref/PubChemIndexCacheProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/chemref/PubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/citation/CitationAdapter.py` & `rcsb.exdb-0.96/rcsb/exdb/citation/CitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/citation/CitationExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/citation/CitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/citation/CitationUtils.py` & `rcsb.exdb-0.96/rcsb/exdb/citation/CitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/cli/ExDbExec.py` & `rcsb.exdb-0.96/rcsb/exdb/cli/ExDbExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/entry/EntryInfoProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/entry/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/AnnotationExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/AnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/LigandNeighborMappingExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/LigandNeighborMappingProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/LigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/PolymerEntityExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/PolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/TaxonomyExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/TaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/UniProtCoreEtlWorker.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/UniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/seq/UniProtExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/seq/UniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/fixturePdbxLoader.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/fixturePdbxLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testAnnotationExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testAnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testBranchedEntityExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testBranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testChemRefLoader.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testChemRefMappingProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testCitationAdapter.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testCitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testCitationExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testCitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testCitationUtils.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testCitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testEntryInfoProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testEntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testExDbWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testExDbWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testGlycanEtlWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testGlycanProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testGlycanUtils.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testGlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testLigandNeighborMappingProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testLigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testObjectExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testObjectTransformer.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testObjectUpdater.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testPolymerEntityExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testPolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemDataCacheProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemEtlWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemEtlWrapper.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testPubChemIndexCacheProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testPubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testTaxonomyExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testTaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testTreeNodeListWorker.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testTreeNodeListWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testUniProtCoreEtlWorker.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tests/testUniProtExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/tests/testUniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/tree/TreeNodeListWorker.py` & `rcsb.exdb-0.96/rcsb/exdb/tree/TreeNodeListWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # File: TreeNodeListWorker.py
 # Date: 9-Apr-2019  jdw
 #
 # Loading worker for tree node list data.
 #
 # Updates:
 #  9-Sep-2019 jdw add AtcProvider() and ChemrefExtractor() for ATC tree.
-# JDW TODO TEST
+# 12-Apr-2023 dwp add CARD ontology tree
+#
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
@@ -19,14 +20,15 @@
 from rcsb.db.mongo.DocumentLoader import DocumentLoader
 from rcsb.db.processors.DataExchangeStatus import DataExchangeStatus
 from rcsb.exdb.chemref.ChemRefExtractor import ChemRefExtractor
 from rcsb.exdb.seq.AnnotationExtractor import AnnotationExtractor
 from rcsb.exdb.seq.TaxonomyExtractor import TaxonomyExtractor
 from rcsb.utils.chemref.AtcProvider import AtcProvider
 from rcsb.utils.ec.EnzymeDatabaseProvider import EnzymeDatabaseProvider
+from rcsb.utils.targets.CARDTargetOntologyProvider import CARDTargetOntologyProvider
 from rcsb.utils.go.GeneOntologyProvider import GeneOntologyProvider
 from rcsb.utils.struct.CathClassificationProvider import CathClassificationProvider
 from rcsb.utils.struct.EcodClassificationProvider import EcodClassificationProvider
 from rcsb.utils.struct.ScopClassificationProvider import ScopClassificationProvider
 from rcsb.utils.struct.Scop2ClassificationProvider import Scop2ClassificationProvider
 from rcsb.utils.taxonomy.TaxonomyProvider import TaxonomyProvider
 
@@ -168,14 +170,22 @@
             edbu = EnzymeDatabaseProvider(cachePath=self.__cachePath, useCache=useCache)
             nL = edbu.getTreeNodeList()
             logger.info("Starting load of EC node tree length %d", len(nL))
             if doLoad:
                 collectionName = "tree_ec_node_list"
                 ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
                 self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
+            # ---- CARD
+            cou = CARDTargetOntologyProvider(cachePath=self.__cachePath, useCache=False)
+            nL = cou.getTreeNodeList()
+            logger.info("Starting load of EC node tree length %d", len(nL))
+            if doLoad:
+                collectionName = "tree_card_node_list"
+                ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=nL, indexAttributeList=["update_id"], keyNames=None, addValues=addValues, schemaLevel=None)
+                self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
             # ---- Taxonomy
             # Get the taxon coverage in the current data set -
             epe = TaxonomyExtractor(self.__cfgOb)
             tL = epe.getUniqueTaxons()
             logger.info("Taxon coverage length %d", len(tL))
             #
             tU = TaxonomyProvider(cachePath=self.__cachePath, useCache=useCache)
```

### Comparing `rcsb.exdb-0.95/rcsb/exdb/utils/ObjectExtractor.py` & `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/utils/ObjectTransformer.py` & `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/utils/ObjectUpdater.py` & `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/utils/ObjectValidator.py` & `rcsb.exdb-0.96/rcsb/exdb/utils/ObjectValidator.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/wf/EntryInfoEtlWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/wf/EntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/wf/ExDbWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/wf/ExDbWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/wf/GlycanEtlWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/wf/GlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb/exdb/wf/PubChemEtlWorkflow.py` & `rcsb.exdb-0.96/rcsb/exdb/wf/PubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/rcsb.exdb.egg-info/PKG-INFO` & `rcsb.exdb-0.96/rcsb.exdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 0.95
+Version: 0.96
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.exdb-0.95/rcsb.exdb.egg-info/SOURCES.txt` & `rcsb.exdb-0.96/rcsb.exdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-0.95/setup.py` & `rcsb.exdb-0.96/setup.py`

 * *Files identical despite different names*

