# Comparing `tmp/TB2J-0.7.4rc2.tar.gz` & `tmp/TB2J-0.7.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.7.4rc2.tar", last modified: Wed Jun 29 19:32:22 2022, max compression
+gzip compressed data, was "TB2J-0.7.4rc3.tar", last modified: Thu Jun 30 13:33:31 2022, max compression
```

## Comparing `TB2J-0.7.4rc2.tar` & `TB2J-0.7.4rc3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.879549 TB2J-0.7.4rc2/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1327 2020-07-08 14:12:19.000000 TB2J-0.7.4rc2/LICENSE
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1257 2022-06-29 19:32:22.879549 TB2J-0.7.4rc2/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1914 2022-06-29 07:51:51.000000 TB2J-0.7.4rc2/README.md
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.875549 TB2J-0.7.4rc2/TB2J/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7082 2022-06-28 09:12:36.000000 TB2J-0.7.4rc2/TB2J/Jdownfolder.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1771 2022-06-28 09:12:36.000000 TB2J-0.7.4rc2/TB2J/Jtensor.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3994 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/Oiju.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7423 2022-04-19 18:59:46.000000 TB2J-0.7.4rc2/TB2J/Oiju_epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       26 2022-06-29 10:23:38.000000 TB2J-0.7.4rc2/TB2J/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2884 2022-02-27 23:27:25.000000 TB2J-0.7.4rc2/TB2J/citation.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2489 2022-01-16 11:30:39.000000 TB2J-0.7.4rc2/TB2J/contour.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2939 2022-06-29 10:43:12.000000 TB2J-0.7.4rc2/TB2J/cut_cell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3518 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    28490 2022-06-28 09:12:36.000000 TB2J-0.7.4rc2/TB2J/exchange.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    11693 2022-04-30 07:59:01.000000 TB2J-0.7.4rc2/TB2J/exchangeCL2.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     8372 2022-04-30 07:59:33.000000 TB2J-0.7.4rc2/TB2J/exchange_pert.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9017 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/exchange_qspace.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.875549 TB2J-0.7.4rc2/TB2J/external/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      137 2022-04-30 08:05:35.000000 TB2J-0.7.4rc2/TB2J/external/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5943 2022-04-30 07:58:12.000000 TB2J-0.7.4rc2/TB2J/external/p_tqdm.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6630 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/gpaw_wrapper.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12273 2022-02-27 23:27:25.000000 TB2J-0.7.4rc2/TB2J/green.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1571 2022-02-27 23:27:25.000000 TB2J-0.7.4rc2/TB2J/greentest.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.875549 TB2J-0.7.4rc2/TB2J/io_exchange/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       32 2020-07-08 14:12:19.000000 TB2J-0.7.4rc2/TB2J/io_exchange/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    16889 2022-06-29 19:25:14.000000 TB2J-0.7.4rc2/TB2J/io_exchange/io_exchange.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6720 2022-04-19 18:45:40.000000 TB2J-0.7.4rc2/TB2J/io_exchange/io_multibinit.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4024 2022-04-19 18:44:14.000000 TB2J-0.7.4rc2/TB2J/io_exchange/io_tomsasd.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10198 2022-04-19 18:43:25.000000 TB2J-0.7.4rc2/TB2J/io_exchange/io_txt.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3190 2022-04-19 18:40:58.000000 TB2J-0.7.4rc2/TB2J/io_exchange/io_uppasd.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5563 2022-06-28 09:12:36.000000 TB2J-0.7.4rc2/TB2J/io_exchange/io_vampire.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     6921 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/io_merge.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      533 2022-03-01 14:26:44.000000 TB2J-0.7.4rc2/TB2J/kpoints.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    18281 2021-11-24 10:31:21.000000 TB2J-0.7.4rc2/TB2J/manager.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    17881 2022-04-19 19:02:24.000000 TB2J-0.7.4rc2/TB2J/myTB.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4722 2021-10-04 10:59:57.000000 TB2J-0.7.4rc2/TB2J/orbmap.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     4092 2022-02-27 23:27:25.000000 TB2J-0.7.4rc2/TB2J/pauli.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1223 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/pert.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1435 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/plot.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1126 2021-05-27 13:46:56.000000 TB2J-0.7.4rc2/TB2J/rotate_atoms.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10355 2022-04-19 18:50:05.000000 TB2J-0.7.4rc2/TB2J/sisl_wrapper.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.879549 TB2J-0.7.4rc2/TB2J/spinham/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-07-08 14:12:19.000000 TB2J-0.7.4rc2/TB2J/spinham/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2234 2021-09-17 19:59:43.000000 TB2J-0.7.4rc2/TB2J/spinham/base_parser.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      741 2020-07-08 14:12:19.000000 TB2J-0.7.4rc2/TB2J/spinham/constants.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    13322 2022-04-19 18:57:57.000000 TB2J-0.7.4rc2/TB2J/spinham/hamiltonian.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9870 2021-11-24 10:31:21.000000 TB2J-0.7.4rc2/TB2J/spinham/hamiltonian_terms.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     7011 2022-04-19 19:03:09.000000 TB2J-0.7.4rc2/TB2J/spinham/plot.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2176 2021-10-04 10:59:57.000000 TB2J-0.7.4rc2/TB2J/spinham/qsolver.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2238 2021-02-01 11:14:39.000000 TB2J-0.7.4rc2/TB2J/spinham/spin_api.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10923 2022-04-19 19:03:17.000000 TB2J-0.7.4rc2/TB2J/spinham/spin_xml.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.4rc2/TB2J/spinham/supercell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    19588 2022-06-29 10:42:47.000000 TB2J-0.7.4rc2/TB2J/supercell.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3896 2022-04-19 19:03:29.000000 TB2J-0.7.4rc2/TB2J/utest.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     9358 2022-04-19 18:53:16.000000 TB2J-0.7.4rc2/TB2J/utils.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      276 2022-04-13 09:35:56.000000 TB2J-0.7.4rc2/TB2J/versioninfo.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.879549 TB2J-0.7.4rc2/TB2J/wannier/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       70 2021-10-04 10:59:57.000000 TB2J-0.7.4rc2/TB2J/wannier/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3664 2022-02-27 23:27:25.000000 TB2J-0.7.4rc2/TB2J/wannier/w90_parser.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.875549 TB2J-0.7.4rc2/TB2J.egg-info/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1257 2022-06-29 19:32:22.000000 TB2J-0.7.4rc2/TB2J.egg-info/PKG-INFO
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1402 2022-06-29 19:32:22.000000 TB2J-0.7.4rc2/TB2J.egg-info/SOURCES.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2022-06-29 19:32:22.000000 TB2J-0.7.4rc2/TB2J.egg-info/dependency_links.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       68 2022-06-29 19:32:22.000000 TB2J-0.7.4rc2/TB2J.egg-info/requires.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        5 2022-06-29 19:32:22.000000 TB2J-0.7.4rc2/TB2J.egg-info/top_level.txt
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-29 19:32:22.879549 TB2J-0.7.4rc2/scripts/
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1663 2021-03-27 13:32:37.000000 TB2J-0.7.4rc2/scripts/TB2J_downfold.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1185 2022-06-29 10:14:59.000000 TB2J-0.7.4rc2/scripts/TB2J_eigen.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     3379 2022-03-01 14:30:46.000000 TB2J-0.7.4rc2/scripts/TB2J_magnon.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1277 2021-02-01 11:14:39.000000 TB2J-0.7.4rc2/scripts/TB2J_merge.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)      715 2021-11-24 10:31:21.000000 TB2J-0.7.4rc2/scripts/TB2J_rotate.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     5083 2022-02-27 23:27:25.000000 TB2J-0.7.4rc2/scripts/siesta2J.py
--rwxrwxr-x   0 hexu      (1000) hexu      (1000)     7092 2021-11-24 10:31:21.000000 TB2J-0.7.4rc2/scripts/wann2J.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2022-06-29 19:32:22.879549 TB2J-0.7.4rc2/setup.cfg
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     1789 2022-06-29 19:32:18.000000 TB2J-0.7.4rc2/setup.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.601678 TB2J-0.7.4rc3/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1327 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/LICENSE
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1257 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/PKG-INFO
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1914 2022-06-29 07:51:51.000000 TB2J-0.7.4rc3/README.md
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.589678 TB2J-0.7.4rc3/TB2J/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     7082 2022-06-28 09:12:36.000000 TB2J-0.7.4rc3/TB2J/Jdownfolder.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1771 2022-06-28 09:12:36.000000 TB2J-0.7.4rc3/TB2J/Jtensor.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3994 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/Oiju.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     7423 2022-04-19 18:59:46.000000 TB2J-0.7.4rc3/TB2J/Oiju_epc.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       26 2022-06-29 10:23:38.000000 TB2J-0.7.4rc3/TB2J/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2884 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/citation.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2489 2022-01-16 11:30:39.000000 TB2J-0.7.4rc3/TB2J/contour.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2952 2022-06-30 13:32:49.000000 TB2J-0.7.4rc3/TB2J/cut_cell.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3518 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/epc.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    28490 2022-06-30 11:14:23.000000 TB2J-0.7.4rc3/TB2J/exchange.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    11699 2022-06-30 11:12:22.000000 TB2J-0.7.4rc3/TB2J/exchangeCL2.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     8372 2022-04-30 07:59:33.000000 TB2J-0.7.4rc3/TB2J/exchange_pert.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     9017 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/exchange_qspace.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.593678 TB2J-0.7.4rc3/TB2J/external/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      137 2022-04-30 08:05:35.000000 TB2J-0.7.4rc3/TB2J/external/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     5943 2022-04-30 07:58:12.000000 TB2J-0.7.4rc3/TB2J/external/p_tqdm.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     6630 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/gpaw_wrapper.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    12273 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/green.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1571 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/greentest.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.593678 TB2J-0.7.4rc3/TB2J/io_exchange/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       32 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/TB2J/io_exchange/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    16889 2022-06-29 19:25:14.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_exchange.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     6720 2022-04-19 18:45:40.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_multibinit.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     4024 2022-04-19 18:44:14.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_tomsasd.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10198 2022-04-19 18:43:25.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_txt.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3190 2022-04-19 18:40:58.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_uppasd.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     5563 2022-06-28 09:12:36.000000 TB2J-0.7.4rc3/TB2J/io_exchange/io_vampire.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     6921 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/io_merge.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      533 2022-03-01 14:26:44.000000 TB2J-0.7.4rc3/TB2J/kpoints.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    18281 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/TB2J/manager.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    17881 2022-04-19 19:02:24.000000 TB2J-0.7.4rc3/TB2J/myTB.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     4722 2021-10-04 10:59:57.000000 TB2J-0.7.4rc3/TB2J/orbmap.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     4092 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/pauli.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1223 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/pert.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1435 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/plot.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1126 2021-05-27 13:46:56.000000 TB2J-0.7.4rc3/TB2J/rotate_atoms.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10355 2022-04-19 18:50:05.000000 TB2J-0.7.4rc3/TB2J/sisl_wrapper.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/TB2J/spinham/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2234 2021-09-17 19:59:43.000000 TB2J-0.7.4rc3/TB2J/spinham/base_parser.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      741 2020-07-08 14:12:19.000000 TB2J-0.7.4rc3/TB2J/spinham/constants.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    13322 2022-04-19 18:57:57.000000 TB2J-0.7.4rc3/TB2J/spinham/hamiltonian.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     9870 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/TB2J/spinham/hamiltonian_terms.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     7011 2022-04-19 19:03:09.000000 TB2J-0.7.4rc3/TB2J/spinham/plot.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2176 2021-10-04 10:59:57.000000 TB2J-0.7.4rc3/TB2J/spinham/qsolver.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2238 2021-02-01 11:14:39.000000 TB2J-0.7.4rc3/TB2J/spinham/spin_api.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10923 2022-04-19 19:03:17.000000 TB2J-0.7.4rc3/TB2J/spinham/spin_xml.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    12149 2021-03-23 09:04:55.000000 TB2J-0.7.4rc3/TB2J/spinham/supercell.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    19588 2022-06-29 10:42:47.000000 TB2J-0.7.4rc3/TB2J/supercell.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3896 2022-04-19 19:03:29.000000 TB2J-0.7.4rc3/TB2J/utest.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     9358 2022-04-19 18:53:16.000000 TB2J-0.7.4rc3/TB2J/utils.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      276 2022-04-13 09:35:56.000000 TB2J-0.7.4rc3/TB2J/versioninfo.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/TB2J/wannier/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       70 2021-10-04 10:59:57.000000 TB2J-0.7.4rc3/TB2J/wannier/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3664 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/TB2J/wannier/w90_parser.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.593678 TB2J-0.7.4rc3/TB2J.egg-info/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1257 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/PKG-INFO
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1402 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/SOURCES.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        1 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/dependency_links.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       68 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/requires.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        5 2022-06-30 13:33:31.000000 TB2J-0.7.4rc3/TB2J.egg-info/top_level.txt
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2022-06-30 13:33:31.597678 TB2J-0.7.4rc3/scripts/
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1663 2021-03-27 13:32:37.000000 TB2J-0.7.4rc3/scripts/TB2J_downfold.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1185 2022-06-29 10:14:59.000000 TB2J-0.7.4rc3/scripts/TB2J_eigen.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     3379 2022-03-01 14:30:46.000000 TB2J-0.7.4rc3/scripts/TB2J_magnon.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     1277 2021-02-01 11:14:39.000000 TB2J-0.7.4rc3/scripts/TB2J_merge.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)      715 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/scripts/TB2J_rotate.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     5083 2022-02-27 23:27:25.000000 TB2J-0.7.4rc3/scripts/siesta2J.py
+-rwxrwxr-x   0 hexu      (1000) hexu      (1000)     7092 2021-11-24 10:31:21.000000 TB2J-0.7.4rc3/scripts/wann2J.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2022-06-30 13:33:31.601678 TB2J-0.7.4rc3/setup.cfg
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     1789 2022-06-30 13:33:28.000000 TB2J-0.7.4rc3/setup.py
```

### Comparing `TB2J-0.7.4rc2/LICENSE` & `TB2J-0.7.4rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/PKG-INFO` & `TB2J-0.7.4rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.4rc2
+Version: 0.7.4rc3
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.4rc2/README.md` & `TB2J-0.7.4rc3/README.md`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/Jdownfolder.py` & `TB2J-0.7.4rc3/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/Jtensor.py` & `TB2J-0.7.4rc3/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/Oiju.py` & `TB2J-0.7.4rc3/TB2J/Oiju.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/Oiju_epc.py` & `TB2J-0.7.4rc3/TB2J/Oiju_epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/citation.py` & `TB2J-0.7.4rc3/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/contour.py` & `TB2J-0.7.4rc3/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/cut_cell.py` & `TB2J-0.7.4rc3/TB2J/cut_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     :param path: the original TB2J_results path
     :param output_path: the output path.
     :param sc_matrix: the matrix which maps the primitive cell to supercell.
     :param origin: the origin of the primitive cell.
     :param thr: the atoms which the reduced position is within -thr to 1.0+thr are considered as inside the primitive atoms
     :returns:
     """
-
+    sc_matrix = np.asarray(sc_matrix, dtype=int)
     sc_excparams = SpinIO.load_pickle(path=path, fname='TB2J.pickle')
     sc_atoms = sc_excparams.atoms
     uc_atoms, ids = find_primitive_cell(sc_atoms,
                                         sc_matrix,
                                         origin_atom_id=origin_atom_id,
                                         thr=thr,
                                         perfect=False)
@@ -65,18 +65,18 @@
 
     uc_exc.write_all(output_path)
 
 
 def run_cut_cell(
     path="TB2J_results",
     output_path="./TB2J_cutted",
-    sc_matrix=[[1, 1, 0], [-1, 1, 0], [0, 0, 2]],
+    sc_matrix=np.array([[1, 1, 0], [-1, 1, 0], [0, 0, 2]]),
 ):
-    cut_cell_exchange(path,
-                      output_path,
-                      np.array(sc_matrix),
-                      origin_atom_id=0,
-                      thr=1e-19)
+    cut_cell(path,
+             output_path,
+             np.array(sc_matrix),
+             origin_atom_id=0,
+             thr=1e-19)
 
 
 if __name__ == "__main__":
     run_cut_cell()
```

