# Comparing `tmp/mthree-2.3.0.tar.gz` & `tmp/mthree-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mthree-2.3.0.tar", last modified: Fri Mar 24 16:05:35 2023, max compression
+gzip compressed data, was "mthree-2.4.0.tar", last modified: Thu Apr 13 15:43:06 2023, max compression
```

## Comparing `mthree-2.3.0.tar` & `mthree-2.4.0.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:05:35.962284 mthree-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-24 16:05:18.000000 mthree-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-24 16:05:18.000000 mthree-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-24 16:05:35.962284 mthree-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-24 16:05:18.000000 mthree-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:05:35.954284 mthree-2.3.0/mthree/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)   157710 2023-03-24 16:05:30.000000 mthree-2.3.0/mthree/compute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/compute.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/compute.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   130970 2023-03-24 16:05:30.000000 mthree-2.3.0/mthree/converters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/converters.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/converters.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   922387 2023-03-24 16:05:31.000000 mthree-2.3.0/mthree/expval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/expval.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   819866 2023-03-24 16:05:32.000000 mthree-2.3.0/mthree/hamming.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/hamming.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   979501 2023-03-24 16:05:33.000000 mthree-2.3.0/mthree/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/matrix.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1001414 2023-03-24 16:05:34.000000 mthree-2.3.0/mthree/matvec.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/matvec.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    32457 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/mitigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)   182341 2023-03-24 16:05:34.000000 mthree-2.3.0/mthree/probability.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/probability.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:05:35.962284 mthree-2.3.0/mthree/test/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   888690 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree/test/column_testing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/column_testing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   209920 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree/test/converters_testing.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/converters_testing.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:05:35.962284 mthree-2.3.0/mthree/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/data/8Qcal_Hanoi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_balanced_cals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_default_shots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_expvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_extra_cals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_faulty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_hamming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_list_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_marginals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_matvec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_meas_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_odd_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_quasi_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_qubits_from_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_reduced_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_sdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/test/test_v2_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-03-24 16:05:18.000000 mthree-2.3.0/mthree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-24 16:05:29.000000 mthree-2.3.0/mthree/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:05:35.954284 mthree-2.3.0/mthree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-24 16:05:35.000000 mthree-2.3.0/mthree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 16:05:18.000000 mthree-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 16:05:18.000000 mthree-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 16:05:35.962284 mthree-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-03-24 16:05:18.000000 mthree-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.861947 mthree-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-13 15:42:48.000000 mthree-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 15:42:48.000000 mthree-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-13 15:43:06.861947 mthree-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-13 15:42:48.000000 mthree-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.857947 mthree-2.4.0/mthree/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157773 2023-04-13 15:43:01.000000 mthree-2.4.0/mthree/compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/compute.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/compute.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   131033 2023-04-13 15:43:01.000000 mthree-2.4.0/mthree/converters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/converters.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/converters.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   924041 2023-04-13 15:43:02.000000 mthree-2.4.0/mthree/expval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/expval.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   819929 2023-04-13 15:43:02.000000 mthree-2.4.0/mthree/hamming.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/hamming.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   981155 2023-04-13 15:43:04.000000 mthree-2.4.0/mthree/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/matrix.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1003068 2023-04-13 15:43:05.000000 mthree-2.4.0/mthree/matvec.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/matvec.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    34995 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182404 2023-04-13 15:43:05.000000 mthree-2.4.0/mthree/probability.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/probability.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.861947 mthree-2.4.0/mthree/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   890344 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree/test/column_testing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/column_testing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   209983 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree/test/converters_testing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/converters_testing.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.861947 mthree-2.4.0/mthree/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/data/8Qcal_Hanoi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_balanced_cals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_default_shots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_expvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_extra_cals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_faulty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_hamming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_inoperable_qubits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_list_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_marginals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_meas_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_multi_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_odd_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_quasi_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_qubits_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_reduced_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_sdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/test/test_v2_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-13 15:42:48.000000 mthree-2.4.0/mthree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 15:43:00.000000 mthree-2.4.0/mthree/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:43:06.857947 mthree-2.4.0/mthree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 15:43:06.000000 mthree-2.4.0/mthree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 15:42:48.000000 mthree-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 15:42:48.000000 mthree-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:43:06.861947 mthree-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-13 15:42:48.000000 mthree-2.4.0/setup.py
```

### Comparing `mthree-2.3.0/LICENSE.txt` & `mthree-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/PKG-INFO` & `mthree-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mthree
-Version: 2.3.0
+Version: 2.4.0
 Summary: M3: Matrix-free measurement mitigation
 Home-page: UNKNOWN
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,15 +32,15 @@
 
 Matrix-free Measurement Mitigation (M3).
 
 M3 is a measurement mitigation technique that solves for corrected measurement probabilities using a dimensionality reduction step followed by either direct LU factorization or a preconditioned iterative method that nominally converges in O(1) steps, and can be computed in parallel. For example, M3 can compute corrections on 42 qubit GHZ problems in under two seconds on a quad-core machine (depending on the number of unique bitstrings in the output).
 
 ## Documentation
 
