# Comparing `tmp/cctk-v0.1.4.tar.gz` & `tmp/cctk-v0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cctk-v0.1.4.tar", last modified: Fri Mar 27 18:28:55 2020, max compression
+gzip compressed data, was "dist/cctk-v0.1.5.tar", last modified: Thu Apr  9 12:00:13 2020, max compression
```

## Comparing `cctk-v0.1.4.tar` & `cctk-v0.1.5.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/
--rw-r--r--   0 cwagen     (501) staff       (20)     5843 2020-03-27 18:28:55.000000 cctk-v0.1.4/PKG-INFO
--rw-r--r--   0 cwagen     (501) staff       (20)     4290 2020-03-27 18:03:57.000000 cctk-v0.1.4/README.md
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/cctk/
--rw-r--r--   0 cwagen     (501) staff       (20)      373 2020-03-27 01:13:44.000000 cctk-v0.1.4/cctk/__init__.py
--rw-r--r--   0 cwagen     (501) staff       (20)     3951 2020-03-27 18:05:33.000000 cctk-v0.1.4/cctk/array.py
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/cctk/data/
--rw-r--r--   0 cwagen     (501) staff       (20)        0 2019-12-02 21:46:22.000000 cctk-v0.1.4/cctk/data/__init__.py
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/cctk/data/__pycache__/
--rw-r--r--   0 cwagen     (501) staff       (20)      111 2019-12-03 01:10:12.000000 cctk-v0.1.4/cctk/data/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 cwagen     (501) staff       (20)      136 2020-01-16 12:15:13.000000 cctk-v0.1.4/cctk/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 cwagen     (501) staff       (20)     1615 2019-12-02 21:46:22.000000 cctk-v0.1.4/cctk/data/covalent_radii.csv
--rw-r--r--   0 cwagen     (501) staff       (20)     9062 2019-12-02 21:46:22.000000 cctk-v0.1.4/cctk/data/isotopes.csv
--rw-r--r--   0 cwagen     (501) staff       (20)    15207 2020-03-27 18:05:52.000000 cctk-v0.1.4/cctk/ensemble.py
--rw-r--r--   0 cwagen     (501) staff       (20)     2493 2020-03-17 03:23:02.000000 cctk-v0.1.4/cctk/file.py
--rw-r--r--   0 cwagen     (501) staff       (20)    17635 2020-03-27 18:18:40.000000 cctk-v0.1.4/cctk/gaussian_file.py
--rw-r--r--   0 cwagen     (501) staff       (20)     6754 2020-03-20 17:44:46.000000 cctk-v0.1.4/cctk/group.py
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/cctk/groups/
--rw-r--r--   0 cwagen     (501) staff       (20)      465 2020-03-17 21:28:45.000000 cctk-v0.1.4/cctk/groups/AcH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      227 2020-03-17 21:25:38.000000 cctk-v0.1.4/cctk/groups/BrH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      369 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/CF3H.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      321 2020-03-17 21:28:29.000000 cctk-v0.1.4/cctk/groups/CHOH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      227 2020-03-17 21:25:23.000000 cctk-v0.1.4/cctk/groups/ClH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      513 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/EtH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      217 2020-03-17 21:25:13.000000 cctk-v0.1.4/cctk/groups/FH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      273 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/HCN.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      505 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/HCO2Me.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      323 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/HNO2.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      225 2020-03-17 21:25:54.000000 cctk-v0.1.4/cctk/groups/IH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      361 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/MeH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      321 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/NH3.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      562 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/NHAcH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      613 2020-03-18 16:14:43.000000 cctk-v0.1.4/cctk/groups/NMe2H.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      273 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/OH2.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      417 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/OMeH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      465 2020-03-17 21:26:46.000000 cctk-v0.1.4/cctk/groups/SF5H.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      417 2020-03-17 21:27:31.000000 cctk-v0.1.4/cctk/groups/SO3HH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)        0 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/__init__.py
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/cctk/groups/__pycache__/
--rw-r--r--   0 cwagen     (501) staff       (20)      134 2020-02-09 17:55:43.000000 cctk-v0.1.4/cctk/groups/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 cwagen     (501) staff       (20)      666 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/iPrH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)      825 2019-12-26 16:38:30.000000 cctk-v0.1.4/cctk/groups/tBuH.mol2
--rw-r--r--   0 cwagen     (501) staff       (20)     8371 2020-03-27 18:07:42.000000 cctk-v0.1.4/cctk/helper_functions.py
--rw-r--r--   0 cwagen     (501) staff       (20)     1727 2020-03-18 15:29:47.000000 cctk-v0.1.4/cctk/load_groups.py
--rw-r--r--   0 cwagen     (501) staff       (20)    11228 2020-03-27 18:08:04.000000 cctk-v0.1.4/cctk/mae_file.py
--rw-r--r--   0 cwagen     (501) staff       (20)    13524 2020-03-27 18:08:49.000000 cctk-v0.1.4/cctk/mol2_file.py
--rw-r--r--   0 cwagen     (501) staff       (20)    42165 2020-03-27 18:09:06.000000 cctk-v0.1.4/cctk/molecule.py
--rw-r--r--   0 cwagen     (501) staff       (20)     3537 2020-03-27 18:09:12.000000 cctk-v0.1.4/cctk/orca_file.py
--rw-r--r--   0 cwagen     (501) staff       (20)    11635 2020-03-27 18:09:18.000000 cctk-v0.1.4/cctk/parse_gaussian.py
--rw-r--r--   0 cwagen     (501) staff       (20)     1841 2020-03-27 18:09:26.000000 cctk-v0.1.4/cctk/pdb_file.py
--rw-r--r--   0 cwagen     (501) staff       (20)     2684 2020-03-27 18:09:32.000000 cctk-v0.1.4/cctk/xyz_file.py
--rw-r--r--   0 cwagen     (501) staff       (20)       40 2020-01-30 17:46:04.000000 cctk-v0.1.4/setup.cfg
--rw-r--r--   0 cwagen     (501) staff       (20)     1115 2020-03-27 18:28:24.000000 cctk-v0.1.4/setup.py
-drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-03-27 18:28:55.000000 cctk-v0.1.4/test/
--rw-r--r--   0 cwagen     (501) staff       (20)     8886 2020-03-27 00:15:12.000000 cctk-v0.1.4/test/test_core.py
--rw-r--r--   0 cwagen     (501) staff       (20)     2598 2020-03-27 15:41:33.000000 cctk-v0.1.4/test/test_gaussian.py
--rw-r--r--   0 cwagen     (501) staff       (20)      738 2020-03-27 11:51:48.000000 cctk-v0.1.4/test/test_helper.py
--rw-r--r--   0 cwagen     (501) staff       (20)     2077 2020-03-20 11:13:54.000000 cctk-v0.1.4/test/test_indexing.py
--rw-r--r--   0 cwagen     (501) staff       (20)     5184 2020-03-27 16:50:50.000000 cctk-v0.1.4/test/test_molecule.py
--rw-r--r--   0 cwagen     (501) staff       (20)     3030 2020-03-27 18:03:57.000000 cctk-v0.1.4/test/test_nmr.py
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/
+-rw-r--r--   0 cwagen     (501) staff       (20)     5843 2020-04-09 12:00:13.000000 cctk-v0.1.5/PKG-INFO
+-rw-r--r--   0 cwagen     (501) staff       (20)     4290 2020-03-27 18:03:57.000000 cctk-v0.1.5/README.md
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/cctk/
+-rw-r--r--   0 cwagen     (501) staff       (20)      373 2020-03-27 01:13:44.000000 cctk-v0.1.5/cctk/__init__.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     5141 2020-04-03 11:34:50.000000 cctk-v0.1.5/cctk/array.py
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/cctk/data/
+-rw-r--r--   0 cwagen     (501) staff       (20)        0 2019-12-02 21:46:22.000000 cctk-v0.1.5/cctk/data/__init__.py
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/cctk/data/__pycache__/
+-rw-r--r--   0 cwagen     (501) staff       (20)      111 2019-12-03 01:10:12.000000 cctk-v0.1.5/cctk/data/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 cwagen     (501) staff       (20)      136 2020-01-16 12:15:13.000000 cctk-v0.1.5/cctk/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 cwagen     (501) staff       (20)     1615 2019-12-02 21:46:22.000000 cctk-v0.1.5/cctk/data/covalent_radii.csv
+-rw-r--r--   0 cwagen     (501) staff       (20)     9062 2019-12-02 21:46:22.000000 cctk-v0.1.5/cctk/data/isotopes.csv
+-rw-r--r--   0 cwagen     (501) staff       (20)    17284 2020-04-09 11:37:03.000000 cctk-v0.1.5/cctk/ensemble.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     2493 2020-03-17 03:23:02.000000 cctk-v0.1.5/cctk/file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)    23645 2020-04-09 11:35:14.000000 cctk-v0.1.5/cctk/gaussian_file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     6754 2020-03-20 17:44:46.000000 cctk-v0.1.5/cctk/group.py
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/cctk/groups/
+-rw-r--r--   0 cwagen     (501) staff       (20)      465 2020-03-17 21:28:45.000000 cctk-v0.1.5/cctk/groups/AcH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      227 2020-03-17 21:25:38.000000 cctk-v0.1.5/cctk/groups/BrH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      369 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/CF3H.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      321 2020-03-17 21:28:29.000000 cctk-v0.1.5/cctk/groups/CHOH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      227 2020-03-17 21:25:23.000000 cctk-v0.1.5/cctk/groups/ClH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      513 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/EtH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      217 2020-03-17 21:25:13.000000 cctk-v0.1.5/cctk/groups/FH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      273 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/HCN.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      505 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/HCO2Me.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      323 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/HNO2.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      225 2020-03-17 21:25:54.000000 cctk-v0.1.5/cctk/groups/IH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      361 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/MeH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      321 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/NH3.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      562 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/NHAcH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      613 2020-03-18 16:14:43.000000 cctk-v0.1.5/cctk/groups/NMe2H.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      273 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/OH2.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      417 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/OMeH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      465 2020-03-17 21:26:46.000000 cctk-v0.1.5/cctk/groups/SF5H.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      417 2020-03-17 21:27:31.000000 cctk-v0.1.5/cctk/groups/SO3HH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)        0 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/__init__.py
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/cctk/groups/__pycache__/
+-rw-r--r--   0 cwagen     (501) staff       (20)      134 2020-02-09 17:55:43.000000 cctk-v0.1.5/cctk/groups/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 cwagen     (501) staff       (20)      666 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/iPrH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)      825 2019-12-26 16:38:30.000000 cctk-v0.1.5/cctk/groups/tBuH.mol2
+-rw-r--r--   0 cwagen     (501) staff       (20)    19368 2020-04-08 19:58:45.000000 cctk-v0.1.5/cctk/helper_functions.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     1727 2020-03-18 15:29:47.000000 cctk-v0.1.5/cctk/load_groups.py
+-rw-r--r--   0 cwagen     (501) staff       (20)    11129 2020-04-09 11:16:48.000000 cctk-v0.1.5/cctk/mae_file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)    13415 2020-04-09 11:24:13.000000 cctk-v0.1.5/cctk/mol2_file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)    42387 2020-04-05 17:35:38.000000 cctk-v0.1.5/cctk/molecule.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     3537 2020-03-27 18:09:12.000000 cctk-v0.1.5/cctk/orca_file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)    14223 2020-04-09 11:36:35.000000 cctk-v0.1.5/cctk/parse_gaussian.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     1843 2020-04-09 11:30:46.000000 cctk-v0.1.5/cctk/pdb_file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     2684 2020-03-27 18:09:32.000000 cctk-v0.1.5/cctk/xyz_file.py
+-rw-r--r--   0 cwagen     (501) staff       (20)       40 2020-01-30 17:46:04.000000 cctk-v0.1.5/setup.cfg
+-rw-r--r--   0 cwagen     (501) staff       (20)     1115 2020-04-09 11:59:30.000000 cctk-v0.1.5/setup.py
+drwxr-xr-x   0 cwagen     (501) staff       (20)        0 2020-04-09 12:00:13.000000 cctk-v0.1.5/test/
+-rw-r--r--   0 cwagen     (501) staff       (20)     1763 2020-04-06 11:55:07.000000 cctk-v0.1.5/test/test_align.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     4971 2020-04-09 11:28:22.000000 cctk-v0.1.5/test/test_core.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     4454 2020-04-06 14:45:14.000000 cctk-v0.1.5/test/test_ensemble.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     4317 2020-04-09 11:36:09.000000 cctk-v0.1.5/test/test_gaussian.py
+-rw-r--r--   0 cwagen     (501) staff       (20)      858 2020-04-05 20:18:09.000000 cctk-v0.1.5/test/test_group.py
+-rw-r--r--   0 cwagen     (501) staff       (20)      953 2020-04-05 21:04:22.000000 cctk-v0.1.5/test/test_helper.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     2263 2020-04-03 15:44:46.000000 cctk-v0.1.5/test/test_indexing.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     5184 2020-03-27 16:50:50.000000 cctk-v0.1.5/test/test_molecule.py
+-rw-r--r--   0 cwagen     (501) staff       (20)     4655 2020-04-08 19:58:45.000000 cctk-v0.1.5/test/test_nmr.py
```

### Comparing `cctk-v0.1.4/PKG-INFO` & `cctk-v0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: cctk
-Version: v0.1.4
+Version: v0.1.5
 Summary: computational chemistry toolkit
 Home-page: https://github.com/ekwan/cctk
 Author: Corin Wagen and Eugene Kwan
 Author-email: corin.wagen@gmail.com
 License: Apache 2.O