### Comparing `TB2J-0.7.4rc2/TB2J/epc.py` & `TB2J-0.7.4rc3/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/exchange.py` & `TB2J-0.7.4rc3/TB2J/exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/exchangeCL2.py` & `TB2J-0.7.4rc3/TB2J/exchangeCL2.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         """
         self.tbmodel_up, self.tbmodel_dn = tbmodels
         self.backend_name = self.tbmodel_up.name
         self.Gup = TBGreen(self.tbmodel_up,
                            self.kmesh,
                            self.efermi,
                            use_cache=self._use_cache,
-                           cache_path='TB2J_results/cache/spinup',
+                           #cache_path='TB2J_results/cache/spinup',
                            nproc=self.np)
         self.Gdn = TBGreen(self.tbmodel_dn,
                            self.kmesh,
                            self.efermi,
                            use_cache=self._use_cache,
-                           cache_path='TB2J_results/cache/spindn',
+                           #cache_path='TB2J_results/cache/spindn',
                            nproc=self.np)
         self.norb = self.Gup.norb
         self.nbasis = self.Gup.nbasis + self.Gdn.nbasis
         self.rho_up_list = []
         self.rho_dn_list = []
         self.rho_up = np.zeros((self.norb, self.norb), dtype=float)
         self.rho_dn = np.zeros((self.norb, self.norb), dtype=float)
