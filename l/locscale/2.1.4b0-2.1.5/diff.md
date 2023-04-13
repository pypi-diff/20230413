# Comparing `tmp/locscale-2.1.4b0.tar.gz` & `tmp/locscale-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/locscale-2.1.4b0.tar", last modified: Thu Apr 13 15:09:06 2023, max compression
+gzip compressed data, was "dist/locscale-2.1.5.tar", last modified: Thu Apr 13 15:14:46 2023, max compression
```

## Comparing `locscale-2.1.4b0.tar` & `locscale-2.1.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)      112 2023-04-13 14:56:22.000000 locscale-2.1.4b0/MANIFEST.in
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12585 2023-04-13 15:09:06.000000 locscale-2.1.4b0/PKG-INFO
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    11879 2023-04-13 14:56:22.000000 locscale-2.1.4b0/README.md
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3145 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)       24 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/__version__.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/automate/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/automate/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    19847 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/automate/tools.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/emmernet/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8207 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/emmernet_functions.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     1513 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/prepare_inputs.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8544 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/run_emmernet.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     6807 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/emmernet/utils.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/__init__.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    21182 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/FDRutil.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/__init__.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     6395 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/confidenceMapMain.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    28996 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/locscaleUtil.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     9543 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/confidenceMapUtil/mapUtil.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/emmer/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/__init__.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      451 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/headers.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/__init__.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      301 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/common_map_headers.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     8135 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/emdb_class.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     4899 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/fft_util.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     6459 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/filter.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    18483 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/fsc_util.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12535 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/map_quality_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22698 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/map_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    24544 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/map_utils.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     5382 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/plotContourMap.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    15302 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/plots.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     1239 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/power.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22355 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/profile_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      703 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/ndimage/simulate.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/__init__.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      471 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/common_pdb_headers.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      977 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     5196 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/fitting_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3749 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     4171 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/get_dssp.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)      941 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/modify_pdb.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     8502 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_to_map.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22212 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    30907 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_utils.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    39092 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    29183 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/apply_rotation_matrix.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)   136871 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/fcodes_fast.f90
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3335 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/include/symmetry_emda/symmetrize_map.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     2181 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/main.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/preprocessing/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    31098 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/headers.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    15239 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/pipeline.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    13909 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/pseudomodel_classes.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    13077 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/preprocessing/pseudomodel_solvers.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/tests/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8246 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/locscale_modules.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3442 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/test_emmernet.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    10021 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/test_locscale.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3046 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/test_symmetry.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     2114 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/tests/utils.py
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale/utils/
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/__init__.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    17346 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/file_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    10962 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/general.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8644 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/map_quality.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     1108 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/math_tools.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8721 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/parse_utils.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    11144 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/plot_tools.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    21576 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/prepare_inputs.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    34587 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/scaling_tools.py
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     7000 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/startup_utils.py
--rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    10678 2023-04-13 14:56:22.000000 locscale-2.1.4b0/locscale/utils/theoretical_profiles.pickle
-drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12585 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/PKG-INFO
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     2957 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/SOURCES.txt
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)        1 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/dependency_links.txt
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)       48 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/entry_points.txt
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)        1 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/not-zip-safe
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)      374 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/requires.txt
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)       21 2023-04-13 15:09:06.000000 locscale-2.1.4b0/locscale.egg-info/top_level.txt
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)      138 2023-04-13 14:56:22.000000 locscale-2.1.4b0/pyproject.toml
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)      107 2023-04-13 15:09:06.000000 locscale-2.1.4b0/setup.cfg
--rw-r-----   0 abharadwaj1 (450985) domain users (10513)     4899 2023-04-13 14:56:22.000000 locscale-2.1.4b0/setup.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      112 2023-04-13 14:56:22.000000 locscale-2.1.5/MANIFEST.in
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12583 2023-04-13 15:14:46.000000 locscale-2.1.5/PKG-INFO
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    11879 2023-04-13 14:56:22.000000 locscale-2.1.5/README.md
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3145 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)       19 2023-04-13 15:14:22.000000 locscale-2.1.5/locscale/__version__.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/automate/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/automate/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    19847 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/automate/tools.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/emmernet/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/emmernet/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8207 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/emmernet/emmernet_functions.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     1513 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/emmernet/prepare_inputs.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8544 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/emmernet/run_emmernet.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     6807 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/emmernet/utils.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/include/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/__init__.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/include/confidenceMapUtil/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    21182 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/confidenceMapUtil/FDRutil.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/confidenceMapUtil/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     6395 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/confidenceMapUtil/confidenceMapMain.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    28996 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/confidenceMapUtil/locscaleUtil.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     9543 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/confidenceMapUtil/mapUtil.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/include/emmer/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      451 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/headers.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/include/emmer/ndimage/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      301 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/common_map_headers.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     8135 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/emdb_class.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     4899 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/fft_util.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     6459 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/filter.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    18483 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/fsc_util.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12535 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/map_quality_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22698 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/map_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    24544 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/map_utils.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     5382 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/plotContourMap.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    15302 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/plots.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     1239 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/power.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22355 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/profile_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      703 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/ndimage/simulate.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/include/emmer/pdb/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/__init__.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      471 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/common_pdb_headers.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)      977 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     5196 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/fitting_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3749 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     4171 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/get_dssp.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      941 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/modify_pdb.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     8502 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/pdb_to_map.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    22212 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/pdb_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    30907 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/emmer/pdb/pdb_utils.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/include/symmetry_emda/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    39092 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/symmetry_emda/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    29183 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/symmetry_emda/apply_rotation_matrix.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)   136871 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/symmetry_emda/fcodes_fast.f90
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3335 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/include/symmetry_emda/symmetrize_map.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     2181 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/main.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/preprocessing/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/preprocessing/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    31098 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/preprocessing/headers.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    15239 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/preprocessing/pipeline.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    13909 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/preprocessing/pseudomodel_classes.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    13077 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/preprocessing/pseudomodel_solvers.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/tests/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/tests/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8246 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/tests/locscale_modules.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     3442 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/tests/test_emmernet.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    10021 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/tests/test_locscale.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3046 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/tests/test_symmetry.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     2114 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/tests/utils.py
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale/utils/
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)     3108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/__init__.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    17346 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/file_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    10962 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/general.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8644 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/map_quality.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     1108 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/math_tools.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     8721 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/parse_utils.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    11144 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/plot_tools.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    21576 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/prepare_inputs.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    34587 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/scaling_tools.py
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     7000 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/startup_utils.py
+-rwxr-x---   0 abharadwaj1 (450985) domain users (10513)    10678 2023-04-13 14:56:22.000000 locscale-2.1.5/locscale/utils/theoretical_profiles.pickle
+drwxr-x---   0 abharadwaj1 (450985) domain users (10513)        0 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)    12583 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/PKG-INFO
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     2957 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/SOURCES.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)        1 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/dependency_links.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)       48 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/entry_points.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)        1 2023-04-13 15:09:06.000000 locscale-2.1.5/locscale.egg-info/not-zip-safe
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      374 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/requires.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)       21 2023-04-13 15:14:46.000000 locscale-2.1.5/locscale.egg-info/top_level.txt
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      138 2023-04-13 14:56:22.000000 locscale-2.1.5/pyproject.toml
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)      107 2023-04-13 15:14:46.000000 locscale-2.1.5/setup.cfg
+-rw-r-----   0 abharadwaj1 (450985) domain users (10513)     4899 2023-04-13 14:56:22.000000 locscale-2.1.5/setup.py
```

### Comparing `locscale-2.1.4b0/PKG-INFO` & `locscale-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locscale
-Version: 2.1.4b0
+Version: 2.1.5
 Summary: Contrast optimization for cryo-EM maps
 Home-page: https://gitlab.tudelft.nl/aj-lab/locscale
 Author: Alok Bharadwaj, Arjen J. Jakobi, Reinier de Bruin
 License: 3-clause BSD
 Project-URL: Bug Tracker, https://gitlab.tudelft.nl/aj-lab/locscale/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `locscale-2.1.4b0/README.md` & `locscale-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/__init__.py` & `locscale-2.1.5/locscale/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/automate/__init__.py` & `locscale-2.1.5/locscale/automate/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/automate/tools.py` & `locscale-2.1.5/locscale/automate/tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/emmernet/__init__.py` & `locscale-2.1.5/locscale/emmernet/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/emmernet/emmernet_functions.py` & `locscale-2.1.5/locscale/emmernet/emmernet_functions.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/emmernet/prepare_inputs.py` & `locscale-2.1.5/locscale/emmernet/prepare_inputs.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/emmernet/run_emmernet.py` & `locscale-2.1.5/locscale/emmernet/run_emmernet.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/emmernet/utils.py` & `locscale-2.1.5/locscale/emmernet/utils.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/__init__.py` & `locscale-2.1.5/locscale/include/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/confidenceMapUtil/FDRutil.py` & `locscale-2.1.5/locscale/include/confidenceMapUtil/FDRutil.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/confidenceMapUtil/confidenceMapMain.py` & `locscale-2.1.5/locscale/include/confidenceMapUtil/confidenceMapMain.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/confidenceMapUtil/locscaleUtil.py` & `locscale-2.1.5/locscale/include/confidenceMapUtil/locscaleUtil.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/confidenceMapUtil/mapUtil.py` & `locscale-2.1.5/locscale/include/confidenceMapUtil/mapUtil.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/__init__.py` & `locscale-2.1.5/locscale/include/emmer/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/__init__.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/emdb_class.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/emdb_class.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/fft_util.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/fft_util.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/filter.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/filter.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/fsc_util.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/fsc_util.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/map_quality_tools.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/map_quality_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/map_tools.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/map_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/map_utils.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/map_utils.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/plotContourMap.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/plotContourMap.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/plots.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/plots.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/power.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/power.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/profile_tools.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/profile_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/ndimage/simulate.py` & `locscale-2.1.5/locscale/include/emmer/ndimage/simulate.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/__init__.py` & `locscale-2.1.5/locscale/include/emmer/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py` & `locscale-2.1.5/locscale/include/emmer/pdb/convert_pdb_to_mmcif.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/fitting_tools.py` & `locscale-2.1.5/locscale/include/emmer/pdb/fitting_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py` & `locscale-2.1.5/locscale/include/emmer/pdb/get_associated_pdbs_for_all_emdb.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/get_dssp.py` & `locscale-2.1.5/locscale/include/emmer/pdb/get_dssp.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/modify_pdb.py` & `locscale-2.1.5/locscale/include/emmer/pdb/modify_pdb.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_to_map.py` & `locscale-2.1.5/locscale/include/emmer/pdb/pdb_to_map.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_tools.py` & `locscale-2.1.5/locscale/include/emmer/pdb/pdb_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/emmer/pdb/pdb_utils.py` & `locscale-2.1.5/locscale/include/emmer/pdb/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py` & `locscale-2.1.5/locscale/include/symmetry_emda/GenerateOperators_v9_ky4.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/symmetry_emda/__init__.py` & `locscale-2.1.5/locscale/include/symmetry_emda/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/symmetry_emda/apply_rotation_matrix.py` & `locscale-2.1.5/locscale/include/symmetry_emda/apply_rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/symmetry_emda/fcodes_fast.f90` & `locscale-2.1.5/locscale/include/symmetry_emda/fcodes_fast.f90`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/include/symmetry_emda/symmetrize_map.py` & `locscale-2.1.5/locscale/include/symmetry_emda/symmetrize_map.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/main.py` & `locscale-2.1.5/locscale/main.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/preprocessing/__init__.py` & `locscale-2.1.5/locscale/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/preprocessing/headers.py` & `locscale-2.1.5/locscale/preprocessing/headers.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/preprocessing/pipeline.py` & `locscale-2.1.5/locscale/preprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/preprocessing/pseudomodel_classes.py` & `locscale-2.1.5/locscale/preprocessing/pseudomodel_classes.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/preprocessing/pseudomodel_solvers.py` & `locscale-2.1.5/locscale/preprocessing/pseudomodel_solvers.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/tests/__init__.py` & `locscale-2.1.5/locscale/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/tests/locscale_modules.py` & `locscale-2.1.5/locscale/tests/locscale_modules.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/tests/test_emmernet.py` & `locscale-2.1.5/locscale/tests/test_emmernet.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/tests/test_locscale.py` & `locscale-2.1.5/locscale/tests/test_locscale.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/tests/test_symmetry.py` & `locscale-2.1.5/locscale/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/tests/utils.py` & `locscale-2.1.5/locscale/tests/utils.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/__init__.py` & `locscale-2.1.5/locscale/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/file_tools.py` & `locscale-2.1.5/locscale/utils/file_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/general.py` & `locscale-2.1.5/locscale/utils/general.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/map_quality.py` & `locscale-2.1.5/locscale/utils/map_quality.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/math_tools.py` & `locscale-2.1.5/locscale/utils/math_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/parse_utils.py` & `locscale-2.1.5/locscale/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/plot_tools.py` & `locscale-2.1.5/locscale/utils/plot_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/prepare_inputs.py` & `locscale-2.1.5/locscale/utils/prepare_inputs.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/scaling_tools.py` & `locscale-2.1.5/locscale/utils/scaling_tools.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/startup_utils.py` & `locscale-2.1.5/locscale/utils/startup_utils.py`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale/utils/theoretical_profiles.pickle` & `locscale-2.1.5/locscale/utils/theoretical_profiles.pickle`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/locscale.egg-info/PKG-INFO` & `locscale-2.1.5/locscale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locscale
-Version: 2.1.4b0
+Version: 2.1.5
 Summary: Contrast optimization for cryo-EM maps
 Home-page: https://gitlab.tudelft.nl/aj-lab/locscale
 Author: Alok Bharadwaj, Arjen J. Jakobi, Reinier de Bruin
 License: 3-clause BSD
 Project-URL: Bug Tracker, https://gitlab.tudelft.nl/aj-lab/locscale/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `locscale-2.1.4b0/locscale.egg-info/SOURCES.txt` & `locscale-2.1.5/locscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locscale-2.1.4b0/setup.py` & `locscale-2.1.5/setup.py`

 * *Files identical despite different names*