-Download-URL: https://github.com/ekwan/cctk/archive/v0.1.3.tar.gz
+Download-URL: https://github.com/ekwan/cctk/archive/v0.1.5.tar.gz
 Description: 
         # cctk
         ## computational chemistry toolkit
         
         *A Python 3-based library for working with computational chemistry data*.
         
         [![PyPI version](https://badge.fury.io/py/cctk.svg)](https://badge.fury.io/py/cctk)
```

### Comparing `cctk-v0.1.4/README.md` & `cctk-v0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/array.py` & `cctk-v0.1.5/cctk/array.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,17 +41,31 @@
                 return super().__getitem__(index)
             elif index.ndim == 1:
                 index[index >= 1] += -1
                 return super().__getitem__(index)
             else:
                 index[0][index >= 1] += -1
                 return super().__getitem__(index)
+        elif isinstance(index, list):
+            if isinstance(index[0], bool):
+                return super().__getitem__(index)
+            elif isinstance(index[0], list):
+                if isinstance(index[0][0], bool):
+                    return super().__getitem__(index)
+                for i, v in enumerate(index[0]):
+                    if v >= 1:
+                        index[i] += -1
+                return super().__getitem__(index)
+            else:
+                for i, v in enumerate(index):
+                    if v >= 1:
+                        index[i] += -1
+                return super().__getitem__(index)
         else:
             return super().__getitem__(index)
-#            raise IndexError(f"invalid index {index} for OneIndexedArray")
 
     def __setitem__(self, index, value):
         index = copy.deepcopy(index)
         if isinstance(index, int):
             if index > 0:
                 if self.ndim == 1:
                     super().__setitem__(index-1, value)
@@ -79,14 +93,29 @@
                 super().__setitem__(index, value)
             elif index.ndim == 1:
                 index[index >= 1] += -1
                 super().__setitem__(index, value)
             else:
                 index[0][index >= 1] += -1
                 super().__setitem__(index, value)
+        elif isinstance(index, list):
+            if isinstance(index[0], bool):
+                super().__setitem__(index, value)
+            elif isinstance(index[0], list):
+                if isinstance(index[0][0], bool):
+                    super().__setitem__(index, value)
+                for i, v in enumerate(index[0]):
+                    if v >= 1:
+                        index[i] += -1
+                super().__setitem__(index, value)
+            else:
+                for i, v in enumerate(index):
+                    if v >= 1:
+                        index[i] += -1
+                super().__setitem__(index, value)
         else:
             super().__setitem__(index, value)
 #            raise IndexError(f"invalid index {index} for OneIndexedArray")
 
     def __iter__(self):
         for idx in range(1,len(self)+1):
             yield self.__getitem__(idx)
```

### Comparing `cctk-v0.1.4/cctk/data/covalent_radii.csv` & `cctk-v0.1.5/cctk/data/covalent_radii.csv`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/data/isotopes.csv` & `cctk-v0.1.5/cctk/data/isotopes.csv`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/ensemble.py` & `cctk-v0.1.5/cctk/ensemble.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,142 +1,198 @@
 import sys
 import re
 import numpy as np
 import copy
 
+import cctk
 from cctk import Molecule
-from cctk.helper_functions import align_matrices, compute_RMSD
+from cctk.helper_functions import align_matrices
 
 
 class Ensemble:
     """
     Class that represents a group of molecules. They do not all need to have the same atoms or bonds.
 
-    Calling ``ensemble[x]`` is shorthand for calling ``ensemble.molecules[x]``.
+    Ensembles are composed of molecules and properties. Molecules are ``Molecule`` objects, whereas properties are ``dict`` objects containing calculation-specific information.
+
+    There are various shortcuts for handling ``Ensemble`` objects:
+    - ``Ensemble`` can be treated like a list of ``Molecule`` objects, so ``ensemble[0]`` will return the first molecule, ``len(ensemble)`` the number of molecules, and so forth.
+    - ``Ensemble`` can also return the corresponding properties, when passed a molecule: so ``ensemble[molecule]`` will return the corresponding properties dictionary.
+    - ``Ensemble`` can also take tuples, allowing for dataframe-like behavior: so ``ensemble[1:3, "energy"]`` will return the energies of molecules 2-4.
 
     Attributes:
         name (str): name, for identification
-        molecules (np.ndarray): list of `Molecule` objects
-        energies (np.ndarray): list of energies
+        _items (dict):
+            keys: ``Molecule`` objects
+            values: dictionaries containing properties from each molecule, variable. should always be one layer deep.
     """
 
-    def __init__(self, name=None, **kwargs):
+    def __init__(self, name=None):
         """
-        Create new instance, and optionally create a bunch of molecules too.
+        Create new instance.
 
         Args:
             name (str): name of Ensemble
-            **kwargs: to pass to ``self.batch_add()``
         """
         self.name = name
-        self.molecules = np.array([])
-        self.energies = np.array([])
+        self._items = {}
 
-        if all(arg in kwargs for arg in ["atomic_numbers", "geometries"]):
-            self.batch_add(**kwargs)
+    def __str__(self):
+        name = "None" if self.name is None else self.name
+        return f"Ensemble (name={name}, {len(_items)} molecules)"
 
     def __getitem__(self, key):
-        return self.molecules[key]
+        if isinstance(key, Molecule):
+            return self._items[key]
+        elif isinstance(key, int):
+            return list(self._items)[key]
+        elif isinstance(key, list):
+            return [self[k] for k in key]
+        elif isinstance(key, slice):
+            start, stop, step = key.indices(len(self))
+            return [self[i] for i in range(start, stop, step)]
+        elif isinstance(key, tuple):
+            (key1, key2) = key
+            mols = self[key1]
+            if isinstance(key1, list):
+                if all(isinstance(k, Molecule) for k in key1):
+                    mols = key1
+            elif isinstance(key1, Molecule):
+                mols = key1
+            if key2 is None:
+                return mols
+            else:
+                try:
+                    if isinstance(mols, list):
+                        return [self[mol][key2] for mol in mols]
+                    else:
+                        return self[mols][key2]
+                except KeyError as e:
+                    raise KeyError(f"property {key2} not defined for all molecules!")
+        else:
+            raise KeyError(f"not a valid datatype for Ensemble key: {type(key)}")
 
     def __setitem__(self, key, item):
-        self.molecules[key] = item
+        if isinstance(key, Molecule):
+            assert isinstance(item, dict), "properties must be dict"
+            self._items[key] = item
+        elif isinstance(key, int):
+            assert isinstance(item, Molecule), "can't add something that isn't a molecule to keys of ensemble!"
+            list(self._items)[key] = item
+        elif isinstance(key, list):
+            assert len(item) == len(key), "wrong number of items to assign to list index!"
+            for k, i in zip(key, item):
+                self[k] = i
+        elif isinstance(key, slice):
+            start, stop, step = key.indices(len(self))
+            assert len(item) == len(range(start, stop, step)), "wrong number of items to assign to slice index!"
+            for i in range(start, stop, step):
+                self[i] = item[i]
+        elif isinstance(key, tuple):
+            (key1, key2) = key
+            mols = self[key1]
+            if isinstance(key1, list):
+                if all(isinstance(k, Molecule) for k in key1):
+                    mols = key1
+            elif isinstance(key1, Molecule):
+                mols = key1
+            if isinstance(mols, list):
+                assert len(item) == len(mols), "wrong number of items to assign to tuple index"
+                for m, i in zip(mols, item):
+                    self[m][key2] = i
+            else:
+                self[mols][key2] = item
+        else:
+            raise KeyError(f"not a valid datatype for Ensemble key: {type(key)}")
 
     def __len__(self):
-        return len(self.molecules)
-
-    def batch_add(self, atomic_numbers, geometries, bonds=None, charges=None, multiplicities=None):
-        """
-        Automatically generates ``Molecule`` objects and adds them using ``self.add_molecule()``.
-
-        Args:
-            atomic_numbers (list): list of lists of atomic numbers.
-            geometry (list): list of 3-tuples of xyz coordinates
-            bonds (list): list of edges (i.e. an n x 2 ``numpy`` array).
-            charges (int): list of molecular charges - will default to 0 for all molecules.
-            multiplicities (int): list of multiplicities - will default to 1 (singlet) for all molecules.
-        """
-        if (atomic_numbers is None) or (geometries is None):
-            return
+        return len(self._items)
 
-        if charges is None:
-            charges = list(np.zeros(shape=len(atomic_numbers)))
+    def __iter__(self):
+        return iter(self.items())
 
-        if multiplicities is None:
-            multiplicities = list(np.ones(shape=len(atomic_numbers)))
+    def keys(self):
+        return self._items.keys()
 
-        if (bonds is None) or len(bonds) == 0:
-            bonds = [None] * len(atomic_numbers)
+    def values(self):
+        return self._items.values()
 
-        n_atoms = len(atomic_numbers)
-        n_geometries = len(geometries)
-        n_bonds = len(bonds)
-        n_charges = len(charges)
-        n_multiplicities = len(multiplicities)
+    def has_property(self, idx, prop):
+        """
+        Returns ``True`` if property is defined for index ``idx`` and ``False`` otherwise.
+        """
+        if prop in list(self._items[self[idx]].keys()):
+            return True
+        else:
+            return False
 
-        assert n_atoms == n_geometries, f"there are {n_atoms} atomic number lists, but {n_geometries} geometry lists"
-        assert n_atoms == n_bonds, f"there are {n_atoms} atomic number lists, but found {n_bonds} bond lists"
-        assert n_atoms == n_charges, f"there are {n_atoms} atomic number lists, but found {n_charges} charge lists"
-        assert n_atoms == n_multiplicities, f"there are {n_atoms} atomic number lists, but found {n_multiplicities} multiplicity lists"
+    def items(self):
+        """
+        Returns a list of (molecule, properties) tuple pairs.
+        """
+        return self._items.items()
 
-        for numbers, geometry, bond_edges, charge, multiplicity in zip(atomic_numbers, geometries, bonds, charges, multiplicities):
-            if len(numbers) != len(geometry):
-                raise TypeError(f"expected {len(numbers)} atoms but found {len(geometry)}")
+    def molecules(self):
+        """
+        Returns a list of the constituent molecules.
+        """
+        return list(self.keys())
 
-            mol = Molecule(numbers, geometry, bonds=bond_edges, charge=charge, multiplicity=multiplicity)
-            self.add_molecule(mol)
+    def properties(self):
+        """
+        Returns a list of the constituent properties.
+        """
+        return list(self.values())
 
-    def add_molecule(self, molecule, energy=None):
+    def add_molecule(self, molecule, properties={}, copy=False):
         """
-        Adds a molecule to the ensemble. ``copy.deepcopy`` is used so that an independent copy of the molecule is saved.
+        Adds a molecule to the ensemble.
 
         Args:
             molecule (Molecule): the molecule to be added
+            properties (dict): property name (str) to property value
+            copy (bool): whether to store an independent copy of the molecule
         """
         if not isinstance(molecule, Molecule):
             raise TypeError("molecule is not a Molecule - so it can't be added!")
+        assert isinstance(properties, dict), "properties must be a dict"
 
-        self.molecules = np.append(self.molecules, [copy.deepcopy(molecule)])
-        self.energies = np.append(self.energies, [energy])
+        if copy:
+            molecule = copy.deepcopy(molecule)
+        self._items[molecule] = properties
 
     def _check_molecule_number(self, number):
         """
         Helper method which performs quick checks on the validity of a given molecule number.
         """
         try:
             number = int(number)
         except:
             raise TypeError(f"atom number {number} must be integer")
 
-        if number >= len(self.molecules):
+        if number >= len(self._items):
             raise ValueError(f"atom number {number} too large!")
 
     @classmethod
     def join_ensembles(cls, ensembles, name=None):
         """
         Creates a new Ensemble object from existing ensembles.
 
         If every ensemble has energies defined, then the new ensemble will have energies defined too.
 
         Args:
             name (str): name of Ensemble created
             ensembles (list of Ensembles): Ensemble objects to join
         """
         new_ensemble = Ensemble(name=name)
-        use_energies = True
         for ensemble in ensembles:
             assert isinstance(ensemble, Ensemble), "can't join an object that isn't an Ensemble!"
-            if len(ensemble.energies) != len(ensemble.molecules):
-                use_energies = False
 
         for ensemble in ensembles:
-            for idx, mol in np.ndenumerate(ensemble.molecules):
-                if use_energies:
-                    new_ensemble.add_molecule(mol, energy=ensemble.energies[idx])
-                else:
-                    new_ensemble.add_molecule(mol)
+            new_ensemble._items.update(ensemble.items)
 
         return new_ensemble
 
 
 class ConformationalEnsemble(Ensemble):
     """
     Class that represents a group of conformers. All members must have the same atom types in the same order.
@@ -144,133 +200,136 @@
     Allows you to align and remove redundant molecules, unlike ``Ensemble``.
 
     Attributes:
         name (str): name, for identification
         molecules (list): list of `Molecule` objects
     """
 
-    def batch_add(self, atomic_numbers=None, geometries=None, bonds=None, charge=0, multiplicity=1):
-        """
-        Automatically generates ``Molecule`` objects and adds them.
-
-        Takes only a single molecule's value for ``charge``/``multiplicity``/``atomic_numbers``/``bonds``, not a list of lists like ``Ensemble.__init__()``.
-
-        Args:
-            atomic_numbers (list): list of atomic numbers.
-            geometry (np.ndarray): list of 3-tuples of xyz coordinates
-            bonds (list): list of edges (i.e. an n x 2 `numpy` array).
-            charge (int): molecular charge - will default to 0 for all molecules.
-            multiplicity (int): spin multiplicity - will default to 1 (singlet) for all molecules.
-        """
-        if (atomic_numbers is None) or (geometries is None):
-            return
-
-        assert all(len(g) == len(geometries[0]) for g in geometries), "not all geometries match; can't make ConformationalEnsemble!"
-
-        for g in geometries:
-            mol = Molecule(atomic_numbers, g, bonds=bonds, charge=charge, multiplicity=multiplicity)
-            self.add_molecule(mol)
+    def __str__(self):
+        n_atoms = 0
+        if len(self._items) > 0:
+            first_molecule = self[0]
+            n_atoms = first_molecule.num_atoms()
+        if self.name is not None:
+            return f"ConformationalEnsemble (name={self.name}, {len(self._items)} molecules, {n_atoms} atoms)"
+        else:
+            return f"ConformationalEnsemble ({len(self._items)} molecules, {n_atoms} atoms)"
 
-    def add_molecule(self, molecule, energy=None):
+    def add_molecule(self, molecule, properties={}, copy=False):
         """
         Checks that the molecule contains the same atom types in the same order as existing molecules, and that the molecule has the same charge/multiplicity.
         """
-        if len(self.molecules) > 0:
-            if molecule.num_atoms() != self.molecules[0].num_atoms():
+        if len(self._items) > 0:
+            if molecule.num_atoms() != self[0].num_atoms():
                 raise ValueError("wrong number of atoms for this ensemble")
 
-            if molecule.charge != self.molecules[0].charge:
+            if molecule.charge != self[0].charge:
                 raise ValueError("wrong charge for this ensemble")
 
-            if molecule.multiplicity != self.molecules[0].multiplicity:
+            if molecule.multiplicity != self[0].multiplicity:
                 raise ValueError("wrong spin multiplicity for this ensemble")
 
-            if not np.array_equal(molecule.atomic_numbers, self.molecules[0].atomic_numbers):
+            if not np.array_equal(molecule.atomic_numbers, self[0].atomic_numbers):
                 raise ValueError("wrong atom types for this ensemble")
 
-        super().add_molecule(molecule, energy=energy)
+            #### only save one copy to save space
+            molecule.bonds = self[0].bonds
+            molecule.atomic_numbers = self[0].atomic_numbers
+
+        super().add_molecule(molecule, properties, copy)
 
     @classmethod
-    def join_ensembles(cls, ensembles, name=None):
+    def join_ensembles(cls, ensembles, name=None, copy=False):
         """
         Creates a new ConformationalEnsemble object from existing ensembles.
-
-        If every ensemble has energies defined, then the new ensemble will have energies defined too.
+        Both molecules and properties are copied.
 
         Args:
             name (str): name of ConformationalEnsemble created
             ensembles (list of ConformationalEnsembles): ConformationalEnsemble objects to join
+            copy (bool): whether to make copies of the component molecules
         """
         new_ensemble = ConformationalEnsemble(name=name)
-        use_energies = True
         for ensemble in ensembles:
-            assert isinstance(ensemble, ConformationalEnsemble), "can't join an object that isn't an ConformationalEnsemble!"
-            if len(ensemble.energies) != len(ensemble.molecules):
-                use_energies = False
+            assert isinstance(ensemble, ConformationalEnsemble), "can't join an object that isn't a ConformationalEnsemble!"
 
         for ensemble in ensembles:
-            for idx, mol in np.ndenumerate(ensemble.molecules):
-                if use_energies:
-                    new_ensemble.add_molecule(mol, energy=ensemble.energies[idx])
-                else:
-                    new_ensemble.add_molecule(mol)
+            for mol, prop in ensemble.items():
+                    new_ensemble.add_molecule(mol, prop, copy)
 
         return new_ensemble
 
-    def align(self, align_to=0, atoms=None, return_rmsd=False):
+    def align(self, to_geometry=0, comparison_atoms="heavy", compute_RMSD=False):
         """
-        Aligns every geometry to the specified geometry based on the atoms in `atom_numbers`. If `atom_numbers` is `None`, then a full alignment is performed.
+        Aligns every geometry in this ensemble to the specified geometry,
+        optionally computing the root-mean-square distance between each
+        geometry and the reference geometry.
 
         Args:
-            align_to (int): which geometry to align to (0-indexed)
-            atoms (list): which atoms to align in each molecule (1-indexed; must be at least 3)
-                alternatively, specify ``None`` for all atoms or "heavy" for all heavy atoms
-            return_rmsd (Bool): whether to return RMSD before and after rotation
+            to_geometry (int): the reference geometry to align to (0-indexed)
+            comparison_atoms (str or list): which atoms to use when computing alignments
+                                            "heavy" for all non-hydrogen atoms,
+                                            "all" for all atoms, or
+                                            a list of 1-indexed atom numbers
+            compute_RMSD (Bool): whether to return RMSD before and after rotation
+
+        Aligns every geometry to the specified geometry based on the atoms in `atom_numbers`.
+        If `atom_numbers` is `None`, then a full alignment is performed.
+        The original ensemble will not be altered.  RMSDs will be calculated over the
+        comparison atoms only.
 
         Returns:
-            a new ``Ensemble()`` object with the objects aligned
-            (optional) before rmsd and after rmsd
+            new aligned ``ConformationalEnsemble`` or
+            new aligned ``ConformationalEnsemble``, before_RMSD array, after_RMSD array
         """
-        self._check_molecule_number(align_to)
+        # check inputs
+        self._check_molecule_number(to_geometry)
+        n_atoms = self[0].num_atoms()
+
+        if isinstance(comparison_atoms, str):
+            if comparison_atoms == "all":
+                comparison_atoms = np.arange(1, n_atoms + 1)
+            elif comparison_atoms == "heavy":
+                comparison_atoms = self[0].get_heavy_atoms()
 
-        if atoms is None:
-            atoms = np.arange(1, self.molecules[0].num_atoms() + 1)
-        elif isinstance(atoms, str) and (atoms == "heavy"):
-            atoms = self.molecules[0].get_heavy_atoms()
-        else:
-            try:
-                atoms = np.array(atoms)
-                if len(atoms) < 3:
-                    raise ValueError("not enough atoms for alignment - need 3 in 3D space!")
-
-            except:
-                raise ValueError("atom numbers is not a recognized keyword and cannot be cast to numpy array... try again!")
-
-        #### move everything to the center!
-        for molecule in self.molecules:
-            molecule.center()
-
-        template = self.molecules[align_to].geometry[atoms]
-        before_rmsd = 0
-        after_rmsd = 0
+        assert len(comparison_atoms) >= 3, f"need at least 3 atoms for alignment, but only got {len(comparison_atoms)}"
 
-        #### perform alignment using Kabsch algorithm
+        # duplicate the ensemble
         new_ensemble = copy.deepcopy(self)
-        for molecule in new_ensemble.molecules:
-            before_rmsd += compute_RMSD(template, molecule.geometry[atoms])
-            new_geometry = align_matrices(molecule.geometry[atoms], molecule.geometry, template)
-            molecule.geometry = new_geometry
-            after_rmsd += compute_RMSD(template, molecule.geometry[atoms])
 
-            assert len(molecule.geometry) == len(molecule.atomic_numbers), "wrong number of geometry elements!"
+        # translate all molecules to the origin
+        # with respect to the comparison atoms
+        for molecule, _ in new_ensemble:
+            full_geometry = molecule.geometry
+            partial_geometry = full_geometry[comparison_atoms]
+            translation_vector = -partial_geometry.mean(axis=0)
+            molecule.translate_molecule(translation_vector)
+
+        full_template_geometry = new_ensemble[to_geometry].geometry
+        partial_template_geometry = full_template_geometry[comparison_atoms]
+        before_RMSDs = []
+        after_RMSDs = []
+
+        # perform alignment using Kabsch algorithm
+        for i, (molecule, _) in enumerate(new_ensemble):
+            full_geometry = molecule.geometry
+            partial_geometry = full_geometry[comparison_atoms]
+            if compute_RMSD:
+                before_RMSD = cctk.helper_functions.compute_RMSD(partial_template_geometry, partial_geometry)
+                before_RMSDs.append(before_RMSD)
+            new_geometry = align_matrices(partial_geometry, full_geometry, partial_template_geometry)
+            molecule.geometry = new_geometry
+            if compute_RMSD:
+                after_RMSD = cctk.helper_functions.compute_RMSD(new_ensemble[0], new_ensemble[i], comparison_atoms)
+                after_RMSDs.append(after_RMSD)
+            assert len(molecule.geometry) == n_atoms, f"wrong number of geometry elements! expected {n_atoms}, got {len(molecule.geometry)}"
 
-        if return_rmsd:
-            return new_ensemble, before_rmsd, after_rmsd
-        else:
-            return new_ensemble
+        if compute_RMSD:
+            return new_ensemble, before_RMSDs, after_RMSDs
+        return new_ensemble
 
     def eliminate_redundant(self, cutoff=0.5, heavy_only=True, atom_numbers=None):
         """
         Returns non-redundant conformations. When redundancies are found, only the first geometry is kept.
         This will change the numbering of all the ensembles!
 
         Args:
```

### Comparing `cctk-v0.1.4/cctk/file.py` & `cctk-v0.1.5/cctk/file.py`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/gaussian_file.py` & `cctk-v0.1.5/cctk/gaussian_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,93 +10,95 @@
 
 
 class JobType(Enum):
     """
     Class to contain allowed Gaussian job types. Not an exhaustive list, but should be fairly comprehensive.
 
     The value should be the Gaussian keyword, to permit automatic assignment.
+
+    All jobs have type ``SP`` by default.
     """
 
     SP = "sp"
     OPT = "opt"
     FREQ = "freq"
     IRC = "irc"
     NMR = "nmr"
     POP = "pop"
     FORCE = "force"
 
+#### This static variable tells what properties are expected from each JobType.
+EXPECTED_PROPERTIES = {
+    "sp": ["energy", "scf_iterations",],
+    "opt": ["rms_displacement", "rms_force", ],
+    "freq": ["gibbs_free_energy", "enthalpy", "frequencies",],
+    "nmr": ["isotropic_shielding",],
+    "pop": [],
+    "force": ["forces",],
+}
+
 
 class GaussianFile(File):
     """
     Class for Gaussian files. Composes ``ConformationalEnsemble``.
 
     Attributes:
         molecules (Ensemble): ``ConformationalEnsemble`` instance
         job_types (list): list of `job_type` instances
         route_card (str): optional, route card of .gjf file
         link0 (dict): optional, dictionary of Link 0 commands (e.g. {"mem": "32GB", "nprocshared": 16})
         footer (str): optional, footer of .gjf file
         success (int): number of successful terminations (should be 1 for an opt, 2 for opt and then freq, 1 for a single point energy, etc)
-        energies (list): list of energies for each cycle
-        scf_iterations (list): number of iterations per cycle
-        max_displacements (list): list of max displacement values for each cycle
-        rms_displacements (list): list of rms displacement values for each cycle
-        max_forces (list): list of max force values for each cycle
-        rms_forces (list): list of rms force values for each cycle
-        gradients (list): list of gradient values for each cycle
-        frequencies (list): list of frequencies
-        gibbs_free_energy (float): gibbs free energy, from vibrational correction
-        enthalpy (float): enthalpy, from vibrational correction
         title (str): optional, title of .gjf file
     """
 
     def __init__(
-        self, atomic_numbers, geometries, bonds=None, charge=None, multiplicity=None, job_types=None, route_card=None, link0=None, footer=None, title="title",
+        self, job_types, route_card=None, link0=None, footer=None, title="title", success=0
     ):
         """
         Create new GaussianFile object.
 
 		Args:
-            atomic_numbers (list): list of atomic numbers
-            geometries (list): list of lists of 3-tuples of xyz coordinates
-            bonds (nx.Graph): Graph object containing connectivity information (1-indexed)
-            charges (int): the charge of the molecules
-            multiplicities (int): the spin states of the molecules (1 corresponds to singlet, 2 to doublet, 3 to triplet, etc. -- so a multiplicity of 1 is equivalent to S=0)
             job_types (list): list of ``job_type`` instances
             route_card (str): optional, route card of ``.gjf`` file
             link0 (dict): optional, Link 0 commands of ``.gjf`` file
             footer (str): optional, footer of ``.gjf`` file
             title (str): optional, title of ``.gjf`` file
+            success (int): num successful terminations
 		"""
 
         if route_card and not isinstance(route_card, str):
             raise TypeError("route card needs to be a string")
 
         if link0 and not isinstance(link0, dict):
             raise TypeError("link0 needs to be a dict")
 
         if footer and not isinstance(footer, str):
             raise TypeError("footer needs to be a string")
 
         if title and not isinstance(title, str):
             raise TypeError("title needs to be a string")
 
+        if success and not isinstance(success, int):
+            raise TypeError("success needs to be an integer")
+
         if job_types is not None:
             if not all(isinstance(job, JobType) for job in job_types):
                 raise TypeError(f"invalid job type {job}")
 
-        if (len(atomic_numbers) > 0) and (len(geometries) > 0):
-            arguments = {"atomic_numbers": atomic_numbers, "geometries": geometries, "bonds": bonds, "charge": charge, "multiplicity": multiplicity}
-            self.molecules = ConformationalEnsemble(**arguments)
-
+        self.molecules = ConformationalEnsemble()
         self.route_card = route_card
         self.link0 = link0
         self.footer = footer
         self.title = title
         self.job_types = job_types
+        self.success = success
+
+    def __str__(self):
+        return f"GaussianFile (title=\"{str(self.title)}\", {len(self.molecules)} entries in Ensemble)"
 
     @classmethod
     def write_molecule_to_file(cls, filename, molecule, route_card, link0={"mem": "32GB", "nprocshared": 16}, footer=None, title="title", append=False, print_symbol=False):
         """
         Write a ``.gjf`` file using the given molecule.
 
         Args:
@@ -111,14 +113,16 @@
         """
         if not isinstance(molecule, Molecule):
             raise TypeError("need a valid molecule to write a file!")
 
         if (route_card is None) or (not isinstance(route_card, str)):
             raise ValueError("can't write a file without a route card")
 
+        assert re.match(r"^#p", route_card), f"route card doesn't start with #p: {route_card}"
+
         #### generate the text
         text = ""
         if append:
             text += "--Link1--\n"
 
         if isinstance(link0, dict):
             for key, val in link0.items():
@@ -127,15 +131,17 @@
         text += f"{route_card.strip()}\n\n{title}\n\n"
 
         text += f"{int(molecule.charge)} {int(molecule.multiplicity)}\n"
         for index, Z in enumerate(molecule.atomic_numbers, start=1):
             line = molecule.get_vector(index)
             if print_symbol:
                 Z = get_symbol(Z)
-            text += f"{Z:2d}       {line[0]:>13.8f} {line[1]:>13.8f} {line[2]:>13.8f}\n"
+                text += f"{Z:>2}       {line[0]:>13.8f} {line[1]:>13.8f} {line[2]:>13.8f}\n"
+            else:
+                text += f"{Z:2d}       {line[0]:>13.8f} {line[1]:>13.8f} {line[2]:>13.8f}\n"
 
         text += "\n"
         if footer is not None:
             text += f"{footer.strip()}\n\n"
 
         #### write the file
         if append:
@@ -177,41 +183,45 @@
         return len(self.imaginaries())
 
     def imaginaries(self):
         """
         Returns the imaginary frequencies, rounded to the nearest integer.
         """
         if JobType.FREQ in self.job_types:
-            return list(map(int, np.array(self.frequencies)[np.array(self.frequencies) < 0]))
+            return list(map(int, np.array(self.properties["frequencies"])[np.array(self.properties["frequencies"]) < 0]))
         else:
             raise TypeError("not a frequency job! can't get # imaginary frequencies!")
 
     @classmethod
     def read_file(cls, filename, return_lines=False):
         """
         Reads a Gaussian``.out`` or ``.gjf`` file and populates the attributes accordingly.
         Only footers from ``opt=modredundant`` can be read automatically --  ``genecep`` custom basis sets, &c must be specified manually.
 
+        Note:
+
         Will throw ``ValueError`` if there have been no successful iterations.
 
         Args:
             filename (str): path to the out file
             return_lines (Bool): whether the lines of the file should be returned
         Returns:
             ``GaussianFile`` object (or list of ``GaussianFile`` objects for Link1 files)
             (optional) the lines of the file (or list of lines of file for Link1 files)
         """
         if re.search("gjf$", filename):
             return cls._read_gjf_file(filename, return_lines)
 
         link1_lines = parse.split_link1(super().read_file(filename))
         files = []
-        for lines in link1_lines:
+        for link1idx, lines in enumerate(link1_lines):
             #### automatically assign job types based on header
             header = parse.search_for_block(lines, "#p", "----")
+            if header is None:
+                raise ValueError("can't find route card! (perhaps '#p' wasn't employed?)")
             job_types = cls._assign_job_types(header)
 
             link0 = parse.extract_link0(lines)
 
             #### extract parameters
             success = 0
             for line in lines:
@@ -233,54 +243,88 @@
                 footer = "\n".join(list(footer.split("\n"))[1:])  # get rid of the first line
                 footer = "\n".join([" ".join(list(filter(None, line.split(" ")))) for line in footer.split("\n")])
 
             bonds = parse.read_bonds(lines)
             charge = parse.find_parameter(lines, "Multiplicity", expected_length=6, which_field=2)[0]
             multip = parse.find_parameter(lines, "Multiplicity", expected_length=6, which_field=5)[0]
 
-            f = GaussianFile(atomic_numbers, geometries, bonds, job_types=job_types, charge=charge, multiplicity=multip)
-            f.energies = energies
-            f.scf_iterations = scf_iterations
-            f.route_card = header
-            f.link0 = link0
-            f.footer = footer
-            f.success = success
+            f = GaussianFile(job_types=job_types, route_card=header, link0=link0, footer=footer, success=success)
+
+            molecules = [None] * len(geometries)
+            properties = [{} for _ in range(len(geometries))]
+            for idx, geom in enumerate(geometries):
+                molecules[idx] = Molecule(atomic_numbers, geom, charge=charge, multiplicity=multip, bonds=bonds)
+                properties[idx]["energy"] = energies[idx]
+                properties[idx]["scf_iterations"] = scf_iterations[idx]
+                properties[idx]["link1_idx"] = link1idx
+                properties[idx]["filename"] = filename
 
             #### now for some job-type specific attributes
             if JobType.OPT in job_types:
-                f.rms_forces = parse.find_parameter(lines, "RMS\s+Force", expected_length=5, which_field=2)
-                f.rms_displacements = parse.find_parameter(lines, "RMS\s+Displacement", expected_length=5, which_field=2)
+                rms_forces = parse.find_parameter(lines, "RMS\s+Force", expected_length=5, which_field=2)
+                rms_displacements = parse.find_parameter(lines, "RMS\s+Displacement", expected_length=5, which_field=2)
+
+                for idx, force in enumerate(rms_forces):
+                    properties[idx]["rms_force"] = force
+                    properties[idx]["rms_displacement"] = rms_displacements[idx]
 
             if JobType.FREQ in job_types:
                 enthalpies = parse.find_parameter(lines, "thermal Enthalpies", expected_length=7, which_field=6)
                 if len(enthalpies) == 1:
-                    f.enthalpy = enthalpies[0]
+                    properties[-1]["enthalpy"] = enthalpies[0]
                 elif len(enthalpies) > 1:
                     raise ValueError("too many enthalpies found!")
 
                 gibbs_vals = parse.find_parameter(lines, "thermal Free Energies", expected_length=8, which_field=7)
                 if len(gibbs_vals) == 1:
-                    f.gibbs_free_energy = gibbs_vals[0]
+                    properties[-1]["gibbs_free_energy"] = gibbs_vals[0]
                 elif len(gibbs_vals) > 1:
                     raise ValueError("too many gibbs free energies found!")
 
                 frequencies = []
                 try:
                     frequencies += parse.find_parameter(lines, "Frequencies", expected_length=5, which_field=2)
                     frequencies += parse.find_parameter(lines, "Frequencies", expected_length=5, which_field=3)
                     frequencies += parse.find_parameter(lines, "Frequencies", expected_length=5, which_field=4)
-                    f.frequencies = sorted(frequencies)
+                    properties[-1]["frequencies"] = sorted(frequencies)
                 except:
                     raise ValueError("error finding frequencies")
 
             if JobType.NMR in job_types:
-                assert len(f.molecules) == 1, "NMR jobs should not be combined with optimizations!"
-                nmr_shifts = parse.read_nmr_shifts(lines, f.molecules[-1].num_atoms())
-                f.molecules[0].nmr_isotropic = nmr_shifts.view(OneIndexedArray)
+                assert len(molecules) == 1, "NMR jobs should not be combined with optimizations!"
+                nmr_shifts = parse.read_nmr_shifts(lines, molecules[0].num_atoms())
+                properties[0]["isotropic_shielding"] = nmr_shifts.view(OneIndexedArray)
+
+            if JobType.FORCE in job_types:
+                assert len(molecules) == 1, "force jobs should not be combined with optimizations!"
+                forces = parse.read_forces(lines)
+                properties[0]["forces"] = forces
+
+            if JobType.POP in job_types:
+                if re.search("hirshfeld", f.route_card):
+                    charges, spins = parse.read_hirshfeld_charges(lines)
+                    properties[-1]["hirshfeld_charges"] = charges
+                    properties[-1]["hirshfeld_spins"] = spins
 
+            try:
+                charges = parse.read_mulliken_charges(lines)
+                properties[-1]["mulliken_charges"] = charges
+            except:
+                pass
+
+            try:
+                dipole = parse.read_dipole_moment(lines)
+                properties[-1]["dipole_moment"] = dipole
+            except:
+                pass
+
+            for mol, prop in zip(molecules, properties):
+                f.molecules.add_molecule(mol, properties=prop)
+
+            f.check_has_properties()
             files.append(f)
 
         if return_lines:
             if len(link1_lines) == 1:
                 return files[0], link1_lines[0]
             else:
                 return files, link1_lines
@@ -308,15 +352,15 @@
         footer = None
         header_done = False
         title = None
         charge = None
         multip = None
         in_geom = False
         atomic_numbers = []
-        geometries = []
+        geometry = []
 
         for idx, line in enumerate(lines):
             if header is None:
                 if re.match("\%", line):
                     pieces = line[1:].split("=")
                     link0[pieces[0]] = pieces[1]
                     continue
@@ -349,38 +393,32 @@
                 if len(line.strip()) == 0:
                     in_geom = False
                 else:
                     pieces = list(filter(None, line.split(" ")))
                     assert len(pieces) == 4, f"can't parse line {line}"
 
                     atomic_numbers.append(pieces[0])
-                    geometries.append([pieces[1], pieces[2], pieces[3]])
+                    geometry.append([pieces[1], pieces[2], pieces[3]])
 
-            if (in_geom == False) and (len(geometries) > 0):
+            if (in_geom == False) and (len(geometry) > 0):
                 if footer:
                     footer = footer + "\n" + line
                 else:
                     if len(line.strip()) > 0:
                         footer = line
 
         try:
             atomic_numbers = np.array(atomic_numbers, dtype=np.int8)
         except:
             atomic_numbers = np.array(list(map(get_number, atomic_numbers)), dtype=np.int8)
 
-        geometries = np.array([geometries])
         job_types = cls._assign_job_types(header)
 
-        f = GaussianFile(atomic_numbers, geometries, job_types=job_types, charge=charge, multiplicity=multip)
-        f.route_card = header
-        f.link0 = link0
-        f.footer = footer
-        f.title = title
-        f.success = 0
-
+        f = GaussianFile(job_types=job_types, route_card=header, link0=link0, footer=footer, title=title)
+        f.molecules.add_molecule(Molecule(atomic_numbers, geometry, charge=charge, multiplicity=multip))
         if return_lines:
             return f, lines
         else:
             return f
 
     def get_molecule(self, num=None):
         """
@@ -394,42 +432,117 @@
 
         if not isinstance(num, int):
             raise TypeError("num must be int")
 
         return self.molecules[num]
 
     @classmethod
-    def write_ensemble_to_file(cls, filename, ensemble, route_cards, kwargs):
-        """
-        Writes an Ensemble to a file using Link1 specification.
-
-        Args:
-            filename (str): where to write the file
-            ensemble (Ensemble): ``Ensemble`` object to write
-            headers (list): headers for each ``write_molecule_to_file`` call
-            kwargs (list of dict): arguments for each ``write_molecule_to_file`` call
-        """
-        for idx, molecule in enumerate(ensemble.molecules):
-            if idx == 0:
-                cls.write_molecule_to_file(filename, molecule, route_cards[idx], append=False, **kwargs[idx])
-            else:
-                cls.write_molecule_to_file(filename, molecule, route_cards[idx], append=True, **kwargs[idx])
-
-
-    @classmethod
     def _assign_job_types(cls, header):
         """
-        Assigns ``JobType`` objects from route card.
+        Assigns ``JobType`` objects from route card. ``Job.Type.SP`` is assigned by default.
 
-        For instance, "#p opt freq=noraman" would give an output of [JobType.OPT, JobType.FREQ].
+        For instance, "#p opt freq=noraman" would give an output of ``[JobType.SP, JobType.OPT, JobType.FREQ]``.
 
         Args:
             header (str): Gaussian route card
 
         Returns:
             list of ``JobType`` objects
         """
         job_types = []
         for name, member in JobType.__members__.items():
             if re.search(f" {member.value}", str(header), re.IGNORECASE):
                 job_types.append(member)
+        if JobType.SP not in job_types:
+            job_types.append(JobType.SP)
         return job_types
+
+    def check_has_properties(self):
+        """
+        Checks that the file has all the appropriate properties for its job types, and raises ValueError if not.
+
+        This only checks the last molecule in ``self.molecules``, for now.
+        """
+        for job_type in self.job_types:
+            for prop in EXPECTED_PROPERTIES[job_type.value]:
+                if not self.molecules.has_property(-1, prop):
+                    raise ValueError(f"expected property {prop} for job type {job_type}, but it's not there!")
+
+    @classmethod
+    def write_ensemble_to_file(cls, filename, ensemble, route_card, link0={"mem": "32GB", "nprocshared": 16}, footer=None, title="title", print_symbol=False):
+            """
+            Write each structure in the specified ensemble to a single Gaussian input file
+            by using the Link1 specification.
+
+            Args:
+                filename (str): where to write the file
+                ensemble (Ensemble): ``Ensemble`` object to write
+                route_card (str or list): to use the same route card for every link, use a single string;
+                                          otherwise, provide a list whose entries parallel the ensemble members
+                link0 (dict or list of dicts): to use the same memory/processors for every link, use a single string;
+                                               otherwise, provide a list
+                footer (None/str or list): use None for no text after geometry, provide a str to specify a footer,
+                                           or provide some combination of the above as a list
+                title (str or list): use a single string to provide a generic title for every link or a list as above
+                print_symbol (bool or list): whether to print atomic symbols or atomic numbers in the geometry specification;
+                                             use a single bool or a list as above
+
+            """
+            n_geometries = len(ensemble)
+            assert len(ensemble) > 0, "cannot write a blank ensemble"
+
+            if isinstance(route_card, str):
+                assert re.match(r"^#p", route_card), "route card should start with #p: {route_card}"
+                route_card = [route_card for m in ensemble._items]
+            elif isinstance(route_card, list):
+                assert len(route_card) == n_geometries, f"expected {n_geometries} route cards but got {len(route_card)}"
+                for card in route_card:
+                    assert isinstance(card, str), "expected route card to be a str"
+                    assert re.match(r"^#p", route_card), "route card should start with #p: f{card}"
+            else:
+                raise ValueError(f"unexpected type for route_card: {str(type(route_card))}")
+
+            if isinstance(link0, dict):
+                link0 = [link0 for m in ensemble._items]
+            elif isinstance(link0, list):
+                assert len(link0) == n_geometries, f"expected {n_geometries} link0 entries, but got {len(link0)}"
+                for d in link0:
+                    assert isinstance(d, dict), f"expected dict for link0 but got {str(type(d))}"
+            else:
+                raise ValueError(f"unexpected type for link0: {str(type(link0))}")
+
+            if footer is None or isinstance(footer, str):
+                footer = [footer for m in ensemble._items]
+            elif isinstance(footer, list):
+                assert len(footer) == n_geometries, f"expected {n_geometries} footers, but got {len(footer)}"
+                for f in footer:
+                    assert f is None or isinstance(f, str), f"expected str or None for footer but got {str(type(f))}"
+            else:
+                raise ValueError(f"unexpected type for footer: {str(type(footer))}")
+
+            if isinstance(title, str):
+                assert len(title.strip()) > 0, "zero-length titles not allowed"
+                title = [title for m in ensemble._items]
+            elif isinstance(title, list):
+                assert len(title) == n_geometries, f"expected {n_geometries} route cards but got {len(title)}"
+                for card in title:
+                    assert isinstance(card, str), "expected title to be a str"
+                    assert len(title.strip()) > 0, "zero-length titles are not allowed"
+            else:
+                raise ValueError(f"unexpected type for title: {str(type(title))}")
+
+            if isinstance(print_symbol, bool):
+                print_symbol = [print_symbol for m in ensemble._items]
+            elif isinstance(print_symbol, list):
+                assert len(print_symbol) == n_geometries, f"expected {n_geometries} print_symbol entries but got {len(print_symbol)}"
+                for s in print_symbol:
+                    assert isinstance(s, bool), f"expected bool for print_symbol but got {str(type(s))}"
+            else:
+                raise ValueError(f"unexpected type for print_symbol: {str(type(print_symbol))}")
+
+            for idx, molecule in enumerate(ensemble._items):
+                if idx == 0:
+                    cls.write_molecule_to_file(filename, molecule, route_card[idx], link0[idx], footer=footer[idx], title=title[idx], print_symbol=print_symbol[idx], append=False)
+                else:
+                    cls.write_molecule_to_file(filename, molecule, route_card[idx], link0[idx], footer=footer[idx], title=title[idx], print_symbol=print_symbol[idx], append=True)
+
+
```

### Comparing `cctk-v0.1.4/cctk/group.py` & `cctk-v0.1.5/cctk/group.py`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/groups/EtH.mol2` & `cctk-v0.1.5/cctk/groups/EtH.mol2`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/groups/NHAcH.mol2` & `cctk-v0.1.5/cctk/groups/NHAcH.mol2`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/groups/NMe2H.mol2` & `cctk-v0.1.5/cctk/groups/NMe2H.mol2`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/groups/iPrH.mol2` & `cctk-v0.1.5/cctk/groups/iPrH.mol2`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/groups/tBuH.mol2` & `cctk-v0.1.5/cctk/groups/tBuH.mol2`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/load_groups.py` & `cctk-v0.1.5/cctk/load_groups.py`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/mae_file.py` & `cctk-v0.1.5/cctk/mae_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import numpy as np
 import networkx as nx
 
 from abc import abstractmethod
 
-from cctk import File, Ensemble, ConformationalEnsemble
+from cctk import File, Ensemble, ConformationalEnsemble, Molecule
 from cctk.helper_functions import get_symbol, get_number
 
 
 class MAEFile(File):
     """
     Generic class for all ``.mae`` files.
 
@@ -36,19 +36,22 @@
             property_values (list)
         """
 
         file = MAEFile(name=name)
 
         (geometries, symbols, bonds, p_names, p_vals, conformers) = cls._read_mae(filename, **kwargs)
         atomic_numbers = np.array([get_number(z) for z in symbols], dtype=np.int8)
+
         if conformers == True:
-            file.molecules = ConformationalEnsemble(geometries=geometries, atomic_numbers=atomic_numbers, bonds=bonds.edges())
+            file.molecules = ConformationalEnsemble()
         else:
-            atomic_numbers = np.tile(atomic_numbers, (len(geometries), 1))
-            file.molecules = Ensemble(geometries=geometries, atomic_numbers=atomic_numbers, bonds=[b.edges() for b in bonds])
+            file.molecules = Ensemble()
+
+        for geom in geometries:
+            file.molecules.add_molecule(Molecule(atomic_numbers, geom, bonds=bonds.edges))
 
         return file, p_names, p_vals
 
     @classmethod
     def _read_mae(
         cls, filename, contains_conformers="check", save_memory_for_conformers=True, print_status_messages=False,
     ):
```

### Comparing `cctk-v0.1.4/cctk/mol2_file.py` & `cctk-v0.1.5/cctk/mol2_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,22 @@
             MOL2File object
         """
 
         file = MOL2File(name=name)
 
         (geometries, symbols, atom_types, bonds, conformers) = cls._read_mol2(filename, **kwargs)
         atomic_numbers = np.array([get_number(z) for z in symbols], dtype=np.int8)
+
         if conformers == True:
-            file.molecules = ConformationalEnsemble(geometries=geometries, atomic_numbers=atomic_numbers, bonds=bonds.edges())
+            file.molecules = ConformationalEnsemble()
         else:
-            atomic_numbers = np.tile(atomic_numbers, (len(geometries), 1))
-            file.molecules = Ensemble(geometries=geometries, atomic_numbers=atomic_numbers, bonds=[b.edges() for b in bonds])
+            file.molecules = Ensemble()
+
+        for geom in geometries:
+            file.molecules.add_molecule(Molecule(atomic_numbers, geom, bonds=bonds.edges))
 
         return file
 
     @classmethod
     def _read_mol2(
         cls, filename, contains_conformers="check", save_memory_for_conformers=True, print_status_messages=False,
     ):
```

### Comparing `cctk-v0.1.4/cctk/molecule.py` & `cctk-v0.1.5/cctk/molecule.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,20 @@
 
         self.bonds = nx.Graph()
         self.bonds.add_nodes_from(range(1, len(atomic_numbers) + 1))
         if bonds:
             for bond in bonds:
                 self.add_bond(bond[0], bond[1])
 
+    def __str__(self):
+        if self.name is not None:
+            return f"Molecule (name={self.name}, {len(self.atomic_numbers)} atoms)"
+        else:
+            return f"Molecule ({len(self.atomic_numbers)} atoms)"
+
     def assign_connectivity(self, cutoff=0.5):
         """
         Automatically recalculates bonds based on covalent radii. If two atoms are closer than the sum of their covalent radii + 0.5 Angstroms, then they are considered bonded.
 
         Args:
             cutoff (float): the threshold (in Angstroms) for how close two covalent radii must be to be considered bonded
```

### Comparing `cctk-v0.1.4/cctk/orca_file.py` & `cctk-v0.1.5/cctk/orca_file.py`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/cctk/parse_gaussian.py` & `cctk-v0.1.5/cctk/parse_gaussian.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import re
 
 from cctk.helper_functions import get_symbol
+from cctk import OneIndexedArray
 
 """
 Functions to help with parsing Gaussian files
 """
 
 
 def read_geometries_and_energies(lines):
@@ -291,15 +292,16 @@
 
     Returns:
         list of isotropic NMR shifts (np.ndarray)
     """
     # assumes that lines only come from one Link1 section
     shieldings = []
     for line in lines:
-        if line[14:23] == "Isotropic":
+        fields = line.split()
+        if len(fields) == 8 and fields[2] == "Isotropic" and fields[5] == "Anisotropy":
             fields = line.split()
             assert len(fields) == 8, f"Expected 8 fields on an NMR shielding output line but found {len(fields)} instead!"
             try:
                 shielding = float(fields[4])
             except:
                 raise ValueError(f"Error parsing NMR shielding output line:\n{line}")
             shieldings.append(shielding)
@@ -356,7 +358,91 @@
     #### and search within that little block for lines matching the right description
     for line in lines[start_idx:end_idx]:
         if re.match(" \%", line):
             pieces = line[2:].split("=")
             output[pieces[0]] = pieces[1]
 
     return output
+
+def read_forces(lines):
+    """
+    Reads forces from a Gaussian ``force`` job.
+
+    Args:
+        lines (list): list of lines in file
+
+    Returns:
+        (n x 3) ``cctk.OneIndexedArray`` of forces
+    """
+    forces = []
+    force_block = search_for_block(lines, "Forces \(Hartrees/Bohr\)", "Cartesian Forces", join="\n")
+    for line in force_block.split("\n")[2:]:
+        fields = re.split(" +", line)
+        fields = list(filter(None, fields))
+
+        if len(fields) == 5:
+            forces.append([float(fields[2]), float(fields[3]), float(fields[4])])
+
+    return OneIndexedArray(forces)
+
+def read_mulliken_charges(lines):
+    """
+    Reads charges from a Gaussian ``pop`` job.
+
+    Args:
+        lines (list): list of lines in file
+
+    Returns:
+        ``cctk.OneIndexedArray`` of charges
+    """
+    charges = []
+    charge_block = search_for_block(lines, " Mulliken charges:", " Sum of Mulliken charges", join="\n")
+    for line in charge_block.split("\n")[2:]:
+        fields = re.split(" +", line)
+        fields = list(filter(None, fields))
+
+        if len(fields) == 3:
+            charges.append(float(fields[2]))
+
+    return OneIndexedArray(charges)
+
+def read_hirshfeld_charges(lines):
+    """
+    Reads charges from a Gaussian ``pop`` job.
+
+    Args:
+        lines (list): list of lines in file
+
+    Returns:
+        ``cctk.OneIndexedArray`` of charges
+        ``cctk.OneIndexedArray`` of spin densities
+    """
+    charges = []
+    spins = []
+    charge_block = search_for_block(lines, "Hirshfeld charges, spin densities, dipoles, and CM5 charges", " Hirshfeld charges", join="\n")
+    for line in charge_block.split("\n")[2:]:
+        fields = re.split(" +", line)
+        fields = list(filter(None, fields))
+
+        if len(fields) == 8:
+            charges.append(float(fields[2]))
+            spins.append(float(fields[3]))
+
+    return OneIndexedArray(charges), OneIndexedArray(spins)
+
+def read_dipole_moment(lines):
+    """
+    Reads dipole moment from a Gaussian job.
+
+    Args:
+        lines (list): list of lines in file
+
+    Returns:
+        dipole moment (magnitude only)
+    """
+    dipole_block = search_for_block(lines, "Dipole moment \(field-independent basis, Debye\)", "Quadrupole moment \(field-independent basis, Debye-Ang\):", join="\n")
+    for line in dipole_block.split("\n")[1:]:
+        fields = re.split(" +", line)
+        fields = list(filter(None, fields))
+
+        if len(fields) == 8:
+            return float(fields[7])
```

### Comparing `cctk-v0.1.4/cctk/pdb_file.py` & `cctk-v0.1.5/cctk/pdb_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,13 +50,13 @@
         """
         Writes a ``ConformationalEnsemble`` to a trajectory file.
 
         Args:
             filename (str): where to write the file
             ensemble (Ensemble): ``Ensemble`` object to write
         """
-        for idx, molecule in enumerate(ensemble.molecules):
+        for idx, molecule in enumerate(ensemble.molecules()):
             if idx == 0:
                 cls.write_molecule_to_file(filename, molecule, num=idx+1, append=False)
             else:
                 cls.write_molecule_to_file(filename, molecule, num=idx+1, append=True)
```

### Comparing `cctk-v0.1.4/cctk/xyz_file.py` & `cctk-v0.1.5/cctk/xyz_file.py`

 * *Files identical despite different names*

### Comparing `cctk-v0.1.4/setup.py` & `cctk-v0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     long_description = f.read()
 
 setup(
     name="cctk",
     packages=["cctk", "cctk.data", "cctk.groups"],
 #    include_package_data=True,
     package_data={"cctk.data": ["*"], "cctk.groups": ["*"],},
-    version="v0.1.4",
+    version="v0.1.5",
     license="Apache 2.O",
     description="computational chemistry toolkit",
     author="Corin Wagen and Eugene Kwan",
     author_email="corin.wagen@gmail.com",
     url="https://github.com/ekwan/cctk",
-    download_url="https://github.com/ekwan/cctk/archive/v0.1.3.tar.gz",
+    download_url="https://github.com/ekwan/cctk/archive/v0.1.5.tar.gz",
     install_requires=["numpy", "networkx", "importlib_resources"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Science/Research",
```

### Comparing `cctk-v0.1.4/test/test_gaussian.py` & `cctk-v0.1.5/test/test_gaussian.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import cctk
 
 class TestGaussian(unittest.TestCase):
     def test_read_gjf_file(self):
         path = "test/static/gaussian_file.gjf"
         file = cctk.GaussianFile.read_file(path)
         self.assertEqual(file.route_card, "#p opt freq=noraman m062x/6-31g(d) scrf=(smd,solvent=diethylether)")
-        self.assertListEqual(file.job_types, [cctk.JobType.OPT, cctk.JobType.FREQ])
+        self.assertListEqual(file.job_types, [cctk.JobType.OPT, cctk.JobType.FREQ, cctk.JobType.SP])
         self.assertDictEqual(file.link0, {"mem": "1GB", "chk": "test.chk"})
         self.assertEqual(file.title, "title")
         self.assertEqual(file.footer, None)
 
         mol = file.get_molecule()
         self.assertTrue(isinstance(mol, cctk.Molecule))
         self.assertEqual(mol.num_atoms(), 31)
@@ -19,19 +19,22 @@
         self.assertEqual(mol.multiplicity, 1)
 
     def test_read_out_file(self):
         path = "test/static/gaussian_file.out"
         file = cctk.GaussianFile.read_file(path)
         self.assertEqual(file.route_card, "#p opt freq=noraman m062x/6-31g(d) scrf=(smd,solvent=diethylether)")
         self.assertDictEqual(file.link0, {"mem": "32GB",  "nprocshared": "16"})
-        self.assertListEqual(file.job_types, [cctk.JobType.OPT, cctk.JobType.FREQ])
+        self.assertListEqual(file.job_types, [cctk.JobType.OPT, cctk.JobType.FREQ, cctk.JobType.SP])
         self.assertEqual(file.title, "title")
         self.assertEqual(file.footer, None)
         self.assertTrue(isinstance(file.molecules, cctk.ConformationalEnsemble))
 
+        for mol, prop in file.molecules.items():
+            self.assertEqual(prop["filename"], path)
+
         mol = file.get_molecule()
         self.assertTrue(isinstance(mol, cctk.Molecule))
         self.assertEqual(mol.num_atoms(), 31)
         self.assertEqual(mol.charge, 0)
         self.assertEqual(mol.multiplicity, 1)
 
         old_path = "test/static/gaussian_file.gjf"
@@ -52,13 +55,57 @@
         path = "test/static/ethane.out"
         f, lines = cctk.GaussianFile.read_file(path, return_lines=True)
 
         self.assertEqual(len(lines), 3)
         self.assertEqual(len(f), 3)
         self.assertTrue(all(isinstance(file, cctk.GaussianFile) for file in f))
 
-        self.assertListEqual(f[0].job_types, [cctk.JobType.OPT, cctk.JobType.FREQ])
-        self.assertListEqual(f[1].job_types, [cctk.JobType.NMR])
-        self.assertListEqual(f[2].job_types, [cctk.JobType.NMR])
+        self.assertListEqual(f[0].job_types, [cctk.JobType.OPT, cctk.JobType.FREQ, cctk.JobType.SP])
+        self.assertListEqual(f[1].job_types, [cctk.JobType.NMR, cctk.JobType.SP])
+        self.assertListEqual(f[2].job_types, [cctk.JobType.NMR, cctk.JobType.SP])
+
+
+    def test_write_ensemble(self):
+        path = "test/static/gaussian_file.out"
+        file = cctk.GaussianFile.read_file(path)
+        ense = file.molecules
+
+        old_path = "test/static/ensemble.gjf"
+        new_path = "test/static/new_ensemble.gjf"
+        cctk.GaussianFile.write_ensemble_to_file(new_path, ense, "#p opt freq=noraman b3lyp/6-31g(d)", print_symbol=True)
+
+        with open(old_path) as old:
+            with open(new_path) as new:
+                self.assertListEqual(
+                    list(new),
+                    list(old)
+                )
+
+        os.remove(new_path)
+
+    def test_force_extraction(self):
+        path = "test/static/dcm_force.out"
+        file = cctk.GaussianFile.read_file(path)
+        ense = file.molecules
+
+        self.assertListEqual(list(ense[0, "forces"][1]), [2.672010074,2.672010074,0.0])
+
+    def test_charges(self):
+        path = "test/static/dcm_force.out"
+        file = cctk.GaussianFile.read_file(path)
+        ense = file.molecules
+        self.assertEqual(ense[-1, "mulliken_charges"][1], -0.051271)
+
+        path = "test/static/h2o.out"
+        file = cctk.GaussianFile.read_file(path)
+        ense = file.molecules
+        self.assertEqual(ense[-1, "hirshfeld_charges"][1], -0.312885)
+        self.assertEqual(ense[-1, "hirshfeld_spins"][1], 0)
+
+    def test_dipole(self):
+        path = "test/static/dcm_force.out"
+        file = cctk.GaussianFile.read_file(path)
+        ense = file.molecules
+        self.assertEqual(ense[-1, "dipole_moment"], 0.3316)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cctk-v0.1.4/test/test_helper.py` & `cctk-v0.1.5/test/test_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,9 +15,14 @@
 
     def test_get_symbol(self):
         self.assertEqual(helper.get_symbol(0), "Bq")
         self.assertEqual(helper.get_symbol(62), "Sm")
         self.assertEqual(helper.get_symbol(46), "Pd")
         self.assertEqual(helper.get_symbol(6), "C")
 
+    def test_isotope(self):
+        m, w = helper.get_isotopic_distribution(1)
+        self.assertListEqual(list(m), [1.007825, 2.014102, 3.016049])
+        self.assertListEqual(list(w), [0.999885, 0.000115, 0.0])
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cctk-v0.1.4/test/test_indexing.py` & `cctk-v0.1.5/test/test_indexing.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,20 @@
         new_a = cctk.OneIndexedArray(array)
 
         self.assertEqual(len(new_a), 5)
         self.assertEqual(str(new_a), "[1 2 3 4 5]")
         self.assertEqual(str(new_a[1:3]), "[1 2]")
         self.assertEqual(new_a[5], 5)
         self.assertEqual(new_a[1], 1)
+
+        self.assertTrue(isinstance(cctk.OneIndexedArray(new_a), cctk.OneIndexedArray))
+
+        self.assertEqual(new_a[[1]], 1)
+        self.assertListEqual(list(new_a[[1,2]]), [1,2])
+
         new_a[1] = 8
         self.assertEqual(str(new_a), "[8 2 3 4 5]")
         self.assertEqual(new_a[1], 8)
 
         a_2d = [[1,1,1],[2,2,2],[3,3,3]]
         new_a_2d = cctk.OneIndexedArray(a_2d)
         self.assertEqual(new_a_2d[1,1], 1)
```

### Comparing `cctk-v0.1.4/test/test_molecule.py` & `cctk-v0.1.5/test/test_molecule.py`

 * *Files identical despite different names*