@@ -203,17 +203,17 @@
             tdn = np.real(np.trace(self.rho_dn[np.ix_(iorb, iorb)]))
             self.charges[iatom] = tup + tdn
             self.spinat[iatom, 2] = tup - tdn
 
     def finalize(self):
         self.Gup.clean_cache()
         self.Gdn.clean_cache()
-        path = 'TB2J_results/cache'
-        if os.path.exists(path):
-            shutil.rmtree(path)
+        #path = 'TB2J_results/cache'
+        # if os.path.exists(path):
+        #    shutil.rmtree(path)
 
     def integrate(self, method="simpson"):
         if method == "trapezoidal":
             integrate = trapezoidal_nonuniform
         elif method == 'simpson':
             integrate = simpson_nonuniform
         self.rho_up = np.imag(integrate(self.contour.path, self.rho_up_list))
```

### Comparing `TB2J-0.7.4rc2/TB2J/exchange_pert.py` & `TB2J-0.7.4rc3/TB2J/exchange_pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/exchange_qspace.py` & `TB2J-0.7.4rc3/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/external/p_tqdm.py` & `TB2J-0.7.4rc3/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/gpaw_wrapper.py` & `TB2J-0.7.4rc3/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/green.py` & `TB2J-0.7.4rc3/TB2J/green.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/greentest.py` & `TB2J-0.7.4rc3/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_exchange/io_exchange.py` & `TB2J-0.7.4rc3/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.7.4rc3/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.7.4rc3/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_exchange/io_txt.py` & `TB2J-0.7.4rc3/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.7.4rc3/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_exchange/io_vampire.py` & `TB2J-0.7.4rc3/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/io_merge.py` & `TB2J-0.7.4rc3/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/kpoints.py` & `TB2J-0.7.4rc3/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/manager.py` & `TB2J-0.7.4rc3/TB2J/manager.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/myTB.py` & `TB2J-0.7.4rc3/TB2J/myTB.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/orbmap.py` & `TB2J-0.7.4rc3/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/pauli.py` & `TB2J-0.7.4rc3/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/pert.py` & `TB2J-0.7.4rc3/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/plot.py` & `TB2J-0.7.4rc3/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/rotate_atoms.py` & `TB2J-0.7.4rc3/TB2J/rotate_atoms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/sisl_wrapper.py` & `TB2J-0.7.4rc3/TB2J/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/base_parser.py` & `TB2J-0.7.4rc3/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/constants.py` & `TB2J-0.7.4rc3/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/hamiltonian.py` & `TB2J-0.7.4rc3/TB2J/spinham/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.7.4rc3/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/plot.py` & `TB2J-0.7.4rc3/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/qsolver.py` & `TB2J-0.7.4rc3/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/spin_api.py` & `TB2J-0.7.4rc3/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/spin_xml.py` & `TB2J-0.7.4rc3/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/spinham/supercell.py` & `TB2J-0.7.4rc3/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/supercell.py` & `TB2J-0.7.4rc3/TB2J/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/utest.py` & `TB2J-0.7.4rc3/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/utils.py` & `TB2J-0.7.4rc3/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J/wannier/w90_parser.py` & `TB2J-0.7.4rc3/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/TB2J.egg-info/PKG-INFO` & `TB2J-0.7.4rc3/TB2J.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.7.4rc2
+Version: 0.7.4rc3
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.7.4rc2/TB2J.egg-info/SOURCES.txt` & `TB2J-0.7.4rc3/TB2J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/TB2J_downfold.py` & `TB2J-0.7.4rc3/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/TB2J_eigen.py` & `TB2J-0.7.4rc3/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/TB2J_magnon.py` & `TB2J-0.7.4rc3/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/TB2J_merge.py` & `TB2J-0.7.4rc3/scripts/TB2J_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/TB2J_rotate.py` & `TB2J-0.7.4rc3/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/siesta2J.py` & `TB2J-0.7.4rc3/scripts/siesta2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/scripts/wann2J.py` & `TB2J-0.7.4rc3/scripts/wann2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.7.4rc2/setup.py` & `TB2J-0.7.4rc3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.7.4.rc2"
+__version__ = "0.7.4.rc3"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name='TB2J',
     version=__version__,
     description='TB2J: First principle to Heisenberg exchange J using tight-binding Green function method',
```