-[Online Documentation @ Qiskit.org](https://qiskit.org/documentation/partners/mthree/)
+[Online Documentation @ Qiskit.org](https://qiskit.org/ecosystem/mthree/)
 
 ## Installation
 
 You can `pip` install M3 in serial mode using PyPi via:
 
 ```bash
 pip install mthree
```

### Comparing `mthree-2.3.0/README.md` & `mthree-2.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Matrix-free Measurement Mitigation (M3).
 
 M3 is a measurement mitigation technique that solves for corrected measurement probabilities using a dimensionality reduction step followed by either direct LU factorization or a preconditioned iterative method that nominally converges in O(1) steps, and can be computed in parallel. For example, M3 can compute corrections on 42 qubit GHZ problems in under two seconds on a quad-core machine (depending on the number of unique bitstrings in the output).
 
 ## Documentation
 
-[Online Documentation @ Qiskit.org](https://qiskit.org/documentation/partners/mthree/)
+[Online Documentation @ Qiskit.org](https://qiskit.org/ecosystem/mthree/)
 
 ## Installation
 
 You can `pip` install M3 in serial mode using PyPi via:
 
 ```bash
 pip install mthree
```

### Comparing `mthree-2.3.0/mthree/__init__.py` & `mthree-2.4.0/mthree/__init__.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/_helpers.py` & `mthree-2.4.0/mthree/_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Parameters:
         backend (BackendV1 or BackendV2): A Qiskit backend
 
     Returns:
         dict: Backend information
     """
     info_dict = {}
+    info_dict["inoperable_qubits"] = []
     if isinstance(backend, BackendV1):
         config = backend.configuration()
         info_dict["name"] = backend.name()
         info_dict["num_qubits"] = config.num_qubits
         info_dict["max_shots"] = config.max_shots
         info_dict["simulator"] = config.simulator
         # A hack for Qiskit/Terra #9572
@@ -47,8 +48,12 @@
         # No other way to tell outside of configuration
         # E.g. how to tell that ibmq_qasm_simulator is sim, but real devices not
         # outside of configuration?
         if hasattr(backend, 'configuration'):
             info_dict["simulator"] = backend.configuration().simulator
     else:
         raise M3Error('Invalid backend passed.')
+    # Look for faulty qubits.  Renaming to 'inoperable' here
+    if hasattr(backend, 'properties'):
+        if hasattr(backend.properties(), 'faulty_qubits'):
+            info_dict["inoperable_qubits"] = backend.properties().faulty_qubits()
     return info_dict
```

### Comparing `mthree-2.3.0/mthree/circuits.py` & `mthree-2.4.0/mthree/circuits.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/classes.py` & `mthree-2.4.0/mthree/classes.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/compute.cpp` & `mthree-2.4.0/mthree/compute.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -225,15 +225,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -264,15 +264,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
```

### Comparing `mthree-2.3.0/mthree/compute.pxd` & `mthree-2.4.0/mthree/compute.pxd`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/compute.pyx` & `mthree-2.4.0/mthree/compute.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/converters.cpp` & `mthree-2.4.0/mthree/converters.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -32,16 +32,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -226,15 +226,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -265,15 +265,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
```

### Comparing `mthree-2.3.0/mthree/converters.pxd` & `mthree-2.4.0/mthree/converters.pxd`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/converters.pyx` & `mthree-2.4.0/mthree/converters.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/exceptions.py` & `mthree-2.4.0/mthree/exceptions.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/expval.cpp` & `mthree-2.4.0/mthree/expval.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -38,16 +38,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -232,15 +232,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -271,15 +271,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2104,20 +2104,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -19153,52 +19161,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -20428,28 +20451,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22182,44 +22205,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `mthree-2.3.0/mthree/expval.pyx` & `mthree-2.4.0/mthree/expval.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/hamming.cpp` & `mthree-2.4.0/mthree/hamming.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -225,15 +225,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -264,15 +264,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -18017,28 +18017,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `mthree-2.3.0/mthree/hamming.pyx` & `mthree-2.4.0/mthree/hamming.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/matrix.cpp` & `mthree-2.4.0/mthree/matrix.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -38,16 +38,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -232,15 +232,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -271,15 +271,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2117,20 +2117,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -20336,52 +20344,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -21737,28 +21760,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -23179,44 +23202,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `mthree-2.3.0/mthree/matrix.pyx` & `mthree-2.4.0/mthree/matrix.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/matvec.cpp` & `mthree-2.4.0/mthree/matvec.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -38,16 +38,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -232,15 +232,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -271,15 +271,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2113,20 +2113,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -21012,52 +21020,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -22337,28 +22360,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -23829,44 +23852,62 @@
     return -1;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `mthree-2.3.0/mthree/matvec.pyx` & `mthree-2.4.0/mthree/matvec.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/mitigation.py` & `mthree-2.4.0/mthree/mitigation.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,29 +19,34 @@
 
 import psutil
 import numpy as np
 import scipy.linalg as la
 import scipy.sparse.linalg as spla
 import orjson
 from qiskit import execute
-from qiskit.providers import Backend
+from qiskit.providers import Backend, BackendV2, BackendV1
 
-from mthree.circuits import (_tensor_meas_states, _marg_meas_states,
-                             balanced_cal_strings, balanced_cal_circuits)
+from mthree.circuits import (
+    _tensor_meas_states,
+    _marg_meas_states,
+    balanced_cal_strings,
+    balanced_cal_circuits,
+)
 from mthree.matrix import _reduced_cal_matrix, sdd_check
 from mthree.utils import counts_to_vector, vector_to_quasiprobs
 from mthree.norms import ainv_onenorm_est_lu, ainv_onenorm_est_iter
 from mthree.matvec import M3MatVec
 from mthree.exceptions import M3Error
 from mthree.classes import QuasiCollection
 from ._helpers import system_info
 
 
-class M3Mitigation():
+class M3Mitigation:
     """Main M3 calibration class."""
+
     def __init__(self, system=None, iter_threshold=4096):
         """Main M3 calibration class.
 
         Parameters:
             system (Backend): Target backend.
             iter_threshold (int): Sets the bitstring count at which iterative mode
                                   is turned on (assuming reasonable error rates).
@@ -55,51 +60,53 @@
         """
         self.system = system
         self.system_info = system_info(system) if system else {}
         self.single_qubit_cals = None
         self.num_qubits = self.system_info["num_qubits"] if system else None
         self.iter_threshold = iter_threshold
         self.cal_shots = None
-        self.cal_method = 'balanced'
+        self.cal_method = "balanced"
         self.cal_timestamp = None  # The time at which the cals result was generated
         self.rep_delay = None
         # attributes for handling threaded job
         self._thread = None
         self._job_error = None
         # Holds the cals file
         self.cals_file = None
         # faulty qubits
         self.faulty_qubits = []
+        # The number of shots used for balanced denominator
+        self._balanced_shots = None
 
     def __getattribute__(self, attr):
         """This allows for checking the status of the threaded cals call
 
         For certain attr this will join the thread and/or raise an error.
         """
-        __dict__ = super().__getattribute__('__dict__')
+        __dict__ = super().__getattribute__("__dict__")
         if attr in __dict__:
-            if attr in ['single_qubit_cals']:
+            if attr in ["single_qubit_cals"]:
                 self._thread_check()
         return super().__getattribute__(attr)
 
     def _form_cals(self, qubits):
         """Form the 1D cals array from tensored cals data
 
         Parameters:
             qubits (array_like): The qubits to calibrate over.
 
         Returns:
             ndarray: 1D Array of float cals data.
         """
         qubits = np.asarray(qubits, dtype=int)
-        cals = np.zeros(4*qubits.shape[0], dtype=float)
+        cals = np.zeros(4 * qubits.shape[0], dtype=float)
 
         # Reverse index qubits for easier indexing later
         for kk, qubit in enumerate(qubits[::-1]):
-            cals[4*kk:4*kk+4] = self.single_qubit_cals[qubit].ravel()
+            cals[4 * kk: 4 * kk + 4] = self.single_qubit_cals[qubit].ravel()
         return cals
 
     def _check_sdd(self, counts, qubits, distance=None):
         """Checks if reduced A-matrix is SDD or not
 
         Parameters:
             counts (dict): Dictionary of counts.
@@ -116,38 +123,52 @@
         num_bits = len(qubits)
         if distance is None:
             distance = num_bits
 
         # check if len of bitstrings does not equal number of qubits passed.
         bitstring_len = len(next(iter(counts)))
         if bitstring_len != num_bits:
-            raise M3Error('Bitstring length ({}) does not match'.format(bitstring_len) +
-                          ' number of qubits ({})'.format(num_bits))
+            raise M3Error(
+                "Bitstring length ({}) does not match".format(bitstring_len)
+                + " number of qubits ({})".format(num_bits)
+            )
         cals = self._form_cals(qubits)
         return sdd_check(counts, cals, num_bits, distance)
 
-    def tensored_cals_from_system(self, qubits=None, shots=None,  method='balanced',
-                                  rep_delay=None, cals_file=None):
+    def tensored_cals_from_system(
+        self, qubits=None, shots=None, method="balanced", rep_delay=None, cals_file=None
+    ):
         """Grab calibration data from system.
 
         Parameters:
             qubits (array_like): Qubits over which to correct calibration data. Default is all.
             shots (int): Number of shots per circuit. Default is min(1e4, max_shots).
             method (str): Type of calibration, 'balanced' (default), 'independent', or 'marginal'.
             rep_delay (float): Delay between circuits on IBM Quantum backends.
             cals_file (str): Output path to write JSON calibration data to.
         """
         warnings.warn("This method is deprecated, use 'cals_from_system' instead.")
-        self.cals_from_system(qubits=qubits, shots=shots, method=method,
-                              rep_delay=rep_delay,
-                              cals_file=cals_file)
-
-    def cals_from_system(self, qubits=None, shots=None, method=None,
-                         initial_reset=False, rep_delay=None, cals_file=None,
-                         async_cal=False):
+        self.cals_from_system(
+            qubits=qubits,
+            shots=shots,
+            method=method,
+            rep_delay=rep_delay,
+            cals_file=cals_file,
+        )
+
+    def cals_from_system(
+        self,
+        qubits=None,
+        shots=None,
+        method=None,
+        initial_reset=False,
+        rep_delay=None,
+        cals_file=None,
+        async_cal=False,
+    ):
         """Grab calibration data from system.
 
         Parameters:
             qubits (array_like): Qubits over which to correct calibration data. Default is all.
             shots (int): Number of shots per circuit. min(1e4, max_shots).
             method (str): Type of calibration, 'balanced' (default for hardware),
                          'independent' (default for simulators), or 'marginal'.
@@ -156,76 +177,98 @@
             cals_file (str): Output path to write JSON calibration data to.
             async_cal (bool): Do calibration async in a separate thread, default is False.
 
         Raises:
             M3Error: Called while a calibration currently in progress.
         """
         if self._thread:
-            raise M3Error('Calibration currently in progress.')
+            raise M3Error("Calibration currently in progress.")
         if qubits is None:
             qubits = range(self.num_qubits)
+            # Remove faulty qubits if any
+            if any(self.system_info["inoperable_qubits"]):
+                qubits = list(
+                    filter(
+                        lambda item: item not in self.system_info["inoperable_qubits"],
+                        list(range(self.num_qubits)),
+                    )
+                )
+                warnings.warn(
+                    "Backend reporting inoperable qubits."
+                    + " Skipping calibrations for: {}".format(
+                        self.system_info["inoperable_qubits"]
+                    )
+                )
         if method is None:
-            method = 'balanced'
+            method = "balanced"
             if self.system_info["simulator"]:
-                method = 'independent'
+                method = "independent"
         self.cal_method = method
         self.rep_delay = rep_delay
         self.cals_file = cals_file
         self.cal_timestamp = None
-        self._grab_additional_cals(qubits, shots=shots,  method=method,
-                                   rep_delay=rep_delay, initial_reset=initial_reset,
-                                   async_cal=async_cal)
+        self._grab_additional_cals(
+            qubits,
+            shots=shots,
+            method=method,
+            rep_delay=rep_delay,
+            initial_reset=initial_reset,
+            async_cal=async_cal,
+        )
 
     def cals_from_file(self, cals_file):
         """Generated the calibration data from a previous runs output
 
         Parameters:
             cals_file (str): A string path to the saved counts file from an
                              earlier run.
         Raises:
                 M3Error: Calibration in progress.
         """
         if self._thread:
-            raise M3Error('Calibration currently in progress.')
-        with open(cals_file, 'r', encoding='utf-8') as fd:
+            raise M3Error("Calibration currently in progress.")
+        with open(cals_file, "r", encoding="utf-8") as fd:
             loaded_data = orjson.loads(fd.read())
             if isinstance(loaded_data, dict):
-                self.single_qubit_cals = [np.asarray(cal) if cal else None
-                                          for cal in loaded_data['cals']]
-                self.cal_timestamp = loaded_data['timestamp']
-                self.cal_shots = loaded_data.get('shots', None)
+                self.single_qubit_cals = [
+                    np.asarray(cal) if cal else None for cal in loaded_data["cals"]
+                ]
+                self.cal_timestamp = loaded_data["timestamp"]
+                self.cal_shots = loaded_data.get("shots", None)
             else:
-                warnings.warn('Loading from old M3 file format.  Save again to update.')
+                warnings.warn("Loading from old M3 file format.  Save again to update.")
                 self.cal_timestamp = None
                 self.cal_shots = None
-                self.single_qubit_cals = [np.asarray(cal) if cal else None
-                                          for cal in loaded_data]
+                self.single_qubit_cals = [
+                    np.asarray(cal) if cal else None for cal in loaded_data
+                ]
         self.faulty_qubits = _faulty_qubit_checker(self.single_qubit_cals)
 
     def cals_to_file(self, cals_file=None):
         """Save calibration data to JSON file.
 
         Parameters:
             cals_file (str): File in which to store calibrations.
 
         Raises:
             M3Error: Calibration filename missing.
             M3Error: Mitigator is not calibrated.
         """
         if not cals_file:
-            raise M3Error('cals_file must be explicitly set.')
+            raise M3Error("cals_file must be explicitly set.")
         if not self.single_qubit_cals:
-            raise M3Error('Mitigator is not calibrated.')
-        save_dict = {'timestamp': self.cal_timestamp,
-                     'backend': self.system_info.get("name", None),
-                     'shots': self.cal_shots,
-                     'cals': self.single_qubit_cals}
-        with open(cals_file, 'wb') as fd:
-            fd.write(orjson.dumps(save_dict,
-                                  option=orjson.OPT_SERIALIZE_NUMPY))
+            raise M3Error("Mitigator is not calibrated.")
+        save_dict = {
+            "timestamp": self.cal_timestamp,
+            "backend": self.system_info.get("name", None),
+            "shots": self.cal_shots,
+            "cals": self.single_qubit_cals,
+        }
+        with open(cals_file, "wb") as fd:
+            fd.write(orjson.dumps(save_dict, option=orjson.OPT_SERIALIZE_NUMPY))
 
     def tensored_cals_from_file(self, cals_file):
         """Generated the tensored calibration data from a previous runs output
 
         Parameters:
             cals_file (str): A string path to the saved counts file from an
                              earlier run.
@@ -243,29 +286,38 @@
 
         Raises:
             M3Error: If system set error if list length != num_qubits on system
         """
         matrices = list(matrices)
         if self.num_qubits:
             if len(matrices) != self.num_qubits:
-                raise M3Error('Input list length not equal to'
-                              ' number of qubits {} != {}'.format(len(matrices), self.num_qubits))
+                raise M3Error(
+                    "Input list length not equal to"
+                    " number of qubits {} != {}".format(len(matrices), self.num_qubits)
+                )
         self.single_qubit_cals = matrices
         self.faulty_qubits = _faulty_qubit_checker(self.single_qubit_cals)
 
     def cals_to_matrices(self):
         """Return single qubit cals as list of NumPy arrays
 
         Returns:
             list: List of cals as NumPy arrays
         """
         return self.single_qubit_cals.copy()
 
-    def _grab_additional_cals(self, qubits, shots=None, method='balanced', rep_delay=None,
-                              initial_reset=False, async_cal=False):
+    def _grab_additional_cals(
+        self,
+        qubits,
+        shots=None,
+        method="balanced",
+        rep_delay=None,
+        initial_reset=False,
+        async_cal=False,
+    ):
         """Grab missing calibration data from backend.
 
         Parameters:
             qubits (array_like): List of measured qubits.
             shots (int): Number of shots to take, min(1e4, max_shots).
             method (str): Type of calibration, 'balanced' (default), 'independent', or 'marginal'.
             rep_delay (float): Delay between circuits on IBM Quantum backends.
@@ -275,81 +327,137 @@
         Raises:
             M3Error: Backend not set.
             M3Error: Faulty qubits found.
         """
         if self.system is None:
             raise M3Error("System is not set.  Use 'cals_from_file'.")
         if self.single_qubit_cals is None:
-            self.single_qubit_cals = [None]*self.num_qubits
+            self.single_qubit_cals = [None] * self.num_qubits
         if self.cal_shots is None:
             if shots is None:
                 shots = min(self.system_info["max_shots"], 10000)
             self.cal_shots = shots
         if self.rep_delay is None:
             self.rep_delay = rep_delay
 
-        if method not in ['independent', 'balanced', 'marginal']:
-            raise M3Error('Invalid calibration method.')
+        if method not in ["independent", "balanced", "marginal"]:
+            raise M3Error("Invalid calibration method.")
 
         if isinstance(qubits, dict):
             # Assuming passed a mapping
             qubits = list(set(qubits.values()))
         elif isinstance(qubits, list):
             # Check if passed a list of mappings
             if isinstance(qubits[0], dict):
                 # Assuming list of mappings, need to get unique elements
                 _qubits = []
                 for item in qubits:
                     _qubits.extend(list(set(item.values())))
                 qubits = list(set(_qubits))
 
+        # Do check for inoperable qubits here
+        inoperable_overlap = list(
+            set(qubits) & set(self.system_info["inoperable_qubits"])
+        )
+        if any(inoperable_overlap):
+            raise M3Error(
+                "Attempting to calibrate inoperable qubits: {}".format(
+                    inoperable_overlap
+                )
+            )
+
         num_cal_qubits = len(qubits)
         cal_strings = []
         # shots is needed here because balanced cals will use a value
         # different from cal_shots
         shots = self.cal_shots
-        if method == 'marginal':
-            trans_qcs = _marg_meas_states(qubits, self.num_qubits,
-                                          initial_reset=initial_reset)
-
-        elif method == 'balanced':
+        if method == "marginal":
+            trans_qcs = _marg_meas_states(
+                qubits, self.num_qubits, initial_reset=initial_reset
+            )
+        elif method == "balanced":
             cal_strings = balanced_cal_strings(num_cal_qubits)
-            trans_qcs = balanced_cal_circuits(cal_strings, qubits,
-                                              self.num_qubits,
-                                              initial_reset=initial_reset)
-            shots = (self.cal_shots + 1) // num_cal_qubits
+            trans_qcs = balanced_cal_circuits(
+                cal_strings, qubits, self.num_qubits, initial_reset=initial_reset
+            )
+            shots = self.cal_shots // num_cal_qubits
+            if self.cal_shots / num_cal_qubits != shots:
+                shots += 1
+            self._balanced_shots = shots * num_cal_qubits
         # Independent
         else:
             trans_qcs = []
             for kk in qubits:
-                trans_qcs.extend(_tensor_meas_states(kk, self.num_qubits,
-                                                     initial_reset=initial_reset))
-
+                trans_qcs.extend(
+                    _tensor_meas_states(
+                        kk, self.num_qubits, initial_reset=initial_reset
+                    )
+                )
+
+        num_circs = len(trans_qcs)
+        # check for max number of circuits per job
+        if isinstance(self.system, BackendV1):
+            # Aer simulator has no 'max_experiments'
+            max_circuits = getattr(self.system.configuration(), "max_experiments", 300)
+        elif isinstance(self.system, BackendV2):
+            max_circuits = self.system.max_circuits
+            # Needed for https://github.com/Qiskit/qiskit-terra/issues/9947
+            if max_circuits is None:
+                max_circuits = 300
+        else:
+            raise M3Error("Unknown backend type")
+        # Determine the number of jobs required
+        num_jobs = num_circs // max_circuits + 1
+        # Get the slice length
+        circ_slice = num_circs // num_jobs + 1
+        circs_list = [
+            trans_qcs[kk * circ_slice: (kk + 1) * circ_slice]
+            for kk in range(num_jobs - 1)
+        ] + [trans_qcs[(num_jobs - 1) * circ_slice:]]
+        # Do job submission here
         # This Backend check is here for Qiskit direct access.  Should be removed later.
+        jobs = []
         if not isinstance(self.system, Backend):
-            job = execute(trans_qcs, self.system, optimization_level=0,
-                          shots=shots, rep_delay=self.rep_delay)
+            for circs in circs_list:
+                _job = execute(
+                    circs,
+                    self.system,
+                    optimization_level=0,
+                    shots=shots,
+                    rep_delay=self.rep_delay,
+                )
+                jobs.append(_job)
         else:
-            job = self.system.run(trans_qcs, shots=shots, rep_delay=self.rep_delay)
+            for circs in circs_list:
+                _job = self.system.run(circs, shots=shots, rep_delay=self.rep_delay)
+                jobs.append(_job)
 
         # Execute job and cal building in new theread.
         self._job_error = None
         if async_cal:
-            thread = threading.Thread(target=_job_thread, args=(job, self, method, qubits,
-                                                                num_cal_qubits, cal_strings))
+            thread = threading.Thread(
+                target=_job_thread,
+                args=(jobs, self, qubits, num_cal_qubits, cal_strings),
+            )
             self._thread = thread
             self._thread.start()
         else:
-            _job_thread(job, self, method, qubits, num_cal_qubits, cal_strings)
+            _job_thread(jobs, self, qubits, num_cal_qubits, cal_strings)
 
-    def apply_correction(self, counts, qubits, distance=None,
-                         method='auto',
-                         max_iter=25, tol=1e-5,
-                         return_mitigation_overhead=False,
-                         details=False):
+    def apply_correction(
+        self,
+        counts,
+        qubits,
+        distance=None,
+        method="auto",
+        max_iter=25,
+        tol=1e-5,
+        return_mitigation_overhead=False,
+        details=False,
+    ):
         """Applies correction to given counts.
 
         Parameters:
             counts (dict, list): Input counts dict or list of dicts.
             qubits (dict, array_like): Qubits on which measurements applied.
             distance (int): Distance to correct for. Default=num_bits
             method (str): Solution method: 'auto', 'direct' or 'iterative'.
@@ -363,64 +471,73 @@
                                                   input is a single dict, else a collection
                                                   of quasiprobabilities.
 
         Raises:
             M3Error: Bitstring length does not match number of qubits given.
         """
         if len(counts) == 0:
-            raise M3Error('Input counts is any empty dict.')
+            raise M3Error("Input counts is any empty dict.")
         given_list = False
         if isinstance(counts, (list, np.ndarray)):
             given_list = True
         if not given_list:
             counts = [counts]
 
         if isinstance(qubits, dict):
             # If a mapping was given for qubits
             qubits = [list(qubits.values())]
         elif not any(isinstance(qq, (list, tuple, np.ndarray, dict)) for qq in qubits):
-            qubits = [qubits]*len(counts)
+            qubits = [qubits] * len(counts)
         else:
             if isinstance(qubits[0], dict):
                 # assuming passed a list of mappings
                 qubits = [list(qu.values()) for qu in qubits]
 
         if len(qubits) != len(counts):
-            raise M3Error('Length of counts does not match length of qubits.')
+            raise M3Error("Length of counts does not match length of qubits.")
 
         # Check if using faulty qubits
         bad_qubits = set()
         for item in qubits:
             for qu in item:
                 if qu in self.faulty_qubits:
                     bad_qubits.add(qu)
         if any(bad_qubits):
-            raise M3Error('Using faulty qubits: {}'.format(bad_qubits))
+            raise M3Error("Using faulty qubits: {}".format(bad_qubits))
 
         quasi_out = []
         for idx, cnts in enumerate(counts):
-
             quasi_out.append(
-                self._apply_correction(cnts, qubits=qubits[idx],
-                                       distance=distance,
-                                       method=method,
-                                       max_iter=max_iter, tol=tol,
-                                       return_mitigation_overhead=return_mitigation_overhead,
-                                       details=details)
-                            )
+                self._apply_correction(
+                    cnts,
+                    qubits=qubits[idx],
+                    distance=distance,
+                    method=method,
+                    max_iter=max_iter,
+                    tol=tol,
+                    return_mitigation_overhead=return_mitigation_overhead,
+                    details=details,
+                )
+            )
 
         if not given_list:
             return quasi_out[0]
         return QuasiCollection(quasi_out)
 
-    def _apply_correction(self, counts, qubits, distance=None,
-                          method='auto',
-                          max_iter=25, tol=1e-5,
-                          return_mitigation_overhead=False,
-                          details=False):
+    def _apply_correction(
+        self,
+        counts,
+        qubits,
+        distance=None,
+        method="auto",
+        max_iter=25,
+        tol=1e-5,
+        return_mitigation_overhead=False,
+        details=False,
+    ):
         """Applies correction to given counts.
 
         Parameters:
             counts (dict): Input counts dict.
             qubits (array_like): Qubits on which measurements applied.
             distance (int): Distance to correct for. Default=num_bits
             method (str): Solution method: 'auto', 'direct' or 'iterative'.
@@ -444,86 +561,101 @@
         num_elems = len(counts)
         if distance is None:
             distance = num_bits
 
         # check if len of bitstrings does not equal number of qubits passed.
         bitstring_len = len(next(iter(counts)))
         if bitstring_len != num_bits:
-            raise M3Error('Bitstring length ({}) does not match'.format(bitstring_len) +
-                          ' number of qubits ({})'.format(num_bits))
+            raise M3Error(
+                "Bitstring length ({}) does not match".format(bitstring_len)
+                + " number of qubits ({})".format(num_bits)
+            )
 
         # Check if no cals done yet
         if self.single_qubit_cals is None:
-            warnings.warn('No calibration data. Calibrating: {}'.format(qubits))
+            warnings.warn("No calibration data. Calibrating: {}".format(qubits))
             self._grab_additional_cals(qubits, method=self.cal_method)
 
         # Check if one or more new qubits need to be calibrated.
         missing_qubits = [qq for qq in qubits if self.single_qubit_cals[qq] is None]
         if any(missing_qubits):
-            warnings.warn('Computing missing calibrations for qubits: {}'.format(missing_qubits))
+            warnings.warn(
+                "Computing missing calibrations for qubits: {}".format(missing_qubits)
+            )
             self._grab_additional_cals(missing_qubits, method=self.cal_method)
 
-        if method == 'auto':
+        if method == "auto":
             current_free_mem = psutil.virtual_memory().available / 1024**3
             # First check if direct method can be run
-            if num_elems <= self.iter_threshold \
-                    and ((num_elems**2+num_elems)*8/1024**3 < current_free_mem/2):
-                method = 'direct'
+            if num_elems <= self.iter_threshold and (
+                (num_elems**2 + num_elems) * 8 / 1024**3 < current_free_mem / 2
+            ):
+                method = "direct"
             else:
-                method = 'iterative'
+                method = "iterative"
 
-        if method == 'direct':
+        if method == "direct":
             st = perf_counter()
-            mit_counts, col_norms, gamma = self._direct_solver(counts, qubits, distance,
-                                                               return_mitigation_overhead)
-            dur = perf_counter()-st
+            mit_counts, col_norms, gamma = self._direct_solver(
+                counts, qubits, distance, return_mitigation_overhead
+            )
+            dur = perf_counter() - st
             mit_counts.shots = shots
             if gamma is not None:
                 mit_counts.mitigation_overhead = gamma * gamma
             if details:
-                info = {'method': 'direct', 'time': dur, 'dimension': num_elems}
-                info['col_norms'] = col_norms
+                info = {"method": "direct", "time": dur, "dimension": num_elems}
+                info["col_norms"] = col_norms
                 return mit_counts, info
             return mit_counts
 
-        elif method == 'iterative':
+        elif method == "iterative":
             iter_count = np.zeros(1, dtype=int)
 
             def callback(_):
                 iter_count[0] += 1
 
             if details:
                 st = perf_counter()
-                mit_counts, col_norms, gamma = self._matvec_solver(counts,
-                                                                   qubits,
-                                                                   distance,
-                                                                   tol,
-                                                                   max_iter,
-                                                                   1,
-                                                                   callback,
-                                                                   return_mitigation_overhead)
-                dur = perf_counter()-st
+                mit_counts, col_norms, gamma = self._matvec_solver(
+                    counts,
+                    qubits,
+                    distance,
+                    tol,
+                    max_iter,
+                    1,
+                    callback,
+                    return_mitigation_overhead,
+                )
+                dur = perf_counter() - st
                 mit_counts.shots = shots
                 if gamma is not None:
                     mit_counts.mitigation_overhead = gamma * gamma
-                info = {'method': 'iterative', 'time': dur, 'dimension': num_elems}
-                info['iterations'] = iter_count[0]
-                info['col_norms'] = col_norms
+                info = {"method": "iterative", "time": dur, "dimension": num_elems}
+                info["iterations"] = iter_count[0]
+                info["col_norms"] = col_norms
                 return mit_counts, info
             # pylint: disable=unbalanced-tuple-unpacking
-            mit_counts, gamma = self._matvec_solver(counts, qubits, distance, tol,
-                                                    max_iter, 0, None,
-                                                    return_mitigation_overhead)
+            mit_counts, gamma = self._matvec_solver(
+                counts,
+                qubits,
+                distance,
+                tol,
+                max_iter,
+                0,
+                None,
+                return_mitigation_overhead,
+            )
             mit_counts.shots = shots
             if gamma is not None:
                 mit_counts.mitigation_overhead = gamma * gamma
             return mit_counts
 
         else:
-            raise M3Error('Invalid method: {}'.format(method))
+            raise M3Error("Invalid method: {}".format(method))
 
     def reduced_cal_matrix(self, counts, qubits, distance=None):
         """Return the reduced calibration matrix used in the solution.
 
         Parameters:
             counts (dict): Input counts dict.
             qubits (array_like): Qubits on which measurements applied.
@@ -542,49 +674,62 @@
         num_bits = len(qubits)
         if distance is None:
             distance = num_bits
 
         # check if len of bitstrings does not equal number of qubits passed.
         bitstring_len = len(next(iter(counts)))
         if bitstring_len != num_bits:
-            raise M3Error('Bitstring length ({}) does not match'.format(bitstring_len) +
-                          ' number of qubits ({})'.format(num_bits))
+            raise M3Error(
+                "Bitstring length ({}) does not match".format(bitstring_len)
+                + " number of qubits ({})".format(num_bits)
+            )
 
         cals = self._form_cals(qubits)
         A, counts, _ = _reduced_cal_matrix(counts, cals, num_bits, distance)
         return A, counts
 
-    def _direct_solver(self, counts, qubits, distance=None,
-                       return_mitigation_overhead=False):
+    def _direct_solver(
+        self, counts, qubits, distance=None, return_mitigation_overhead=False
+    ):
         """Apply the mitigation using direct LU factorization.
 
         Parameters:
             counts (dict): Input counts dict.
             qubits (int): Qubits over which to calibrate.
             distance (int): Distance to correct for. Default=num_bits
             return_mitigation_overhead (bool): Returns the mitigation overhead, default=False.
 
         Returns:
             QuasiDistribution: dict of Quasiprobabilites
         """
         cals = self._form_cals(qubits)
         num_bits = len(qubits)
-        A, sorted_counts, col_norms = _reduced_cal_matrix(counts, cals, num_bits, distance)
+        A, sorted_counts, col_norms = _reduced_cal_matrix(
+            counts, cals, num_bits, distance
+        )
         vec = counts_to_vector(sorted_counts)
         LU = la.lu_factor(A, check_finite=False)
         x = la.lu_solve(LU, vec, check_finite=False)
         gamma = None
         if return_mitigation_overhead:
             gamma = ainv_onenorm_est_lu(A, LU)
         out = vector_to_quasiprobs(x, sorted_counts)
         return out, col_norms, gamma
 
-    def _matvec_solver(self, counts, qubits, distance, tol=1e-5, max_iter=25,
-                       details=0, callback=None,
-                       return_mitigation_overhead=False):
+    def _matvec_solver(
+        self,
+        counts,
+        qubits,
+        distance,
+        tol=1e-5,
+        max_iter=25,
+        details=0,
+        callback=None,
+        return_mitigation_overhead=False,
+    ):
         """Compute solution using GMRES and Jacobi preconditioning.
 
         Parameters:
             counts (dict): Input counts dict.
             qubits (int): Qubits over which to calibrate.
             tol (float): Tolerance to use.
             max_iter (int): Maximum number of iterations to perform.
@@ -597,28 +742,37 @@
             QuasiDistribution: dict of Quasiprobabilites
 
         Raises:
             M3Error: Solver did not converge.
         """
         cals = self._form_cals(qubits)
         M = M3MatVec(dict(counts), cals, distance)
-        L = spla.LinearOperator((M.num_elems, M.num_elems),
-                                matvec=M.matvec, rmatvec=M.rmatvec)
+        L = spla.LinearOperator(
+            (M.num_elems, M.num_elems), matvec=M.matvec, rmatvec=M.rmatvec
+        )
         diags = M.get_diagonal()
 
         def precond_matvec(x):
             out = x / diags
             return out
 
         P = spla.LinearOperator((M.num_elems, M.num_elems), precond_matvec)
         vec = counts_to_vector(M.sorted_counts)
-        out, error = spla.gmres(L, vec, tol=tol, atol=tol, maxiter=max_iter,
-                                M=P, callback=callback)
+        out, error = spla.gmres(
+            L,
+            vec,
+            tol=tol,
+            atol=tol,
+            maxiter=max_iter,
+            M=P,
+            callback=callback,
+            callback_type="legacy",
+        )
         if error:
-            raise M3Error('GMRES did not converge: {}'.format(error))
+            raise M3Error("GMRES did not converge: {}".format(error))
 
         gamma = None
         if return_mitigation_overhead:
             gamma = ainv_onenorm_est_iter(M, tol=tol, max_iter=max_iter)
 
         quasi = vector_to_quasiprobs(out, M.sorted_counts)
         if details:
@@ -635,22 +789,24 @@
             list: List of qubit fidelities.
 
         Raises:
             M3Error: Mitigator is not calibrated.
             M3Error: Qubit indices out of range.
         """
         if self.single_qubit_cals is None:
-            raise M3Error('Mitigator is not calibrated')
+            raise M3Error("Mitigator is not calibrated")
 
         if qubits is None:
             qubits = range(self.num_qubits)
         else:
             outliers = [kk for kk in qubits if kk >= self.num_qubits]
             if any(outliers):
-                raise M3Error('One or more qubit indices out of range: {}'.format(outliers))
+                raise M3Error(
+                    "One or more qubit indices out of range: {}".format(outliers)
+                )
         fids = []
         for kk in qubits:
             qubit = self.single_qubit_cals[kk]
             if qubit is not None:
                 fids.append(np.mean(qubit.diagonal()))
             else:
                 fids.append(None)
@@ -664,98 +820,102 @@
         if self._thread and self._thread != threading.current_thread():
             self._thread.join()
             self._thread = None
         if self._job_error:
             raise self._job_error  # pylint: disable=raising-bad-type
 
 
-def _job_thread(job, mit, method, qubits, num_cal_qubits, cal_strings):
+def _job_thread(jobs, mit, qubits, num_cal_qubits, cal_strings):
     """Run the calibration job in a different thread and post-process
 
     Parameters:
+        jobs (list): A list of job instances
         mit (M3Mitigator): The mitigator instance
-        method (str): The type of calibration
         qubits (list): List of qubits used
         num_cal_qubits (int): Number of calibration qubits
         cal_strings (list): List of cal strings for balanced cals
     """
-    try:
-        res = job.result()
-    # pylint: disable=broad-except
-    except Exception as error:
-        mit._job_error = error
-        return
-    counts = res.get_counts()
+    counts = []
+    for job in jobs:
+        try:
+            res = job.result()
+        # pylint: disable=broad-except
+        except Exception as error:
+            mit._job_error = error
+            return
+        else:
+            _counts = res.get_counts()
+            counts.extend(_counts)
     # attach timestamp
     timestamp = res.date
     # Needed since Aer result date is str but IBMQ job is datetime
     if isinstance(timestamp, datetime.datetime):
         timestamp = timestamp.isoformat()
     # Go to UTC times because we are going to use this for
     # resultsDB storage as well
     dt = datetime.datetime.fromisoformat(timestamp)
     dt_utc = dt.astimezone(datetime.timezone.utc)
     mit.cal_timestamp = dt_utc.isoformat()
     # A list of qubits with bad meas cals
     bad_list = []
-    if method == 'independent':
+    if mit.cal_method == "independent":
         for idx, qubit in enumerate(qubits):
             mit.single_qubit_cals[qubit] = np.zeros((2, 2), dtype=float)
             # Counts 0 has all P00, P10 data, so do that here
-            prep0_counts = counts[2*idx]
-            P10 = prep0_counts.get('1', 0) / mit.cal_shots
-            P00 = 1-P10
+            prep0_counts = counts[2 * idx]
+            P10 = prep0_counts.get("1", 0) / mit.cal_shots
+            P00 = 1 - P10
             mit.single_qubit_cals[qubit][:, 0] = [P00, P10]
             # plus 1 here since zeros data at pos=0
-            prep1_counts = counts[2*idx+1]
-            P01 = prep1_counts.get('0', 0) / mit.cal_shots
-            P11 = 1-P01
+            prep1_counts = counts[2 * idx + 1]
+            P01 = prep1_counts.get("0", 0) / mit.cal_shots
+            P11 = 1 - P01
             mit.single_qubit_cals[qubit][:, 1] = [P01, P11]
             if P01 >= P00:
                 bad_list.append(qubit)
-    elif method == 'marginal':
+    elif mit.cal_method == "marginal":
         prep0_counts = counts[0]
         prep1_counts = counts[1]
         for idx, qubit in enumerate(qubits):
             mit.single_qubit_cals[qubit] = np.zeros((2, 2), dtype=float)
             count_vals = 0
-            index = num_cal_qubits-idx-1
+            index = num_cal_qubits - idx - 1
             for key, val in prep0_counts.items():
-                if key[index] == '0':
+                if key[index] == "0":
                     count_vals += val
             P00 = count_vals / mit.cal_shots
-            P10 = 1-P00
+            P10 = 1 - P00
             mit.single_qubit_cals[qubit][:, 0] = [P00, P10]
             count_vals = 0
             for key, val in prep1_counts.items():
-                if key[index] == '1':
+                if key[index] == "1":
                     count_vals += val
             P11 = count_vals / mit.cal_shots
-            P01 = 1-P11
+            P01 = 1 - P11
             mit.single_qubit_cals[qubit][:, 1] = [P01, P11]
             if P01 >= P00:
                 bad_list.append(qubit)
     # balanced calibration
     else:
         cals = [np.zeros((2, 2), dtype=float) for kk in range(num_cal_qubits)]
 
         for idx, count in enumerate(counts):
-
             target = cal_strings[idx][::-1]
             good_prep = np.zeros(num_cal_qubits, dtype=float)
-            denom = mit.cal_shots
+            # divide by 2 since total shots is double
+            denom = mit._balanced_shots
 
             for key, val in count.items():
                 key = key[::-1]
                 for kk in range(num_cal_qubits):
                     if key[kk] == target[kk]:
                         good_prep[kk] += val
 
             for kk, cal in enumerate(cals):
-                if target[kk] == '0':
+                if target[kk] == "0":
                     cal[0, 0] += good_prep[kk] / denom
                 else:
                     cal[1, 1] += good_prep[kk] / denom
 
         for cal in cals:
             cal[1, 0] = 1.0 - cal[0, 0]
             cal[0, 1] = 1.0 - cal[1, 1]
```

### Comparing `mthree-2.3.0/mthree/norms.py` & `mthree-2.4.0/mthree/norms.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/probability.cpp` & `mthree-2.4.0/mthree/probability.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -32,16 +32,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -226,15 +226,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -265,15 +265,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
```

### Comparing `mthree-2.3.0/mthree/probability.pyx` & `mthree-2.4.0/mthree/probability.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/column_testing.cpp` & `mthree-2.4.0/mthree/test/column_testing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -38,16 +38,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -232,15 +232,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -271,15 +271,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -2092,20 +2092,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -18672,52 +18680,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -20195,28 +20218,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -21503,44 +21526,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `mthree-2.3.0/mthree/test/column_testing.pyx` & `mthree-2.4.0/mthree/test/column_testing.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/converters_testing.cpp` & `mthree-2.4.0/mthree/test/converters_testing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
@@ -32,16 +32,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -226,15 +226,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -265,15 +265,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
```

### Comparing `mthree-2.3.0/mthree/test/converters_testing.pyx` & `mthree-2.4.0/mthree/test/converters_testing.pyx`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/data/8Qcal_Hanoi.json` & `mthree-2.4.0/mthree/test/data/8Qcal_Hanoi.json`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_balanced_cals.py` & `mthree-2.4.0/mthree/test/test_balanced_cals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_collections.py` & `mthree-2.4.0/mthree/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_columns.py` & `mthree-2.4.0/mthree/test/test_columns.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_converters.py` & `mthree-2.4.0/mthree/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_default_shots.py` & `mthree-2.4.0/mthree/test/test_default_shots.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_dynamic.py` & `mthree-2.4.0/mthree/test/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_expvals.py` & `mthree-2.4.0/mthree/test/test_expvals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_extra_cals.py` & `mthree-2.4.0/mthree/test/test_extra_cals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_faulty.py` & `mthree-2.4.0/mthree/test/test_faulty.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_file_io.py` & `mthree-2.4.0/mthree/test/test_file_io.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_full.py` & `mthree-2.4.0/mthree/test/test_full.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_grouping.py` & `mthree-2.4.0/mthree/test/test_grouping.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_hamming.py` & `mthree-2.4.0/mthree/test/test_hamming.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_list_inputs.py` & `mthree-2.4.0/mthree/test/test_list_inputs.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_marginals.py` & `mthree-2.4.0/mthree/test/test_marginals.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_matvec.py` & `mthree-2.4.0/mthree/test/test_matvec.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_meas_mapping.py` & `mthree-2.4.0/mthree/test/test_meas_mapping.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_methods.py` & `mthree-2.4.0/mthree/test/test_methods.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_odd_cases.py` & `mthree-2.4.0/mthree/test/test_odd_cases.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_probability.py` & `mthree-2.4.0/mthree/test/test_probability.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_quasi_attr.py` & `mthree-2.4.0/mthree/test/test_quasi_attr.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_qubits_from_mapping.py` & `mthree-2.4.0/mthree/test/test_qubits_from_mapping.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_reduced_matrix.py` & `mthree-2.4.0/mthree/test/test_reduced_matrix.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_sdd.py` & `mthree-2.4.0/mthree/test/test_sdd.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_sim.py` & `mthree-2.4.0/mthree/test/test_sim.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_threading.py` & `mthree-2.4.0/mthree/test/test_threading.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_utils.py` & `mthree-2.4.0/mthree/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/test/test_v2_backends.py` & `mthree-2.4.0/mthree/test/test_v2_backends.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree/utils.py` & `mthree-2.4.0/mthree/utils.py`

 * *Files identical despite different names*

### Comparing `mthree-2.3.0/mthree.egg-info/PKG-INFO` & `mthree-2.4.0/mthree.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mthree
-Version: 2.3.0
+Version: 2.4.0
 Summary: M3: Matrix-free measurement mitigation
 Home-page: UNKNOWN
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,15 +32,15 @@
 
 Matrix-free Measurement Mitigation (M3).
 
 M3 is a measurement mitigation technique that solves for corrected measurement probabilities using a dimensionality reduction step followed by either direct LU factorization or a preconditioned iterative method that nominally converges in O(1) steps, and can be computed in parallel. For example, M3 can compute corrections on 42 qubit GHZ problems in under two seconds on a quad-core machine (depending on the number of unique bitstrings in the output).
 
 ## Documentation
 
-[Online Documentation @ Qiskit.org](https://qiskit.org/documentation/partners/mthree/)
+[Online Documentation @ Qiskit.org](https://qiskit.org/ecosystem/mthree/)
 
 ## Installation
 
 You can `pip` install M3 in serial mode using PyPi via:
 
 ```bash
 pip install mthree
```

### Comparing `mthree-2.3.0/mthree.egg-info/SOURCES.txt` & `mthree-2.4.0/mthree.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -49,19 +49,21 @@
 mthree/test/test_expvals.py
 mthree/test/test_extra_cals.py
 mthree/test/test_faulty.py
 mthree/test/test_file_io.py
 mthree/test/test_full.py
 mthree/test/test_grouping.py
 mthree/test/test_hamming.py
+mthree/test/test_inoperable_qubits.py
 mthree/test/test_list_inputs.py
 mthree/test/test_marginals.py
 mthree/test/test_matvec.py
 mthree/test/test_meas_mapping.py
 mthree/test/test_methods.py
+mthree/test/test_multi_job.py
 mthree/test/test_odd_cases.py
 mthree/test/test_probability.py
 mthree/test/test_quasi_attr.py
 mthree/test/test_qubits_from_mapping.py
 mthree/test/test_reduced_matrix.py
 mthree/test/test_sdd.py
 mthree/test/test_sim.py
```

### Comparing `mthree-2.3.0/setup.py` & `mthree-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import subprocess
 import setuptools
 
 import numpy as np
 from Cython.Build import cythonize
 
 MAJOR = 2
-MINOR = 3
+MINOR = 4
 MICRO = 0
 
 ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 with open("requirements.txt") as f:
     REQUIREMENTS = f.read().splitlines()
```

