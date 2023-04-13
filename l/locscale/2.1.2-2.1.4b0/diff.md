# Comparing `tmp/locscale-2.1.2.tar.gz` & `tmp/locscale-2.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locscale-2.1.2.tar", last modified: Wed Oct  5 16:48:21 2022, max compression
+gzip compressed data, was "dist/locscale-2.1.4b0.tar", last modified: Thu Apr 13 15:09:06 2023, max compression
```

## Comparing `locscale-2.1.2.tar` & `locscale-2.1.4b0.tar`

### file list

```diff
@@ -1,92 +1,96 @@
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.902202 locscale-2.1.2/
--rw-r--r--   0 alok      (1000) alok      (1000)      112 2022-10-05 16:13:52.000000 locscale-2.1.2/MANIFEST.in
--rw-r--r--   0 alok      (1000) alok      (1000)    12603 2022-10-05 16:48:21.902202 locscale-2.1.2/PKG-INFO
--rwxr-xr-x   0 alok      (1000) alok      (1000)    11879 2022-10-05 16:13:52.000000 locscale-2.1.2/README.md
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.805296 locscale-2.1.2/locscale/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/__init__.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.811174 locscale-2.1.2/locscale/automate/
--rw-r--r--   0 alok      (1000) alok      (1000)     3108 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/automate/__init__.py
--rw-r--r--   0 alok      (1000) alok      (1000)    19807 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/automate/tools.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.817174 locscale-2.1.2/locscale/emmernet/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/emmernet/__init__.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     8207 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/emmernet/emmernet_functions.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     1427 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/emmernet/prepare_inputs.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     6828 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/emmernet/run_emmernet.py
--rw-r--r--   0 alok      (1000) alok      (1000)     4711 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/emmernet/utils.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.818175 locscale-2.1.2/locscale/include/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/__init__.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.824176 locscale-2.1.2/locscale/include/confidenceMapUtil/
--rwxr-xr-x   0 alok      (1000) alok      (1000)    21243 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/confidenceMapUtil/FDRutil.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/confidenceMapUtil/__init__.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     6395 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/confidenceMapUtil/confidenceMapMain.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    28996 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/confidenceMapUtil/locscaleUtil.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     9543 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/confidenceMapUtil/mapUtil.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.826176 locscale-2.1.2/locscale/include/emmer/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/__init__.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)      451 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/headers.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.861738 locscale-2.1.2/locscale/include/emmer/ndimage/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/__init__.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)      314 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/common_map_headers.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     8135 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/emdb_class.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     4899 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/fft_util.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     6459 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/filter.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    18483 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/emmer/ndimage/fsc_util.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    12427 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/map_quality_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    20573 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/emmer/ndimage/map_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    23280 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/emmer/ndimage/map_utils.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     5382 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/plotContourMap.py
--rw-r--r--   0 alok      (1000) alok      (1000)    11142 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/emmer/ndimage/plots.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     1239 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/power.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    22184 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/profile_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)      703 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/ndimage/simulate.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.873689 locscale-2.1.2/locscale/include/emmer/pdb/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/__init__.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)      484 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/common_pdb_headers.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)      977 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3749 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     4171 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/get_dssp.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)      941 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/modify_pdb.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     8516 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/pdb_to_map.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    19343 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/emmer/pdb/pdb_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    29147 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/emmer/pdb/pdb_utils.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.878693 locscale-2.1.2/locscale/include/symmetry_emda/
--rwxr-xr-x   0 alok      (1000) alok      (1000)    39092 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/symmetry_emda/__init__.py
--rw-r--r--   0 alok      (1000) alok      (1000)    29183 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/symmetry_emda/apply_rotation_matrix.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)   136871 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/include/symmetry_emda/fcodes_fast.f90
--rw-r--r--   0 alok      (1000) alok      (1000)     3309 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/include/symmetry_emda/symmetrize_map.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    16808 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/main.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.886794 locscale-2.1.2/locscale/preprocessing/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/preprocessing/__init__.py
--rw-r--r--   0 alok      (1000) alok      (1000)    28773 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/preprocessing/headers.py
--rw-r--r--   0 alok      (1000) alok      (1000)    13109 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/preprocessing/pipeline.py
--rw-r--r--   0 alok      (1000) alok      (1000)    13639 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/preprocessing/pseudomodel_classes.py
--rw-r--r--   0 alok      (1000) alok      (1000)    13077 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/preprocessing/pseudomodel_solvers.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.892199 locscale-2.1.2/locscale/tests/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/tests/__init__.py
--rw-r--r--   0 alok      (1000) alok      (1000)     8246 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/tests/locscale_modules.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3442 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/tests/test_emmernet.py
--rw-r--r--   0 alok      (1000) alok      (1000)     9295 2022-10-05 16:47:49.000000 locscale-2.1.2/locscale/tests/test_locscale.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3046 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/tests/test_symmetry.py
--rw-r--r--   0 alok      (1000) alok      (1000)     2073 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/tests/utils.py
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.901968 locscale-2.1.2/locscale/utils/
--rwxr-xr-x   0 alok      (1000) alok      (1000)     3108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/utils/__init__.py
--rw-r--r--   0 alok      (1000) alok      (1000)    15964 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/utils/file_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    11005 2022-10-05 16:13:52.000000 locscale-2.1.2/locscale/utils/general.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     8598 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/utils/map_quality.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)     1108 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/utils/math_tools.py
--rw-r--r--   0 alok      (1000) alok      (1000)    10774 2022-10-05 16:13:53.000000 locscale-2.1.2/locscale/utils/plot_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    20759 2022-10-05 16:13:53.000000 locscale-2.1.2/locscale/utils/prepare_inputs.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    33896 2022-10-05 16:13:53.000000 locscale-2.1.2/locscale/utils/scaling_tools.py
--rwxr-xr-x   0 alok      (1000) alok      (1000)    10678 2022-06-27 17:49:37.000000 locscale-2.1.2/locscale/utils/theoretical_profiles.pickle
-drwxr-xr-x   0 alok      (1000) alok      (1000)        0 2022-10-05 16:48:21.809175 locscale-2.1.2/locscale.egg-info/
--rw-r--r--   0 alok      (1000) alok      (1000)    12603 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/PKG-INFO
--rw-r--r--   0 alok      (1000) alok      (1000)     2827 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/SOURCES.txt
--rw-r--r--   0 alok      (1000) alok      (1000)        1 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/dependency_links.txt
--rw-r--r--   0 alok      (1000) alok      (1000)       48 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/entry_points.txt
--rw-r--r--   0 alok      (1000) alok      (1000)        1 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/not-zip-safe
--rw-r--r--   0 alok      (1000) alok      (1000)      373 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/requires.txt
--rw-r--r--   0 alok      (1000) alok      (1000)       21 2022-10-05 16:48:21.000000 locscale-2.1.2/locscale.egg-info/top_level.txt
--rw-r--r--   0 alok      (1000) alok      (1000)      138 2022-10-05 16:13:53.000000 locscale-2.1.2/pyproject.toml
--rwxr-xr-x   0 alok      (1000) alok      (1000)      107 2022-10-05 16:48:21.904331 locscale-2.1.2/setup.cfg
--rw-r--r--   0 alok      (1000) alok      (1000)     4468 2022-10-05 16:47:49.000000 locscale-2.1.2/setup.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      112 2023-04-13 14:56:22.000000 locscale-2.1.4b0/MANIFEST.in
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12585 2023-04-13 15:09:06.000000 locscale-2.1.4b0/PKG-INFO
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    11879 2023-04-13 14:56:22.000000 locscale-2.1.4b0/README.md
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3145 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)       24 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/__version__.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/automate/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/automate/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    19847 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/automate/tools.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/emmernet/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8207 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/emmernet_functions.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     1513 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/prepare_inputs.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8544 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/run_emmernet.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     6807 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/utils.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/__init__.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    21182 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/FDRutil.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     6395 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/confidenceMapMain.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    28996 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/locscaleUtil.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     9543 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/mapUtil.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/emmer/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      451 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/headers.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      301 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/common_map_headers.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     8135 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/emdb_class.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     4899 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/fft_util.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     6459 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/filter.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    18483 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/fsc_util.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12535 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/map_quality_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22698 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/map_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    24544 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/map_utils.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     5382 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/plotContourMap.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    15302 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/plots.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     1239 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/power.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22355 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/profile_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      703 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/simulate.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      471 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/common_pdb_headers.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      977 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     5196 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/fitting_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3749 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     4171 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/get_dssp.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      941 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/modify_pdb.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     8502 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_to_map.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22212 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    30907 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_utils.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    39092 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    29183 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/apply_rotation_matrix.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)   136871 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/fcodes_fast.f90
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3335 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/symmetrize_map.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     2181 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/main.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/preprocessing/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    31098 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/headers.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    15239 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/pipeline.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    13909 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/pseudomodel_classes.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    13077 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/pseudomodel_solvers.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/tests/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8246 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/locscale_modules.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3442 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/test_emmernet.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    10021 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/test_locscale.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3046 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/test_symmetry.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     2114 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/utils.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/utils/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    17346 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/file_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    10962 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/general.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8644 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/map_quality.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     1108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/math_tools.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8721 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/parse_utils.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    11144 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/plot_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    21576 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/prepare_inputs.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    34587 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/scaling_tools.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     7000 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/startup_utils.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    10678 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/theoretical_profiles.pickle
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12585 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/PKG-INFO
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     2957 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/SOURCES.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)        1 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/dependency_links.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)       48 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/entry_points.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)        1 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/not-zip-safe
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      374 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/requires.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)       21 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/top_level.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      138 2023-04-13 14:56:22.000000 locscale-2.1.4b0/pyproject.toml
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      107 2023-04-13 15:09:06.000000 locscale-2.1.4b0/setup.cfg
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     4899 2023-04-13 14:56:22.000000 locscale-2.1.4b0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `locscale-2.1.2/PKG-INFO` & `locscale-2.1.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: locscale
-Version: 2.1.2
+Version: 2.1.4b0
 Summary: Contrast optimization for cryo-EM maps
 Home-page: https://gitlab.tudelft.nl/aj-lab/locscale
 Author: Alok Bharadwaj, Arjen J. Jakobi, Reinier de Bruin
 License: 3-clause BSD
 Project-URL: Bug Tracker, https://gitlab.tudelft.nl/aj-lab/locscale/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
@@ -230,9 +229,7 @@
 - A.J. Jakobi, M. Wilmanns and C. Sachse, [Model-based local density sharpening of cryo-EM maps](https://doi.org/10.7554/eLife.27131), eLife 6: e27131 (2017).
 - A. Bharadwaj and A.J. Jakobi, [Electron scattering properties and their use in cryo-EM map sharpening](https://doi.org/10.1039/D2FD00078D), Faraday Discussions D2FD00078D (2022)
 ---
 
 ## Bugs and questions
 
 For bug reports please use the [GitLab issue tracker](https://gitlab.tudelft.nl/aj-lab/locscale/issues).   
-
-
```

### Comparing `locscale-2.1.2/README.md` & `locscale-2.1.4b0/README.md`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/__init__.py` & `locscale-2.1.4b0/locscale/automate/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/automate/__init__.py` & `locscale-2.1.4b0/locscale/emmernet/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/automate/tools.py` & `locscale-2.1.4b0/locscale/automate/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import argparse
 from distutils.cmd import Command
 from genericpath import isfile
 import os
 from socket import timeout
 import sys
 from subprocess import PIPE
-from locscale.main import launch_amplitude_scaling
+from locscale.utils.startup_utils import launch_locscale_no_mpi
 import json
 import pickle
 
 def get_defaults_dictionary():
     """
     Get the default input dictionary.
     """
-    from locscale.main import locscale_parser
+    from locscale.utils.parse_utils import locscale_parser
     defaults_dictionary = {}
     variables = locscale_parser._actions
     for variable in variables:
         # if variable.dest is not help then add to dictionary
         if variable.dest != 'help':
             defaults_dictionary[variable.dest] = variable.default
     
@@ -175,15 +175,15 @@
     def __init__(self, Input, job_name, locscale_run_type, mpi_jobs, data_folder=None):
         self.input = Input.clone()
     
         self.job_name = job_name
         self.locscale_run_type = locscale_run_type
         self.job_file_path = None
         self.job = None
-        self.timeout = 4*3600 # 4 hours
+        self.timeout = 8*3600
         self.mpi_jobs = mpi_jobs
         self.input.check_is_halfmap_input()
         if data_folder is not None:
             self.data_folder = data_folder
         else:
             input_folder = self.input.get_folder_from_input_paths()
             self.data_folder = os.path.join(input_folder, job_name)
@@ -254,15 +254,15 @@
         sys.stderr = log_file
         print("Submitting job {}".format(self.job_name))
 
         args = argparse.Namespace()
         args.__dict__.update(self.job["args"])
 
         # Run LocScale
-        launch_amplitude_scaling(args)
+        launch_locscale_no_mpi(args)
 
         print("Job {} submitted".format(self.job_name))
     
 
     def print_header(self):
         print("~"*80)
         print("Executing job name: {}".format(self.job_name))
@@ -285,15 +285,15 @@
         self.resume_scaling = False
 
         for job in self.input_jobs:
             job.prepare_job()
     
     def launch_locscale(self, job_id):
         from locscale.utils.file_tools import change_directory, check_user_input, get_input_file_directory
-        from locscale.main import print_arguments, print_end_banner, print_start_banner, launch_amplitude_scaling
+        from locscale.utils.startup_utils import print_arguments, print_end_banner, print_start_banner, launch_locscale_no_mpi
         from locscale.utils.prepare_inputs import prepare_mask_and_maps_for_scaling
         from datetime import datetime
         from contextlib import redirect_stdout
 
         ## Collect all preprocessing steps for all jobs
         args = argparse.Namespace()
         args.__dict__.update(self.input_jobs[job_id].job["args"])
@@ -302,15 +302,15 @@
         data_folder = self.input_jobs[job_id].job["data_folder"]
         parsed_dict_pickle = os.path.join(data_folder, "parsed_inputs.pickle")
         job_name = self.input_jobs[job_id].job["job_name"]
         with open(log_file_path, "a") as f:
             with redirect_stdout(f):
                 if not self.dry_run:
                     try:
-                        launch_amplitude_scaling(args)
+                        launch_locscale_no_mpi(args)
                     except Exception as e:
                         print("Error in job {}: {}".format(job_name, e))
                         with open(log_file_path, "a") as f:
                             f.write("Error in job {}: {}".format(job_name, e))
                             f.write("\n")
                         returncode = 1
                     
@@ -335,15 +335,15 @@
         
         returncode = 0
         return returncode
        
         
     def get_parsed_inputs_dict(self, job_id):
         from locscale.utils.file_tools import change_directory, check_user_input, get_input_file_directory
-        from locscale.main import print_arguments, print_end_banner, print_start_banner
+        from locscale.utils.startup_utils import print_arguments, print_end_banner, print_start_banner
         from locscale.utils.prepare_inputs import prepare_mask_and_maps_for_scaling
         from datetime import datetime
         from contextlib import redirect_stdout
 
         ## Collect all preprocessing steps for all jobs
         args = argparse.Namespace()
         args.__dict__.update(self.input_jobs[job_id].job["args"])
@@ -462,22 +462,22 @@
         # Submit jobs
         if self.split_jobs:
 
             # Run the preprocessing steps in parallel
             if self.resume_scaling:
                 print("Resuming scaling from stored state")
             else:
-                joblib.Parallel(n_jobs=self.num_process_preparation, backend="loky", timeout=2*3600)(
+                joblib.Parallel(n_jobs=self.num_process_preparation, backend="loky", timeout=6*3600)(
                     joblib.delayed(self.get_parsed_inputs_dict)(job_id) for job_id in job_list)
 
             ## Run the scaling in parallel
-            result = joblib.Parallel(n_jobs=self.num_process_scaling, backend="loky",timeout=2*3600)(
+            result = joblib.Parallel(n_jobs=self.num_process_scaling, backend="loky",timeout=6*3600)(
                 joblib.delayed(self.scale_amplitudes)(job_id) for job_id in job_list)
         else:
-            result = joblib.Parallel(n_jobs=self.num_process_scaling, backend="loky",timeout=4*3600)(
+            result = joblib.Parallel(n_jobs=self.num_process_scaling, backend="loky",timeout=6*3600)(
                 joblib.delayed(self.launch_locscale)(job_id) for job_id in job_list)
 
         
         # Print the results for each job
         for job_id in job_list:
             print("Job {} finished with status {}".format(job_id, result[job_id]))
```

### Comparing `locscale-2.1.2/locscale/emmernet/__init__.py` & `locscale-2.1.4b0/locscale/include/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/emmernet/emmernet_functions.py` & `locscale-2.1.4b0/locscale/emmernet/emmernet_functions.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/emmernet/prepare_inputs.py` & `locscale-2.1.4b0/locscale/emmernet/prepare_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     xyz_emmap_path = check_axis_order(emmap_path)
     emmernet_type = args.trained_model
     stride = args.stride
     verbose = args.verbose
     outputfile = args.outfile
     batch_size = args.batch_size
     gpu_ids = args.gpu_ids
+    target_map_path = args.target_map_path
     
 
 
 
     inputs_dictionary = {
         "emmap_path": emmap_path,
         'xyz_emmap_path': xyz_emmap_path,
@@ -36,14 +37,15 @@
         "stride": stride,
         "verbose": verbose,
         "outfile": outputfile,
         "batch_size": batch_size,
         "gpu_ids": gpu_ids,
         "emmap_folder": emmap_folder,
         "emmernet_model_folder": emmernet_model_folder,
+        "target_map_path": target_map_path
         }
     
     if verbose:
         print("Inputs parsed successfully")
     print("."*80)
     return inputs_dictionary
```

### Comparing `locscale-2.1.2/locscale/emmernet/run_emmernet.py` & `locscale-2.1.4b0/locscale/emmernet/run_emmernet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ## Script to run EMmerNet on an input map
 ## import the necessary packages from locscale.include.emmer
 
 from locscale.include.emmer.ndimage.map_utils import resample_map, load_map
 from locscale.emmernet.emmernet_functions import standardize_map, minmax_normalize_map, get_cubes, assemble_cubes
+from locscale.emmernet.utils import compute_local_phase_correlations, plot_phase_correlations
+
 import numpy as np
 import os
+from tqdm import tqdm
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'  
 
 
 def run_emmernet(input_dictionary):
     ## Ignore DeprecationWarning
     import warnings
@@ -24,32 +27,45 @@
     emmap_path = input_dictionary["emmap_path"]
     emmernet_type = input_dictionary["emmernet_type"]
     stride = input_dictionary["stride"]
     batch_size = input_dictionary["batch_size"]
     gpu_ids = input_dictionary["gpu_ids"]
     verbose = input_dictionary["verbose"]
     emmernet_model_folder = input_dictionary["emmernet_model_folder"]
+    target_map_path = input_dictionary["target_map_path"]
+    if target_map_path is not None:
+        target_map, _ = load_map(target_map_path)
+        target_map_present = True
+    else:
+        target_map_present = False
+    
 
     emmap, apix = load_map(emmap_path)
+    input_map_shape = emmap.shape
     if verbose:
         print("Emmap loaded from: {}".format(emmap_path))
         print("Emmap shape: {}".format(emmap.shape))
         print("Pixelsize read as: {:.2f}".format(apix))
 
         print("1) Pre-processing commencing...")
     
     ## Preprocess
 
     emmap_preprocessed = preprocess_map(emmap, apix)
+    if target_map_present:
+        target_map_preprocessed = preprocess_map(target_map, apix)
     if verbose:
         print("\tPreprocessing complete")
         print("\tPre-processed map shape: {}".format(emmap_preprocessed.shape))
         print("2) Prediction commencing...")
 
     cubes, cubecenters = get_cubes(emmap_preprocessed, cube_size=EMMERNET_CUBE_SIZE, step_size=stride)
+    if target_map_present:
+        target_cubes, _ = get_cubes(target_map_preprocessed, cube_size=EMMERNET_CUBE_SIZE, step_size=stride)
+        
     if verbose:
         print("\tCubes extracted")
         print("\tNumber of cubes: {}".format(len(cubes)))
     ## Load the model
 
     emmernet_model = load_emmernet_model(emmernet_type, emmernet_model_folder)
     if verbose:
@@ -60,36 +76,46 @@
     # prepare GPU id list
     if gpu_ids is None:
         print("No GPU id specified, running on CPU")
         print("If you want to use GPUs, please specify the GPU id(s) using the --gpu_ids flag")
         print("This may take a while...")
         mirrored_strategy = tf.distribute.MirroredStrategy()
     else:
+        os.environ["CUDA_VISIBLE_DEVICES"] = ",".join([str(gpu_id) for gpu_id in gpu_ids])
+        print("Setting CUDA_VISIBLE_DEVICES to {}".format(os.environ["CUDA_VISIBLE_DEVICES"]))
         gpu_id_list = ["/gpu:"+str(gpu_id) for gpu_id in gpu_ids]
         if verbose:
             print("\tGPU ids: {}".format(gpu_id_list))
         mirrored_strategy = tf.distribute.MirroredStrategy(devices=gpu_id_list)
     
     predicted_cubes = run_emmernet_batch(cubes, emmernet_model, mirrored_strategy, batch_size=batch_size)
 
+    if target_map_present:
+        # Compute phase correlations between predicted and target cubes
+        processing_files_folder = os.path.dirname(emmap_path)
+        phase_correlations, freq = compute_local_phase_correlations(target_cubes=target_cubes, predicted_cubes=predicted_cubes, apix=apix, temp_folder=processing_files_folder)
+        phase_correlations_fig_path = os.path.join(processing_files_folder, "phase_correlations.png")
+        fig = plot_phase_correlations(phase_correlations, freq)
+        fig.savefig(phase_correlations_fig_path)
+        
     if verbose:
         print("\tEMmerNet prediction complete")
         print("\tNumber of predicted cubes: {}".format(len(predicted_cubes)))
     ## Merge the predicted cubes sequence
     
     predicted_map = assemble_cubes(predicted_cubes, cubecenters, emmap_preprocessed.shape[0],EMMERNET_CUBE_SIZE)
     if verbose:
         print("\tPredicted map assembled")
         print("\tPredicted map shape: {}".format(predicted_map.shape))
         print("3) Post-processing commencing...")
     
     
     ## Postprocess
 
-    predicted_map_postprocessed = postprocess_map(predicted_map, apix)
+    predicted_map_postprocessed = postprocess_map(predicted_map, apix, output_shape=input_map_shape)
     if verbose:
         print("\tPost-processing complete")
         print("\tPost-processed map shape: {}".format(predicted_map_postprocessed.shape))
 
     #return predicted_map_postprocessed
 
     emmernet_output_dictionary = {"output":predicted_map_postprocessed}
@@ -116,14 +142,18 @@
     emmernet_folder_path = emmernet_model_folder
     if emmernet_type == "model_based":
         emmernet_model_path = os.path.join(emmernet_folder_path, "EMmerNet_MBfa.hdf5")
     elif emmernet_type == "model_free":
         emmernet_model_path = os.path.join(emmernet_folder_path, "EMmerNet_MFfa.hdf5")
     elif emmernet_type == "ensemble":
         emmernet_model_path = os.path.join(emmernet_folder_path, "EMmerNet_MBMF.hdf5")
+    elif emmernet_type == "hybrid":
+        emmernet_model_path = os.path.join(emmernet_folder_path, "epsilon_hybrid_model_4_final_epoch_15.hdf5")
+    elif emmernet_type == "model_based_no_freqaug":
+        emmernet_model_path = os.path.join(emmernet_folder_path, "EMmerNet_MB.hdf5")
     else:
         raise ValueError("Invalid emmernet_type")
     
     emmernet_model = load_model(emmernet_model_path)
     
     return emmernet_model
 
@@ -168,19 +198,18 @@
     emmap_resampled = resample_map(emmap, apix=apix,apix_new=1)
 
     ## standardize the map
     emmap_standardized = standardize_map(emmap_resampled)
 
     return emmap_standardized
 
-def postprocess_map(predicted_map, apix):
+def postprocess_map(predicted_map, apix, output_shape):
     ## Resample the map to the original pixel size
-    predicted_map_resampled = resample_map(predicted_map, apix=1,apix_new=apix)
+    predicted_map_resampled = resample_map(predicted_map, apix=1,apix_new=apix, assert_shape=output_shape)
 
     ## MinMax normalize the map
     predicted_map_normalized = minmax_normalize_map(predicted_map_resampled)
 
     return predicted_map_normalized
 
 
 
-
```

### Comparing `locscale-2.1.2/locscale/include/__init__.py` & `locscale-2.1.4b0/locscale/include/emmer/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/confidenceMapUtil/FDRutil.py` & `locscale-2.1.4b0/locscale/include/confidenceMapUtil/FDRutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import numpy as np
 import subprocess
 import math
 import gc
 import os
 import sys
 
-
-#Author: Maximilian Beckers, EMBL Heidelberg, Sachse Group
-
 #-------------------------------------------------------------------------------------
 def estimateNoiseFromMap(map, windowSize, boxCoord):
 
 	#**************************************************
 	#****** function to estimate var an mean from *****
 	#**** nonoverlapping boxes outside the particle ***
 	#**************************************************
```

### Comparing `locscale-2.1.2/locscale/include/confidenceMapUtil/confidenceMapMain.py` & `locscale-2.1.4b0/locscale/include/confidenceMapUtil/confidenceMapMain.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,21 +69,21 @@
 	circularMaskData = mapUtil.makeCircularMask(np.copy(em_map), sphere_radius);
 
 	# plot locations of noise estimation
 	if modelMap is None:
 		pp = mapUtil.makeDiagnosticPlot(em_map, wn, False, boxCoord);
 		print(
 			"Generating diagnostic plot of noise estimation. Please have a look in 'diag_image.pdf' that the molecule does not fall into the region used for background noise estimation.");
-		pp.savefig("diag_image.pdf");
+		pp.savefig("diag_image.png");
 		pp.close();
 	else:
 		pp = mapUtil.makeDiagnosticPlot(em_map, wn, True, boxCoord);
 		print(
 			"Generating diagnostic plot of noise estimation. Please have a look in 'diag_image.pdf' that the molecule does not fall into the region used for background noise estimation.");
-		pp.savefig("diag_image.pdf");
+		pp.savefig("diag_image.png");
 		pp.close();
 
 
 	# estimate noise statistics
 	if ((locResMap is None) & (modelMap is None)):  # if no local Resolution map is given,don't do any filtration
 
 		FDRutil.checkNormality(em_map, wn, boxCoord);
```

### Comparing `locscale-2.1.2/locscale/include/confidenceMapUtil/locscaleUtil.py` & `locscale-2.1.4b0/locscale/include/confidenceMapUtil/locscaleUtil.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/confidenceMapUtil/mapUtil.py` & `locscale-2.1.4b0/locscale/include/confidenceMapUtil/mapUtil.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/__init__.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/__init__.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/emdb_class.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/emdb_class.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/fft_util.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/fft_util.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/filter.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/filter.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/fsc_util.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/fsc_util.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/map_quality_tools.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/map_quality_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     mass = tvtk.MassProperties()
     configure_input(mass, iso)
     surface_area = mass.surface_area
     
     return surface_area
 
 def calculate_surface_area_at_threshold(emmap, apix, reference_threshold):
-    binarised_emmap = (emmap>=reference_threshold).astype(np.int_)
+    from locscale.include.emmer.ndimage.map_utils import binarise_map
+    binarised_emmap = binarise_map(emmap, reference_threshold, return_type='int', threshold_type="gteq")
     surface_area = mesh_surface_area(binarised_emmap, 0.9999999, apix)
     return surface_area
 
 
 def count_distinct_regions(emmap, reference_threshold):
     from skimage import measure
```

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/map_tools.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/map_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     com_pixels = np.array(center_of_mass(abs(emmap_data)))
     apix_array = np.array(convert_to_tuple(apix))
     
     com_real = com_pixels * apix_array
     
     return com_real
     
-def add_half_maps(halfmap_1_path, halfmap_2_path, output_filename):
+def add_half_maps(halfmap_1_path, halfmap_2_path, output_filename, fsc_filter=False):
     '''
     Function to add two half maps
 
     Parameters
     ----------
     halfmap_1_path : str
         
@@ -95,33 +95,77 @@
     halfmap1 = mrcfile.open(halfmap_1_path).data
     halfmap2 = mrcfile.open(halfmap_2_path).data
     
     if halfmap1.shape == halfmap2.shape:
        full_map = (halfmap1 + halfmap2)/2
        full_voxel_size = mrcfile.open(halfmap_1_path).voxel_size.tolist()
     
-       full_header = mrcfile.open(halfmap_1_path).header
-       #print(full_voxel_size)
+       if fsc_filter:
+           from locscale.include.emmer.ndimage.fsc_util import apply_fsc_filter
+           full_map = apply_fsc_filter(full_map, apix=full_voxel_size, halfmap_1 = halfmap1, halfmap_2 = halfmap2)[0]
+        
        save_as_mrc(map_data=full_map, output_filename=output_filename, apix=full_voxel_size, verbose=True) 
     
        return output_filename
     else:
       print("Half maps are not of equal dimension.")
 
     
-def estimate_global_bfactor_map(emmap, apix, wilson_cutoff, fsc_cutoff):
+def estimate_global_bfactor_map(emmap_path=None, emmap=None, apix=None, wilson_cutoff=None, fsc_cutoff=None, plot_profiles=False):
     from locscale.include.emmer.ndimage.profile_tools import number_of_segments, frequency_array, compute_radial_profile, estimate_bfactor_through_pwlf
-    
+    from locscale.include.emmer.ndimage.map_utils import load_map
+
+    if emmap_path is not None:
+        emmap, apix = load_map(emmap_path)
+    elif emmap is None or apix is None:
+        raise ValueError("Either emmap_path should be provided or emmap and apix should be provided")
+    assert wilson_cutoff is not None, "wilson_cutoff should be provided"
+    assert fsc_cutoff is not None, "fsc_cutoff should be provided"
+
     rp_unsharp = compute_radial_profile(emmap)
     freq = frequency_array(amplitudes=rp_unsharp, apix=apix)
     num_segments = number_of_segments(fsc_cutoff)
         
-    bfactor,_,(fit,z,slopes) = estimate_bfactor_through_pwlf(freq,rp_unsharp, wilson_cutoff=wilson_cutoff, fsc_cutoff=fsc_cutoff, num_segments=num_segments)
+    bfactor,_,(fit,z,slopes) = estimate_bfactor_through_pwlf(freq,rp_unsharp, \
+                wilson_cutoff=wilson_cutoff, fsc_cutoff=fsc_cutoff, \
+                num_segments=num_segments, standard_notation=True)
+    
+    if plot_profiles:
+        import matplotlib.pyplot as plt
+        plt.figure()
+        x_array = freq**2
+        y_array = np.log(rp_unsharp)
+        plt.plot(x_array, y_array, "b")
+        # draw a vertical line for each z
+        for z_value in z:
+            plt.axvline(x=z_value, color="k", linestyle="--")
+
     
     return bfactor, z, slopes, fit
+
+def estimate_global_bfactor_map_standard(emmap_path=None, emmap=None, apix=None, wilson_cutoff=None, fsc_cutoff=None, plot_profiles=False):
+    from locscale.include.emmer.ndimage.profile_tools import number_of_segments, frequency_array, compute_radial_profile, estimate_bfactor_standard
+    from locscale.include.emmer.ndimage.map_utils import load_map
+
+    if emmap_path is not None:
+        emmap, apix = load_map(emmap_path)
+    elif emmap is None or apix is None:
+        raise ValueError("Either emmap_path should be provided or emmap and apix should be provided")
+    assert wilson_cutoff is not None, "wilson_cutoff should be provided"
+    assert fsc_cutoff is not None, "fsc_cutoff should be provided"
+
+    rp_unsharp = compute_radial_profile(emmap)
+    freq = frequency_array(amplitudes=rp_unsharp, apix=apix)
+        
+    bfactor = estimate_bfactor_standard(freq,rp_unsharp, \
+                wilson_cutoff=wilson_cutoff, fsc_cutoff=fsc_cutoff, \
+                standard_notation=True)
+
+    
+    return bfactor
     
 def compute_scale_factors(em_profile, ref_profile):
     scale_factor = np.sqrt(ref_profile**2/em_profile**2)
     return scale_factor
 
 
 def compute_radial_profile_proper(vol, frequency_map):
@@ -208,15 +252,15 @@
     '''
     from locscale.include.emmer.ndimage.profile_tools import compute_radial_profile, frequency_array
     from locscale.include.emmer.ndimage.map_tools import set_radial_profile, compute_scale_factors
     
     emmap_profile, radii = compute_radial_profile(vol,return_indices=True)
     freq = frequency_array(amplitudes=emmap_profile, apix=apix)
     
-    sharpened_profile = emmap_profile * np.exp(-1*global_bfactor/4 * freq**2)
+    sharpened_profile = emmap_profile * np.exp(global_bfactor/4 * freq**2)
 
     scale_factors = compute_scale_factors(emmap_profile, sharpened_profile)
     sharpened_map = set_radial_profile(vol, scale_factors, radii)
     
     return sharpened_map
     
 def crop_map_between_residues(emmap_path, pdb_path, chain_name, residue_range=None, dilation_radius=3):
@@ -519,15 +563,15 @@
     
 
 def find_unmodelled_mask_region(fdr_mask_path, pdb_path, fdr_threshold=0.99, atomic_mask_threshold=0.5, averaging_window_size=3, fsc_resolution=None):
     """
     Finds the unmodelled regions in the input pdb file.
     """
     from locscale.include.emmer.ndimage.map_tools import get_atomic_model_mask
-    from locscale.include.emmer.ndimage.map_utils import load_map
+    from locscale.include.emmer.ndimage.map_utils import load_map, binarise_map
     from locscale.include.emmer.ndimage.map_utils import save_as_mrc
     import os
     from scipy.ndimage import uniform_filter
     import numpy as np
 
     fdr_mask, apix = load_map(fdr_mask_path)
     if fsc_resolution is None:
@@ -538,16 +582,16 @@
         
     atomic_mask = get_atomic_model_mask(emmap_path = fdr_mask_path, pdb_path = pdb_path, \
         dilation_radius = dilation_radius, save_files = False)
     
     # Binarise 
     # Binarise the atomic model mask and FDR confidence mask at X threshold 
     
-    atomic_model_mask_binarised = (atomic_mask >= atomic_mask_threshold).astype(np.int_)
-    fdr_mask_binarised = (fdr_mask >= fdr_threshold).astype(np.int_)
+    atomic_model_mask_binarised = binarise_map(atomic_mask, atomic_mask_threshold, return_type='int', threshold_type='gteq')
+    fdr_mask_binarised = binarise_map(fdr_mask, fdr_threshold, return_type='int', threshold_type='gteq')
 
     # Compute the difference 
     difference_mask = fdr_mask_binarised - atomic_model_mask_binarised
 
     # Remove negative values
     difference_mask[difference_mask < 0] = 0
```

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/map_utils.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/map_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -211,18 +211,46 @@
         3D numpy array of shape (size x size x size)
 
     '''
     z,y,x = center
     window = im[z-size//2:z+size//2, y-size//2:y+size//2, x-size//2:x+size//2]
     return window
 
-def binarizeMap(emmap, threshold):
-    binary_map = (emmap>=threshold).astype(np.int_)
+def binarize_map(emmap, threshold, return_type="int", threshold_type="gteq"):
+    '''
+    Function to binarize a map
+    '''
+    if threshold_type == "gteq":
+        binary_map = emmap >= threshold
+    elif threshold_type == "gt":
+        binary_map = emmap > threshold
+    elif threshold_type == "lteq":
+        binary_map = emmap <= threshold
+    elif threshold_type == "lt":
+        binary_map = emmap < threshold
+    else:
+        print("Please provide a valid threshold_type")
+        valid_threshold_types = ["gteq (>=)", "gt (>)", "lteq (<=)", "lt (<)"]
+        raise ValueError(f"Invalid threshold_type provided {threshold_type}. Valid threshold_types are {valid_threshold_types}")
+
+    if return_type == "int":
+        binary_map = binary_map.astype(np.int_)
+    elif return_type == "float":
+        binary_map = binary_map.astype(np.float_)
+    elif return_type == "bool":
+        binary_map = binary_map.astype(bool)
+    else:
+        print("Please provide a valid return_type")
+        valid_return_types = ["int", "float", "bool"]
+        raise ValueError(f"Invalid return_type provided {return_type}. Valid return_types are {valid_return_types}")
     return binary_map
 
+def binarise_map(*args, **kwargs):
+    return binarize_map(*args, **kwargs)
+
 def average_voxel_size(voxel_size_record):
     apix_x = voxel_size_record.x
     apix_y = voxel_size_record.y
     apix_z = voxel_size_record.z
     
     average_apix = (apix_x+apix_y+apix_z)/3
     
@@ -430,15 +458,15 @@
         voxelsize = apix
     elif mask_path is None or (mask is None and apix is None):
         print("Input error: Provide atleast mask path, or (mask and apix)")
         return None
     
     ang_to_cm = 1e-8
     
-    mask = (mask>=edge_threshold).astype(np.int_)
+    mask = binarise_map(mask, edge_threshold, return_type='int',threshold_type='gteq')
     
     mask_vol = mask.sum()*(voxelsize*ang_to_cm)**3
     mask_vol_A3 = mask.sum()*voxelsize**3
     #print("\n Volume of the mask generated is: "+str(mask.sum())+" A$^3$ \n")
     # Calculate number of atoms
     protein_mass = protein_density * mask_vol
     num_moles = protein_mass / average_atomic_weight
@@ -677,21 +705,21 @@
     gemmi_st_bfactor = set_atomic_bfactors(input_gemmi_st=gemmi_st, b_iso=bfactor)
     
     simmap = pdb2map(input_pdb=gemmi_st_bfactor, apix=apix, size=mask_shape, set_refmac_blur=True, verbose=True)
     
     simmap_array = simmap.flatten()
     nonzero_array = simmap_array[simmap_array>0]
     threshold = np.percentile(nonzero_array, threshold_factor)
-    binarised_map = (simmap>=threshold).astype(np.int_)
+    binarised_map = binarise_map(simmap, threshold, return_type='int', threshold_type='gteq')
     
     kernel = np.ones((smoothen,smoothen, smoothen))
     smoothened_map = fftconvolve(in1=binarised_map, in2=kernel, mode="same")
     smoothened_map = smoothened_map/smoothened_map.max()
     
-    binarised_map = (smoothened_map>=tight).astype(np.int_)
+    binarised_map = binarise_map(smoothened_map, tight, return_type='int', threshold_type='gteq')
     
     return binarised_map
     
 def check_oversharpening(emmap, apix, fsc_cutoff):
     '''
     Function to check whether a map has been oversharpened based on the slope of the radial profile
     '''
```

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/plotContourMap.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/plotContourMap.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/plots.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/plots.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,115 @@
 Created on Tue Apr 19 13:53:12 2022
 
 @author: alok
 """
 
 import numpy as np
 
+def pretty_plot_radial_profile(freq,list_of_profiles_native, plot_type="make_log", \
+                                legends=None,figsize_cm=(14,8), fontsize=10,linewidth=1, \
+                                marker="o", markersize=5,font="Helvetica",fontscale=1, showlegend=True, showPoints=False, \
+                                alpha=1, variation=None, yticks=None, ylims=None, xlims=None, crop_freq=None, labelsize=None, title=None):
+    import matplotlib.pyplot as plt
+    from matplotlib.pyplot import cm
+    from locscale.include.emmer.ndimage.profile_tools import crop_profile_between_frequency
+    import seaborn as sns
+    import matplotlib 
+    matplotlib.rcParams['pdf.fonttype'] = 42
+    matplotlib.rcParams['ps.fonttype'] = 42
+    # set the global font size for the plot
+
+        
+    plt.rcParams.update({'font.size': fontsize})
+    figsize = (figsize_cm[0]/2.54, figsize_cm[1]/2.54) # convert cm to inches
+    
+    fig, ax1 = plt.subplots(figsize=figsize, dpi=600)  # DPI is fixed to 600 for publication quality
+    sns.set_theme(context="paper", font=font, font_scale=fontscale)
+    # Set font size for all text in the figure
+    sns.set_style("white")
+
+    
+    
+    # Crop frequencies if required
+    if crop_freq is not None:
+        cropped_frequency = crop_profile_between_frequency(freq, list_of_profiles_native[0], crop_freq[0], crop_freq[1])[0]
+        cropped_profiles = [crop_profile_between_frequency(freq, profile, crop_freq[0], crop_freq[1])[1] for profile in list_of_profiles_native]
+    else:
+        cropped_frequency = freq
+        cropped_profiles = list_of_profiles_native
+    
+    final_list_of_profiles = []
+
+    for profile in cropped_profiles:
+        if plot_type=="make_log":
+            profile = np.log(profile)
+            plot_frequency_axis = cropped_frequency**2
+        elif plot_type=="squared_amp":
+            profile = np.log(profile**2)
+            plot_frequency_axis = cropped_frequency**2
+        elif plot_type=="normalise":
+            profile = profile/profile.max()
+            plot_frequency_axis = cropped_frequency
+        else:
+            plot_frequency_axis = cropped_frequency        
+    
+        final_list_of_profiles.append(profile)
+        
+    
+    # Add labels to the plot
+    xlabel_top = r'Resolution, $d (\AA)$'
+    if plot_type=="normalise":
+        xlabel = r'Spatial Frequency, $d^{-1} (\AA^{-1})$'
+        ylabel = r'Normalised $ \langle \mid F \mid \rangle $'
+    elif plot_type=="squared_amp":
+        xlabel = r'Spatial Frequency, $d^{-2} (\AA^{-2})$'
+        ylabel = r'$ln  \langle \mid F \mid ^{2} \rangle $ '
+    elif plot_type=="make_log":
+        xlabel = r'Spatial Frequency, $d^{-2} (\AA^{-2})$'
+        ylabel = r'$ln  \langle \mid F \mid \rangle $'
+    else:
+        xlabel = r'Spatial Frequency, $d^{-1} (\AA^{-1})$'
+        ylabel = r'$ \langle \mid F \mid \rangle $'
+    # Map the colors
+    
+    colors = cm.rainbow(np.linspace(0,1,len(final_list_of_profiles)))
+    
+    ax1.grid(False)
+    ax2 = ax1.twiny()
+
+    for i, profile in enumerate(final_list_of_profiles):
+        if showPoints:
+            ax1.plot(plot_frequency_axis, profile, marker=marker, markersize=markersize, color=colors[i], alpha=alpha, \
+                        linewidth=linewidth, label=legends[i])
+        else:
+            ax1.plot(plot_frequency_axis, profile, color=colors[i], alpha=alpha, linewidth=linewidth, label=legends[i])
+                
+    ax2.set_xticks(ax1.get_xticks())
+    ax2.set_xbound(ax1.get_xbound())
+    ax2.set_xticklabels([round(1/np.sqrt(x),1) for x in ax1.get_xticks()])
+    #ax2.tick_params(axis="both", which="both", labelsize=labelsize)
+
+    if showlegend:
+        ax1.legend(loc="best")
+    ax1.set_xlabel(xlabel)#, fontsize=fontsize)
+    ax1.set_ylabel(ylabel)#, fontsize=fontsize)
+    #ax1.tick_params(axis="both", which="both", labelsize=labelsize)
+    ax2.set_xlabel(xlabel_top)#, fontsize=fontsize)
+    
+    if ylims is not None:
+        plt.ylim(ylims)
+    if yticks is not None:
+        plt.yticks(yticks)
+    if xlims is not None:
+        plt.xlim(xlims)
+
+    if title is not None:
+        plt.title(title)
+    plt.tight_layout()
+    return fig
 
 def plot_radial_profile(freq,list_of_profiles, squared_amplitudes=False, legends=None, normalise=False, font=28,showlegend=True, showPoints=True, alpha=0.05, variation=None, yticks=None, logScale=True, ylims=None, xlims=None, crop_freq=None):
     import matplotlib.pyplot as plt
     from matplotlib.pyplot import cm
     from locscale.include.emmer.ndimage.profile_tools import crop_profile_between_frequency
     
     '''
```

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/power.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/power.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/profile_tools.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/profile_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -601,15 +601,15 @@
         end_index = np.where(freq>=end_freq)[0][0]
     
     crop_freq = freq[start_index:end_index]
     crop_amplitude = amplitude[start_index:end_index]
     
     return crop_freq, crop_amplitude
     
-def estimate_bfactor_through_pwlf(freq,amplitudes,wilson_cutoff,fsc_cutoff, return_all=True, num_segments=None):
+def estimate_bfactor_through_pwlf(freq,amplitudes,wilson_cutoff,fsc_cutoff, return_all=True, num_segments=None, standard_notation=True):
     '''
     Function to automatically find out linear region in a given radial profile 
 
 
     @Manual{pwlf,
             author = {Jekel, Charles F. and Venter,     Gerhard},
             title = {{pwlf:} A Python Library for Fitting 1D Continuous Piecewise Linear Functions},
@@ -634,15 +634,15 @@
     from locscale.include.emmer.ndimage.profile_tools import number_of_segments
     
     if num_segments is None:
             num_segments = number_of_segments(fsc_cutoff)
             
     if num_segments < 2:
         print("Number of segments = 1 using standard method of evaluating bfactor")
-        bfactor, amplitude_zero_freq = estimate_bfactor_standard(freq, amplitudes, wilson_cutoff, fsc_cutoff, return_amplitude=True)
+        bfactor, amplitude_zero_freq = estimate_bfactor_standard(freq, amplitudes, wilson_cutoff, fsc_cutoff, return_amplitude=True, standard_notation=standard_notation)
         piecewise_linfit = amplitude_zero_freq * np.exp(0.25 * bfactor * freq**2)
         z = [(1/wilson_cutoff)**2, (1/fsc_cutoff)**2]
         slopes = [bfactor / 4]
     
     else:
         
         start_freq = 1 / wilson_cutoff
@@ -664,14 +664,19 @@
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=RuntimeWarning)
             piecewise_linfit = pwlf.PiecewiseLinFit(x_data, y_data)
             z = piecewise_linfit.fit(n_segments=num_segments, disp=False)
             slopes = piecewise_linfit.calc_slopes()
         
         bfactor = slopes[-1] * 4
+
+        if standard_notation:
+            bfactor = -1 * bfactor
+        else:
+            bfactor = bfactor
         
         
         amplitude_zero_freq = piecewise_linfit.predict(0)
     
     if return_all:
         return bfactor, amplitude_zero_freq, (piecewise_linfit, z, slopes)
     else:
```

### Comparing `locscale-2.1.2/locscale/include/emmer/ndimage/simulate.py` & `locscale-2.1.4b0/locscale/include/emmer/ndimage/simulate.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/__init__.py` & `locscale-2.1.4b0/locscale/include/symmetry_emda/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/get_dssp.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/get_dssp.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/modify_pdb.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/modify_pdb.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/pdb_to_map.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_to_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jul 14 10:06:12 2021
 """
 
 import numpy as np
-import pypdb
 import gemmi
 from locscale.include.emmer.pdb.pdb_tools import get_unit_cell_estimate, set_to_center_of_unit_cell
 from locscale.include.emmer.pdb.pdb_utils import shift_coordinates
 from locscale.include.emmer.ndimage.filter import low_pass_filter
 from locscale.include.emmer.ndimage.map_utils import save_as_mrc
 
 def detect_pdb_input(input_pdb):
@@ -173,15 +172,15 @@
         dencalc.put_model_density_on_grid(model)
 
     emmap = np.array(dencalc.grid,copy=False)
     
     if set_refmac_blur:
         if verbose:
             print("Applying a unblur for the sampled density equal to: {:.2f}".format(-inv_d2))
-        emmap = sharpen_maps(emmap, apix=apix_gemmi[0], global_bfactor=-inv_d2)
+        emmap = sharpen_maps(emmap, apix=apix_gemmi[0], global_bfactor=inv_d2)
         
     
     if align_output:
         from scipy.ndimage import rotate
         emmap_flipped = np.flip(emmap,axis=2)
         emmap_rotated = rotate(emmap_flipped, angle=90, axes=(2,0))
         emmap = emmap_rotated
```

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/pdb_tools.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # but do not have so many distinct features that they warrent their own script.
 
 # global imports
 import mrcfile
 import gemmi
 import numpy as np
 import json
-import pypdb
 import os
 import sys
 from scipy import signal
 #from emmer.ndimage.filter import *
 from scipy.optimize import curve_fit
 from scipy.interpolate import interp1d
 
@@ -457,22 +456,22 @@
     from locscale.include.emmer.ndimage.map_utils import measure_mask_parameters, load_map, save_as_mrc
     from locscale.include.emmer.pdb.pdb_tools import combine_pdb_structures_into_one
     from locscale.include.emmer.ndimage.map_tools import find_unmodelled_mask_region
     import os
 
     mask, apix = load_map(mask_path)
     # Get the difference mask 
-    difference_mask = find_unmodelled_mask_region(fdr_mask_path = mask_path, pdb_path = pdb_path, fdr_threshold = 0.99, \
+    difference_mask = find_unmodelled_mask_region(fdr_mask_path = mask_path, pdb_path = pdb_path, fdr_threshold = mask_threshold, \
         atomic_mask_threshold = 0.5, averaging_window_size = averaging_window, fsc_resolution = fsc_resolution)
     
     difference_mask_path_filename = mask_path[:-4] + "_difference_mask.mrc"
     difference_mask_path = os.path.join(os.path.dirname(mask_path), difference_mask_path_filename)
     save_as_mrc(difference_mask, difference_mask_path, apix)
 
-    num_atoms, _ = measure_mask_parameters(mask_path = difference_mask_path, edge_threshold=0.5, verbose=False)
+    num_atoms, _ = measure_mask_parameters(mask_path = difference_mask_path, edge_threshold=mask_threshold, verbose=False)
     pdb_filename = os.path.basename(pdb_path)
     print("Adding {} pseudoatoms to {}".format(num_atoms, pdb_filename))
 
     partial_pseudo_model_path = run_pam(emmap_path = emmap_path, mask_path = difference_mask_path, threshold = mask_threshold, \
        num_atoms = num_atoms, method=pseudomodel_method, bl=bond_length, total_iterations = pseudomodel_iteration, verbose=False)
 
     combined_structure, final_chain_counts = combine_pdb_structures_into_one([pdb_path, partial_pseudo_model_path], return_chain_counts=return_chain_counts)
@@ -483,33 +482,94 @@
     if return_difference_mask:
         return_elements.append(difference_mask_path)
     
     if not return_chain_counts and not return_difference_mask:
         return combined_structure
     else:
         return tuple(return_elements)
+def get_coordinate_bfactors(st):
+    atom_info = []
+    for cra in st[0].all():
+        atom = cra.atom
+        atom_info.append((atom.pos, atom.b_iso))
+    
+    return atom_info
 
-        
+def check_if_atomic_position_in_mask(atomic_pos, mask, apix):
+    x, y, z = atomic_pos
+    int_x, int_y, int_z = int(round(x/apix)), int(round(y/apix)), int(round(z/apix))
+    return mask[int_z, int_y, int_x]
+
+
+def neighborhood_bfactor_correlation_sample(input_pdb, min_radius=1, max_radius=10, num_steps=10, sample_size=1000, mask_path=None, invert=False):
+    import gemmi
+    from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
+    from locscale.include.emmer.pdb.pdb_utils import get_coordinates, get_bfactors
+    from locscale.include.emmer.ndimage.map_utils import convert_pdb_to_mrc_position, load_map
+    from tqdm import tqdm
+    import random
+    from scipy.stats import pearsonr
+    st = detect_pdb_input(input_pdb)
+    atom_info = get_coordinate_bfactors(st)
+    if mask_path is not None:
+        mask, apix = load_map(mask_path)
+        mask = (mask > 0.5).astype(bool)   
+        if invert:
+            mask = np.logical_not(mask) 
+        atom_info_filtered = [atom for atom in atom_info if check_if_atomic_position_in_mask(atom[0], mask, apix)] 
+    else:
+        atom_info_filtered = atom_info
+
+    sample_atom_info = random.sample(atom_info_filtered, sample_size)
 
-def neighborhood_bfactor_correlation(input_pdb, min_radius=1, max_radius=10, num_steps=10):
+    bfactor_correlation_with_distance = {}
+    for r in tqdm(np.linspace(min_radius,max_radius,num_steps), total=num_steps, desc="Finding neighborhood bfactor correlation"):
+        sample_bfactors = []
+        sample_coordinates = []
+        ns_pseudo = gemmi.NeighborSearch(st[0], st.cell, r).populate()
+        neighborhood_bfactor_list = []
+        for sample_info in sample_atom_info:
+            sample_bfactors.append(sample_info[1])
+            sample_coordinates.append(sample_info[0].tolist())
+            gemmi_coord = sample_info[0]
+            neighbors = ns_pseudo.find_atoms(gemmi_coord, '\0', radius=r)
+            if len(neighbors) > 0:
+                neighborhood_bfactor_list.append(np.mean([n.to_cra(st[0]).atom.b_iso for n in neighbors]))
+                
+        bfactor_correlation_at_r = pearsonr(sample_bfactors, neighborhood_bfactor_list)
+        bfactor_correlation_with_distance[r] = [sample_bfactors, neighborhood_bfactor_list, bfactor_correlation_at_r, sample_coordinates]
+
+    return bfactor_correlation_with_distance
+
+def neighborhood_bfactor_correlation(input_pdb, min_radius=1, max_radius=10, num_steps=10, mask_path=None, invert=False):
     import gemmi
     from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
+    from locscale.include.emmer.ndimage.map_utils import convert_pdb_to_mrc_position, load_map
     from tqdm import tqdm
     from scipy.stats import pearsonr
     st = detect_pdb_input(input_pdb)
     model = st[0]
+    if mask_path is not None:
+        mask, apix = load_map(mask_path)
+        mask = (mask > 0.5).astype(bool)
+        if invert:
+            mask = np.logical_not(mask)
+
 
     bfactor_correlation_with_distance = {}
     for r in tqdm(np.linspace(min_radius,max_radius,num_steps), total=num_steps, desc="Finding neighborhood bfactor correlation"):
         ns_pseudo = gemmi.NeighborSearch(st[0], st.cell, r).populate()
         individual_bfactor_list = []
         neighborhood_bfactor_list = []
         atomic_position_list = []
         for cra in model.all():
             atom = cra.atom
+            if mask_path is not None:
+                if not check_if_atomic_position_in_mask(atom.pos, mask, apix):
+                    continue
             atomic_biso = atom.b_iso
             neighbors = ns_pseudo.find_atoms(atom.pos, '\0', radius=r)
             neigbor_atoms = [x.to_cra(model).atom for x in neighbors]
             atomic_bfactor_list = np.array([x.b_iso for x in neigbor_atoms])
             average_bfactor_neighbors = atomic_bfactor_list.mean()
             individual_bfactor_list.append(atomic_biso)
             neighborhood_bfactor_list.append(average_bfactor_neighbors)
```

### Comparing `locscale-2.1.2/locscale/include/emmer/pdb/pdb_utils.py` & `locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -286,20 +286,20 @@
     
     if return_array:
         return atomic_distance
     else:
         return np.mean(atomic_distance)
 
 def check_mrc_indexing(input_mask, threshold=0.9):
-    from locscale.include.emmer.ndimage.map_utils import parse_input
+    from locscale.include.emmer.ndimage.map_utils import parse_input, binarise_map
     from locscale.include.emmer.ndimage.map_utils import get_all_voxels_inside_mask
 
     mask_data = parse_input(input_mask)
     
-    binary_mask = (mask_data>=threshold).astype(np.int_)
+    binary_mask = binarise_map(mask_data, threshold, return_type='int', threshold_type='gteq')
     
     zero_data = np.zeros(mask_data.shape)
     voxels_inside_mask = set([tuple(x) for x in get_all_voxels_inside_mask(mask_input=mask_data, mask_threshold=threshold)])  ## ZYX format
     
     for voxel in voxels_inside_mask:
         zero_data[voxel[0],voxel[1],voxel[2]] = 1
     
@@ -339,19 +339,28 @@
         if d > apix:
             raise UserWarning("Problem with converting mrc to pdb positions! Getting maximum distance: {} when apix was {}".format(round(d,2), round(apix,2)))
     
     
     print("================== OK =========================")
     
 def get_atomic_point_map(mrc_positions, mask_shape):
-    zero_map = np.zeros(mask_shape)
-    for mrc in mrc_positions:
-        zero_map[mrc[0],mrc[1],mrc[2]] = 1
+    # mrc_positions is a list of positions in mrc format
+    # mask_shape is the shape of the mask
+    # returns a map of the atomic positions in the mask equal to 1
+    mrc_positions = np.array(mrc_positions)
+    atomic_point_map = np.zeros(mask_shape)
+    atomic_point_map[mrc_positions[:,0], mrc_positions[:,1], mrc_positions[:,2]] = 1
+    return atomic_point_map
+
+
+    # zero_map = np.zeros(mask_shape)
+    # for mrc in mrc_positions:
+    #     zero_map[mrc[0],mrc[1],mrc[2]] = 1
     
-    return zero_map
+    # return zero_map
 
 def pick_random_point_within_sphere_of_influence(center_atom, binarised_mask_full, radius_of_influence, apix):
     from locscale.include.emmer.ndimage.map_utils import convert_pdb_to_mrc_position, convert_mrc_to_pdb_position, dilate_mask
     import random
     
     mrc_position = convert_pdb_to_mrc_position([center_atom], apix)[0]
     single_atomic_point_map = get_atomic_point_map([mrc_position], binarised_mask_full.shape)
@@ -396,15 +405,15 @@
     
     
     
     
     
 def shake_pdb_within_mask(pdb_path, mask_path, rmsd_magnitude, use_pdb_mask=True, masking="strict", threshold=0.5):
     from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
-    from locscale.include.emmer.ndimage.map_utils import parse_input
+    from locscale.include.emmer.ndimage.map_utils import parse_input, binarise_map
     from locscale.include.emmer.pdb.pdb_tools import get_all_atomic_positions, set_all_atomic_positions
     from locscale.include.emmer.ndimage.map_utils import convert_pdb_to_mrc_position, get_all_voxels_inside_mask, convert_mrc_to_pdb_position
     from locscale.include.emmer.ndimage.map_tools import get_atomic_model_mask
     from tqdm import tqdm
     import mrcfile
     import random
     
@@ -413,15 +422,15 @@
     
     # If required, use PDB mask with the same shape and apix as a supplied mask_path
     if use_pdb_mask:
         mask = parse_input(get_atomic_model_mask(emmap_path=mask_path, pdb_path=pdb_path, dilation_radius=3))
     else:
         mask = parse_input(mask_path)
     
-    outside_mask = np.logical_not(mask>=threshold)
+    outside_mask = np.logical_not(binarise_map(mask, threshold=threshold))
     apix = mrcfile.open(mask_path).voxel_size.tolist()[0]
     
     
     voxel_positions_mask = get_all_voxels_inside_mask(mask, mask_threshold=0.5)
     pdb_positions_mask = convert_mrc_to_pdb_position(voxel_positions_mask, apix)
     
        
@@ -438,17 +447,17 @@
     # Get shaken positions in both real units (XYZ) and MRC units (ZYX)
     print("Checking for atoms outside the mask...")
     shaken_atomic_position_native = list(atomic_positions_values + convert_polar_to_cartesian(shake_vectors_polar, multiple=True))
     rmsd_native = compute_rmsd_two_pdb(shaken_atomic_position_native, atomic_positions_values, use_gemmi_structure=False)
     
     shaken_atomic_position= shaken_atomic_position_native.copy()
     
-    shaken_mrc_position_list = [tuple(x) for x in convert_pdb_to_mrc_position(shaken_atomic_position, apix)]  ## ZYX
+    shaken_mrc_position_list = convert_pdb_to_mrc_position(shaken_atomic_position, apix)  ## ZYX
     
-    binarised_mask = (mask>=threshold).astype(np.int_)
+    binarised_mask = binarise_map(mask, threshold=threshold)
     mrc_point_map = get_atomic_point_map(shaken_mrc_position_list, binarised_mask.shape)
     available_voxels = get_all_voxels_inside_mask(binarised_mask - mrc_point_map, 1)  
        
     
     random_sample_mrc = random.sample(available_voxels, len(shaken_mrc_position_list))
     random_sample_pdb = convert_mrc_to_pdb_position(random_sample_mrc, apix)
     
@@ -503,23 +512,23 @@
     print("RMSD between input structure and native shaken structure: {} A".format(round(rmsd_native,2)))
     print("RMSD between the input and output structure is: {} A".format(round(rmsd,2)))
     
     return shaken_structure
 
 def test_pdb_within_mask(input_pdb, mask_path, mask_threshold):
     from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
-    from locscale.include.emmer.ndimage.map_utils import convert_pdb_to_mrc_position, get_all_voxels_inside_mask, convert_mrc_to_pdb_position
+    from locscale.include.emmer.ndimage.map_utils import convert_pdb_to_mrc_position, get_all_voxels_inside_mask, convert_mrc_to_pdb_position, binarise_map
     from locscale.include.emmer.pdb.pdb_tools import get_all_atomic_positions
     import mrcfile
 
     st = detect_pdb_input(input_pdb)
     mask_data = mrcfile.open(mask_path).data
     apix = mrcfile.open(mask_path).voxel_size.tolist()[0]
         
-    binarised_mask = (mask_data>=mask_threshold).astype(np.int_)
+    binarised_mask = binarise_map(mask_data, mask_threshold)
     
     pdb_positions = get_all_atomic_positions(st)
     mrc_positions = convert_pdb_to_mrc_position(pdb_positions, apix)
     
     count = 0
     for mrc in mrc_positions:
         count += binarised_mask[mrc[0],mrc[1],mrc[2]]
@@ -570,20 +579,21 @@
                         
                     new_pos = current_pos + shake_vector_cartesian
                         
                     atom.pos = gemmi.Position(new_pos[0], new_pos[1], new_pos[2])
     
     return input_gemmi_st
 
-def get_bfactors(in_model_path, return_as_list=True):
+def get_bfactors(input_pdb, return_as_list=True):
     """
     Get B-factors of atoms
     """
+    from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
     dict_chain = {}
-    structure = gemmi.read_structure(in_model_path)
+    structure = detect_pdb_input(input_pdb)
     list_bfact = []
     for model in structure:
         for chain in model:
             polymer = chain.get_polymer()
             #skip non polymers
             #if not polymer: continue
             if not chain.name in dict_chain:
@@ -598,16 +608,15 @@
         break # ignore other models
     
     if return_as_list:
         return list_bfact
     else:
         return dict_chain
 
-def add_atomic_bfactors(in_model_path=None, input_gemmi_st=None,
-                        additional_biso=None, out_file_path=None):
+def add_atomic_bfactors(input_pdb, additional_biso=None, minimum_biso=0.5, out_file_path=None):
     '''
     Function to modify atomic bfactors uniformly by adding or subtracting b factors to each atom present in the PDB.
     
 
     Parameters
     ----------
     in_model_path : str, optional
@@ -618,46 +627,65 @@
         Parameter to specify how the bfactors of the atomic model be modified
 
     Returns
     -------
     If in_model_path is passed, returns the output model path.. Else returns the gemmi.Structure()
 
     '''
-    
-    if in_model_path is not None:
-        gemmi_st = gemmi.read_pdb(in_model_path)
-    elif input_gemmi_st is not None:
-        gemmi_st = input_gemmi_st.clone()
-    else:
-        print("Pass either the PDB path or the gemmi structure! \n")
-        return 0
-    
+    from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
+    gemmi_st = detect_pdb_input(input_pdb)
+        
     if additional_biso is not None:
         add_b_iso = additional_biso
     else:
         print("Enter the b factor to add")
         return 0
     
     for model in gemmi_st:
         for chain in model:
             for res in chain:
                 for atom in res:
-                    atom.b_iso += add_b_iso
-    
-    if in_model_path is not None:
-        if out_file_path is not None:
-            output_filepath = out_file_path
-        else:
-            output_filepath = in_model_path[:-4]+'_modified_bfactor.pdb'
-    
-        gemmi_st.write_pdb(output_filepath)
+                    original_biso = atom.b_iso
+                    new_biso = original_biso + add_b_iso
+                    if new_biso < minimum_biso:
+                        new_biso = minimum_biso
+                    atom.b_iso = new_biso
+    
+   
+    return gemmi_st
+
+def get_lower_bound_threshold(bfactor_array, probability_threshold=0.01):
+    # Using a Gaussian Kernel Density Estimation to get the lower bound threshold for the B-factors
+    from scipy.stats import invgamma
+    
+    bfactor_array = np.array(bfactor_array)
+    # fit a invgamma distribution to the data
+    param = invgamma.fit(bfactor_array)
+    # calculate the lower bound threshold
+    lower_bound_threshold = invgamma.ppf(probability_threshold, *param)
     
+    return lower_bound_threshold
+
+def shift_bfactors_by_probability(input_pdb, probability_threshold=0.01, minimum_bfactor=0.5, return_shift_values=True):
+    from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
+
+    bfactor_array = get_bfactors(input_pdb=input_pdb)
+    lower_bound_threshold = get_lower_bound_threshold(bfactor_array, probability_threshold=probability_threshold)
+    if lower_bound_threshold < minimum_bfactor:
+        print(f"Lower bound threshold {lower_bound_threshold} is less than the minimum bfactor. Setting lower bound threshold to {minimum_bfactor}")
+        lower_bound_threshold = minimum_bfactor
+        print(f"Lower bound threshold is now {lower_bound_threshold}")
+        
+    shifted_pdb = add_atomic_bfactors(input_pdb=input_pdb, additional_biso=-1*lower_bound_threshold, minimum_biso=minimum_bfactor)
+
+    if return_shift_values:
+        return shifted_pdb, lower_bound_threshold
     else:
-        return gemmi_st
-    
+        return shifted_pdb
+
 def set_atomic_bfactors(in_model_path=None, input_gemmi_st=None,
                         b_iso=None, out_file_path=None):
     '''
     Function to modify atomic bfactors uniformly by adding or subtracting b factors to each atom present in the PDB.
     
 
     Parameters
@@ -775,17 +803,18 @@
                             break #first atom
                 if len(residue_centre) > 0:
                     dict_coord[model.name][str(chain.name)][str(residue.seqid.num)] = \
                                             [residue_centre, residue.name]
 
     return dict_coord
 
-def get_coordinates(in_model_path):
+def get_coordinates(input_pdb):
+    from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
     list_coord = []
-    structure = gemmi.read_structure(in_model_path)
+    structure = detect_pdb_input(input_pdb)
     for model in structure:
         for chain in model:
             polymer = chain.get_polymer()
             #skip non polymers
             if not polymer: continue
             for residue in chain:
                 residue_id = str(residue.seqid.num)+'_'+residue.name
```

### Comparing `locscale-2.1.2/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py` & `locscale-2.1.4b0/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/symmetry_emda/__init__.py` & `locscale-2.1.4b0/locscale/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/symmetry_emda/apply_rotation_matrix.py` & `locscale-2.1.4b0/locscale/include/symmetry_emda/apply_rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/symmetry_emda/fcodes_fast.f90` & `locscale-2.1.4b0/locscale/include/symmetry_emda/fcodes_fast.f90`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/include/symmetry_emda/symmetrize_map.py` & `locscale-2.1.4b0/locscale/include/symmetry_emda/symmetrize_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     _, _, ops = operators_from_symbol(pg)
     #uc, arr, orig = em.get_data(imap)
     unitcell = np.array([emmap.shape[0]*apix, emmap.shape[1]*apix, emmap.shape[2]*apix, 90, 90, 90])
     #arr2 = double_the_axes(emmap)
     #print("Double the axes: {}".format(arr2.shape))
     f1 = fftshift(fftn(fftshift(emmap)))
     nbin, res_arr, bin_idx = get_resolution_array(unitcell, f1)
-    frs_sum = f1
+    frs_sum = np.zeros(f1.shape, f1.dtype)
     i=0
     for op in ops:
         frs = apply_op(f1, op,bin_idx,nbin)
         i+=1
         frs_sum += frs
     avg_f = frs_sum / len(ops)
     avgmap = ifftshift(np.real(ifftn(ifftshift(avg_f))))
```

### Comparing `locscale-2.1.2/locscale/preprocessing/__init__.py` & `locscale-2.1.4b0/locscale/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/preprocessing/headers.py` & `locscale-2.1.4b0/locscale/preprocessing/headers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,115 +7,92 @@
 """
 
 import numpy as np
 from locscale.utils.plot_tools import tab_print
 
 tabbed_print = tab_print(2)
 tprint = tabbed_print.tprint
-def prepare_sharpen_map(emmap_path,wilson_cutoff,fsc_resolution,add_blur=20,return_processed_files=False, output_file_path=None,verbose=True,Cref=None):
+def prepare_sharpen_map(emmap_path,wilson_cutoff,fsc_resolution,target_bfactor=20, output_file_path=None,verbose=True,Cref=None, apply_filter=True):
     '''
     Function to prepare target map for refinement 
 
     Parameters
     ----------
     emmap_path : str
         Path to the EM map which needs sharpening. Example: 'path/to/map.mrc'
     wilson_cutoff : float
         Wilson cutoff for determining the B factor of the EM map
     fsc_resolution : float
         Resolution at which FSC curve is computed used to compute B factor
-    add_blur : float, optional
+    target_bfactor : float, optional
         Additional blur to be added to the EM map. The default is 20   
     
     Returns
     -------
     sharpen_map_path : str
         Path to the sharpened EM map. Example: 'path/to/sharpen_map.mrc'
 
 
     '''
 
     from locscale.include.emmer.ndimage.profile_tools import compute_radial_profile, estimate_bfactor_through_pwlf, frequency_array
     from locscale.include.emmer.ndimage.map_utils import average_voxel_size, save_as_mrc, check_oversharpening
-    from locscale.include.emmer.ndimage.map_tools import sharpen_maps, estimate_global_bfactor_map
+    from locscale.include.emmer.ndimage.map_tools import sharpen_maps, estimate_global_bfactor_map_standard
     from locscale.include.emmer.ndimage.filter import apply_filter_to_map, low_pass_filter
     from locscale.include.emmer.ndimage.fsc_util import apply_fsc_filter
     import mrcfile
     import warnings
 
     emmap_mrc = mrcfile.open(emmap_path)
     emmap_unsharpened = emmap_mrc.data
     apix=average_voxel_size(emmap_mrc.voxel_size)
     
     if verbose:
         tprint("Estimating global B-factor using breakpoints\n")
     
     ### Estimate global B-factor ### 
     
-    bfactor, z, slopes, fit = estimate_global_bfactor_map(emmap=emmap_unsharpened, apix=apix,
+    bfactor = estimate_global_bfactor_map_standard(emmap=emmap_unsharpened, apix=apix,
                                     wilson_cutoff=wilson_cutoff, fsc_cutoff=fsc_resolution)
     
     if verbose:
-        tprint("Global bfactor: {:.3f}\n".format(-1*bfactor))
-        tprint("Breakpoints: {}".format(1/np.sqrt(z)))
-        tprint("Slopes: {}".format(slopes))
+        tprint("Global bfactor: {:.3f}\n".format(bfactor))
     
     if verbose:
         tprint("Calculating final b-factor of target map")
-    if add_blur != 0:
-        bfactor  += add_blur  ## Use add_blur if you wanna add blur to the emmap before refining
+    if target_bfactor != 0:
+        sharpening_bfactor = bfactor - target_bfactor
+    else:
+        sharpening_bfactor = bfactor
     if verbose:
-        tprint("Final overall bfactor of emmap expected to be {:.2f}".format(add_blur))
+        tprint("Final overall bfactor of emmap expected to be {:.2f}".format(target_bfactor))
+        tprint("Using bfactor of {:.2f} for sharpening".format(sharpening_bfactor))
+        tprint("If this number is negative then the map will be blurred to achieve the target bfactor\n Else it will be sharpened")
+
     
 
     ### Globally sharpen EM Map ###
-    sharpened_map = sharpen_maps(emmap_unsharpened, apix=apix, global_bfactor=bfactor)
+    sharpened_map = sharpen_maps(emmap_unsharpened, apix=apix, global_bfactor=sharpening_bfactor)
        
-    bfactor_final, z_final, slopes_final, fit_final = estimate_global_bfactor_map(emmap=sharpened_map, apix=apix, 
-                                                    wilson_cutoff=wilson_cutoff, fsc_cutoff=fsc_resolution)
+    bfactor_final = estimate_global_bfactor_map_standard(emmap=sharpened_map, apix=apix, 
+                                    wilson_cutoff=wilson_cutoff, fsc_cutoff=fsc_resolution)
     
     if verbose:
-        tprint("Final overall bfactor of emmap computed to be {:.2f}".format(-1*bfactor_final))
-        tprint("Breakpoints: {}".format(1/np.sqrt(z_final)))
-        tprint("Slopes: {}".format(slopes_final))
-        
-    
-    output_filename = emmap_path[:-4] +"_global_sharpened.mrc"
-    output_filename_filtered_map = emmap_path[:-4] +"_global_sharpened_filtered.mrc"
-    
-    save_as_mrc(map_data=sharpened_map, output_filename=output_filename, apix=apix)
-    if Cref is not None:
-        tprint("Applying Cref filter to final sharpened map")
-        fsc_filtered_map, _ = apply_fsc_filter(sharpened_map, apix=apix, Cref=Cref)
-        oversharpening_check = check_oversharpening(fsc_filtered_map, apix=apix, fsc_cutoff=fsc_resolution)
-        if oversharpening_check:
-            print("WARNING: Oversharpening detected in the target map for refinement. Please check the FSC curve")
-            output_filename_fsc_filtered = emmap_path[:-4] +"_global_sharpened_Cref_filtered_temp.mrc"
-            save_as_mrc(map_data=fsc_filtered_map, output_filename=output_filename_fsc_filtered, apix=apix)
-            
-            # Low pass filter the FSC filtered map at the resolution of the map
-            print("Low pass filtering the map at FSC resolution {}".format(fsc_resolution))
-            fsc_filtered_low_pass_filtered = low_pass_filter(fsc_filtered_map, cutoff=fsc_resolution, apix=apix)
-            save_as_mrc(map_data=fsc_filtered_low_pass_filtered, output_filename=output_filename_filtered_map, apix=apix)
-
-        else:
-            print("No oversharpening detected in the target map for refinement")
-            save_as_mrc(map_data=fsc_filtered_map, output_filename=output_filename_filtered_map, apix=apix)
+        tprint("Final overall bfactor of emmap computed to be {:.2f}".format(bfactor_final))
+           
+    if output_file_path is None:
+        sharpened_map_path = emmap_path[:-4] +"_global_sharpened.mrc"
     else:
-        tprint("Applying filter at FSC resolution to final sharpened map")
-        apply_filter_to_map(output_filename, dmin=fsc_resolution, output_filename=output_filename_filtered_map)
+        sharpened_map_path = output_file_path
     
-    if return_processed_files:
-        if verbose:
-            tprint("Returning: sharpend_map_path (filtered at FSC), [rp_unsharp, rp_sharp, bfactor]")
-        return output_filename_filtered_map, fit
-    else:                    
-        return output_filename_filtered_map
+    save_as_mrc(map_data=sharpened_map, output_filename=sharpened_map_path, apix=apix)
+
+    return sharpened_map_path
 
-def run_FDR(emmap_path,window_size,fdr=0.01,verbose=True,filter_cutoff=None):
+def run_FDR(emmap_path,window_size,fdr=0.01,verbose=True,filter_cutoff=None, averaging_filter_size=3):
     '''
     Function to calculate FDR mask for a map
 
     Parameters
     ----------
     emmap_path : string
         Path to the EM Map which needs thresholding. Example: 'path/to/map.mrc'
@@ -131,25 +108,27 @@
     mask_path : string
         path to mask file. Example: 'path/to/mask.mrc'
 
     '''
     import os, sys
     from subprocess import run, PIPE
     import mrcfile
+    from scipy.ndimage import uniform_filter
     # Preprocessing EM Map Path
     
     # Apply filter if filter_cutoff is not None
 
     if verbose:
         tprint("Now starting FDR procedure using the following parameters: \n"
                  "Window size: "+str(window_size)+"\n"
                  "Filter cutoff: "+str(filter_cutoff))
     
         
-    from locscale.include.emmer.ndimage.map_utils import average_voxel_size, compute_FDR_confidenceMap_easy, save_as_mrc
+    from locscale.include.emmer.ndimage.map_utils import average_voxel_size, compute_FDR_confidenceMap_easy, save_as_mrc, binarise_map
+    from locscale.include.emmer.ndimage.filter import get_cosine_mask
     
     current_directory = os.getcwd()
 
     processing_folder = os.path.dirname(emmap_path)
     os.chdir(processing_folder)    
 
     emmap = mrcfile.open(emmap_path).data
@@ -159,25 +138,35 @@
     fdr_mask, fdr_threshold = compute_FDR_confidenceMap_easy(
         emmap, apix=apix, fdr=fdr, window_size=window_size, 
         lowPassFilter_resolution=filter_cutoff, remove_temp_files=False)
     
     
     emmap_path_without_ext = emmap_path[:-4]
     mask_path = emmap_path_without_ext + "_confidenceMap.mrc"
-    
-    save_as_mrc(fdr_mask, output_filename=mask_path, 
-                apix=voxel_size_record.tolist(), origin=0)
+    mask_path_raw = emmap_path_without_ext + "_confidenceMap_raw.mrc"
+    # Apply averaging filter to the mask
+    save_as_mrc(fdr_mask, output_filename=mask_path.replace(".mrc","_raw.mrc"), apix=voxel_size_record.tolist(), origin=0)
+    if averaging_filter_size > 1:
+        tprint("Applying averaging filter of size {} to the mask".format(averaging_filter_size))
+        #fdr_mask = binarise_map(fdr_mask, threshold=0.99, return_type='int',threshold_type='gteq')
+        fdr_mask = uniform_filter(fdr_mask, averaging_filter_size)
+        #fdr_mask = binarise_map(fdr_mask, threshold=0.5, return_type='int',threshold_type='gteq')
+        #fdr_mask = get_cosine_mask(fdr_mask, 3)
+        
+
+        
+    save_as_mrc(fdr_mask, output_filename=mask_path, apix=voxel_size_record.tolist(), origin=0)
     
     os.chdir(current_directory)
-    if os.path.exists(mask_path):
+    if os.path.exists(mask_path) and os.path.exists(mask_path_raw) :
         if verbose:
             tprint("FDR Procedure completed. \n"+
                     "Mask path: "+mask_path+"\n")
         
-        return mask_path
+        return mask_path , mask_path_raw
     else:
         tprint("FDR process failed. Returning none")
         return None
          
 def run_pam(emmap_path,mask_path,threshold,num_atoms,method,bl,
             g=None,friction=None,scale_map=None,scale_lj=None,total_iterations=100,verbose=True):
     '''
@@ -322,15 +311,17 @@
                         num_waters += 1
     
     if num_waters == num_atoms:
         return True
     else:
         return False
     
-def run_servalcat_iterative(model_path, map_path, resolution, num_iter, pseudomodel_refinement, refmac5_path=None, verbose=True, hybrid_model_refinement=False, final_chain_counts=None):
+def run_servalcat_iterative(model_path, map_path, resolution, num_iter, pseudomodel_refinement, \
+                            refmac5_path=None, verbose=True, hybrid_model_refinement=False, \
+                            final_chain_counts=None, cif_info=None):
     import os
     from subprocess import run, PIPE, Popen
     from locscale.include.emmer.pdb.pdb_utils import get_bfactors, set_atomic_bfactors
     import mrcfile
 
     if hybrid_model_refinement: 
         assert final_chain_counts is not None, "Please provide the final chain counts for the hybrid model refinement"
@@ -338,15 +329,15 @@
     tprint(" Running iterative refinement of the model using One Cycle ServalCat")
     normal_refinement = not pseudomodel_refinement and not hybrid_model_refinement
     if normal_refinement:
         tprint("This is a refinement of a real atomic model")
         servalcat_refined_path = run_refmac_servalcat(
             model_path=model_path, map_path=map_path, resolution=resolution, \
             num_iter=num_iter, pseudomodel_refinement=pseudomodel_refinement, \
-            refmac5_path=refmac5_path, verbose=verbose)
+            refmac5_path=refmac5_path, verbose=verbose, cif_info=cif_info)
         
         return servalcat_refined_path
         
     else:
         tprint("This is a refinement of a pseudo-atomic model")
         tprint("Running iterative refinement of the model")
         for cycle in range(num_iter):
@@ -356,33 +347,39 @@
                 initialise_bfactors = True
             else:
                 assert os.path.exists(servalcat_refinement_next_cycle_path), "Servalcat refinement failed in the previous cycle "
                 model_path_input = servalcat_refinement_next_cycle_path
                 initialise_bfactors = False
             
             servalcat_refined_once_path = run_refmac_servalcat(
-                model_path_input, map_path, resolution, num_iter=1, pseudomodel_refinement=pseudomodel_refinement,
-                refmac5_path=refmac5_path, verbose=verbose, initialise_bfactors=initialise_bfactors, hybrid_model_refinement=hybrid_model_refinement)
+                model_path_input, map_path, resolution, num_iter=1, pseudomodel_refinement=pseudomodel_refinement,\
+                refmac5_path=refmac5_path, verbose=verbose, initialise_bfactors=initialise_bfactors, \
+                hybrid_model_refinement=hybrid_model_refinement, cif_info=cif_info)
             
             servalcat_refinement_next_cycle_path = os.path.join(
                 os.path.dirname(servalcat_refined_once_path), "servalcat_refinement_cycle_"+str(cycle+1)+".pdb")
             
             tprint("Averaging the bfactors with radius of 3 angstroms")
             window_averaged_bfactors_structure = average_atomic_bfactors_window(
                 input_pdb=servalcat_refined_once_path, window_radius=3, hybrid_model_refinement = hybrid_model_refinement, final_chain_counts=final_chain_counts)
             window_averaged_bfactors_structure.write_pdb(servalcat_refinement_next_cycle_path)
         
-        tprint("Setting the element composition of the model to match a typical protein composition")
-        tprint("Carbon: 63%, Nitrogen: 17%, Oxygen: 20%")
+        # tprint("Setting the element composition of the model to match a typical protein composition")
+        # tprint("Carbon: 63%, Nitrogen: 17%, Oxygen: 20%")
 
-        proper_element_composition_structure = set_average_composition(input_pdb=servalcat_refinement_next_cycle_path)
-        proper_element_composition_filename = model_path.replace(".pdb", "_proper_element_composition.pdb")
-        proper_element_composition_structure.write_pdb(proper_element_composition_filename)
+        # if hybrid_model_refinement:
+        #     starting_chain_count = final_chain_counts[0]
+        # else:
+        #     starting_chain_count = None
+            
+        # proper_element_composition_structure = set_average_composition(input_pdb=servalcat_refinement_next_cycle_path, starting_chain_count=starting_chain_count)
+        # proper_element_composition_filename = model_path.replace(".pdb", "_proper_element_composition.pdb")
+        # proper_element_composition_structure.write_pdb(proper_element_composition_filename)
         
-        return proper_element_composition_filename
+        return servalcat_refinement_next_cycle_path
         
 def set_average_composition(input_pdb, carbon_percentage=0.63, nitrogen_percentage=0.17, oxygen_percentage=0.2, starting_chain_count=None):
     '''
     Function to convert the oxygen atoms in the structure to carbon, nitrogen and oxygen atoms with probability: 
     Carbon: 0.63, Nitrogen: 0.17, Oxygen: 0.2
 
     Parameters
@@ -420,29 +417,30 @@
         # split chain_letters into two lists one for the first half indicating atomic model and the second half indicating the pseudo-model 
         chain_letters_atomic = chain_letters[:final_chain_count]
         chain_letters_pseudo = chain_letters[final_chain_count:]
         for chain in gemmi_st[0]:
             if chain.name in chain_letters_pseudo:
                 for res in chain:
                     for atom in res:
-                        atom = cra.atom
                         atom.element = np.random.choice([gemmi.Element("C"), gemmi.Element("O"), gemmi.Element("N")], p=[0.63, 0.2, 0.17])
         
         return gemmi_st
         
-def run_refmac_servalcat(model_path, map_path,resolution,  num_iter, pseudomodel_refinement, refmac5_path=None, verbose=True, initialise_bfactors=True, hybrid_model_refinement=False):
+def run_refmac_servalcat(model_path, map_path,resolution,  num_iter, pseudomodel_refinement, \
+                         refmac5_path=None, verbose=True, initialise_bfactors=True, \
+                         hybrid_model_refinement=False, cif_info=None):
     '''
     Function to run Refmac to refine the model and generate a new model with refined B-factors.
 
     Parameters
     ----------
     model_path : string
         Path of the model to be refined
-    map_path : string
-        Path of the map to be used for refinement
+    map_path : string or list of two strings
+        Path of the map to be used for refinement (or half maps if present)
     resolution : float
         Resolution of the map
     num_iter : int
         Number of iterations to run Refmac
     pseudomodel_refinement : bool
         If True, bfactor refinement is performed without any restraints
     refmac5_path : string
@@ -481,21 +479,30 @@
     else:
         servalcat_input = model_path
 
     
     ### Run Servalcat after preparing inputs ###
     output_prefix = model_name[:-4]+"_servalcat_refined"
     servalcat_command = ["servalcat","refine_spa","--model",servalcat_input,\
-        "--resolution",str(round(resolution, 2)), "--map", map_path, "--ncycle",str(int(num_iter)),\
+        "--resolution",str(round(resolution, 2)), "--ncycle",str(int(num_iter)),\
         "--output_prefix",output_prefix]
+
+    ## Add the map path to the command if there is only one map ##
+    if type(map_path) == str:
+        servalcat_command.extend(["--map",map_path])
+    else:
+        assert len(map_path) == 2, "The map_path should be a string or a list of two strings"
+        servalcat_command.extend(["--halfmaps",map_path[0],map_path[1]])
     
     servalcat_command += ["--jellybody","--jellybody_params","0.01","4.2"]
     servalcat_command += ["--hydrogen","no"]
     servalcat_command += ["--no_mask"]
     
+    if cif_info is not None:
+        servalcat_command += ["--ligand",cif_info]
     use_unrestrained_refinement = pseudomodel_refinement and not hybrid_model_refinement 
        
     if use_unrestrained_refinement:
         servalcat_command += ["--keywords","refi bonly","refi type unre"]
     else:
         servalcat_command += ["--keywords","refi bonly"]
 
@@ -508,15 +515,15 @@
     
     ## Create log file for servalcat
     servalcat_log_path = os.path.join(os.path.dirname(model_path),"servalcat_log.txt")
     servalcat_log_file = open(servalcat_log_path,"w")
     
     refmac_output = run(servalcat_command, stdout=servalcat_log_file)
     refined_model_path = output_prefix+".pdb"
-    bfactors = get_bfactors(in_model_path=refined_model_path)
+    bfactors = get_bfactors(refined_model_path)
 
     refined_model_path = os.path.join(processing_files_directory, os.path.basename(refined_model_path))
     
     # Change the active directory back to the original one
     os.chdir(current_directory)
     if verbose:
         tprint("Changing to directory: "+current_directory)
@@ -525,14 +532,76 @@
         if verbose: 
             tprint("The refined PDB model is: "+refined_model_path+"\n\n")    
         return refined_model_path
     else:
         tprint("Uhhoh, something wrong with the REFMAC procedure. Returning None")
         return None
 
+
+def run_profile_prediction_refinement(model_path, map_path,resolution,  num_iter, pseudomodel_refinement, refmac5_path=None, verbose=True, initialise_bfactors=True, hybrid_model_refinement=False):
+    '''
+    Function to run Refmac to refine the model and generate a new model with refined B-factors.
+
+    Parameters
+    ----------
+    model_path : string
+        Path of the model to be refined
+    map_path : string or list of two strings
+        Path of the map to be used for refinement (or half maps if present)
+    resolution : float
+        Resolution of the map
+    num_iter : int
+        Number of iterations to run Refmac
+    pseudomodel_refinement : bool
+        If True, bfactor refinement is performed without any restraints
+    refmac5_path : string
+        Path of the refmac5 executable. If None, the default path will be used.
+    verbose : bool
+        If True, the output of Refmac will be printed.
+    
+    Returns
+    -------
+    refined_model_path : string
+        Path of the refined model
+    
+    '''
+    
+    import os
+    from subprocess import run, PIPE, Popen
+    from locscale.include.emmer.pdb.pdb_utils import get_bfactors, set_atomic_bfactors, get_coordinates
+    from locscale.include.emmer.ndimage.profile_tools import estimate_bfactor_standard, frequency_array, compute_radial_profile
+    from locscale.include.emmer.ndimage.map_utils import convert_mrc_to_pdb_position, convert_pdb_to_mrc_position, extract_window, load_map
+    import gemmi
+    import mrcfile
+    
+    # Get the current working directory
+    current_directory = os.getcwd()
+    processing_files_directory = os.path.dirname(os.path.abspath(model_path))
+    os.chdir(processing_files_directory)
+    if verbose:
+        tprint("Changing to directory: "+processing_files_directory)
+
+    #### Input ####
+    st = gemmi.read_structure(model_path)
+    emmap, apix = load_map(map_path)
+    pdb_positions = get_coordinates(st)
+    
+    mrc_positions = convert_pdb_to_mrc_position(pdb_positions, apix=apix)
+    radial_profiles = []
+    for i, mrc_position in enumerate(mrc_positions):
+        center = mrc_position
+        window = extract_window(emmap, center, size=26)
+        rp_window = compute_radial_profile(window)
+        radial_profiles.append(rp_window)
+    
+    radial_profiles = np.array(radial_profiles)
+    # TBC
+
+    return None
+
 def average_atomic_bfactors_window(input_pdb, window_radius, hybrid_model_refinement=False, final_chain_counts=None):
     '''
     Function to average bfactors over a rolling window of a sphere
     '''
     from locscale.include.emmer.pdb.pdb_to_map import detect_pdb_input
     import gemmi
     import string
@@ -624,15 +693,15 @@
     ## Generate parameters of the simulated map
     apix = grid_input.spacing   
     unitcell = grid_input.unit_cell
     
     ## Simulate a reference map from the input atomic model in the pdb_structure variable
     
     refmap_data, grid_simulated = pdb2map(input_pdb=pdb_structure, unitcell=unitcell, size=emmap_data.shape,
-                                          return_grid=True, align_output=True, verbose=False, set_refmac_blur=True, blur=add_blur)
+                                          return_grid=True, align_output=True, verbose=verbose, set_refmac_blur=True, blur=add_blur)
     
 
     refmap_data_normalised = refmap_data
     
     
     ## Output filename
     reference_map_path = model_path[:-4]+"_4locscale.mrc"
```

### Comparing `locscale-2.1.2/locscale/preprocessing/pipeline.py` & `locscale-2.1.4b0/locscale/preprocessing/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,46 +10,51 @@
     -------
     pseudomodel_modmap : str
         path/to/modmap.mrc
 
     '''
     from locscale.preprocessing.headers import run_FDR, run_pam, run_refmac_servalcat, run_refmap, prepare_sharpen_map, is_pseudomodel, run_servalcat_iterative
     from locscale.include.emmer.ndimage.map_utils import measure_mask_parameters, average_voxel_size
+    from locscale.include.emmer.ndimage.map_tools import estimate_global_bfactor_map, estimate_global_bfactor_map_standard
     from locscale.include.emmer.pdb.pdb_tools import find_wilson_cutoff, add_pseudoatoms_to_input_pdb
-    from locscale.include.emmer.pdb.pdb_utils import get_bfactors
+    from locscale.include.emmer.pdb.pdb_utils import get_bfactors, add_atomic_bfactors, shift_bfactors_by_probability
     from locscale.utils.plot_tools import tab_print
     import mrcfile
+    from scipy.stats import norm
     import pickle
     import numpy as np
     import os
     
     ###########################################################################
     # Extract the inputs from the dictionary
     ###########################################################################
     tabbed_print = tab_print(2)
     
     emmap_path = modmap_args['emmap_path']
-    mask_path = modmap_args['mask_path']
+    halfmap_paths = modmap_args['halfmap_paths']
+    mask_path = modmap_args['mask_path_raw']
     pdb_path = modmap_args['pdb_path']
     pseudomodel_method = modmap_args['pseudomodel_method']
     pam_distance = modmap_args['pam_distance']
     pam_iteration = modmap_args['pam_iteration']
     fsc_resolution = modmap_args['fsc_resolution']
     refmac_iter = modmap_args['refmac_iter']
     add_blur = modmap_args['add_blur']
     skip_refine = modmap_args['skip_refine']
     refmac5_path = modmap_args['refmac5_path']
     pg_symmetry = modmap_args['pg_symmetry']
     model_resolution = modmap_args['model_resolution']
     molecular_weight = modmap_args['molecular_weight']
     build_ca_only = modmap_args['build_ca_only']
     verbose = modmap_args['verbose']
-    Cref = modmap_args['Cref']
+    #Cref = modmap_args['Cref']
     complete_model = modmap_args['complete_model']
     averaging_window = modmap_args['averaging_window']
+    mask_threshold = modmap_args['mask_threshold']
+    cif_info = modmap_args['cif_info']
 
     if verbose:
         print("."*80)
         print("Running model-map generation pipeline \n")
 
 
     if verbose:
@@ -76,15 +81,15 @@
     pam_iteration = pam_iteration
     resolution = fsc_resolution
     verbose = verbose
     ###########################################################################
     # Stage 1: Check the required number of atoms for the pseudomodel
     ###########################################################################
     if molecular_weight is None:
-        num_atoms,mask_dims = measure_mask_parameters(mask_path,verbose=False)
+        num_atoms,mask_dims = measure_mask_parameters(mask_path,verbose=False, edge_threshold=mask_threshold)
     else:
         avg_mass_per_atom = 13.14  #amu
         num_atoms = int(molecular_weight * 1000.0 / avg_mass_per_atom)
     ###########################################################################
     # Stage 1a: Check if the user requires to build only Ca atoms
     ###########################################################################
     if build_ca_only:
@@ -98,104 +103,137 @@
     # Stage 1b: If user has not provided a PDB path then build a 
     # pseudomodel using the run_pam() routine else use the PDB path directly
     ###########################################################################
     if pdb_path is None:
         if verbose:
             print("."*80)
             print("You have not entered a PDB path, running pseudo-atomic model generator!")
-        input_pdb_path = run_pam(emmap_path=emmap_path, mask_path=mask_path, threshold=1, num_atoms=num_atoms, 
+        input_pdb_path = run_pam(emmap_path=emmap_path, mask_path=mask_path, threshold=mask_threshold, num_atoms=num_atoms, 
                                    method=pam_method, bl=pam_bond_length,total_iterations=pam_iteration,verbose=verbose)
+        pseudomodel_refinement = True
         if input_pdb_path is None:
             print("Problem running pseudo-atomic model generator. Returning None")
             return None
         final_chain_counts = None
     else:
-        
+        pseudomodel_refinement = False
         if complete_model:
             if verbose:
                 print("."*80)
                 print("Adding pseudo-atoms to the regions of the mask that are not modelled by the user-provided PDB")
-            integrated_structure, final_chain_counts, difference_mask_path = add_pseudoatoms_to_input_pdb(pdb_path=pdb_path, mask_path=mask_path, emmap_path=emmap_path,\
-                averaging_window=averaging_window, pseudomodel_method=pam_method, pseudomodel_iteration=pam_iteration, mask_threshold=0.5, fsc_resolution=fsc_resolution, \
+            integrated_structure, final_chain_counts, difference_mask_path = add_pseudoatoms_to_input_pdb(
+                pdb_path=pdb_path, mask_path=mask_path, emmap_path=emmap_path,\
+                averaging_window=averaging_window, pseudomodel_method=pam_method, pseudomodel_iteration=pam_iteration, \
+                mask_threshold=mask_threshold, fsc_resolution=fsc_resolution, \
                 return_chain_counts=True, return_difference_mask=True) 
 
             input_pdb_path = pdb_path[:-4] + '_integrated_pseudoatoms.pdb'
             integrated_structure.write_pdb(input_pdb_path)
         else:
             final_chain_counts = None
             if verbose:
                 print("."*80)
                 print("Using user-provided PDB path: {}".format(pdb_path))    
             input_pdb_path = pdb_path
     ###########################################################################
     # Stage 2: Refine the reference model usign servalcat
     ###########################################################################
-    if is_pseudomodel(input_pdb_path):
-        pseudomodel_refinement = True
-    else:
-        pseudomodel_refinement = False
             
     wilson_cutoff = find_wilson_cutoff(mask_path=mask_path, return_as_frequency=False, verbose=False)
     
-    #############################################################################
-    # Stage 2a: Prepare the target map for refinement by globally sharpening
-    # the input map
-    #############################################################################
-    if verbose:
-        print("."*80)
-        print("Preparing target map for refinement\n")
-    globally_sharpened_map = prepare_sharpen_map(emmap_path,fsc_resolution=fsc_resolution,
-                                           wilson_cutoff=wilson_cutoff, add_blur=add_blur,
-                                           verbose=verbose,Cref=Cref)
+    # #############################################################################
+    # # Stage 2a: Prepare the target map for refinement by globally sharpening
+    # # the input map
+    # #############################################################################
+    # if verbose:
+    #     print("."*80)
+    #     print("Preparing target map for refinement\n")
+    # globally_sharpened_map = prepare_sharpen_map(emmap_path,fsc_resolution=fsc_resolution,
+    #                                        wilson_cutoff=wilson_cutoff, add_blur=add_blur,
+    #                                        verbose=verbose,Cref=Cref)
+    # 
+
+    # Using the original emmap for refinement 
     
     #############################################################################
     # Stage 2b: Run servalcat to refine the reference model (either 
     # using the input PDB or the pseudo-atomic model)
     #############################################################################
     if verbose:
         print("."*80)
         print("Running model refinement\n")
     if skip_refine:
         if verbose: 
             tabbed_print.tprint("Skipping model refinements based on user input\n")
         refined_model_path = input_pdb_path
     else:
-        refined_model_path = run_servalcat_iterative(model_path=input_pdb_path,  map_path=globally_sharpened_map,\
-                    pseudomodel_refinement=pseudomodel_refinement, resolution=resolution, num_iter=refmac_iter,
-                    refmac5_path=refmac5_path,verbose=verbose, hybrid_model_refinement=complete_model, final_chain_counts=final_chain_counts)
+        if halfmap_paths is None:
+            target_map = emmap_path
+        else:
+            target_map = halfmap_paths
+        nyquist_resolution = 2*apix + 0.1
+        refined_model_path = run_servalcat_iterative(model_path=input_pdb_path,  map_path=target_map,\
+                    pseudomodel_refinement=pseudomodel_refinement, resolution=nyquist_resolution, num_iter=refmac_iter,\
+                    refmac5_path=refmac5_path,verbose=verbose, hybrid_model_refinement=complete_model, \
+                    final_chain_counts=final_chain_counts, cif_info=cif_info)
         
         if refined_model_path is None:
             tabbed_print.tprint("Problem running servalcat. Returning None")
             return None
         
     if os.path.exists(refined_model_path):
-        bfactors = get_bfactors(in_model_path=refined_model_path)
+        bfactors = get_bfactors(refined_model_path)
             
         if verbose: 
             tabbed_print.tprint("ADP statistics for the refined model")
             tabbed_print.tprint("Mean B-factor: {}".format(np.mean(bfactors)))
             tabbed_print.tprint("Median B-factor: {}".format(np.median(bfactors)))
             tabbed_print.tprint("Max B-factor: {}".format(np.max(bfactors)))
             tabbed_print.tprint("Min B-factor: {}".format(np.min(bfactors)))
             ## If range of bfactors is too small then warn the user
             if max(bfactors)-min(bfactors) < 10:
                 tabbed_print.tprint("Warning: The range of B-factors in the refined model is too small. Please check the model.")
-                tabbed_print.tprint("Consider increasing the bfactor of the target map for refinement using the --add_blur option")
-                tabbed_print.tprint("Current value used for add_blur = {}".format(add_blur))
+                #tabbed_print.tprint("Consider increasing the bfactor of the target map for refinement using the --add_blur option") # Not required 
+                #tabbed_print.tprint("Current value used for add_blur = {}".format(add_blur))
         
+        ## Now shift the refined bfactors to sharpen the emmap if required
+        if not skip_refine:
+
+            
+            minimum_bfactor = 0    
+            shifted_bfactors_structure, shift_value = shift_bfactors_by_probability(
+                                        input_pdb=refined_model_path, probability_threshold=0.01, minimum_bfactor=minimum_bfactor)
+            if verbose:
+                tabbed_print.tprint("Shifting B-factor such that bfactor of p(<0.01) is {} (default)".format(minimum_bfactor))
+                tabbed_print.tprint("Shifted B-factor by {}".format(shift_value))
+            shifted_model_path = refined_model_path[:-4] + '_shifted_bfactors.pdb'
+            shifted_bfactors_structure.write_pdb(shifted_model_path)
+
+            if verbose:
+                tabbed_print.tprint("Writing the shifted model to {}".format(shifted_model_path))
+                # Print the statistics of the shifted model
+                bfactors = get_bfactors(shifted_model_path)
+                tabbed_print.tprint("ADP statistics for the shifted model")
+                tabbed_print.tprint("Mean B-factor: {}".format(np.mean(bfactors)))
+                tabbed_print.tprint("Median B-factor: {}".format(np.median(bfactors)))
+                tabbed_print.tprint("Max B-factor: {}".format(np.max(bfactors)))
+                tabbed_print.tprint("Min B-factor: {}".format(np.min(bfactors)))
+        else:
+            shifted_model_path = refined_model_path
+
     #############################################################################
     # Stage 3: Convert the refined model to a model-map using the 
     # run_refmap() function
     #############################################################################
 
     if verbose:
         print("."*80)
         print("Simulating model-map using refined structure factors\n")
     
-    pseudomodel_modmap = run_refmap(model_path=refined_model_path, emmap_path=emmap_path, mask_path=mask_path, verbose=verbose)
+    pseudomodel_modmap = run_refmap(model_path=shifted_model_path, emmap_path=emmap_path, mask_path=mask_path, verbose=verbose)
     
     #############################################################################
     # Stage 3a: If the user has specified symmetry, then apply the PG symmetry
     #############################################################################
     if pg_symmetry != "C1":
         if verbose:
             tabbed_print.tprint("Imposing a symmetry condition of {}".format(pg_symmetry))
@@ -236,16 +274,16 @@
         print("."*80)
         print("Collecting intermediate files and dumping into a pickle file\n")
     preprocessing_pipeline_directory = os.path.dirname(emmap_path)
     if not complete_model:
         difference_mask_path = "not_used"
     intermediate_outputs = {
         "refined_model_path": refined_model_path,
+        "shifted_model_path": shifted_model_path,
         "pseudomodel_modmap": pseudomodel_modmap,
-        "globally_sharpened_map": globally_sharpened_map,
         "mask_path": mask_path,
         "emmap_path": emmap_path,
         "input_pdb_path": input_pdb_path,
         "difference_mask_path": difference_mask_path,
         "preprocessing_pipeline_directory": preprocessing_pipeline_directory,
     }
```

### Comparing `locscale-2.1.2/locscale/preprocessing/pseudomodel_classes.py` & `locscale-2.1.4b0/locscale/preprocessing/pseudomodel_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,60 +230,63 @@
                 res_count = 0
                 model = self.add_residue(model,chain_count,res_count)
         
         return model
     
     def add_atom(self,model, chain_num, res_num, atom_num, pseudoAtom):
          
-         if pseudoAtom.pdb_position.magnitude() == 0:
-              position = pseudoAtom.position.get()
-         else:
-              position = pseudoAtom.pdb_position.get()
-         atom = gemmi.Atom()
-         atom.element = gemmi.Element('O')
-         atom.pos = gemmi.Position(position[0],position[1],position[2])
-         atom.b_iso = pseudoAtom.bfactor
-         atom.occ = pseudoAtom.occ
-         atom.name = "O"
-         
-         model[chain_num][res_num].add_atom(atom,atom_num)
-         
-         return model
+        if pseudoAtom.pdb_position.magnitude() == 0:
+            position = pseudoAtom.position.get()
+        else:
+            position = pseudoAtom.pdb_position.get()
+        atom = gemmi.Atom()
+        element_choice = np.random.choice(["C","O","N"], p=[0.63,0.2,0.17])
+        atom.element = gemmi.Element(element_choice)
+        atom.pos = gemmi.Position(position[0],position[1],position[2])
+        atom.b_iso = pseudoAtom.bfactor
+        atom.occ = pseudoAtom.occ
+        atom.name = element_choice
+        
+        model[chain_num][res_num].add_atom(atom,atom_num)
+        
+        return model
         
              
     def add_residue(self,model, chain_num, res_num):
-         model[chain_num].add_residue(gemmi.Residue(),res_num)
-         model[chain_num][res_num].name = 'HOH'
-         model[chain_num][res_num].seqid.num = res_num
-     
-         return model
+        model[chain_num].add_residue(gemmi.Residue(),res_num)
+        amino_acid_residues = ['TYR','THR','SER','PRO','PHE','MET','LEU','ILE','HIS','GLY','GLU','GLN','ASP','ASN','ALA','ARG','TRP','CYS']
+        model[chain_num][res_num].name = np.random.choice(amino_acid_residues)
+        model[chain_num][res_num].seqid.num = res_num
+    
+        return model
 
     def update_unitcell(self,apix,unitcell=None):
         from locscale.include.emmer.pdb.pdb_tools import get_unit_cell_estimate
         
         if unitcell is not None:
             self.unitcell = unitcell
         else:
             apix = self.apix
             num = len(self.list)
             self.unitcell = get_unit_cell_estimate(number_of_atoms=num, vsize=apix)
         self.apix = apix
 
     def write_pdb(self,output_string,apix,unitcell=None):
-          self.update_unitcell(apix,unitcell)
-          gemmi_model = self.convert_to_gemmi_model()
-          
-          structure = gemmi.Structure()
-          structure.add_model(gemmi_model)
-          structure.cell = self.unitcell
-          structure.write_pdb(output_string)
-          
+        self.update_unitcell(apix,unitcell)
+        self.update_pdb_positions(apix)
+        gemmi_model = self.convert_to_gemmi_model()
+        
+        structure = gemmi.Structure()
+        structure.add_model(gemmi_model)
+        structure.cell = self.unitcell
+        structure.write_pdb(output_string)
+        
     def update_pdb_positions(self,apix=1):
-         for atom in self.list:
-              atom.pdb_position = atom.position.scale(apix)
+        for atom in self.list:
+            atom.pdb_position = atom.position.scale(apix)
 
 def extract_model_from_mask(mask,num_atoms,threshold=1,ignore_these=None):
     from locscale.preprocessing.pseudomodel_classes import Atom
     import random
     x1,x2,x3 = mask.shape
     buffer = 2 ## To ensure no atoms near edge get picked 
     ones_array = np.ones((x1-2*buffer, x2-2*buffer, x3-2*buffer))
```

### Comparing `locscale-2.1.2/locscale/preprocessing/pseudomodel_solvers.py` & `locscale-2.1.4b0/locscale/preprocessing/pseudomodel_solvers.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/tests/__init__.py` & `locscale-2.1.4b0/locscale/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/tests/locscale_modules.py` & `locscale-2.1.4b0/locscale/tests/locscale_modules.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/tests/test_emmernet.py` & `locscale-2.1.4b0/locscale/tests/test_emmernet.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/tests/test_locscale.py` & `locscale-2.1.4b0/locscale/tests/test_locscale.py`

 * *Files 7% similar despite different names*

```diff
@@ -157,25 +157,39 @@
         with TemporaryDirectory() as tempDir: 
             from locscale.include.emmer.ndimage.map_tools import compute_real_space_correlation as rsc
             import os
             import gemmi
             from subprocess import run
             
             # copy emmap
-            copied_emmap_path = self.copy_files(self.emmap_path_full, tempDir)
-            copied_mask_path = self.copy_files(self.mask_path_full, tempDir)
+            copied_emmap_path = self.copy_files(self.emmap_path, tempDir)
+            copied_mask_path = self.copy_files(self.mask_path, tempDir)
             copied_model_coordinates = self.copy_files(self.model_coordinates, tempDir)
+
+            # delete first few residues 
+            st = gemmi.read_structure(copied_model_coordinates)
+            num_atoms_original = st[0].count_atom_sites()
+            chain = st[0][0]
+            for i in range(250):
+                chain.__delitem__(0)
             
+            num_atoms_trimmed = st[0].count_atom_sites()
+            print("Number of atoms in original model: ",num_atoms_original)
+            print("Number of atoms in trimmed model: ",num_atoms_trimmed)
+            print("Difference: ",num_atoms_original-num_atoms_trimmed)
+            copied_model_coordinates_trimmed = copied_model_coordinates.replace(".pdb","_trimmed.pdb")
+            st.write_pdb(copied_model_coordinates_trimmed)
+                        
             os.chdir(tempDir)
 
             output_locscale_path = os.path.join(tempDir, "locscale_MBI_unittest.mrc")
             locscale_script_path = os.path.join(self.locscale,"locscale","main.py")
             
             locscale_command = ["python",locscale_script_path,"run_locscale","--emmap_path",\
-                copied_emmap_path, "--model_coordinates",copied_model_coordinates,"--mask",copied_mask_path, \
+                copied_emmap_path, "--model_coordinates",copied_model_coordinates_trimmed,"--mask",copied_mask_path, \
                 "--ref_resolution","3.4","--outfile",output_locscale_path,"-ref_it","1","-pm_it","1","--verbose","--complete_model"]
             
             locscale_test_run = run(locscale_command)
             
             self.assertTrue(os.path.exists(output_locscale_path))
 
     def test_no_reference_scaling(self):
```

### Comparing `locscale-2.1.2/locscale/tests/test_symmetry.py` & `locscale-2.1.4b0/locscale/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/tests/utils.py` & `locscale-2.1.4b0/locscale/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 def download_test_data_from_url(download_folder):
     import wget
     print("\nDownloading test data... \n")
     #url_test_data = "https://surfdrive.surf.nl/files/index.php/s/xJKxGXR0LWGBDWM/download"
    # url_test_data = "https://surfdrive.surf.nl/files/index.php/s/lk9CdNO5gszFll1/download"
-    url_test_data = "https://data.4tu.nl/ndownloader/files/35988275/download=1"
+    url_test_data = "https://data.4tu.nl/file/ebf034e4-a348-4094-b03a-3c15c6eebd66/78f706b7-4a8b-4192-99dd-825ec1d9aaef"
     wget.download(url_test_data, download_folder, bar=None)
     
 
 def extract_tar_files_in_folder(tar_folder, use_same_folder=True):
     import tarfile
     import os
     if use_same_folder:
```

### Comparing `locscale-2.1.2/locscale/utils/__init__.py` & `locscale-2.1.4b0/locscale/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+from .__version__ import __version__
 # -*- coding: utf-8 -*-
 #                                      ....                                         
 #                            :-=+======----======+=-:                               
 #                       :=++=:.                    .:=++=:                          
 #                   .=*+:                                -++-                       
 #                 =+=.                                      :++-                    
 #              .++:                                            :++.
```

### Comparing `locscale-2.1.2/locscale/utils/file_tools.py` & `locscale-2.1.4b0/locscale/utils/file_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -289,14 +289,28 @@
             is_test_path_valid = False
             return is_test_path_valid
     
     ## If all tests passed then return True
     is_test_path_valid = True
     return is_test_path_valid
 
+def simple_test_model_to_map_fit(args):
+    '''
+    Test the model to map fit
+    '''
+    from locscale.include.emmer.pdb.fitting_tools import compute_model_to_map_correlation
+    unsharpened_emmap_path, _  = get_emmap_path_from_args(args)
+    model_path = args.model_coordinates
+
+    correlation = compute_model_to_map_correlation(emmap_path=unsharpened_emmap_path, pdb_path=model_path)
+
+    return correlation
+
+
+
 def check_user_input(args):
     '''
     Check user inputs for errors and conflicts
 
     Parameters
     ----------
     args : TYPE
@@ -350,40 +364,48 @@
     if emmap_absent and half_maps_absent:
         raise UserWarning("Please input either an unsharpened map or two half maps")
           
     
     if model_coordinates_present and model_map_present:
         raise UserWarning("Please provide either a model map or a model coordinates. Not both")
     
-    ## If neither model map or model coordinates are provided, then users cannot use --ignore_profiles and --skip_refine flags
+    ## If neither model map or model coordinates are provided, then users cannot use --skip_refine flags
     if model_coordinates_absent and model_map_absent:
-        if args.ignore_profiles:
-            raise UserWarning("You have not provided a Model Map or Model Coordinates. Thus, pseudo-atomic model will be used for \
-                              local sharpening. Please do not raise the --ignore_profiles flag")
         if args.skip_refine:
             raise UserWarning("You have not provided a Model Map or Model Coordinates. Performing REFMAC refinement is essential for \
                               succesful operation of the procedue. Please do not raise the --skip_refine flag")
         
         if args.ref_resolution is None:
             raise UserWarning("You have not provided a Model Map or Model Coordinates. To use REFMAC refinement, resolution target is necessary. \
                               Please provide a target resolution using -res or --ref_resolution")
                             
-    
+    if model_coordinates_present:
+        # Check the model to map fit
+        correlation = simple_test_model_to_map_fit(args)
+        correlation_threshold = 0.3
+        if correlation < correlation_threshold:
+            print(f"Warning: The model to map correlation is {correlation:.2f}. This is below the threshold of {correlation_threshold}")
+        
+
     if model_coordinates_present and model_map_absent:
         if args.skip_refine:
             print("You have asked to skip REFMAC refinement. Atomic bfactors from the input model will be used for simulating Model Map")
         else:
             if args.ref_resolution is None:
                 raise UserWarning("You have provided Model Coordinates. By default, the model bfactors will be refined using REFMAC. \
                                   For this, a target resolution is required. Please provide this resolution target using -res or --ref_resolution. \
                                       Instead if you think model bfactors are accurate, then raise the --skip_refine flag to ignore bfactor refinement.")
             
 
-   
-    
+    if model_coordinates_present and args.complete_model:
+        if args.skip_refine:
+            raise UserWarning("You have asked to skip REFMAC refinement. \
+                                However, you have asked to complete a partially built model. This requires a refined pseudo-atomic model. \
+                                Please do not raise the --skip_refine flag")
+        
     ## Check for window size < 10 A
     if args.window_size is not None:
         window_size_pixels = int(args.window_size)
         if window_size_pixels%2 > 0:
             print("You have input an odd window size. For best performance, an even numbered window size is required. Adding 1 to the provided window size ")
         if args.apix is not None:
             apix = float(args.apix)
@@ -409,15 +431,27 @@
             The constant b-factor is set to 20 by default. When using with reconstruction where the local resolution has a spatial variation \
             then it is not optimal to set the local b-factor to a constant value as it likely boost noise present in high resolution regions. " 
         
         print(fill(disclaimer, width=80))
         ## Pause 
         import time
         time.sleep(2)
-        
+
+def get_cref_from_inputs(parsed_inputs):
+    from locscale.include.emmer.ndimage.filter import get_cosine_mask
+    from locscale.include.emmer.ndimage.fsc_util import get_fsc_filter
+    from locscale.include.emmer.ndimage.map_utils import load_map
+
+    softmask = get_cosine_mask(parsed_inputs["xyz_mask"], 5)
+    halfmap_1, apix = load_map(parsed_inputs["halfmap_paths"][0])
+    halfmap_2, apix = load_map(parsed_inputs["halfmap_paths"][1])
+
+    cref = get_fsc_filter(halfmap_1*softmask, halfmap_2*softmask)
+    return cref
+
 def get_cref_from_arguments(args, mask):
     '''
     Get the cref value from the arguments
     
     Parameters
     ----------
     args : TYPE
```

### Comparing `locscale-2.1.2/locscale/utils/general.py` & `locscale-2.1.4b0/locscale/utils/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     
 ##### SAVE FUNCTIONS #####
 
 def save_list_as_map(values_list, masked_indices, map_shape, map_path, apix):
     from locscale.include.emmer.ndimage.map_utils import save_as_mrc
     from locscale.utils.general import put_scaled_voxels_back_in_original_volume_including_padding
     value_map = put_scaled_voxels_back_in_original_volume_including_padding(values_list, masked_indices, map_shape)
-    save_as_mrc(value_map, output_filename=map_path, apix=apix)
+    return value_map
 
 def write_out_final_volume_window_back_if_required(args, LocScaleVol, parsed_inputs_dict):
     from locscale.utils.general import pad_or_crop_volume
     from locscale.include.emmer.ndimage.map_utils import save_as_mrc
     from locscale.utils.plot_tools import make_locscale_report
     import mrcfile
     import os
```

### Comparing `locscale-2.1.2/locscale/utils/map_quality.py` & `locscale-2.1.4b0/locscale/utils/map_quality.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,45 +46,44 @@
     if mask_path is not None:
         mask = mrcfile.open(mask_path).data
         emmap = emmap * mask
     k = kurtosis(emmap.flatten())
     print("Map kurtosis is: {}".format(round(k,2)))
     return k
 
-def map_quality_pdb_multiple(list_of_emmap_path, mask_path, pdb_path):
+def map_quality_pdb_multiple(list_of_emmap_path, pdb_path):
     from locscale.include.emmer.ndimage.map_tools import compute_real_space_correlation as rscc
     from locscale.include.emmer.ndimage.fsc_util import calculate_fsc_maps
     from locscale.include.emmer.pdb.pdb_utils import set_atomic_bfactors
-    from locscale.include.emmer.pdb.pdb_to_map import pdb2map
+    from locscale.include.emmer.ndimage.map_tools import get_atomic_model_mask
+    from locscale.include.emmer.ndimage.map_utils import load_map
+    from locscale.include.emmer.pdb.pdb_to_map import pdb2map, detect_pdb_input
     from locscale.include.emmer.ndimage.profile_tools import frequency_array
     
     metrics_per_emmap = {}
-    mask = mrcfile.open(mask_path).data
-    apix = mrcfile.open(mask_path).voxel_size.tolist()[0]
-    size=mask.shape
+    
+    emmap, apix = load_map(list_of_emmap_path[0])
+    size = emmap.shape
+
     st = gemmi.read_structure(pdb_path)
     st_0 = set_atomic_bfactors(input_gemmi_st=st, b_iso=0)
     simmap = pdb2map(st_0, apix=apix, size=size, verbose=False, set_refmac_blur=True)
-    masked_simmap = simmap * mask
+    mask = get_atomic_model_mask(list_of_emmap_path[0], pdb_path, save_files=False)
+    boolean_mask = (mask > 0.5).astype(bool)
         
     for emmap_path in list_of_emmap_path:
         metric_dictionary = {}
         emmap = mrcfile.open(emmap_path).data
-
-        
-        masked_emmap = emmap * mask
         
-        
-        metric_dictionary['rscc'] = rscc(masked_emmap, masked_simmap)
- 
-        fsc_curve = calculate_fsc_maps(masked_emmap, masked_simmap)
-        freq = frequency_array(fsc_curve, apix=apix)
+        metric_dictionary['rscc'] = rscc(emmap[boolean_mask], simmap[boolean_mask])
+        fsc_curve = calculate_fsc_maps(mask*emmap, mask*simmap)
         metric_dictionary['fsc'] = fsc_curve.mean()
+
         metrics_per_emmap[emmap_path] = metric_dictionary
-        print(emmap_path.split("/")[-1], metrics_per_emmap[emmap_path])
+        
 
     return metrics_per_emmap
 
 def map_quality_pdb(emmap_path, mask_path, pdb_path, test='rscc'):
     from locscale.include.emmer.ndimage.map_tools import compute_real_space_correlation as rscc
     from locscale.include.emmer.ndimage.fsc_util import calculate_fsc_maps
     from locscale.include.emmer.pdb.pdb_utils import set_atomic_bfactors
```

### Comparing `locscale-2.1.2/locscale/utils/math_tools.py` & `locscale-2.1.4b0/locscale/utils/math_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale/utils/plot_tools.py` & `locscale-2.1.4b0/locscale/utils/plot_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 ## PLOT FUNCTIONS
 import numpy as np
+import os
 
 def plot_regression(data_input, x_col, y_col, x_label=None, y_label=None, title_text=None):
     from matplotlib.offsetbox import AnchoredText
     import matplotlib.pyplot as plt
     from scipy.optimize import curve_fit
     from locscale.utils.math_tools import general_quadratic, r2
     
@@ -109,48 +110,53 @@
         print(text)
     
 
 
 def print_input_arguments(args):
     import matplotlib.pyplot as plt
     
-    fig, ax =plt.subplots(figsize=(16,16))
+    fig, ax =plt.subplots()
     
     ax.axis('off')
     
     text = []
     path_arguments = [x for x in vars(args) if x in ["emmap_path","half_map1","half_map2","model_map",
                                                   "mask","model_coordinates","outfile"]]
     for arg in vars(args):
         val = getattr(args, arg)
         if arg in path_arguments and val is not None:
             full_path = val
             filename = full_path.split("/")[-1]
-            text.append([arg, filename])
+            text.append([arg, os.path.basename(filename)])
         else:
-            text.append([arg, val])
+            # if value is a numpy array or a list, just skip it
+            if type(val) == list or type(val) == np.ndarray:
+                continue
+            else:
+                text.append([arg, str(val)])
     
     
     table= ax.table(cellText=text, loc="center", colLabels=["Parameter","Values"], cellLoc='center')
     table.auto_set_font_size(False)
     table.set_fontsize(16)
     table.scale(1,2)
     return fig
    
 def plot_bfactor_distribution_standard(unsharpened_emmap_path, locscale_map_path, mask_path, fsc_resolution):
-    from locscale.include.emmer.ndimage.map_tools import get_bfactor_distribution
+    from locscale.include.emmer.ndimage.map_tools import get_bfactor_distribution, get_bfactor_distribution_multiple
     import matplotlib.pyplot as plt
     import seaborn as sns
     
     fig, ax =plt.subplots(figsize=(8,8))
     
-    unsharped_emmap_dist = get_bfactor_distribution(unsharpened_emmap_path, mask_path, fsc_resolution)
-   
-    locscale_dist = get_bfactor_distribution(locscale_map_path, mask_path, fsc_resolution)
-    
+    bfactor_distributions = get_bfactor_distribution_multiple([unsharpened_emmap_path, locscale_map_path], mask_path, fsc_resolution, num_centers=2000, wilson_cutoff="standard")
+
+    unsharped_emmap_dist = list(bfactor_distributions.values())[0]
+    locscale_dist = list(bfactor_distributions.values())[1]
+       
     unsharpened_array = np.array([x[0] for x in unsharped_emmap_dist.values()])
     locscale_array = np.array([x[0] for x in locscale_dist.values()])
    
     sns.kdeplot(unsharpened_array)
    
     sns.kdeplot(locscale_array)
     
@@ -189,15 +195,15 @@
     from locscale.include.emmer.ndimage.plots import plot_emmap_section, plot_radial_profile
     from locscale.utils.plot_tools import plot_pickle_output
     from locscale.include.emmer.ndimage.profile_tools import compute_radial_profile, frequency_array 
     from matplotlib.backends.backend_pdf import PdfPages
     import os
     import mrcfile
     from locscale.include.emmer.ndimage.fsc_util import plot_fsc_maps
-    from locscale.utils.file_tools import get_fsc_curve_from_arguments
+    from locscale.utils.file_tools import get_fsc_curve_from_arguments, get_cref_from_inputs
     from locscale.utils.general import pad_or_crop_volume
     import matplotlib.pyplot as plt
     
     ## Input-Output characteristics
     locscale_map = mrcfile.open(locscale_path).data
     
     
@@ -237,15 +243,15 @@
     except Exception as e:
         print("Could not print radial profiles")
         print(e)
     
     #2a FSC curve halfmaps
     try:
         fsc_curve = get_fsc_curve_from_arguments(args)
-        cref = parsed_input['Cref']
+        cref = get_cref_from_inputs(vars(args))
         if cref is not None:
             fig, ax = plt.subplots(figsize=(8,8))
             ax.plot(freq, fsc_curve,'b')
             ax.plot(freq, cref, 'r')
             ax.set_xlabel("Frequency (1/A)")
             ax.set_ylabel("FSC")
             ax.legend(["FSC curve","Cref"])
```

### Comparing `locscale-2.1.2/locscale/utils/scaling_tools.py` & `locscale-2.1.4b0/locscale/utils/scaling_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 import os
+
+from locscale.include.emmer.ndimage.map_utils import save_as_mrc
 #import gemmi
 
 
 def compute_radial_profile_proper(vol, frequency_map):
 
     vol_fft = np.fft.rfftn(vol, norm="ortho");
     dim = vol_fft.shape;
@@ -304,15 +306,15 @@
     else:
         progress_bar=tqdm(total=len(scaling_dictionary['masked_xyz_locs']), desc="LocScale")
     
     ###############################################################################
     # Stage 2: Perform the scaling in a rolling window fashion
     ###############################################################################
     frequency_map_window = FDRutil.calculate_frequency_map(np.zeros((wn, wn, wn)));
-
+    
     for k, j, i in scaling_dictionary['masked_xyz_locs'] - wn / 2:
         try:
             # k,j,i are indices of the corner voxel in each cube. Ensure it is rounded up to integer.
             k,j,i,wn = round_up_proper(k), round_up_proper(j), round_up_proper(i), round_up_proper(wn)
             
             #######################################################################
             # Stage 2a: Extract the cube from the EM map and model maps
@@ -338,14 +340,15 @@
                 k_center, j_center, i_center = round_up_proper(k + wn // 2), round_up_proper(j + wn // 2), round_up_proper(i + wn // 2)
 
                 central_voxel_inside_mask = difference_mask_bool[k_center, j_center, i_center]
                 use_theoretical_profile = central_voxel_inside_mask
             else:
                 use_theoretical_profile = scaling_dictionary['use_theoretical_profile']
 
+
             scale_factor_result = compute_scale_factors(
                 em_profile,mod_profile, apix=apix, check_scaling=check_scaling, \
                 scale_factor_arguments=scaling_dictionary['scale_factor_arguments'], \
                 use_theoretical_profile=use_theoretical_profile)
             
             scale_factors = scale_factor_result['scale_factors']
             bfactor = scale_factor_result['bfactor']
@@ -438,14 +441,15 @@
         if audit and scaling_dictionary['use_theoretical_profile']:
             import os
             
             pickle_file_output = os.path.join(temp_folder,"profiles_audit.pickle")
             with open(pickle_file_output,"wb") as audit:
                 pickle.dump(profiles_audit, audit)
 
+    
     ###############################################################################
     # Stage 4: Convert to numpy array and return the values
     ###############################################################################                                
     sharpened_vals_array = np.array(sharpened_vals, dtype=np.float32)
     bfactor_vals_array = np.array(bfactor_voxels, dtype=np.float32)
     qfit_vals_array = np.array(qfit_voxels, dtype=np.float32)
     
@@ -455,15 +459,15 @@
 def run_window_function_including_scaling(parsed_inputs_dict):
     """
     This is a function which performs high level data processing for Locscale
 
     """
     from locscale.utils.general import get_xyz_locs_and_indices_after_edge_cropping_and_masking
     from locscale.utils.general import save_list_as_map, put_scaled_voxels_back_in_original_volume_including_padding
-    from locscale.utils.general import merge_sequence_of_sequences, split_sequence_evenly
+    from locscale.utils.general import merge_sequence_of_sequences, split_sequence_evenly, write_out_final_volume_window_back_if_required
     from joblib import Parallel, delayed
     ###############################################################################
     # Stage 1: Collect inputs from the dictionary
     ###############################################################################
 
     scaling_dictionary = parsed_inputs_dict
     
@@ -480,15 +484,15 @@
     scaling_dictionary["map_shape"] = map_shape
     
 
     scaling_dictionary_split = {}
     for i in range(scaling_dictionary['number_processes']):
         scaling_dictionary_split[i] = scaling_dictionary.copy()
         scaling_dictionary_split[i]["masked_xyz_locs"] = masked_xyz_locs_split[i]
-        scaling_dictionary_split[i]["use_mpi"] = True
+        scaling_dictionary_split[i]["use_mpi"] = False
     ###############################################################################
     # Stage 3: Run the window function to get sharpened values and bfactor information
     ###############################################################################
     # Use joblib to parallelize the window function 
     if scaling_dictionary['number_processes'] > 1:
         results = Parallel(n_jobs=scaling_dictionary['number_processes'])(
             delayed(get_central_scaled_pixel_vals_after_scaling)(scaling_dictionary_split[i]) for i in range(scaling_dictionary['number_processes']))
@@ -517,16 +521,25 @@
     
     ###############################################################################
     # Stage 5: Save processing files such as bfactor map and qfit maps 
     ###############################################################################
     
     bfactor_path = os.path.join(scaling_dictionary['processing_files_folder'], "bfactor_map.mrc")
     qfit_path = os.path.join(scaling_dictionary['processing_files_folder'], "qfit_map.mrc")
-    save_list_as_map(bfactor_vals, masked_indices, map_shape, bfactor_path, scaling_dictionary['apix'])
-    save_list_as_map(qfit_vals, masked_indices, map_shape, qfit_path, scaling_dictionary['apix'])
+    bfactor_map = save_list_as_map(bfactor_vals, masked_indices, map_shape, bfactor_path, scaling_dictionary['apix'])
+    qfit_map = save_list_as_map(qfit_vals, masked_indices, map_shape, qfit_path, scaling_dictionary['apix'])
+
+    if scaling_dictionary["win_bleed_pad"]:
+        #map_shape = [(LocScaleVol.shape[0] - wn), (LocScaleVol.shape[1] - wn), (LocScaleVol.shape[2] - wn)]
+        from locscale.utils.general import pad_or_crop_volume
+        map_shape = scaling_dictionary["original_map_shape"]
+        bfactor_map = pad_or_crop_volume(bfactor_map, (map_shape))
+        qfit_map = pad_or_crop_volume(qfit_map, (map_shape))
+    save_as_mrc(bfactor_map, bfactor_path, scaling_dictionary['apix'])
+    save_as_mrc(qfit_map, qfit_path, scaling_dictionary['apix'])
 
     ###############################################################################
     # Stage 6: Return the scaled map
     ###############################################################################
     return map_scaled
 
 def run_window_function_including_scaling_mpi(parsed_inputs_dict):
```

### Comparing `locscale-2.1.2/locscale/utils/theoretical_profiles.pickle` & `locscale-2.1.4b0/locscale/utils/theoretical_profiles.pickle`

 * *Files identical despite different names*

### Comparing `locscale-2.1.2/locscale.egg-info/PKG-INFO` & `locscale-2.1.4b0/locscale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: locscale
-Version: 2.1.2
+Version: 2.1.4b0
 Summary: Contrast optimization for cryo-EM maps
 Home-page: https://gitlab.tudelft.nl/aj-lab/locscale
 Author: Alok Bharadwaj, Arjen J. Jakobi, Reinier de Bruin
 License: 3-clause BSD
 Project-URL: Bug Tracker, https://gitlab.tudelft.nl/aj-lab/locscale/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
@@ -230,9 +229,7 @@
 - A.J. Jakobi, M. Wilmanns and C. Sachse, [Model-based local density sharpening of cryo-EM maps](https://doi.org/10.7554/eLife.27131), eLife 6: e27131 (2017).
 - A. Bharadwaj and A.J. Jakobi, [Electron scattering properties and their use in cryo-EM map sharpening](https://doi.org/10.1039/D2FD00078D), Faraday Discussions D2FD00078D (2022)
 ---
 
 ## Bugs and questions
 
 For bug reports please use the [GitLab issue tracker](https://gitlab.tudelft.nl/aj-lab/locscale/issues).   
-
-
```

### Comparing `locscale-2.1.2/locscale.egg-info/SOURCES.txt` & `locscale-2.1.4b0/locscale.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 locscale/__init__.py
+locscale/__version__.py
 locscale/main.py
 locscale.egg-info/PKG-INFO
 locscale.egg-info/SOURCES.txt
 locscale.egg-info/dependency_links.txt
 locscale.egg-info/entry_points.txt
 locscale.egg-info/not-zip-safe
 locscale.egg-info/requires.txt
@@ -40,14 +41,15 @@
 locscale/include/emmer/ndimage/plots.py
 locscale/include/emmer/ndimage/power.py
 locscale/include/emmer/ndimage/profile_tools.py
 locscale/include/emmer/ndimage/simulate.py
 locscale/include/emmer/pdb/__init__.py
 locscale/include/emmer/pdb/common_pdb_headers.py
 locscale/include/emmer/pdb/convert_pdb_to_mmcif.py
+locscale/include/emmer/pdb/fitting_tools.py
 locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py
 locscale/include/emmer/pdb/get_dssp.py
 locscale/include/emmer/pdb/modify_pdb.py
 locscale/include/emmer/pdb/pdb_to_map.py
 locscale/include/emmer/pdb/pdb_tools.py
 locscale/include/emmer/pdb/pdb_utils.py
 locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py
@@ -67,11 +69,13 @@
 locscale/tests/test_symmetry.py
 locscale/tests/utils.py
 locscale/utils/__init__.py
 locscale/utils/file_tools.py
 locscale/utils/general.py
 locscale/utils/map_quality.py
 locscale/utils/math_tools.py
+locscale/utils/parse_utils.py
 locscale/utils/plot_tools.py
 locscale/utils/prepare_inputs.py
 locscale/utils/scaling_tools.py
+locscale/utils/startup_utils.py
 locscale/utils/theoretical_profiles.pickle
```

### Comparing `locscale-2.1.2/setup.py` & `locscale-2.1.4b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,109 +1,118 @@
 from __future__ import division, absolute_import, print_function
-import setuptools
 from setuptools import find_packages
 from setuptools.command.install import install
 from setuptools.command.develop import develop
 from numpy.distutils.core import Extension, setup
 import unittest
 import pathlib
-locscale_path=pathlib.Path(__file__).parent.resolve()
 
-ex1 = Extension(name = 'fcodes_fast',
-                sources = ['locscale/include/symmetry_emda/fcodes_fast.f90'])
+locscale_path = pathlib.Path(__file__).parent.resolve()
+
+ex1 = Extension(name='fcodes_fast',
+                sources=['locscale/include/symmetry_emda/fcodes_fast.f90'])
 
 long_description = (locscale_path / "README.md").read_text()
 
+
+def get_version():
+    version_text = (locscale_path / "locscale" / "__version__.py").read_text()
+    version = version_text.split("=")[1][1:-1]
+    return version
+
+
 def locscale_test_suite():
-  test_loader = unittest.TestLoader()
-  test_suite = test_loader.discover('tests', pattern='test_*.py')
-  return test_suite
+    test_loader = unittest.TestLoader()
+    test_suite = test_loader.discover('tests', pattern='test_*.py')
+    return test_suite
+
 
 class PostDevelopCommand(develop):
-  """ Post-installation for development mode. """
-  def run(self):
-    import os
-    develop.run(self)   
-
-    from subprocess import run
-    from shutil import which
-    import os
-
-    ## Install conda packages   
-    run(["conda", "install", "-c", "conda-forge", "cudatoolkit=11.3.1","--yes"])
-    run(["conda", "install", "-c", "conda-forge", "cudnn=8.2.1","--yes"])
-    run(["conda", "install", "-c", "conda-forge", "openmpi=4.1.2","--yes"])
-    run(["conda", "install", "-c", "conda-forge", "mpi4py=3.1","--yes"])
-
-    # Check if refmac5 is installed
-    refmac5_path = which("refmac5")
-    if refmac5_path is None:
-      raise UserWarning("Refmac5 is not installed. Please install it and try again.")
-    else:
-      print("Refmac5 is installed at {}".format(refmac5_path))
-      print("If you want to use a different binary please use the --refmac5_path option or alias it to refmac5")
-    
+    """ Post-installation for development mode. """
+
+    def run(self):
+        develop.run(self)
+
+        from subprocess import run
+        from shutil import which
+
+        # Install conda packages
+        run(["conda", "install", "-c", "conda-forge", "cudatoolkit=11.3.1", "--yes"])
+        run(["conda", "install", "-c", "conda-forge", "cudnn=8.2.1", "--yes"])
+        run(["conda", "install", "-c", "conda-forge", "openmpi=4.1.2", "--yes"])
+        run(["conda", "install", "-c", "conda-forge", "mpi4py=3.1", "--yes"])
+
+        # Check if refmac5 is installed
+        refmac5_path = which("refmac5")
+        if refmac5_path is None:
+            raise UserWarning(
+                "Refmac5 is not installed. Please install it and try again.")
+        else:
+            print("Refmac5 is installed at {}".format(refmac5_path))
+            print("If you want to use a different binary please use the --refmac5_path option or alias it to refmac5")
+
 
 class PostInstallCommand(install):
-  """Post-installation for installation mode."""
-  def run(self):
-    install.run(self)
-    
-    from subprocess import run
-    from shutil import which
-    import os
-
-    ## Install conda packages   
-    run(["conda", "install", "-c", "conda-forge", "cudatoolkit=11.3.1","--yes"])
-    run(["conda", "install", "-c", "conda-forge", "cudnn=8.2.1","--yes"])
-    run(["conda", "install", "-c", "conda-forge", "openmpi=4.1.2","--yes"])
-    run(["conda", "install", "-c", "conda-forge", "mpi4py=3.1","--yes"])
-
-    # Check if refmac5 is installed
-    refmac5_path = which("refmac5")
-    if refmac5_path is None:
-      raise UserWarning("Refmac5 is not installed. Please install CCP4 before running locscale. Without Refmac locscale cannot refine the input atomic structure.")
-    else:
-      print("Refmac5 is installed at {}".format(refmac5_path))
-      print("If you want to use a different binary please use the --refmac5_path option or alias it to refmac5")
+    """Post-installation for installation mode."""
+
+    def run(self):
+        install.run(self)
+
+        from subprocess import run
+        from shutil import which
+
+        # Install conda packages
+        run(["conda", "install", "-c", "conda-forge", "cudatoolkit=11.3.1", "--yes"], check=True)
+        run(["conda", "install", "-c", "conda-forge", "cudnn=8.2.1", "--yes"], check=True)
+        run(["conda", "install", "-c", "conda-forge", "openmpi=4.1.2", "--yes"], check=True)
+        run(["conda", "install", "-c", "conda-forge", "mpi4py=3.1", "--yes"], check=True)
+
+        # Check if refmac5 is installed
+        refmac5_path = which("refmac5")
+        if refmac5_path is None:
+            raise UserWarning(
+                "Refmac5 is not installed. Please install CCP4 before running locscale. Without Refmac locscale cannot refine the input atomic structure.")
+        else:
+            print("Refmac5 is installed at {}".format(refmac5_path))
+            print("If you want to use a different binary please use the --refmac5_path option or alias it to refmac5")
 
 
 setup(name='locscale',
-    version='2.1.2',
-    author='Alok Bharadwaj, Arjen J. Jakobi, Reinier de Bruin',
-    url='https://gitlab.tudelft.nl/aj-lab/locscale',
-    project_urls={
-        "Bug Tracker": "https://gitlab.tudelft.nl/aj-lab/locscale/issues",
-    },
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "License :: OSI Approved :: BSD License",
-    ],
-    description= 'Contrast optimization for cryo-EM maps',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    license='3-clause BSD',
-    packages=find_packages(),
-    include_package_data=True,
-    package_data={'locscale': ['utils/*.pickle', 'include/symmetry_emda/*.f90', 'emmernet/emmernet_models/*.tar.gz', 'emmernet/emmernet_models/*.hdf5']},
-    install_requires=['matplotlib>=3.3.4','biopython>=1.78','numpy==1.19.2','scipy>=1.5.4','pandas>=1.1.5',\
-                      'mrcfile>=1.3.0','gemmi>=0.4.8','pypdb>=2.0','sklearn>=0.0','pwlf>=2.0.4','tqdm>=4.62.3',\
-                      'more_itertools>=8.10.0','servalcat>=0.2.23','tensorflow==2.6','tensorflow-addons==0.14.0',\
-                      'keras==2.6.0','tensorflow_datasets==4.5.2','pyfiglet>=0.8.post1', 'wget>=3.2','seaborn>=0.11' 'locscale'],
-    extras_require={'mac': ['tensorflow-macos==2.7','tensorflow-metal']},
-    entry_points={
-      'console_scripts': [
-          'locscale = locscale.main:main',
-                          ],
+      version=get_version(),
+      author='Alok Bharadwaj, Arjen J. Jakobi, Reinier de Bruin',
+      url='https://gitlab.tudelft.nl/aj-lab/locscale',
+      project_urls={
+          "Bug Tracker": "https://gitlab.tudelft.nl/aj-lab/locscale/issues",
       },
-    test_suite = 'setup.locscale_test_suite',
-    ext_modules =[ex1],
-    cmdclass={'develop': PostDevelopCommand,
-              'install': PostInstallCommand},
-
-    zip_safe= False)
+      classifiers=[
+          "Development Status :: 4 - Beta",
+          "Intended Audience :: Science/Research",
+          "Topic :: Scientific/Engineering",
+          "Operating System :: OS Independent",
+          "Programming Language :: Python :: 3.7",
+          "Programming Language :: Python :: 3.8",
+          "License :: OSI Approved :: BSD License",
+      ],
+      description='Contrast optimization for cryo-EM maps',
+      long_description=long_description,
+      long_description_content_type="text/markdown",
+      license='3-clause BSD',
+      packages=find_packages(),
+      include_package_data=True,
+      package_data={'locscale': ['utils/*.pickle', 'include/symmetry_emda/*.f90',
+                                 'emmernet/emmernet_models/*.tar.gz', 'emmernet/emmernet_models/*.hdf5']},
+      install_requires=['matplotlib>=3.3.4', 'biopython>=1.78', 'numpy==1.19.2', 'scipy>=1.5.4', 'pandas>=1.1.5',
+                        'mrcfile>=1.3.0', 'gemmi>=0.4.8', 'pypdb==2.0', 'scikit-learn', 'pwlf>=2.0.4', 'tqdm>=4.62.3',
+                        'more_itertools>=8.10.0', 'servalcat>=0.2.23', 'tensorflow==2.6', 'tensorflow-addons==0.14.0',
+                        'keras==2.6.0', 'tensorflow_datasets==4.5.2', 'pyfiglet>=0.8.post1', 'wget>=3.2', 'seaborn>=0.11', 'locscale'],
+      extras_require={'mac': ['tensorflow-macos==2.7', 'tensorflow-metal']},
+      entry_points={
+          'console_scripts': [
+              'locscale = locscale.main:main',
+          ],
+      },
+      test_suite='setup.locscale_test_suite',
+      ext_modules=[ex1],
+      cmdclass={'develop': PostDevelopCommand,
+                'install': PostInstallCommand},
 
+      zip_safe=False)
```

