# Comparing `tmp/mlpro_mpps-1.0.1.tar.gz` & `tmp/mlpro_mpps-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro_mpps-1.0.1.tar", last modified: Mon Feb 27 15:26:58 2023, max compression
+gzip compressed data, was "mlpro_mpps-1.1.0.tar", last modified: Thu Apr 13 12:59:08 2023, max compression
```

## Comparing `mlpro_mpps-1.0.1.tar` & `mlpro_mpps-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.890575 mlpro_mpps-1.0.1/
--rw-rw-rw-   0        0        0    11591 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4069 2023-02-27 15:26:58.890575 mlpro_mpps-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3504 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      756 2023-02-27 15:26:58.895578 mlpro_mpps-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.844634 mlpro_mpps-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.853808 mlpro_mpps-1.0.1/src/mlpro_mpps/
--rw-rw-rw-   0        0        0        0 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/__init__.py
--rw-rw-rw-   0        0        0    50878 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/mpps.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.871578 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/
--rw-rw-rw-   0        0        0        2 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.881576 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/
--rw-rw-rw-   0        0        0    10928 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C001_Silo.py
--rw-rw-rw-   0        0        0     5581 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C002_Hopper.py
--rw-rw-rw-   0        0        0     8649 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C003_ConveyorBelt.py
--rw-rw-rw-   0        0        0     8020 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C004_VibratoryConveyor.py
--rw-rw-rw-   0        0        0     4866 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C005_RotaryFeeder.py
--rw-rw-rw-   0        0        0     8709 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C006_VacuumPump1.py
--rw-rw-rw-   0        0        0     4873 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C007_VacuumPump2.py
--rw-rw-rw-   0        0        0     5224 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C008_VacuumPump3.py
--rw-rw-rw-   0        0        0     4075 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C009_Inventory.py
--rw-rw-rw-   0        0        0     8236 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C010_SiloLoading.py
--rw-rw-rw-   0        0        0        2 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.885587 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/
--rw-rw-rw-   0        0        0     1941 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M001_Loading.py
--rw-rw-rw-   0        0        0     2026 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M002_Storing.py
--rw-rw-rw-   0        0        0     2014 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M003_Weighing.py
--rw-rw-rw-   0        0        0     1736 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M004_Filling.py
--rw-rw-rw-   0        0        0        2 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.887576 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mpps/
--rw-rw-rw-   0        0        0    11290 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mpps/PS001_bglp.py
--rw-rw-rw-   0        0        0        2 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mpps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.889575 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/rl_environment/
--rw-rw-rw-   0        0        0    16261 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/rl_environment/RL001_bglp.py
--rw-rw-rw-   0        0        0        2 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/src/mlpro_mpps/pool/rl_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.869603 mlpro_mpps-1.0.1/src/mlpro_mpps.egg-info/
--rw-rw-rw-   0        0        0     4069 2023-02-27 15:26:58.000000 mlpro_mpps-1.0.1/src/mlpro_mpps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2023-02-27 15:26:58.000000 mlpro_mpps-1.0.1/src/mlpro_mpps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 15:26:58.000000 mlpro_mpps-1.0.1/src/mlpro_mpps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-27 15:26:58.000000 mlpro_mpps-1.0.1/src/mlpro_mpps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-27 15:26:58.000000 mlpro_mpps-1.0.1/src/mlpro_mpps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-27 15:26:58.889575 mlpro_mpps-1.0.1/test/
--rw-rw-rw-   0        0        0     1215 2023-02-27 15:19:02.000000 mlpro_mpps-1.0.1/test/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.452777 mlpro_mpps-1.1.0/
+-rw-rw-rw-   0        0        0    11390 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5952 2023-04-13 12:59:08.452777 mlpro_mpps-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5320 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/README.md
+-rw-rw-rw-   0        0        0      103 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      756 2023-04-13 12:59:08.452777 mlpro_mpps-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.363162 mlpro_mpps-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.383701 mlpro_mpps-1.1.0/src/mlpro_mpps/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.415904 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/
+-rw-rw-rw-   0        0        0        1 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/__init__.py
+-rw-rw-rw-   0        0        0     5822 2023-03-28 15:03:05.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_001_set_up_components_and_modules_in_MPPS.py
+-rw-rw-rw-   0        0        0     3861 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_002_set_up_MPPS.py
+-rw-rw-rw-   0        0        0     8654 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_003_run_RL_on_BGLP_using_MPPS.py
+-rw-rw-rw-   0        0        0     8494 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_004_run_GT_on_BGLP_using_MPPS.py
+-rw-rw-rw-   0        0        0     8439 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_005_run_RL_on_LS_using_MPPS.py
+-rw-rw-rw-   0        0        0    15001 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_006_run_EA_on_LS_using_MPPS.py
+-rw-rw-rw-   0        0        0    24807 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/examples/howto_007_run_using_LS_MPPS_data_generation.py
+-rw-rw-rw-   0        0        0    49405 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/mpps.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.415904 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/
+-rw-rw-rw-   0        0        0        1 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.432560 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/
+-rw-rw-rw-   0        0        0    10650 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C001_Silo.py
+-rw-rw-rw-   0        0        0     5454 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C002_Hopper.py
+-rw-rw-rw-   0        0        0     8442 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C003_ConveyorBelt.py
+-rw-rw-rw-   0        0        0     7821 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C004_VibratoryConveyor.py
+-rw-rw-rw-   0        0        0     4760 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C005_RotaryFeeder.py
+-rw-rw-rw-   0        0        0     8498 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C006_VacuumPump1.py
+-rw-rw-rw-   0        0        0     4767 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C007_VacuumPump2.py
+-rw-rw-rw-   0        0        0     5099 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C008_VacuumPump3.py
+-rw-rw-rw-   0        0        0     3971 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C009_Inventory.py
+-rw-rw-rw-   0        0        0     8035 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C010_SiloLoading.py
+-rw-rw-rw-   0        0        0    11768 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS002_C001_Tank.py
+-rw-rw-rw-   0        0        0     7990 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS002_C002_Pump1.py
+-rw-rw-rw-   0        0        0     8072 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS002_C003_Pump2.py
+-rw-rw-rw-   0        0        0     8072 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS002_C004_Pump3.py
+-rw-rw-rw-   0        0        0        1 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.434112 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.436468 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/ea_environment/
+-rw-rw-rw-   0        0        0    15282 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/ea_environment/EA001_LS.py
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/ea_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.437733 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/rl_environment/
+-rw-rw-rw-   0        0        0    16026 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/rl_environment/RL001_BGLP.py
+-rw-rw-rw-   0        0        0    15282 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/rl_environment/RL002_LS.py
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/rl_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.441662 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/sl_environment/
+-rw-rw-rw-   0        0        0    15204 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/sl_environment/SL001_LS.py
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/sl_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.448886 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/
+-rw-rw-rw-   0        0        0     1895 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M001_Loading.py
+-rw-rw-rw-   0        0        0     1978 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M002_Storing.py
+-rw-rw-rw-   0        0        0     1966 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M003_Weighing.py
+-rw-rw-rw-   0        0        0     1694 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M004_Filling.py
+-rw-rw-rw-   0        0        0     1904 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS002_M001_Station.py
+-rw-rw-rw-   0        0        0        1 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.451566 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mpps/
+-rw-rw-rw-   0        0        0    10975 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mpps/PS001_BGLP.py
+-rw-rw-rw-   0        0        0     7150 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mpps/PS002_Liquid_Station.py
+-rw-rw-rw-   0        0        0        1 2023-03-28 14:46:26.000000 mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mpps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.401077 mlpro_mpps-1.1.0/src/mlpro_mpps.egg-info/
+-rw-rw-rw-   0        0        0     5952 2023-04-13 12:59:08.000000 mlpro_mpps-1.1.0/src/mlpro_mpps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2373 2023-04-13 12:59:08.000000 mlpro_mpps-1.1.0/src/mlpro_mpps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:59:08.000000 mlpro_mpps-1.1.0/src/mlpro_mpps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 12:59:08.000000 mlpro_mpps-1.1.0/src/mlpro_mpps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 12:59:08.000000 mlpro_mpps-1.1.0/src/mlpro_mpps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 12:59:08.452777 mlpro_mpps-1.1.0/test/
+-rw-rw-rw-   0        0        0     1499 2023-04-13 12:53:45.000000 mlpro_mpps-1.1.0/test/test_examples.py
```

### Comparing `mlpro_mpps-1.0.1/LICENSE` & `mlpro_mpps-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [2023] [South Westphalia University of Applied Sciences, Germany]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2023] [South Westphalia University of Applied Sciences, Germany]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `mlpro_mpps-1.0.1/setup.cfg` & `mlpro_mpps-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6c70 726f 5f6d 7070 730d 0a76   = mlpro_mpps..v
-00000020: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
+00000020: 6572 7369 6f6e 203d 2031 2e31 2e30 0d0a  ersion = 1.1.0..
 00000030: 6175 7468 6f72 203d 204d 4c50 726f 2054  author = MLPro T
 00000040: 6561 6d0d 0a61 7574 686f 725f 656d 6169  eam..author_emai
 00000050: 6c20 3d20 6d6c 7072 6f40 6c69 7374 656e  l = mlpro@listen
 00000060: 2e66 682d 7377 662e 6465 0d0a 6465 7363  .fh-swf.de..desc
 00000070: 7269 7074 696f 6e20 3d20 4d4c 5072 6f2d  ription = MLPro-
 00000080: 4d50 5053 202d 2041 2043 7573 746f 6d69  MPPS - A Customi
 00000090: 7a61 626c 6520 4d75 6c74 692d 5075 7270  zable Multi-Purp
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/mpps.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/mpps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1518 +1,1518 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps
-## -- Module  : mpps.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-22  0.0.0     SY/ML    Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Add p_setup on Component Class, debugging, restructuring
-## -- 2023-01-13  1.0.2     SY       Add documentation
-## -- 2023-01-16  1.0.3     SY       Update due to __call__ of TransferFunction
-## -- 2023-02-01  1.1.0     SY       Refactoring and adding functionalities
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.1.0 (2023-02-01)
-
-This module provides a multi-purpose environment for continuous and batch production systems with
-modular setting and high-flexibility.
-
-The users are able to develop and simulate their own production systems including setting up own
-actuators, reservoirs, processes, modules/stations, and components.
-We also provide the default implementations of actuators, reservoirs, components, processes and
-modules, which can be found in the pool of objects.
-
-To be noted, the usage of this simulation is not limited to machine learning tasks, but it also
-can be as a testing environment for any kind of simulations, including GT tasks, evolutionary
-algorithms, supervised learning, model predictive control, domain learning, transfer learning,
-and many more.
-"""
-
-
-from mlpro.rl.models import *
-from mlpro.bf.various import *
-from mlpro.bf.math import *
-from mlpro.bf.systems import *
-import numpy as np
-import random
-import uuid
-import math
-import matplotlib.pyplot as plt
-
-
-
-
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SimActuator(Actuator, ScientificObject):
-    """
-    This class serves as a base class of actuators in MPPS, which provides the main attributes of an
-    actuator in a simulation mode.
-    An actuator is a component of a machine that is responsible for moving and controlling a mechanism
-    or system.
-    
-    Parameters
-    ----------
-    p_name_short : str
-        Short name of dimension
-    p_base_set 
-        Base set of dimension. See constants C_BASE_SET_*. Default = C_BASE_SET_R.
-    p_name_long :str
-        Long name of dimension (optional)
-    p_name_latex : str
-        LaTeX name of dimension (optional)
-    p_unit : str
-        Unit (optional)
-    p_unit_latex : str
-        LaTeX code of unit (optional)
-    p_boundaries : List
-        List with minimum and maximum value (optional)
-    p_description : str
-        Description of dimension (optional)
-    p_symmetrical : bool
-        Information about the symmetry of the dimension (optional, default is False)
-    p_logging
-        Log level (see constants of class Log). Default: Log.C_LOG_ALL
-    p_kwargs : dict
-        Further keyword arguments
-        
-    Attributes
-    ----------
-    C_TYPE : str
-        Type of the base class. Default: 'SimActuator'.
-    C_NAME : str
-        Name of the actuator. Default:''.
-    """
-
-    C_TYPE = 'SimActuator'
-    C_NAME = ''
-
-    
-## -------------------------------------------------------------------------------------------------
-    def __init__(self, 
-                 p_name_short, 
-                 p_base_set=Dimension.C_BASE_SET_R, 
-                 p_name_long='', 
-                 p_name_latex='', 
-                 p_unit='',
-                 p_unit_latex='', 
-                 p_boundaries:list=[], 
-                 p_description='',
-                 p_symmetrical:bool=False,
-                 p_logging=Log.C_LOG_NOTHING,
-                 **p_kwargs):
-              
-        Actuator.__init__(self,
-                          p_name_short=p_name_short, 
-                          p_base_set=p_base_set, 
-                          p_name_long=p_name_long, 
-                          p_name_latex=p_name_latex, 
-                          p_unit=p_unit,
-                          p_unit_latex=p_unit_latex, 
-                          p_boundaries=p_boundaries, 
-                          p_description=p_description,
-                          p_symmetrical=p_symmetrical,
-                          p_logging=p_logging,
-                          p_kwargs=p_kwargs)
-        self._value = None
-        self._status = False
-            
-
-## -------------------------------------------------------------------------------------------------
-    def set_value(self, p_input) -> bool:
-        """
-        This method provides a functionality to set a value of the actuator.
-
-        Parameters
-        ----------
-        p_input : float
-            input parameters to set a value.
-
-        Returns
-        -------
-        bool
-            if set value is successful, then True. Otherwise False.
-        """
-        if p_input >= self.get_boundaries()[0] and p_input <= self.get_boundaries()[1]:
-            self._value = p_input
-            self._status = True
-            self.log(Log.C_LOG_TYPE_I, 'Actuator ' + self.get_name_short() + ' is updated.')
-            return True
-        else:
-            self.deactivate()
-            self.log(Log.C_LOG_TYPE_E, 'Actuator ' + self.get_name_short() + ' fails to be updated.')
-            return False
-            
-
-## -------------------------------------------------------------------------------------------------
-    def deactivate(self) -> bool:
-        """
-        This method provides a functionality to deactivate the actuator.
-
-        Returns
-        -------
-        bool
-            if deactivate is successful, then True. Otherwise False.
-        """
-        self._value = None
-        self._status = False
-        self.log(Log.C_LOG_TYPE_I, 'Actuator ' + self.get_name_short() + ' is deactivated.')
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def get_status(self) -> bool:
-        """
-        This method provides a functionality to get the status of the actuator.
-
-        Returns
-        -------
-        bool
-            Status is on/off. True means on, false means off.
-        """
-        return self._status
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def get_value(self):
-        """
-        This method provides a functionality to get the actual value of the actuator.
-
-        Returns
-        -------
-        value
-            The actual value of the actuator.
-        """
-        return self._value
-
-
-
-
-    
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SimSensor(Sensor, ScientificObject):
-    """
-    This class serves as a base class of sensors in MPPS, which provides the main attributes of a
-    sensor in a simulation mode.
-    A sensor is a component of a machine that is responsible for sensing the actual state of the
-    system.
-    
-    Parameters
-    ----------
-    p_name_short : str
-        Short name of dimension
-    p_base_set 
-        Base set of dimension. See constants C_BASE_SET_*. Default = C_BASE_SET_R.
-    p_name_long :str
-        Long name of dimension (optional)
-    p_name_latex : str
-        LaTeX name of dimension (optional)
-    p_unit : str
-        Unit (optional)
-    p_unit_latex : str
-        LaTeX code of unit (optional)
-    p_boundaries : List
-        List with minimum and maximum value (optional)
-    p_description : str
-        Description of dimension (optional)
-    p_symmetrical : bool
-        Information about the symmetry of the dimension (optional, default is False)
-    p_logging
-        Log level (see constants of class Log). Default: Log.C_LOG_ALL
-    p_kwargs : dict
-        Further keyword arguments
-        
-    Attributes
-    ----------
-    C_TYPE : str
-        Type of the base class. Default: 'SimSensor'.
-    C_NAME : str
-        Name of the sensor. Default:''.
-    """
-
-    C_TYPE = 'SimSensor'
-    C_NAME = ''
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self, 
-                 p_name_short, 
-                 p_base_set=Dimension.C_BASE_SET_R, 
-                 p_name_long='', 
-                 p_name_latex='', 
-                 p_unit='',
-                 p_unit_latex='', 
-                 p_boundaries:list=[], 
-                 p_description='',
-                 p_symmetrical:bool=False,
-                 p_logging=Log.C_LOG_NOTHING,
-                 **p_kwargs):
-              
-        Sensor.__init__(self,
-                        p_name_short=p_name_short, 
-                        p_base_set=p_base_set, 
-                        p_name_long=p_name_long, 
-                        p_name_latex=p_name_latex, 
-                        p_unit=p_unit,
-                        p_unit_latex=p_unit_latex, 
-                        p_boundaries=p_boundaries, 
-                        p_description=p_description,
-                        p_symmetrical=p_symmetrical,
-                        p_logging=p_logging,
-                        p_kwargs=p_kwargs)
-        self._value = None
-        self._status = True
-        self._function = self._setup_function()
-            
-
-## -------------------------------------------------------------------------------------------------
-    def set_value(self, p_input) -> bool:
-        """
-        This method provides a functionality to set a value of the sensor to be read.
-
-        Parameters
-        ----------
-        p_input : float
-            input parameters to set a value.
-
-        Returns
-        -------
-        bool
-            if set value is successful, then True. Otherwise False.
-        """
-        if p_input >= self.get_boundaries()[0] and p_input <= self.get_boundaries()[1]:
-            self._value = p_input
-            self._status = True
-            self.log(Log.C_LOG_TYPE_I, 'Sensor ' + self.get_name_short() + ' is updated.')
-            return True
-        else:
-            self.deactivate()
-            self.log(Log.C_LOG_TYPE_E, 'Sensor ' + self.get_name_short() + ' fails to be updated.')
-            return False
-            
-
-## -------------------------------------------------------------------------------------------------
-    def deactivate(self) -> bool:
-        """
-        This method provides a functionality to deactivate the sensor.
-
-        Returns
-        -------
-        bool
-            if deactivate is successful, then True. Otherwise False.
-        """
-        self._value = None
-        self._status = False
-        self.log(Log.C_LOG_TYPE_I, 'Sensor ' + self.get_name_short() + ' is deactivated.')
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def get_status(self) -> bool:
-        """
-        This method provides a functionality to get the status of the related components.
-
-        Returns
-        -------
-        bool
-            Status is on/off. True means on, false means off.
-
-        """
-        return self._status
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def get_value(self):
-        """
-        This method provides a functionality to get the actual value read by the sensor.
-
-        Returns
-        -------
-        value
-            The actual value of the state.
-        """
-        return self._value
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        """
-        This is a custom method, in which a specific TransferFunction object is incorporated.
-        The TransferFunction object describes how the sensor obtain the actual information with
-        respect to input signals according to a mathematical calculation.
-
-        Returns
-        -------
-        TransferFunction
-            TransferFunction object.
-        """
-        raise NotImplementedError
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def simulate(self, p_input_signal, p_range=None) -> bool:
-        """
-        This method provides a functionality to simulate the sensor.
-
-        Returns
-        -------
-        bool
-            True means successful, otherwise False.
-        """
-        output = self._function(p_input_signal, p_range)
-        self.set_value(output)
-        return True
-
-
-
-    
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SimState(Dimension, ScientificObject):
-    """
-    This class serves as a base class of states (extra informations) for a component in MPPS,
-    which provides the main attributes of a component state in a simulation mode.
-    This could be included the dynamics of the systems that can not be read by the sensors but
-    important for the simulations or triggering other components.
-    
-    Parameters
-    ----------
-    p_name_short : str
-        Short name of dimension
-    p_base_set 
-        Base set of dimension. See constants C_BASE_SET_*. Default = C_BASE_SET_R.
-    p_name_long :str
-        Long name of dimension (optional)
-    p_name_latex : str
-        LaTeX name of dimension (optional)
-    p_unit : str
-        Unit (optional)
-    p_unit_latex : str
-        LaTeX code of unit (optional)
-    p_boundaries : List
-        List with minimum and maximum value (optional)
-    p_description : str
-        Description of dimension (optional)
-    p_symmetrical : bool
-        Information about the symmetry of the dimension (optional, default is False)
-    p_logging
-        Log level (see constants of class Log). Default: Log.C_LOG_ALL
-    p_kwargs : dict
-        Further keyword arguments
-        
-    Attributes
-    ----------
-    C_TYPE : str
-        Type of the base class. Default: 'SimState'.
-    C_NAME : str
-        Name of the component state. Default:''.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = ''
-
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self, 
-                 p_name_short, 
-                 p_base_set=Dimension.C_BASE_SET_R, 
-                 p_name_long='', 
-                 p_name_latex='', 
-                 p_unit='',
-                 p_unit_latex='', 
-                 p_boundaries:list=[], 
-                 p_description='',
-                 p_symmetrical:bool=False,
-                 p_logging=Log.C_LOG_NOTHING,
-                 **p_kwargs):
-              
-        Dimension.__init__(self,
-                           p_name_short=p_name_short, 
-                           p_base_set=p_base_set, 
-                           p_name_long=p_name_long, 
-                           p_name_latex=p_name_latex, 
-                           p_unit=p_unit,
-                           p_unit_latex=p_unit_latex, 
-                           p_boundaries=p_boundaries, 
-                           p_description=p_description,
-                           p_symmetrical=p_symmetrical,
-                           p_logging=p_logging,
-                           p_kwargs=p_kwargs)
-        self._value = None
-        self._function = self._setup_function()
-            
-
-## -------------------------------------------------------------------------------------------------
-    def set_value(self, p_input) -> bool:
-        """
-        This method provides a functionality to set a value of the state.
-
-        Parameters
-        ----------
-        p_input : float
-            input parameters to set a value.
-
-        Returns
-        -------
-        bool
-            if set value is successful, then True. Otherwise False.
-        """
-        if p_input >= self.get_boundaries()[0] and p_input <= self.get_boundaries()[1]:
-            self._value = p_input
-            self.log(Log.C_LOG_TYPE_I, 'State ' + self.get_name_short() + ' is updated.')
-            return True
-        else:
-            self.log(Log.C_LOG_TYPE_E, 'State ' + self.get_name_short() + ' fails to be updated.')
-            return False
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def get_value(self):
-        """
-        This method provides a functionality to get the actual value of the state.
-
-        Returns
-        -------
-        value
-            The actual value of the state.
-        """
-        return self._value
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        """
-        This is a custom method, in which a specific TransferFunction object is incorporated.
-        The TransferFunction object describes what is the current state of the component with
-        respect to input signals according to a mathematical calculation.
-
-        Returns
-        -------
-        TransferFunction
-            TransferFunction object.
-        """
-        raise NotImplementedError
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def simulate(self, p_input_signal, p_range=None) -> bool:
-        """
-        This method provides a functionality to simulate the sensor.
-
-        Returns
-        -------
-        bool
-            True means successful, otherwise False.
-        """
-        output = self._function(p_input_signal, p_range)
-        self.set_value(output)
-        return True
-
-    
-
-
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class Component(PersonalisedStamp, EventManager, ScientificObject):
-    """
-    This class serves as a base class of components in MPPS, which provides the main attributes of a
-    component in a simulation mode.
-    A component can consist of actuators, sensors, and component states.
-    
-    Parameters
-    ----------
-    p_name_short : str
-        Short name of a component
-    p_id : int
-        Unique id. Default: None
-    p_logging
-        Log level (see constants of class Log). Default: Log.C_LOG_ALL
-    p_setup : bool
-        Whether setup component is required. Default: True
-    p_kwargs : dict
-        Further keyword arguments
-        
-    Attributes
-    ----------
-    C_TYPE : str
-        Type of the base class. Default: 'Component'.
-    C_NAME : str
-        Name of the component. Default:''.
-    """
-
-    C_TYPE = 'Component'
-    C_NAME = ''
-
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self,
-                 p_name:str,
-                 p_id:int=None,
-                 p_logging=Log.C_LOG_ALL,
-                 p_setup:bool=True,
-                 **p_kwargs):
-        
-        self._kwargs = p_kwargs.copy()
-        self._sensors = Set()
-        self._actuators = Set()
-        self._states = Set()
-        
-        PersonalisedStamp.__init__(self, p_name, p_id)
-        EventManager.__init__(self, p_logging=p_logging)
-        if p_setup:
-            self._setup_component()
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_name_short(self) -> str:
-        """
-        This method provides a functionality to get the unique name of the related component.
-
-        Returns
-        -------
-        str
-            The unique name of the related component.
-
-        """
-        return self._name
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_base_set(self) -> str:
-        """
-        This is just a dummy function.
-
-        Returns
-        -------
-        str
-            'Z'.
-
-        """
-        return 'Z'
-            
-
-## -------------------------------------------------------------------------------------------------
-    def deactivate(self) -> bool:
-        """
-        This method provides a functionality to deactivate the component.
-
-        Returns
-        -------
-        bool
-            if deactivate is successful, then True. Otherwise False.
-        """
-        for ids in self._sensors.get_dim_ids():
-            self.get_sensor(p_id=ids).deactivate()
-
-        for ids in self._actuators.get_dim_ids():
-            self.get_actuator(p_id=ids).deactivate()
-
-        return True
-
-
-## -------------------------------------------------------------------------------------------------
-    def _add_sensor(self, p_sensor:SimSensor):
-        """
-        This method provides a functionality to add a sensor to the component.
-
-        Parameters
-        ----------
-        p_sensor : SimSensor
-            SimSensor object to be added.
-        """
-        self._sensors.add_dim(p_dim=p_sensor)
-
-    
-## -------------------------------------------------------------------------------------------------
-    def get_sensors(self) -> Set:
-        """
-        This method provides a functionality to return the internal set of sensors.
-
-        Returns
-        -------
-        sensors : Set
-            Set of sensors.
-        """
-        return self._sensors
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_sensor(self, p_id) -> SimSensor:
-        """
-        This method provides a functionality to return a specific sensor according to the desired id.
-
-        Returns
-        -------
-        sensor : SimSensor
-            The sensor with the specific id.
-        """
-        return self._sensors.get_dim(p_id=p_id)
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_sensor_value(self, p_id):
-        """
-        This method provides a functionality to determine the value of a sensor.
-
-        Parameters
-        ----------
-        p_id
-            Id of the sensor.
-
-        Returns
-        -------
-            Current value of the sensor or None. None means that the sensor is deactivated or the
-            value has not been set.
-        """
-        return self.get_sensor(p_id).get_value()
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_sensor_status(self, p_id):
-        """
-        This method provides a functionality to determine the status of a sensor.
-
-        Parameters
-        ----------
-        p_id
-            Id of the sensor.
-
-        Returns
-        -------
-            Sensor is switched on or off.
-        """
-        return self.get_sensor(p_id).get_status()
-
-
-## -------------------------------------------------------------------------------------------------
-    def set_sensor_value(self, p_id, p_value) -> bool:
-        """
-        This method provides a functionality to set the value of a sensor.
-
-        Parameters
-        ----------
-        p_id
-            Id of the sensor.
-        p_value
-            New sensor value.
-
-        Returns
-        -------
-            Set value is succeesful or fails.
-        """
-        try:
-            self.get_sensor(p_id).set_value(p_value)
-            return True
-        except:
-            return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _add_actuator(self, p_actuator:SimActuator):
-        """
-        This method provides a functionality to add an actuator to the component.
-
-        Parameters
-        ----------
-        p_actuator : SimActuator
-            SimActuator object to be added.
-        """
-        self._actuators.add_dim(p_dim=p_actuator)
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuators(self) -> Set:
-        """
-        This method provides a functionality to return the internal set of actuators.
-
-        Returns
-        -------
-        actuators : Set
-            Set of actuators.
-        """
-        return self._actuators
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuator(self, p_id) -> SimActuator:
-        """
-        This method provides a functionality to return a specific actuator according to the desired id.
-
-        Returns
-        -------
-        actuator : SimActuator
-            The actuator with the specific id.
-        """
-        return self._actuators.get_dim(p_id=p_id)
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuator_value(self, p_id):
-        """
-        This method provides a functionality to determine the value of an actuator.
-
-        Parameters
-        ----------
-        p_id
-            Id of the actuator.
-
-        Returns
-        -------
-            Current value of the actuator or None. None means that the actuator is deactivated or the
-            value has not been set.
-        """
-        return self.get_actuator(p_id).get_value()
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuator_status(self, p_id):
-        """
-        This method provides a functionality to determine the status of an actuator.
-
-        Parameters
-        ----------
-        p_id
-            Id of the actuator.
-
-        Returns
-        -------
-            Actuator is switched on or off.
-        """
-        return self.get_actuator(p_id).get_status()
-
-
-## -------------------------------------------------------------------------------------------------
-    def set_actuator_value(self, p_id, p_value) -> bool:
-        """
-        This method provides a functionality to set the value of an actuator.
-
-        Parameters
-        ----------
-        p_id
-            Id of the actuator.
-        p_value
-            New actuator value.
-
-        Returns
-        -------
-            Set value is succeesful or fails.
-        """
-        try:
-            self.get_actuator(p_id).set_value(p_value)
-            return True
-        except:
-            return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _add_component_states(self, p_comp_states:SimState):
-        """
-        This method provides a functionality to add a simulatable state to the component.
-
-        Parameters
-        ----------
-        p_comp_states : SimState
-            SimState object to be added.
-        """
-        self._states.add_dim(p_dim=p_comp_states)
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_states(self) -> Set:
-        """
-        This method provides a functionality to return the internal set of simulatable states.
-
-        Returns
-        -------
-        states : Set
-            Set of simulatable states.
-        """
-        return self._states
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_state(self, p_id) -> SimState:
-        """
-        This method provides a functionality to return a specific simulatable state according to the
-        desired id.
-
-        Returns
-        -------
-        state : SimState
-            The simulatable state with the specific id.
-        """
-        return self._states.get_dim(p_id=p_id)
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_state_value(self, p_id):
-        """
-        This method provides a functionality to determine the value of a simulatable state.
-
-        Parameters
-        ----------
-        p_id
-            Id of the simulatable state.
-
-        Returns
-        -------
-            Current value of the simulatable state or None.
-        """
-        return self.get_component_state(p_id).get_value()
-
-
-## -------------------------------------------------------------------------------------------------
-    def set_component_state_value(self, p_id, p_value) -> bool:
-        """
-        This method provides a functionality to set the value of a simulatable state.
-
-        Parameters
-        ----------
-        p_id
-            Id of the simulatable state.
-        p_value
-            New simulatable state value.
-
-        Returns
-        -------
-            Set value is succeesful or fails.
-        """
-        try:
-            self.get_component_state(p_id).set_value(p_value)
-            return True
-        except:
-            return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        Custom method to setup a component. An howto and documentation related to setting up
-        a component will be available soon.
-        """
-
-        # self._add_actuator(...)
-        # self._add_component_states(...)
-        # self._add_sensor(...)
-
-        raise NotImplementedError
-
-
-
-        
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class Module(Component):
-    """
-    This class serves as a base class of modules in MPPS, which provides the main attributes of a
-    module in a simulation mode.
-    A module can consist of components.
-    
-    Parameters
-    ----------
-    p_name_short : str
-        Short name of a module
-    p_id : int
-        Unique id. Default: None
-    p_logging
-        Log level (see constants of class Log). Default: Log.C_LOG_ALL
-    p_kwargs : dict
-        Further keyword arguments
-        
-    Attributes
-    ----------
-    C_TYPE : str
-        Type of the base class. Default: 'Module'.
-    C_NAME : str
-        Name of the module. Default:''.
-    """
-
-    C_TYPE = 'Module'
-    C_NAME = ''
-
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self,
-                 p_name:str,
-                 p_id:int=None,
-                 p_logging=Log.C_LOG_ALL,
-                 **p_kwargs):
-        
-        self._components = Set()
-        
-        Component.__init__(self,
-                           p_name=p_name,
-                           p_id=p_id,
-                           p_logging=p_logging,
-                           p_setup=False,
-                           p_kwargs=p_kwargs)
-        self._setup_module()
-            
-
-## -------------------------------------------------------------------------------------------------
-    def deactivate(self) -> bool:
-        """
-        This method provides a functionality to deactivate the modules.
-
-        Returns
-        -------
-        bool
-            if deactivate is successful, then True. Otherwise False.
-        """
-        for ids in self._components.get_dim_ids():
-            self.get_component(p_id=ids).deactivate()
-
-        return True
-
-
-## -------------------------------------------------------------------------------------------------
-    def _add_component(self, p_component:Component):
-        """
-        This method provides a functionality to add a component to the module.
-
-        Parameters
-        ----------
-        p_sensor : Component
-            Component object to be added.
-        """
-        self._components.add_dim(p_dim=p_component)
-
-    
-## -------------------------------------------------------------------------------------------------
-    def get_components(self) -> Set:
-        """
-        This method provides a functionality to return the internal set of components.
-
-        Returns
-        -------
-        components : Set
-            Set of components.
-        """
-        return self._components
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component(self, p_id) -> Component:
-        """
-        This method provides a functionality to return a specific component according to the
-        desired id.
-
-        Returns
-        -------
-        component : Component
-            The component with the specific id.
-        """
-        return self._components.get_dim(p_id=p_id)
-
-    
-## -------------------------------------------------------------------------------------------------
-    def get_sensors(self) -> list:
-        """
-        This method provides a functionality to return the internal sets of sensors.
-
-        Returns
-        -------
-        _sensors : list
-            List of set of sensors.
-        """
-        _sensors = []
-
-        for ids in self._components.get_dim_ids():
-            _sensors.extend(self.get_component(p_id=ids).get_sensors().get_dims())
-            
-        return _sensors
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_sensor(self, p_id) -> SimSensor:
-        """
-        This method provides a functionality to return a specific sensor according to the desired id.
-
-        Returns
-        -------
-        _sensor : SimSensor
-            The sensor with the specific id.
-        """
-        for sens in self.get_sensors():
-            try:
-                _sensor = sens.get_dim(p_id=p_id)
-                return _sensor
-            except:
-                pass
-        
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuators(self) -> list:
-        """
-        This method provides a functionality to return the internal sets of actuators.
-
-        Returns
-        -------
-        actuators : list
-            List of set of actuators.
-        """
-        _actuators = []
-
-        for ids in self._components.get_dim_ids():
-            _actuators.extend(self.get_component(p_id=ids).get_actuators().get_dims())
-            
-        return _actuators
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuator(self, p_id) -> SimActuator:
-        """
-        This method provides a functionality to return a specific actuator according to the desired id.
-
-        Returns
-        -------
-        actuator : SimActuator
-            The actuator with the specific id.
-        """
-        for acts in self.get_actuators():
-            try:
-                _actuator = acts.get_dim(p_id=p_id)
-                return _actuator
-            except:
-                pass
-        
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_states(self) -> list:
-        """
-        This method provides a functionality to return the internal sets of simulatable states.
-
-        Returns
-        -------
-        states : list
-            List of set of simulatable states.
-        """
-        _states = []
-
-        for ids in self._components.get_dim_ids():
-            _states.extend(self.get_component(p_id=ids).get_component_states().get_dims())
-            
-        return _states
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_state(self, p_id) -> SimState:
-        """
-        This method provides a functionality to return a specific simulatable state according
-        to the desired id.
-
-        Returns
-        -------
-        state : SimState
-            The simulatable state with the specific id.
-        """
-        for st in self.get_actuators():
-            try:
-                _state = st.get_dim(p_id=p_id)
-                return _state
-            except:
-                pass
-        
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_module(self):
-        """
-        Custom method to setup a module. An howto and documentation related to setting up
-        a module will be available soon.
-        """
-
-        # self._add_component(...)
-
-        raise NotImplementedError
-
-
-
-    
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SimMPPS(FctSTrans, PersonalisedStamp, ScientificObject):
-    """
-    This class serves as a base class of SimMPPS, which provides the main attributes of a
-    MPPS in a simulation mode.
-    
-    [Description of SimMPPS] -- to be added
-    
-    Parameters
-    ----------
-    p_name_short : str
-        Short name of a module
-    p_id : int
-        Unique id. Default: None
-    p_logging
-        Log level (see constants of class Log). Default: Log.C_LOG_ALL
-    p_auto_adjust_names : bool
-        Auto adjusting duplicated names of the elements. Default: True
-    p_kwargs : dict
-        Further keyword arguments
-        
-    Attributes
-    ----------
-    C_TYPE : str
-        Type of the base class. Default: 'SimMPPS'.
-    C_NAME : str
-        Name of the SimMPPS. Default:''.
-    """
-
-    C_TYPE = 'SimMPPS'
-    C_NAME = ''
-
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self,
-                 p_name:str,
-                 p_id:int=None,
-                 p_logging=Log.C_LOG_ALL,
-                 p_auto_adjust_names:bool=True,
-                 **p_kwargs):
-        
-        self._elements = Set()
-        self._kwargs = p_kwargs.copy()
-        self._actions_in_order = False
-        
-        PersonalisedStamp.__init__(self, p_name, p_id)
-        FctSTrans.__init__(self, p_logging)
-        self._signals = []
-        self._setup_mpps(p_auto_adjust_names)
-
-
-## -------------------------------------------------------------------------------------------------
-    def _add_element(self, p_elem:Component):
-        """
-        This method provides a functionality to add an element to the MPPS.
-
-        Parameters
-        ----------
-        p_elem : Component
-            Component object to be added. Module object can also be added due to inheritance from 
-            Component object.
-        """
-        self._elements.add_dim(p_dim=p_elem)
-
-
-## -------------------------------------------------------------------------------------------------
-    def _add_signal(self, p_updated_elem, *p_input_fcts):
-        """
-        This method provides a functionality to add a signal for simulating the MPPS.
-
-        Parameters
-        ----------
-        p_updated_elem :
-            the element (Sensor, Actuator, or States) that is simulated, if the signal is called.
-        p_input_fcts : list
-            required information to simulate the element. 
-        """
-        _sig = []
-        _sig.append(p_updated_elem)
-        _sig.extend(p_input_fcts)
-        self._signals.append(_sig)
-
-    
-## -------------------------------------------------------------------------------------------------
-    def get_elements(self) -> Set:
-        """
-        This method provides a functionality to return the internal set of elements.
-
-        Returns
-        -------
-        _elements : Set
-            Set of elements.
-        """
-        return self._elements
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_element(self, p_id) -> Component:
-        """
-        This method provides a functionality to return a specific element according to the desired id.
-
-        Returns
-        -------
-        element : Component
-            The element with the specific id.
-        """
-        return self._elements.get_dim(p_id=p_id)
-
-    
-## -------------------------------------------------------------------------------------------------
-    def get_sensors(self) -> dict:
-        """
-        This method provides a functionality to return the internal sets of sensors.
-
-        Returns
-        -------
-        _sensors : dict
-            Dict of set of sensors, {'short_name': element}.
-        """
-        _sensors = {}
-
-        for ids in self.get_elements().get_dim_ids():
-            for el in self.get_element(p_id=ids).get_sensors():
-                _sensors[el.get_name_short()] = el
-            
-        return _sensors
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_sensor(self, p_id) -> SimSensor:
-        """
-        This method provides a functionality to return a specific sensor according to the desired id.
-
-        Returns
-        -------
-        _sensor : SimSensor
-            The sensor with the specific id.
-        """
-        for sens in self.get_sensors():
-            try:
-                _sensor = sens.get_dim(p_id=p_id)
-                return _sensor
-            except:
-                pass
-        
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuators(self) -> dict:
-        """
-        This method provides a functionality to return the internal sets of actuators.
-
-        Returns
-        -------
-        actuators : dict
-            Dict of set of actuators, {'short_name': element}.
-        """
-        _actuators = {}
-
-        for ids in self.get_elements().get_dim_ids():
-            for el in self.get_element(p_id=ids).get_actuators():
-                _actuators[el.get_name_short()] = el
-            
-        return _actuators
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_actuator(self, p_id) -> SimActuator:
-        """
-        This method provides a functionality to return a specific actuator according to the
-        desired id.
-
-        Returns
-        -------
-        actuator : SimActuator
-            The actuator with the specific id.
-        """
-        for acts in self.get_actuators():
-            try:
-                _actuator = acts.get_dim(p_id=p_id)
-                return _actuator
-            except:
-                pass
-        
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_states(self) -> dict:
-        """
-        This method provides a functionality to return the internal sets of simulatable states.
-
-        Returns
-        -------
-        states : dict
-            Dict of set of simulatable states, {'short_name': element}.
-        """
-        _states = {}
-
-        for ids in self.get_elements().get_dim_ids():
-            for el in self.get_element(p_id=ids).get_component_states():
-                _states[el.get_name_short()] = el
-            
-        return _states
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_component_state(self, p_id) -> SimState:
-        """
-        This method provides a functionality to return a specific simulatable state according to
-        the desired id.
-
-        Returns
-        -------
-        state : SimState
-            The simulatable state with the specific id.
-        """
-        for st in self.get_actuators():
-            try:
-                _state = st.get_dim(p_id=p_id)
-                return _state
-            except:
-                pass
-        
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _elements_names_checker(self) -> bool:
-        """
-        This method provides a functionality to check whether the names of the elements are unique.
-
-        Returns
-        -------
-        bool
-            True means pass the check (no duplication), otherwise False.
-        """
-        _names = []
-
-        for ids in self.get_elements().get_dim_ids():
-            for el in self.get_element(p_id=ids).get_component_states():
-                if el.get_name_short() in _names:
-                    return False
-                else:
-                    _names.append(el.get_name_short())
-            for el in self.get_element(p_id=ids).get_sensors():
-                if el.get_name_short() in _names:
-                    return False
-                else:
-                    _names.append(el.get_name_short())
-            for el in self.get_element(p_id=ids).get_actuators():
-                if el.get_name_short() in _names:
-                    return False
-                else:
-                    _names.append(el.get_name_short())
-        return True
-
-
-## -------------------------------------------------------------------------------------------------
-    def _elements_names_auto_adjust(self):
-        """
-        This method provides a functionality to auto adjust the same elements names.
-        """
-        _names = []
-
-        for ids in self.get_elements().get_dim_ids():
-            for el in self.get_element(p_id=ids).get_component_states():
-                _names.append(el.get_name_short())
-                _counter = _names.count(el.get_name_short())
-                if _counter > 1:
-                    el._name_short = _names[-1]+'_'+str(_counter-1)
-            for el in self.get_element(p_id=ids).get_sensors():
-                _names.append(el.get_name_short())
-                _counter = _names.count(el.get_name_short())
-                if _counter > 1:
-                    el._name_short = _names[-1]+'_'+str(_counter-1)
-            for el in self.get_element(p_id=ids).get_actuators():
-                _names.append(el.get_name_short())
-                _counter = _names.count(el.get_name_short())
-                if _counter > 1:
-                    el._name_short = _names[-1]+'_'+str(_counter-1)
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_mpps(self, p_auto_adjust_names:bool):
-        """
-        Custom method to setup a mpps. An howto and documentation related to setting up MPPS will be
-        available soon.
-        
-        Parameters
-        ----------
-        p_auto_adjust_names : bool
-            Auto adjusting duplicated names of the elements. Default: True
-        """
-        
-        # 1. Add elements
-        # self._add_element(p_elem:Component)
-        
-        # 2. Check duplications of the elements names
-        # while not self._elements_names_checker():
-        #     if p_auto_adjust_names:
-        #         self._elements_names_auto_adjust()
-        #     else:
-        #         raise NameError('There are duplications of the elements names. You can just simply set p_auto_adjust_names to True.')
-
-
-        # 3. Setup which actions connected to which actuators
-
-        # Option 1: The actions are sorted in the same order as self.get_actuators() 
-        # self._actions_in_order = True
-
-        # Option 2: The actions are not sorted in any orders
-        # self._actions_in_order = False
-
-
-        # 4. Setup input signals for updating sensors or component states values
-
-        # _signals = []
-        # _sens = self.get_sensors()
-        # _acts = self.get_actuators()
-        # _sts = self.get_component_states()
-        # _signals.append([sensor/state id, input signal 1, input signal 2, ...., input signal x])
-        # _signals.append([_sens['Sensor1'], _sts['States1'].get_value])
-        # _signals.append([_sts['States1'], _acts['Actuator2'].get_value, _acts['Actuator10'].get_value])
-
-
-        # 5. Return _actions_in_order and _signals
-        # return _actions_in_order, _signals
-
-        raise NotImplementedError
-
-
-
-## -------------------------------------------------------------------------------------------------
-    def _simulate_reaction(self, p_state: State, p_action: Action) -> State:
-        """
-        Custom method for a simulated state transition. See method simulate_reaction() for further
-        details.
-
-        Parameters
-        ----------
-        p_state : State
-            System state.
-        p_action : Action
-            Action to be processed.
-
-        Returns
-        -------
-        new_state : State
-            Result state after state transition.
-        """
-        # 1. Set values to actuators
-        if self._actions_in_order:
-            actions = Action.get_sorted_values()
-            for idx, acts in enumerate(self.get_actuators()):
-                acts.set_value(actions[idx])
-        else:
-            raise NotImplementedError
-        
-        # 2. Update values of the sensors and component states
-        for sig in self._signals:
-            if len(sig[1:]) == 1:
-                input = sig[1]()
-            else:
-                input = []
-                for x in range(len(sig[1:])):
-                    input.append(sig[x+1]())
-            sig[0].simulate(input, p_range=None)
-
-        # 3. Return the resulted states in the form of State object
-        raise NotImplementedError
-        
-
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps
+## -- Module  : mpps.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-22  0.0.0     SY/ML    Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Add p_setup on Component Class, debugging, restructuring
+## -- 2023-01-13  1.0.2     SY       Add documentation
+## -- 2023-01-16  1.0.3     SY       Update due to __call__ of TransferFunction
+## -- 2023-02-01  1.1.0     SY       Refactoring and adding functionalities
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.1.0 (2023-02-01)
+
+This module provides a multi-purpose environment for continuous and batch production systems with
+modular setting and high-flexibility.
+
+The users are able to develop and simulate their own production systems including setting up own
+actuators, reservoirs, processes, modules/stations, and components.
+We also provide the default implementations of actuators, reservoirs, components, processes and
+modules, which can be found in the pool of objects.
+
+To be noted, the usage of this simulation is not limited to machine learning tasks, but it also
+can be as a testing environment for any kind of simulations, including GT tasks, evolutionary
+algorithms, supervised learning, model predictive control, domain learning, transfer learning,
+and many more.
+"""
+
+
+from mlpro.rl.models import *
+from mlpro.bf.various import *
+from mlpro.bf.math import *
+from mlpro.bf.systems import *
+import numpy as np
+import random
+import uuid
+import math
+import matplotlib.pyplot as plt
+from mlpro.bf.physics import TransferFunction
+
+
+
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SimActuator(Actuator, ScientificObject):
+    """
+    This class serves as a base class of actuators in MPPS, which provides the main attributes of an
+    actuator in a simulation mode.
+    An actuator is a component of a machine that is responsible for moving and controlling a mechanism
+    or system.
+    
+    Parameters
+    ----------
+    p_name_short : str
+        Short name of dimension
+    p_base_set 
+        Base set of dimension. See constants C_BASE_SET_*. Default = C_BASE_SET_R.
+    p_name_long :str
+        Long name of dimension (optional)
+    p_name_latex : str
+        LaTeX name of dimension (optional)
+    p_unit : str
+        Unit (optional)
+    p_unit_latex : str
+        LaTeX code of unit (optional)
+    p_boundaries : List
+        List with minimum and maximum value (optional)
+    p_description : str
+        Description of dimension (optional)
+    p_symmetrical : bool
+        Information about the symmetry of the dimension (optional, default is False)
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_kwargs : dict
+        Further keyword arguments
+        
+    Attributes
+    ----------
+    C_TYPE : str
+        Type of the base class. Default: 'SimActuator'.
+    C_NAME : str
+        Name of the actuator. Default:''.
+    """
+
+    C_TYPE = 'SimActuator'
+    C_NAME = ''
+
+    
+## -------------------------------------------------------------------------------------------------
+    def __init__(self, 
+                 p_name_short, 
+                 p_base_set=Dimension.C_BASE_SET_R, 
+                 p_name_long='', 
+                 p_name_latex='', 
+                 p_unit='',
+                 p_unit_latex='', 
+                 p_boundaries:list=[], 
+                 p_description='',
+                 p_symmetrical:bool=False,
+                 p_logging=Log.C_LOG_NOTHING,
+                 **p_kwargs):
+              
+        Actuator.__init__(self,
+                          p_name_short=p_name_short, 
+                          p_base_set=p_base_set, 
+                          p_name_long=p_name_long, 
+                          p_name_latex=p_name_latex, 
+                          p_unit=p_unit,
+                          p_unit_latex=p_unit_latex, 
+                          p_boundaries=p_boundaries, 
+                          p_description=p_description,
+                          p_symmetrical=p_symmetrical,
+                          p_logging=p_logging,
+                          p_kwargs=p_kwargs)
+        self._value = None
+        self._status = False
+            
+
+## -------------------------------------------------------------------------------------------------
+    def set_value(self, p_input) -> bool:
+        """
+        This method provides a functionality to set a value of the actuator.
+
+        Parameters
+        ----------
+        p_input : float
+            input parameters to set a value.
+
+        Returns
+        -------
+        bool
+            if set value is successful, then True. Otherwise False.
+        """
+        if p_input >= self.get_boundaries()[0] and p_input <= self.get_boundaries()[1]:
+            self._value = p_input
+            self._status = True
+            self.log(Log.C_LOG_TYPE_I, 'Actuator ' + self.get_name_short() + ' is updated.')
+            return True
+        else:
+            self.deactivate()
+            self.log(Log.C_LOG_TYPE_E, 'Actuator ' + self.get_name_short() + ' fails to be updated.')
+            return False
+            
+
+## -------------------------------------------------------------------------------------------------
+    def deactivate(self) -> bool:
+        """
+        This method provides a functionality to deactivate the actuator.
+
+        Returns
+        -------
+        bool
+            if deactivate is successful, then True. Otherwise False.
+        """
+        self._value = None
+        self._status = False
+        self.log(Log.C_LOG_TYPE_I, 'Actuator ' + self.get_name_short() + ' is deactivated.')
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def get_status(self) -> bool:
+        """
+        This method provides a functionality to get the status of the actuator.
+
+        Returns
+        -------
+        bool
+            Status is on/off. True means on, false means off.
+        """
+        return self._status
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def get_value(self):
+        """
+        This method provides a functionality to get the actual value of the actuator.
+
+        Returns
+        -------
+        value
+            The actual value of the actuator.
+        """
+        return self._value
+
+
+
+
+    
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SimSensor(Sensor, ScientificObject):
+    """
+    This class serves as a base class of sensors in MPPS, which provides the main attributes of a
+    sensor in a simulation mode.
+    A sensor is a component of a machine that is responsible for sensing the actual state of the
+    system.
+    
+    Parameters
+    ----------
+    p_name_short : str
+        Short name of dimension
+    p_base_set 
+        Base set of dimension. See constants C_BASE_SET_*. Default = C_BASE_SET_R.
+    p_name_long :str
+        Long name of dimension (optional)
+    p_name_latex : str
+        LaTeX name of dimension (optional)
+    p_unit : str
+        Unit (optional)
+    p_unit_latex : str
+        LaTeX code of unit (optional)
+    p_boundaries : List
+        List with minimum and maximum value (optional)
+    p_description : str
+        Description of dimension (optional)
+    p_symmetrical : bool
+        Information about the symmetry of the dimension (optional, default is False)
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_kwargs : dict
+        Further keyword arguments
+        
+    Attributes
+    ----------
+    C_TYPE : str
+        Type of the base class. Default: 'SimSensor'.
+    C_NAME : str
+        Name of the sensor. Default:''.
+    """
+
+    C_TYPE = 'SimSensor'
+    C_NAME = ''
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self, 
+                 p_name_short, 
+                 p_base_set=Dimension.C_BASE_SET_R, 
+                 p_name_long='', 
+                 p_name_latex='', 
+                 p_unit='',
+                 p_unit_latex='', 
+                 p_boundaries:list=[], 
+                 p_description='',
+                 p_symmetrical:bool=False,
+                 p_logging=Log.C_LOG_NOTHING,
+                 **p_kwargs):
+              
+        Sensor.__init__(self,
+                        p_name_short=p_name_short, 
+                        p_base_set=p_base_set, 
+                        p_name_long=p_name_long, 
+                        p_name_latex=p_name_latex, 
+                        p_unit=p_unit,
+                        p_unit_latex=p_unit_latex, 
+                        p_boundaries=p_boundaries, 
+                        p_description=p_description,
+                        p_symmetrical=p_symmetrical,
+                        p_logging=p_logging,
+                        p_kwargs=p_kwargs)
+        self._value = None
+        self._status = True
+        self._function = self._setup_function()
+            
+
+## -------------------------------------------------------------------------------------------------
+    def set_value(self, p_input) -> bool:
+        """
+        This method provides a functionality to set a value of the sensor to be read.
+
+        Parameters
+        ----------
+        p_input : float
+            input parameters to set a value.
+
+        Returns
+        -------
+        bool
+            if set value is successful, then True. Otherwise False.
+        """
+        if p_input >= self.get_boundaries()[0] and p_input <= self.get_boundaries()[1]:
+            self._value = p_input
+            self._status = True
+            self.log(Log.C_LOG_TYPE_I, 'Sensor ' + self.get_name_short() + ' is updated.')
+            return True
+        else:
+            self.deactivate()
+            self.log(Log.C_LOG_TYPE_E, 'Sensor ' + self.get_name_short() + ' fails to be updated.')
+            return False
+            
+
+## -------------------------------------------------------------------------------------------------
+    def deactivate(self) -> bool:
+        """
+        This method provides a functionality to deactivate the sensor.
+
+        Returns
+        -------
+        bool
+            if deactivate is successful, then True. Otherwise False.
+        """
+        self._value = None
+        self._status = False
+        self.log(Log.C_LOG_TYPE_I, 'Sensor ' + self.get_name_short() + ' is deactivated.')
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def get_status(self) -> bool:
+        """
+        This method provides a functionality to get the status of the related components.
+
+        Returns
+        -------
+        bool
+            Status is on/off. True means on, false means off.
+
+        """
+        return self._status
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def get_value(self):
+        """
+        This method provides a functionality to get the actual value read by the sensor.
+
+        Returns
+        -------
+        value
+            The actual value of the state.
+        """
+        return self._value
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        """
+        This is a custom method, in which a specific TransferFunction object is incorporated.
+        The TransferFunction object describes how the sensor obtain the actual information with
+        respect to input signals according to a mathematical calculation.
+
+        Returns
+        -------
+        TransferFunction
+            TransferFunction object.
+        """
+        raise NotImplementedError
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def simulate(self, p_input_signal, p_range=None) -> bool:
+        """
+        This method provides a functionality to simulate the sensor.
+
+        Returns
+        -------
+        bool
+            True means successful, otherwise False.
+        """
+        output = self._function(p_input_signal, p_range)
+        self.set_value(output)
+        return True
+
+
+
+    
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SimState(Dimension, ScientificObject):
+    """
+    This class serves as a base class of states (extra informations) for a component in MPPS,
+    which provides the main attributes of a component state in a simulation mode.
+    This could be included the dynamics of the systems that can not be read by the sensors but
+    important for the simulations or triggering other components.
+    
+    Parameters
+    ----------
+    p_name_short : str
+        Short name of dimension
+    p_base_set 
+        Base set of dimension. See constants C_BASE_SET_*. Default = C_BASE_SET_R.
+    p_name_long :str
+        Long name of dimension (optional)
+    p_name_latex : str
+        LaTeX name of dimension (optional)
+    p_unit : str
+        Unit (optional)
+    p_unit_latex : str
+        LaTeX code of unit (optional)
+    p_boundaries : List
+        List with minimum and maximum value (optional)
+    p_description : str
+        Description of dimension (optional)
+    p_symmetrical : bool
+        Information about the symmetry of the dimension (optional, default is False)
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_kwargs : dict
+        Further keyword arguments
+        
+    Attributes
+    ----------
+    C_TYPE : str
+        Type of the base class. Default: 'SimState'.
+    C_NAME : str
+        Name of the component state. Default:''.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = ''
+
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self, 
+                 p_name_short, 
+                 p_base_set=Dimension.C_BASE_SET_R, 
+                 p_name_long='', 
+                 p_name_latex='', 
+                 p_unit='',
+                 p_unit_latex='', 
+                 p_boundaries:list=[], 
+                 p_description='',
+                 p_symmetrical:bool=False,
+                 p_logging=Log.C_LOG_NOTHING,
+                 **p_kwargs):
+              
+        Dimension.__init__(self,
+                           p_name_short=p_name_short, 
+                           p_base_set=p_base_set, 
+                           p_name_long=p_name_long, 
+                           p_name_latex=p_name_latex, 
+                           p_unit=p_unit,
+                           p_unit_latex=p_unit_latex, 
+                           p_boundaries=p_boundaries, 
+                           p_description=p_description,
+                           p_symmetrical=p_symmetrical,
+                           p_logging=p_logging,
+                           p_kwargs=p_kwargs)
+        self._value = None
+        self._function = self._setup_function()
+            
+
+## -------------------------------------------------------------------------------------------------
+    def set_value(self, p_input) -> bool:
+        """
+        This method provides a functionality to set a value of the state.
+
+        Parameters
+        ----------
+        p_input : float
+            input parameters to set a value.
+
+        Returns
+        -------
+        bool
+            if set value is successful, then True. Otherwise False.
+        """
+        if p_input >= self.get_boundaries()[0] and p_input <= self.get_boundaries()[1]:
+            self._value = p_input
+            self.log(Log.C_LOG_TYPE_I, 'State ' + self.get_name_short() + ' is updated.')
+            return True
+        else:
+            self.log(Log.C_LOG_TYPE_E, 'State ' + self.get_name_short() + ' fails to be updated.')
+            return False
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def get_value(self):
+        """
+        This method provides a functionality to get the actual value of the state.
+
+        Returns
+        -------
+        value
+            The actual value of the state.
+        """
+        return self._value
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        """
+        This is a custom method, in which a specific TransferFunction object is incorporated.
+        The TransferFunction object describes what is the current state of the component with
+        respect to input signals according to a mathematical calculation.
+
+        Returns
+        -------
+        TransferFunction
+            TransferFunction object.
+        """
+        raise NotImplementedError
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def simulate(self, p_input_signal, p_range=None) -> bool:
+        """
+        This method provides a functionality to simulate the sensor.
+
+        Returns
+        -------
+        bool
+            True means successful, otherwise False.
+        """
+        output = self._function(p_input_signal, p_range)
+        self.set_value(output)
+        return True
+
+    
+
+
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class Component(PersonalisedStamp, EventManager, ScientificObject):
+    """
+    This class serves as a base class of components in MPPS, which provides the main attributes of a
+    component in a simulation mode.
+    A component can consist of actuators, sensors, and component states.
+    
+    Parameters
+    ----------
+    p_name_short : str
+        Short name of a component
+    p_id : int
+        Unique id. Default: None
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_setup : bool
+        Whether setup component is required. Default: True
+    p_kwargs : dict
+        Further keyword arguments
+        
+    Attributes
+    ----------
+    C_TYPE : str
+        Type of the base class. Default: 'Component'.
+    C_NAME : str
+        Name of the component. Default:''.
+    """
+
+    C_TYPE = 'Component'
+    C_NAME = ''
+
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self,
+                 p_name:str,
+                 p_id:int=None,
+                 p_logging=Log.C_LOG_ALL,
+                 p_setup:bool=True,
+                 **p_kwargs):
+        
+        self._kwargs = p_kwargs.copy()
+        self._sensors = Set()
+        self._actuators = Set()
+        self._states = Set()
+        
+        PersonalisedStamp.__init__(self, p_name, p_id)
+        EventManager.__init__(self, p_logging=p_logging)
+        if p_setup:
+            self._setup_component()
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_name_short(self) -> str:
+        """
+        This method provides a functionality to get the unique name of the related component.
+
+        Returns
+        -------
+        str
+            The unique name of the related component.
+
+        """
+        return self._name
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_base_set(self) -> str:
+        """
+        This is just a dummy function.
+
+        Returns
+        -------
+        str
+            'Z'.
+
+        """
+        return 'Z'
+            
+
+## -------------------------------------------------------------------------------------------------
+    def deactivate(self) -> bool:
+        """
+        This method provides a functionality to deactivate the component.
+
+        Returns
+        -------
+        bool
+            if deactivate is successful, then True. Otherwise False.
+        """
+        for ids in self._sensors.get_dim_ids():
+            self.get_sensor(p_id=ids).deactivate()
+
+        for ids in self._actuators.get_dim_ids():
+            self.get_actuator(p_id=ids).deactivate()
+
+        return True
+
+
+## -------------------------------------------------------------------------------------------------
+    def _add_sensor(self, p_sensor:SimSensor):
+        """
+        This method provides a functionality to add a sensor to the component.
+
+        Parameters
+        ----------
+        p_sensor : SimSensor
+            SimSensor object to be added.
+        """
+        self._sensors.add_dim(p_dim=p_sensor)
+
+    
+## -------------------------------------------------------------------------------------------------
+    def get_sensors(self) -> Set:
+        """
+        This method provides a functionality to return the internal set of sensors.
+
+        Returns
+        -------
+        sensors : Set
+            Set of sensors.
+        """
+        return self._sensors
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_sensor(self, p_id) -> SimSensor:
+        """
+        This method provides a functionality to return a specific sensor according to the desired id.
+
+        Returns
+        -------
+        sensor : SimSensor
+            The sensor with the specific id.
+        """
+        return self._sensors.get_dim(p_id=p_id)
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_sensor_value(self, p_id):
+        """
+        This method provides a functionality to determine the value of a sensor.
+
+        Parameters
+        ----------
+        p_id
+            Id of the sensor.
+
+        Returns
+        -------
+            Current value of the sensor or None. None means that the sensor is deactivated or the
+            value has not been set.
+        """
+        return self.get_sensor(p_id).get_value()
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_sensor_status(self, p_id):
+        """
+        This method provides a functionality to determine the status of a sensor.
+
+        Parameters
+        ----------
+        p_id
+            Id of the sensor.
+
+        Returns
+        -------
+            Sensor is switched on or off.
+        """
+        return self.get_sensor(p_id).get_status()
+
+
+## -------------------------------------------------------------------------------------------------
+    def set_sensor_value(self, p_id, p_value) -> bool:
+        """
+        This method provides a functionality to set the value of a sensor.
+
+        Parameters
+        ----------
+        p_id
+            Id of the sensor.
+        p_value
+            New sensor value.
+
+        Returns
+        -------
+            Set value is succeesful or fails.
+        """
+        try:
+            self.get_sensor(p_id).set_value(p_value)
+            return True
+        except:
+            return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _add_actuator(self, p_actuator:SimActuator):
+        """
+        This method provides a functionality to add an actuator to the component.
+
+        Parameters
+        ----------
+        p_actuator : SimActuator
+            SimActuator object to be added.
+        """
+        self._actuators.add_dim(p_dim=p_actuator)
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuators(self) -> Set:
+        """
+        This method provides a functionality to return the internal set of actuators.
+
+        Returns
+        -------
+        actuators : Set
+            Set of actuators.
+        """
+        return self._actuators
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuator(self, p_id) -> SimActuator:
+        """
+        This method provides a functionality to return a specific actuator according to the desired id.
+
+        Returns
+        -------
+        actuator : SimActuator
+            The actuator with the specific id.
+        """
+        return self._actuators.get_dim(p_id=p_id)
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuator_value(self, p_id):
+        """
+        This method provides a functionality to determine the value of an actuator.
+
+        Parameters
+        ----------
+        p_id
+            Id of the actuator.
+
+        Returns
+        -------
+            Current value of the actuator or None. None means that the actuator is deactivated or the
+            value has not been set.
+        """
+        return self.get_actuator(p_id).get_value()
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuator_status(self, p_id):
+        """
+        This method provides a functionality to determine the status of an actuator.
+
+        Parameters
+        ----------
+        p_id
+            Id of the actuator.
+
+        Returns
+        -------
+            Actuator is switched on or off.
+        """
+        return self.get_actuator(p_id).get_status()
+
+
+## -------------------------------------------------------------------------------------------------
+    def set_actuator_value(self, p_id, p_value) -> bool:
+        """
+        This method provides a functionality to set the value of an actuator.
+
+        Parameters
+        ----------
+        p_id
+            Id of the actuator.
+        p_value
+            New actuator value.
+
+        Returns
+        -------
+            Set value is succeesful or fails.
+        """
+        try:
+            self.get_actuator(p_id).set_value(p_value)
+            return True
+        except:
+            return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _add_component_states(self, p_comp_states:SimState):
+        """
+        This method provides a functionality to add a simulatable state to the component.
+
+        Parameters
+        ----------
+        p_comp_states : SimState
+            SimState object to be added.
+        """
+        self._states.add_dim(p_dim=p_comp_states)
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_states(self) -> Set:
+        """
+        This method provides a functionality to return the internal set of simulatable states.
+
+        Returns
+        -------
+        states : Set
+            Set of simulatable states.
+        """
+        return self._states
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_state(self, p_id) -> SimState:
+        """
+        This method provides a functionality to return a specific simulatable state according to the
+        desired id.
+
+        Returns
+        -------
+        state : SimState
+            The simulatable state with the specific id.
+        """
+        return self._states.get_dim(p_id=p_id)
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_state_value(self, p_id):
+        """
+        This method provides a functionality to determine the value of a simulatable state.
+
+        Parameters
+        ----------
+        p_id
+            Id of the simulatable state.
+
+        Returns
+        -------
+            Current value of the simulatable state or None.
+        """
+        return self.get_component_state(p_id).get_value()
+
+
+## -------------------------------------------------------------------------------------------------
+    def set_component_state_value(self, p_id, p_value) -> bool:
+        """
+        This method provides a functionality to set the value of a simulatable state.
+
+        Parameters
+        ----------
+        p_id
+            Id of the simulatable state.
+        p_value
+            New simulatable state value.
+
+        Returns
+        -------
+            Set value is succeesful or fails.
+        """
+        try:
+            self.get_component_state(p_id).set_value(p_value)
+            return True
+        except:
+            return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        Custom method to setup a component. An howto and documentation related to setting up
+        a component will be available soon.
+        """
+
+        # self._add_actuator(...)
+        # self._add_component_states(...)
+        # self._add_sensor(...)
+
+        raise NotImplementedError
+
+
+
+        
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class Module(Component):
+    """
+    This class serves as a base class of modules in MPPS, which provides the main attributes of a
+    module in a simulation mode.
+    A module can consist of components.
+    
+    Parameters
+    ----------
+    p_name_short : str
+        Short name of a module
+    p_id : int
+        Unique id. Default: None
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_kwargs : dict
+        Further keyword arguments
+        
+    Attributes
+    ----------
+    C_TYPE : str
+        Type of the base class. Default: 'Module'.
+    C_NAME : str
+        Name of the module. Default:''.
+    """
+
+    C_TYPE = 'Module'
+    C_NAME = ''
+
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self,
+                 p_name:str,
+                 p_id:int=None,
+                 p_logging=Log.C_LOG_ALL,
+                 **p_kwargs):
+        
+        self._components = Set()
+        
+        Component.__init__(self,
+                           p_name=p_name,
+                           p_id=p_id,
+                           p_logging=p_logging,
+                           p_setup=False,
+                           p_kwargs=p_kwargs)
+        self._setup_module()
+            
+
+## -------------------------------------------------------------------------------------------------
+    def deactivate(self) -> bool:
+        """
+        This method provides a functionality to deactivate the modules.
+
+        Returns
+        -------
+        bool
+            if deactivate is successful, then True. Otherwise False.
+        """
+        for ids in self._components.get_dim_ids():
+            self.get_component(p_id=ids).deactivate()
+
+        return True
+
+
+## -------------------------------------------------------------------------------------------------
+    def _add_component(self, p_component:Component):
+        """
+        This method provides a functionality to add a component to the module.
+
+        Parameters
+        ----------
+        p_sensor : Component
+            Component object to be added.
+        """
+        self._components.add_dim(p_dim=p_component)
+
+    
+## -------------------------------------------------------------------------------------------------
+    def get_components(self) -> Set:
+        """
+        This method provides a functionality to return the internal set of components.
+
+        Returns
+        -------
+        components : Set
+            Set of components.
+        """
+        return self._components
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component(self, p_id) -> Component:
+        """
+        This method provides a functionality to return a specific component according to the
+        desired id.
+
+        Returns
+        -------
+        component : Component
+            The component with the specific id.
+        """
+        return self._components.get_dim(p_id=p_id)
+
+    
+## -------------------------------------------------------------------------------------------------
+    def get_sensors(self) -> list:
+        """
+        This method provides a functionality to return the internal sets of sensors.
+
+        Returns
+        -------
+        _sensors : list
+            List of set of sensors.
+        """
+        _sensors = []
+
+        for ids in self._components.get_dim_ids():
+            _sensors.extend(self.get_component(p_id=ids).get_sensors().get_dims())
+            
+        return _sensors
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_sensor(self, p_id) -> SimSensor:
+        """
+        This method provides a functionality to return a specific sensor according to the desired id.
+
+        Returns
+        -------
+        _sensor : SimSensor
+            The sensor with the specific id.
+        """
+        for sens in self.get_sensors():
+            try:
+                _sensor = sens.get_dim(p_id=p_id)
+                return _sensor
+            except:
+                pass
+        
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuators(self) -> list:
+        """
+        This method provides a functionality to return the internal sets of actuators.
+
+        Returns
+        -------
+        actuators : list
+            List of set of actuators.
+        """
+        _actuators = []
+
+        for ids in self._components.get_dim_ids():
+            _actuators.extend(self.get_component(p_id=ids).get_actuators().get_dims())
+            
+        return _actuators
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuator(self, p_id) -> SimActuator:
+        """
+        This method provides a functionality to return a specific actuator according to the desired id.
+
+        Returns
+        -------
+        actuator : SimActuator
+            The actuator with the specific id.
+        """
+        for acts in self.get_actuators():
+            try:
+                _actuator = acts.get_dim(p_id=p_id)
+                return _actuator
+            except:
+                pass
+        
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_states(self) -> list:
+        """
+        This method provides a functionality to return the internal sets of simulatable states.
+
+        Returns
+        -------
+        states : list
+            List of set of simulatable states.
+        """
+        _states = []
+
+        for ids in self._components.get_dim_ids():
+            _states.extend(self.get_component(p_id=ids).get_component_states().get_dims())
+            
+        return _states
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_state(self, p_id) -> SimState:
+        """
+        This method provides a functionality to return a specific simulatable state according
+        to the desired id.
+
+        Returns
+        -------
+        state : SimState
+            The simulatable state with the specific id.
+        """
+        for st in self.get_actuators():
+            try:
+                _state = st.get_dim(p_id=p_id)
+                return _state
+            except:
+                pass
+        
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_module(self):
+        """
+        Custom method to setup a module. An howto and documentation related to setting up
+        a module will be available soon.
+        """
+
+        # self._add_component(...)
+
+        raise NotImplementedError
+
+
+
+    
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SimMPPS(FctSTrans, PersonalisedStamp, ScientificObject):
+    """
+    This class serves as a base class of SimMPPS, which provides the main attributes of a
+    MPPS in a simulation mode.
+    
+    [Description of SimMPPS] -- to be added
+    
+    Parameters
+    ----------
+    p_name_short : str
+        Short name of a module
+    p_id : int
+        Unique id. Default: None
+    p_logging
+        Log level (see constants of class Log). Default: Log.C_LOG_ALL
+    p_auto_adjust_names : bool
+        Auto adjusting duplicated names of the elements. Default: True
+    p_kwargs : dict
+        Further keyword arguments
+        
+    Attributes
+    ----------
+    C_TYPE : str
+        Type of the base class. Default: 'SimMPPS'.
+    C_NAME : str
+        Name of the SimMPPS. Default:''.
+    """
+
+    C_TYPE = 'SimMPPS'
+    C_NAME = ''
+
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self,
+                 p_name:str,
+                 p_id:int=None,
+                 p_logging=Log.C_LOG_ALL,
+                 p_auto_adjust_names:bool=True,
+                 **p_kwargs):
+        
+        self._elements = Set()
+        self._kwargs = p_kwargs.copy()
+        self._actions_in_order = False
+        
+        PersonalisedStamp.__init__(self, p_name, p_id)
+        FctSTrans.__init__(self, p_logging)
+        self._signals = []
+        self._setup_mpps(p_auto_adjust_names)
+
+
+## -------------------------------------------------------------------------------------------------
+    def _add_element(self, p_elem:Component):
+        """
+        This method provides a functionality to add an element to the MPPS.
+
+        Parameters
+        ----------
+        p_elem : Component
+            Component object to be added. Module object can also be added due to inheritance from 
+            Component object.
+        """
+        self._elements.add_dim(p_dim=p_elem)
+
+
+## -------------------------------------------------------------------------------------------------
+    def _add_signal(self, p_updated_elem, *p_input_fcts):
+        """
+        This method provides a functionality to add a signal for simulating the MPPS.
+
+        Parameters
+        ----------
+        p_updated_elem :
+            the element (Sensor, Actuator, or States) that is simulated, if the signal is called.
+        p_input_fcts : list
+            required information to simulate the element. 
+        """
+        _sig = []
+        _sig.append(p_updated_elem)
+        _sig.extend(p_input_fcts)
+        self._signals.append(_sig)
+
+    
+## -------------------------------------------------------------------------------------------------
+    def get_elements(self) -> Set:
+        """
+        This method provides a functionality to return the internal set of elements.
+
+        Returns
+        -------
+        _elements : Set
+            Set of elements.
+        """
+        return self._elements
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_element(self, p_id) -> Component:
+        """
+        This method provides a functionality to return a specific element according to the desired id.
+
+        Returns
+        -------
+        element : Component
+            The element with the specific id.
+        """
+        return self._elements.get_dim(p_id=p_id)
+
+    
+## -------------------------------------------------------------------------------------------------
+    def get_sensors(self) -> dict:
+        """
+        This method provides a functionality to return the internal sets of sensors.
+
+        Returns
+        -------
+        _sensors : dict
+            Dict of set of sensors, {'short_name': element}.
+        """
+        _sensors = {}
+
+        for ids in self.get_elements().get_dim_ids():
+            for el in self.get_element(p_id=ids).get_sensors():
+                _sensors[el.get_name_short()] = el
+            
+        return _sensors
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_sensor(self, p_id) -> SimSensor:
+        """
+        This method provides a functionality to return a specific sensor according to the desired id.
+
+        Returns
+        -------
+        _sensor : SimSensor
+            The sensor with the specific id.
+        """
+        for sens in self.get_sensors():
+            try:
+                _sensor = sens.get_dim(p_id=p_id)
+                return _sensor
+            except:
+                pass
+        
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuators(self) -> dict:
+        """
+        This method provides a functionality to return the internal sets of actuators.
+
+        Returns
+        -------
+        actuators : dict
+            Dict of set of actuators, {'short_name': element}.
+        """
+        _actuators = {}
+
+        for ids in self.get_elements().get_dim_ids():
+            for el in self.get_element(p_id=ids).get_actuators():
+                _actuators[el.get_name_short()] = el
+            
+        return _actuators
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_actuator(self, p_id) -> SimActuator:
+        """
+        This method provides a functionality to return a specific actuator according to the
+        desired id.
+
+        Returns
+        -------
+        actuator : SimActuator
+            The actuator with the specific id.
+        """
+        for acts in self.get_actuators():
+            try:
+                _actuator = acts.get_dim(p_id=p_id)
+                return _actuator
+            except:
+                pass
+        
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_states(self) -> dict:
+        """
+        This method provides a functionality to return the internal sets of simulatable states.
+
+        Returns
+        -------
+        states : dict
+            Dict of set of simulatable states, {'short_name': element}.
+        """
+        _states = {}
+
+        for ids in self.get_elements().get_dim_ids():
+            for el in self.get_element(p_id=ids).get_component_states():
+                _states[el.get_name_short()] = el
+            
+        return _states
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_component_state(self, p_id) -> SimState:
+        """
+        This method provides a functionality to return a specific simulatable state according to
+        the desired id.
+
+        Returns
+        -------
+        state : SimState
+            The simulatable state with the specific id.
+        """
+        for st in self.get_actuators():
+            try:
+                _state = st.get_dim(p_id=p_id)
+                return _state
+            except:
+                pass
+        
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _elements_names_checker(self) -> bool:
+        """
+        This method provides a functionality to check whether the names of the elements are unique.
+
+        Returns
+        -------
+        bool
+            True means pass the check (no duplication), otherwise False.
+        """
+        _names = []
+
+        for ids in self.get_elements().get_dim_ids():
+            for el in self.get_element(p_id=ids).get_component_states():
+                if el.get_name_short() in _names:
+                    return False
+                else:
+                    _names.append(el.get_name_short())
+            for el in self.get_element(p_id=ids).get_sensors():
+                if el.get_name_short() in _names:
+                    return False
+                else:
+                    _names.append(el.get_name_short())
+            for el in self.get_element(p_id=ids).get_actuators():
+                if el.get_name_short() in _names:
+                    return False
+                else:
+                    _names.append(el.get_name_short())
+        return True
+
+
+## -------------------------------------------------------------------------------------------------
+    def _elements_names_auto_adjust(self):
+        """
+        This method provides a functionality to auto adjust the same elements names.
+        """
+        _names = []
+
+        for ids in self.get_elements().get_dim_ids():
+            for el in self.get_element(p_id=ids).get_component_states():
+                _names.append(el.get_name_short())
+                _counter = _names.count(el.get_name_short())
+                if _counter > 1:
+                    el._name_short = _names[-1]+'_'+str(_counter-1)
+            for el in self.get_element(p_id=ids).get_sensors():
+                _names.append(el.get_name_short())
+                _counter = _names.count(el.get_name_short())
+                if _counter > 1:
+                    el._name_short = _names[-1]+'_'+str(_counter-1)
+            for el in self.get_element(p_id=ids).get_actuators():
+                _names.append(el.get_name_short())
+                _counter = _names.count(el.get_name_short())
+                if _counter > 1:
+                    el._name_short = _names[-1]+'_'+str(_counter-1)
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_mpps(self, p_auto_adjust_names:bool):
+        """
+        Custom method to setup a mpps. An howto and documentation related to setting up MPPS will be
+        available soon.
+        
+        Parameters
+        ----------
+        p_auto_adjust_names : bool
+            Auto adjusting duplicated names of the elements. Default: True
+        """
+        
+        # 1. Add elements
+        # self._add_element(p_elem:Component)
+        
+        # 2. Check duplications of the elements names
+        # while not self._elements_names_checker():
+        #     if p_auto_adjust_names:
+        #         self._elements_names_auto_adjust()
+        #     else:
+        #         raise NameError('There are duplications of the elements names. You can just simply set p_auto_adjust_names to True.')
+
+
+        # 3. Setup which actions connected to which actuators
+
+        # Option 1: The actions are sorted in the same order as self.get_actuators() 
+        # self._actions_in_order = True
+
+        # Option 2: The actions are not sorted in any orders
+        # self._actions_in_order = False
+
+
+        # 4. Setup input signals for updating sensors or component states values
+
+        # _signals = []
+        # _sens = self.get_sensors()
+        # _acts = self.get_actuators()
+        # _sts = self.get_component_states()
+        # _signals.append([sensor/state id, input signal 1, input signal 2, ...., input signal x])
+        # _signals.append([_sens['Sensor1'], _sts['States1'].get_value])
+        # _signals.append([_sts['States1'], _acts['Actuator2'].get_value, _acts['Actuator10'].get_value])
+
+
+        # 5. Return _actions_in_order and _signals
+        # return _actions_in_order, _signals
+
+        raise NotImplementedError
+
+
+
+## -------------------------------------------------------------------------------------------------
+    def _simulate_reaction(self, p_state: State, p_action: Action) -> State:
+        """
+        Custom method for a simulated state transition. See method simulate_reaction() for further
+        details.
+
+        Parameters
+        ----------
+        p_state : State
+            System state.
+        p_action : Action
+            Action to be processed.
+
+        Returns
+        -------
+        new_state : State
+            Result state after state transition.
+        """
+        # 1. Set values to actuators
+        if self._actions_in_order:
+            actions = Action.get_sorted_values()
+            for idx, acts in enumerate(self.get_actuators()):
+                acts.set_value(actions[idx])
+        else:
+            raise NotImplementedError
+        
+        # 2. Update values of the sensors and component states
+        for sig in self._signals:
+            if len(sig[1:]) == 1:
+                input = sig[1]()
+            else:
+                input = []
+                for x in range(len(sig[1:])):
+                    input.append(sig[x+1]())
+            sig[0].simulate(input, p_range=None)
+
+        # 3. Return the resulted states in the form of State object
+        raise NotImplementedError
+        
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C001_Silo.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS002_C001_Tank.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,278 +1,313 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C001_Silo.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
-## -- 2023-01-18  1.0.3     SY       Update because TransferFunction is shifted to MLPro.bf.systems
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-06  1.0.5     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Silo.
-A silo is a component to temporary store materials that consists of two sensors.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-import sys
-
-
-         
-            
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloSensor1(SimSensor):
-    """
-    This class serves as a sensor in the upper side of the silo to indicate whether the fill-level
-    of the Silo closes to overflow or not.
-    """
-
-    C_TYPE = 'SimSensor'
-    C_NAME = 'SiloSensor1'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_BufferSensor(p_name='TF_SiloSensor1',
-                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                p_dt=0,
-                                theta = 0.8*17.42) # 80% of the maximum fill-level
-        return _func
-
-
-                 
-                    
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloSensor2(SimSensor):
-    """
-    This class serves as a sensor in the lower side of the silo to indicate whether the fill-level
-    of the Silo closes to empty or not.
-    """
-
-    C_TYPE = 'SimSensor'
-    C_NAME = 'SiloSensor2'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_BufferSensor(p_name='TF_SiloSensor2',
-                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                p_dt=0,
-                                theta = 0.2*17.42) # 20% of the maximum fill-level
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_BufferSensor(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.theta = p_args['theta']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        If the fill-level is above the sensor, then the sensor returns True. Otherwise False.
-
-        Parameters
-        ----------
-        p_input : float
-            actual fill level of the silo.
-
-        Returns
-        -------
-        bool
-            True means on, False means off.
-        """
-        if p_input >= self.theta:
-            return True
-        else:
-            return False
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloFillLevel(SimState):
-    """
-    This class serves as a component state to calculate the actual fill-level of the silo.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'SiloFillLevel'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_FillLevel(p_name='TF_FillLevel',
-                             p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                             p_dt=0,
-                             max_vol = 17.42,
-                             min_vol = 0)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_FillLevel(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.max_vol = p_args['max_vol']
-                self.min_vol = p_args['min_vol']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the current fill-level.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Actual fill-level
-            [1] = Volume in
-            [2] = Volume out
-
-        Returns
-        -------
-        float
-            Actual fill-level.
-        """
-        output = p_input[0]+p_input[1]-p_input[2]
-        
-        if output >= self.max_vol:
-            return self.max_vol
-        elif output <= self.min_vol:
-            return self.min_vol
-        else:
-            return output
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloOverflow(SimState):
-    """
-    This class serves as a component state to calculate the overflow level of the silo.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'SiloOverflow'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_Overflow(p_name='TF_Overflow',
-                            p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                            p_dt=0,
-                            max_vol = 17.42)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_Overflow(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.max_vol = p_args['max_vol']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the current overflow level.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Actual fill-level
-            [1] = Volume in
-            [2] = Volume out
-
-        Returns
-        -------
-        float
-            Actual fill-level.
-        """
-        cur_level = p_input[0]+p_input[1]-p_input[2]
-        
-        if cur_level > self.max_vol:
-            return cur_level-self.max_vol
-        else:
-            return 0
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class Silo(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A silo consists of two sensors and two states components.
-        """
-        silo_sensor_1 = SiloSensor1(p_name_short='SiloSensor1',
-                                    p_base_set=Dimension.C_BASE_SET_Z,
-                                    p_boundaries=[0,1])
-        silo_sensor_2 = SiloSensor2(p_name_short='SiloSensor2',
-                                    p_base_set=Dimension.C_BASE_SET_Z,
-                                    p_boundaries=[0,1])
-        silo_fill_level = SiloFillLevel(p_name_short='SiloFillLevel',
-                                        p_base_set=Dimension.C_BASE_SET_R,
-                                        p_unit='L',
-                                        p_boundaries=[0,17.42])
-        silo_overflow = SiloOverflow(p_name_short='SiloOverflow',
-                                     p_base_set=Dimension.C_BASE_SET_R,
-                                     p_unit='L',
-                                     p_boundaries=[0,sys.maxsize])
-        
-        self._add_sensor(p_sensor=silo_sensor_1)
-        self._add_sensor(p_sensor=silo_sensor_2)
-        self._add_component_states(p_comp_states=silo_overflow)
-        self._add_component_states(p_comp_states=silo_fill_level)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS002_C001_Tank.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2023-01-19  0.0.0     ML       Creation
+## -- 2023-03-28  1.0.0     ML/SY    Release of first version
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.0 (2023-03-28)
+
+This module provides a default implementation of a component of the Liquid Station, which is a Tank.
+A Tank is a component to temporary store liquid that consists of three sensors.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+import sys
+
+
+         
+            
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TankSensor1(SimSensor):
+    """
+    This class serves as a sensor in the upper side of the tank to indicate whether the fill-level
+    of the tank closes to overflow or not.
+    """
+
+    C_TYPE = 'SimSensor'
+    C_NAME = 'TankSensor1'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_BufferSensor(p_name='TF_TankSensor1',
+                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                p_dt=0,
+                                theta = 0.75*250) # 75% of the maximum tank volume - 187,5 l
+        return _func
+
+
+
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TankSensor2(SimSensor):
+    """
+    This class serves as a sensor in the middle side of the tank to indicate whether the fill-level
+    of the tank is in the middle.
+    """
+
+    C_TYPE = 'SimSensor'
+    C_NAME = 'TankSensor3'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_BufferSensor(p_name='TF_TankSensor3',
+                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                p_dt=0,
+                                theta = 0.5*250) # 50% of the maximum tank volume - 125 l
+        return _func
+
+
+
+                    
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TankSensor3(SimSensor):
+    """
+    This class serves as a sensor in the lower side of the tank to indicate whether the fill-level
+    of the tank closes to empty or not.
+    """
+
+    C_TYPE = 'SimSensor'
+    C_NAME = 'TankSensor3'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_BufferSensor(p_name='TF_TankSensor3',
+                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                p_dt=0,
+                                theta = 0.25*250) # 25% of the maximum tank volume - 62,5 l
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_BufferSensor(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.theta = p_args['theta']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        If the fill-level is above the sensor, then the sensor returns True. Otherwise False.
+
+        Parameters
+        ----------
+        p_input : float
+            actual fill level of the silo.
+
+        Returns
+        -------
+        bool
+            True means on, False means off.
+        """
+        if p_input >= self.theta:
+            return True
+        else:
+            return False
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TankFillLevel(SimState):
+    """
+    This class serves as a component state to calculate the actual fill-level of the Tank.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'TankFillLevel'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_FillLevel(p_name='TF_FillLevel',
+                             p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                             p_dt=0,
+                             max_vol = 250,
+                             min_vol = 0)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_FillLevel(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.max_vol = p_args['max_vol']
+                self.min_vol = p_args['min_vol']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the current fill-level.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Actual fill-level
+            [1] = Volume in by pump 1
+            [2] = Volume out by pump 2
+            [3] = Volume out by pump 3
+
+        Returns
+        -------
+        float
+            Actual fill-level.
+        """
+        output = p_input[0] + p_input[1] - p_input[2] - p_input[3]
+        
+        # max value - full
+        if output >= self.max_vol:
+            return self.max_vol
+        # min value - empty
+        elif output <= self.min_vol:
+            return self.min_vol
+        # current fill value
+        else:
+            return output
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TankOverflow(SimState):
+    """
+    This class serves as a component state to calculate the overflow level of the Tank.
+    Demage is posible by this component
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'TankOverflow'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_Overflow(p_name='TF_Overflow',
+                            p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                            p_dt=0,
+                            max_vol = 250)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_Overflow(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.max_vol = p_args['max_vol']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the current overflow level.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Actual fill-level
+            [1] = Volume in by pump 1
+            [2] = Volume out by pump 2
+            [3] = Volume out by pump 3
+
+        Returns
+        -------
+        float
+            Actual overflow.
+        """
+        cur_level = p_input[0] + p_input[1] - p_input[2] - p_input[3]
+        
+        # overflow
+        if cur_level > self.max_vol:
+            return cur_level - self.max_vol
+        # no overflow
+        else:
+            return 0
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class Tank(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A Tank consists of three sensors and two states components.
+        """
+        tank_sensor_1 = TankSensor1(p_name_short='TankSensor1',
+                                    p_base_set=Dimension.C_BASE_SET_Z,
+                                    p_boundaries=[0,1])
+        
+        tank_sensor_2 = TankSensor2(p_name_short='TankSensor2',
+                                    p_base_set=Dimension.C_BASE_SET_Z,
+                                    p_boundaries=[0,1])
+        
+        tank_sensor_3 = TankSensor3(p_name_short='TankSensor3',
+                                    p_base_set=Dimension.C_BASE_SET_Z,
+                                    p_boundaries=[0,1])
+        
+        tank_fill_level = TankFillLevel(p_name_short='TankFillLevel',
+                                        p_base_set=Dimension.C_BASE_SET_R,
+                                        p_unit='L',
+                                        p_boundaries=[0,250])
+        
+        tank_overflow = TankOverflow(p_name_short='TankOverflow',
+                                     p_base_set=Dimension.C_BASE_SET_R,
+                                     p_unit='L',
+                                     p_boundaries=[0,sys.maxsize])
+        
+        self._add_sensor(p_sensor=tank_sensor_1)
+        self._add_sensor(p_sensor=tank_sensor_2)
+        self._add_sensor(p_sensor=tank_sensor_3)
+
+        self._add_component_states(p_comp_states=tank_overflow)
+        self._add_component_states(p_comp_states=tank_fill_level)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C002_Hopper.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C002_Hopper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C002_Hopper.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
-## -- 2023-01-18  1.0.3     SY       Update because TransferFunction is shifted to MLPro.bf.systems
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-06  1.0.5     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Mini Hopper.
-A hopper is a component to temporary store materials that consists of a sensor.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-from mlpro_mpps.pool.comps.PS001_C001_Silo import *
-import sys
-
-
-         
-            
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class HopperSensor(SimSensor):
-    """
-    This class serves as a sensor in the upper side of the hopper to indicate whether the fill-level
-    of the hopper closes to overflow or not.
-    """
-
-    C_TYPE = 'SimSensor'
-    C_NAME = 'HopperSensor'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_BufferSensor(p_name='TF_HopperSensor',
-                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                p_dt=0,
-                                theta = 0.8*9.1) # 80% of the maximum fill-level
-        return _func
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class HopperFillLevel(SimState):
-    """
-    This class serves as a component state to calculate the actual fill-level of the hopper.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'HopperFillLevel'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_FillLevel(p_name='TF_FillLevel',
-                             p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                             p_dt=0,
-                             max_vol = 9.1,
-                             min_vol = 0)
-        return _func
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class HopperOverflow(SimState):
-    """
-    This class serves as a component state to calculate the overflow level of the hopper.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'HopperOverflow'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_Overflow(p_name='TF_Overflow',
-                            p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                            p_dt=0,
-                            max_vol = 9.1)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class Hopper(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A silo consists of two sensors and two states components.
-        """
-        hopper_sensor = HopperSensor(p_name_short='SiloSensor1',
-                                     p_base_set=Dimension.C_BASE_SET_Z,
-                                     p_boundaries=[0,1])
-        hopper_fill_level = HopperFillLevel(p_name_short='HopperFillLevel',
-                                            p_base_set=Dimension.C_BASE_SET_R,
-                                            p_unit='L',
-                                            p_boundaries=[0,9.1])
-        hopper_overflow = HopperOverflow(p_name_short='HopperOverflow',
-                                         p_base_set=Dimension.C_BASE_SET_R,
-                                         p_unit='L',
-                                         p_boundaries=[0,sys.maxsize])
-        
-        self._add_sensor(p_sensor=hopper_sensor)
-        self._add_component_states(p_comp_states=hopper_overflow)
-        self._add_component_states(p_comp_states=hopper_fill_level)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C002_Hopper.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-29  0.0.0     SY       Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
+## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
+## -- 2023-01-18  1.0.3     SY       Update because TransferFunction is shifted to MLPro.bf.systems
+## -- 2023-02-01  1.0.4     SY       Refactoring
+## -- 2023-02-06  1.0.5     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.5 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a Mini Hopper.
+A hopper is a component to temporary store materials that consists of a sensor.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+from mlpro_mpps.pool.comps.PS001_C001_Silo import *
+import sys
+
+
+         
+            
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class HopperSensor(SimSensor):
+    """
+    This class serves as a sensor in the upper side of the hopper to indicate whether the fill-level
+    of the hopper closes to overflow or not.
+    """
+
+    C_TYPE = 'SimSensor'
+    C_NAME = 'HopperSensor'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_BufferSensor(p_name='TF_HopperSensor',
+                                p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                p_dt=0,
+                                theta = 0.8*9.1) # 80% of the maximum fill-level
+        return _func
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class HopperFillLevel(SimState):
+    """
+    This class serves as a component state to calculate the actual fill-level of the hopper.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'HopperFillLevel'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_FillLevel(p_name='TF_FillLevel',
+                             p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                             p_dt=0,
+                             max_vol = 9.1,
+                             min_vol = 0)
+        return _func
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class HopperOverflow(SimState):
+    """
+    This class serves as a component state to calculate the overflow level of the hopper.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'HopperOverflow'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_Overflow(p_name='TF_Overflow',
+                            p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                            p_dt=0,
+                            max_vol = 9.1)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class Hopper(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A silo consists of two sensors and two states components.
+        """
+        hopper_sensor = HopperSensor(p_name_short='SiloSensor1',
+                                     p_base_set=Dimension.C_BASE_SET_Z,
+                                     p_boundaries=[0,1])
+        hopper_fill_level = HopperFillLevel(p_name_short='HopperFillLevel',
+                                            p_base_set=Dimension.C_BASE_SET_R,
+                                            p_unit='L',
+                                            p_boundaries=[0,9.1])
+        hopper_overflow = HopperOverflow(p_name_short='HopperOverflow',
+                                         p_base_set=Dimension.C_BASE_SET_R,
+                                         p_unit='L',
+                                         p_boundaries=[0,sys.maxsize])
+        
+        self._add_sensor(p_sensor=hopper_sensor)
+        self._add_component_states(p_comp_states=hopper_overflow)
+        self._add_component_states(p_comp_states=hopper_fill_level)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C003_ConveyorBelt.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C004_VibratoryConveyor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,207 +1,199 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C003_ConveyorBelt.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-13  1.0.2     SY       Debugging
-## -- 2023-01-16  1.0.3     SY       Debugging on TF_PowerBelt_Cont
-## -- 2023-01-18  1.0.3     SY       - Update because TransferFunction is shifted to MLPro.bf.systems
-## --                                - Update transported material function
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-06  1.0.5     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Conveyor Belt.
-A conveyor belt is located on Module 1 of the BGLP to transport materials from Silo A to Hopper A.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-import sys
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class CBTransportedMaterial(SimState):
-    """
-    This class serves as a component state to calculate the transported material.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'CBTransportedMaterial'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_TransBelt_Cont(p_name='TF_TransBelt_Cont',
-                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                  p_dt=0.05,
-                                  coef=0.01/60)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_TransBelt_Cont(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.coef = p_args['coef']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the transported material.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Rotational speed in rpm
-            [1] = Status of the actuator
-            [2] = Fill-level of the previous buffer
-        p_range : float
-            period of measuring the transported material in seconds.
-
-        Returns
-        -------
-        float
-            The transported material.
-        """
-        if p_input[1]:
-            if p_range is None:
-                mass_transport = self.coef*p_input[0]
-            else:
-                mass_transport = self.coef*p_input[0]*p_range
-            
-            if mass_transport > p_input[2]:
-                return p_input[2]
-            else:
-                return mass_transport
-        else:
-            return 0
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class CBPowerConsumption(SimState):
-    """
-    This class serves as a component state to calculate the power consumption.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'CBPowerConsumption'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_PowerBelt_Cont(p_name='TF_PowerBelt_Cont',
-                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                  p_dt=0.05,
-                                  min_power = 40.0,
-                                  max_power = 50.5,
-                                  min_rpm = 450,
-                                  max_rpm = 1850)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_PowerBelt_Cont(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.min_power = p_args['min_power']
-                self.max_power = p_args['max_power']
-                self.min_rpm = p_args['min_rpm']
-                self.max_rpm = p_args['max_rpm']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the power consumption.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Rotational speed in rpm
-            [1] = Status of the actuator
-        p_range : float
-            period of measuring the power consumption in seconds.
-
-        Returns
-        -------
-        float
-            The power consumption in kW.
-        """
-        if p_input[1]:
-            normalized_rpm = (p_input[0]-self.min_rpm)/(self.max_rpm-self.min_rpm)
-            if p_range is None:
-                power  = normalized_rpm*(self.max_power-self.min_power)+self.min_power
-            else:
-                power  = (normalized_rpm*(self.max_power-self.min_power)+self.min_power)*p_range
-            return power/1000.0
-        else:
-            return 0
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class ConveyorBelt(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A conveyor belt consists of an actuator and two states components.
-        """
-        motor = SimActuator(p_name_short='Motor',
-                            p_base_set=Dimension.C_BASE_SET_R,
-                            p_unit='rpm',
-                            p_boundaries=[450,1850])
-        transported_material = CBTransportedMaterial(p_name_short='CBTransportedMaterial',
-                                                     p_base_set=Dimension.C_BASE_SET_R,
-                                                     p_unit='L',
-                                                     p_boundaries=[0,sys.maxsize])
-        power_consumption = CBPowerConsumption(p_name_short='CBPowerConsumption',
-                                               p_base_set=Dimension.C_BASE_SET_R,
-                                               p_unit='kW',
-                                               p_boundaries=[0,sys.maxsize])
-        
-        self._add_actuator(p_actuator=motor)
-        self._add_component_states(p_comp_states=transported_material)
-        self._add_component_states(p_comp_states=power_consumption)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C004_VibratoryConveyor.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-29  0.0.0     SY       Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       - Debugging (sys.maxsize related issue)
+## --                                - Updating TF_PowerBelt_Cont
+## -- 2023-01-15  1.0.2     SY       Debugging
+## -- 2023-01-18  1.0.3     SY       - Update because TransferFunction is shifted to MLPro.bf.systems
+## --                                - Update transported material function
+## -- 2023-02-01  1.0.4     SY       Refactoring
+## -- 2023-02-06  1.0.5     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.5 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a Vibratory
+Conveyor.
+A vibratory conveyor is located on Module 2 of the BGLP to transport materials from Silo B to
+Hopper B.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+import sys
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VCTransportedMaterial(SimState):
+    """
+    This class serves as a component state to calculate the transported material.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'VCTransportedMaterial'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_TransBelt_Binary(p_name='TF_TransBelt_Binary',
+                                    p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                    p_dt=0.05,
+                                    coef=0.40)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_TransBelt_Binary(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.coef = p_args['coef']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the transported material.
+
+        Parameters
+        ----------
+        p_input : boolean
+            [0] Status of the actuator
+            [1] Fill-level of the previous buffer
+        p_range : float
+            period of measuring the transported material in seconds.
+
+        Returns
+        -------
+        float
+            The transported material.
+        """
+        if p_input[0]:
+            if p_range is None:
+                mass_transport = self.coef
+            else:
+                mass_transport = self.coef*p_range
+        
+            if mass_transport > p_input[1]:
+                return p_input[1]
+            else:
+                return mass_transport
+        else:
+            return 0
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VCPowerConsumption(SimState):
+    """
+    This class serves as a component state to calculate the power consumption.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'VCPowerConsumption'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_PowerBelt_Binary(p_name='TF_PowerBelt_Binary',
+                                    p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                    power = 26.9)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_PowerBelt_Binary(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.power = p_args['power']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the power consumption.
+
+        Parameters
+        ----------
+        p_input : boolean
+            Status of the actuator
+        p_range : float
+            period of measuring the power consumption in seconds.
+
+        Returns
+        -------
+        float
+            The power consumption in kW.
+        """
+        if p_input:
+            if p_range is None:
+                power  = self.power
+            else:
+                power  = self.power*p_range
+            return power/1000.0
+        else:
+            return 0
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VibratoryConveyor(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A vibratory conveyor consists of an actuator and two states components.
+        """
+        switch = SimActuator(p_name_short='Switch',
+                             p_base_set=Dimension.C_BASE_SET_Z,
+                             p_unit='',
+                             p_boundaries=[0,1])
+        transported_material = VCTransportedMaterial(p_name_short='VCTransportedMaterial',
+                                                     p_base_set=Dimension.C_BASE_SET_R,
+                                                     p_unit='L',
+                                                     p_boundaries=[0,sys.maxsize])
+        power_consumption = VCPowerConsumption(p_name_short='VCPowerConsumption',
+                                               p_base_set=Dimension.C_BASE_SET_R,
+                                               p_unit='kW',
+                                               p_boundaries=[0,sys.maxsize])
+        
+        self._add_actuator(p_actuator=switch)
+        self._add_component_states(p_comp_states=transported_material)
+        self._add_component_states(p_comp_states=power_consumption)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C005_RotaryFeeder.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C005_RotaryFeeder.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C005_RotaryFeeder.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-18  1.0.2     SY       Update because TransferFunction is shifted to MLPro.bf.systems
-## -- 2023-02-01  1.0.3     SY       Refactoring
-## -- 2023-02-06  1.0.4     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.4 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Rotary Feeder.
-A rotary feeder is located on Module 3 of the BGLP to transport materials from Silo C to Hopper C.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-from mlpro_mpps.pool.comps.PS001_C003_ConveyorBelt import *
-import sys
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class RFTransportedMaterial(SimState):
-    """
-    This class serves as a component state to calculate the transported material.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'RFTransportedMaterial'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_TransBelt_Cont(p_name='TF_TransBelt_Cont',
-                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                  p_dt=0.05,
-                                  coef=0.01249/60)
-        return _func
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class RFPowerConsumption(SimState):
-    """
-    This class serves as a component state to calculate the power consumption.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'RFPowerConsumption'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_PowerBelt_Cont(p_name='TF_PowerBelt_Cont',
-                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                  p_dt=0.05,
-                                  min_power = 114.828,
-                                  max_power = 370,
-                                  min_rpm = 450,
-                                  max_rpm = 1450)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class RotaryFeeder(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A rotary feeder consists of an actuator and two states components.
-        """
-        motor = SimActuator(p_name_short='Motor',
-                            p_base_set=Dimension.C_BASE_SET_R,
-                            p_unit='rpm',
-                            p_boundaries=[450,1450])
-        transported_material = RFTransportedMaterial(p_name_short='RFTransportedMaterial',
-                                                     p_base_set=Dimension.C_BASE_SET_R,
-                                                     p_unit='L',
-                                                     p_boundaries=[0,sys.maxsize])
-        power_consumption = RFPowerConsumption(p_name_short='RFPowerConsumption',
-                                               p_base_set=Dimension.C_BASE_SET_R,
-                                               p_unit='kW',
-                                               p_boundaries=[0,sys.maxsize])
-        
-        self._add_actuator(p_actuator=motor)
-        self._add_component_states(p_comp_states=transported_material)
-        self._add_component_states(p_comp_states=power_consumption)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C005_RotaryFeeder.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-29  0.0.0     SY       Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
+## -- 2023-01-18  1.0.2     SY       Update because TransferFunction is shifted to MLPro.bf.systems
+## -- 2023-02-01  1.0.3     SY       Refactoring
+## -- 2023-02-06  1.0.4     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.4 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a Rotary Feeder.
+A rotary feeder is located on Module 3 of the BGLP to transport materials from Silo C to Hopper C.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+from mlpro_mpps.pool.comps.PS001_C003_ConveyorBelt import *
+import sys
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class RFTransportedMaterial(SimState):
+    """
+    This class serves as a component state to calculate the transported material.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'RFTransportedMaterial'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_TransBelt_Cont(p_name='TF_TransBelt_Cont',
+                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                  p_dt=0.05,
+                                  coef=0.01249/60)
+        return _func
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class RFPowerConsumption(SimState):
+    """
+    This class serves as a component state to calculate the power consumption.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'RFPowerConsumption'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_PowerBelt_Cont(p_name='TF_PowerBelt_Cont',
+                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                  p_dt=0.05,
+                                  min_power = 114.828,
+                                  max_power = 370,
+                                  min_rpm = 450,
+                                  max_rpm = 1450)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class RotaryFeeder(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A rotary feeder consists of an actuator and two states components.
+        """
+        motor = SimActuator(p_name_short='Motor',
+                            p_base_set=Dimension.C_BASE_SET_R,
+                            p_unit='rpm',
+                            p_boundaries=[450,1450])
+        transported_material = RFTransportedMaterial(p_name_short='RFTransportedMaterial',
+                                                     p_base_set=Dimension.C_BASE_SET_R,
+                                                     p_unit='L',
+                                                     p_boundaries=[0,sys.maxsize])
+        power_consumption = RFPowerConsumption(p_name_short='RFPowerConsumption',
+                                               p_base_set=Dimension.C_BASE_SET_R,
+                                               p_unit='kW',
+                                               p_boundaries=[0,sys.maxsize])
+        
+        self._add_actuator(p_actuator=motor)
+        self._add_component_states(p_comp_states=transported_material)
+        self._add_component_states(p_comp_states=power_consumption)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C006_VacuumPump1.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS002_C002_Pump1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,211 +1,205 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C006_VacuumPump1.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-13  1.0.2     SY       Debugging
-## -- 2023-01-18  1.0.3     SY       - Update because TransferFunction is shifted to MLPro.bf.systems
-## --                                - Update transported material function
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-06  1.0.5     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Vacuum Pump.
-This vacuum pump is located on Module 2 of the BGLP to transport materials from Hopper A to Silo B.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-import sys
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VC1TransportedMaterial(SimState):
-    """
-    This class serves as a component state to calculate the transported material.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'VC1TransportedMaterial'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_VacuumPump(p_name='TF_VacuumPump',
-                              p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                              p_dt=0.05,
-                              coef=[0.464, 0.0332])
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_VacuumPump(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.coef = p_args['coef']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the transported material.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Turn-on duration
-            [1] = Status of the actuator
-            [2] = Fill-level of the previous buffer
-        p_range : float
-            period of measuring the transported material in seconds.
-
-        Returns
-        -------
-        float
-            The transported material.
-        """
-        if p_input[1]:
-            if p_range is None:
-                mass_transport = (2*self.coef[1])+self.coef[0]
-            else:
-                if p_input[0] <= p_range:
-                    mass_transport = ((2*self.coef[1])+self.coef[0])*p_input[0]
-                else:
-                    mass_transport = ((2*self.coef[1])+self.coef[0])*p_range
-        
-            if mass_transport > p_input[2]:
-                return p_input[2]
-            else:
-                return mass_transport
-        else:
-            return 0
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VC1PowerConsumption(SimState):
-    """
-    This class serves as a component state to calculate the power consumption.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'VC1PowerConsumption'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_PowerVacuumPump(p_name='TF_PowerVacuumPump',
-                                   p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                   p_dt=0.05,
-                                   min_power = 0,
-                                   max_power = 305,
-                                   min_duration = 0.567,
-                                   max_duration = 4.575)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_PowerVacuumPump(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.min_power = p_args['min_power']
-                self.max_power = p_args['max_power']
-                self.min_duration = p_args['min_duration']
-                self.max_duration = p_args['max_duration']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the power consumption.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Turn-on duration
-            [1] = Status of the actuator
-        p_range : float
-            period of measuring the power consumption in seconds.
-
-        Returns
-        -------
-        float
-            The power consumption in kW.
-        """
-        if p_input[1]:
-            if p_range is None:
-                power = self.max_power
-            else:
-                if p_input[0] <= p_range:
-                    power = self.max_power*p_input[0]
-                else:
-                    power = self.max_power*p_range
-            return power/1000.0
-        else:
-            return 0
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VacuumPump1(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A vacuum pump consists of an actuator and two states components.
-        """
-        timer = SimActuator(p_name_short='Timer',
-                            p_base_set=Dimension.C_BASE_SET_R,
-                            p_unit='s',
-                            p_boundaries=[0.567, 4.575])
-        transported_material = VC1TransportedMaterial(p_name_short='VC1TransportedMaterial',
-                                                      p_base_set=Dimension.C_BASE_SET_R,
-                                                      p_unit='L',
-                                                      p_boundaries=[0,sys.maxsize])
-        power_consumption = VC1PowerConsumption(p_name_short='VC1PowerConsumption',
-                                                p_base_set=Dimension.C_BASE_SET_R,
-                                                p_unit='kW',
-                                                p_boundaries=[0,sys.maxsize])
-        
-        self._add_actuator(p_actuator=timer)
-        self._add_component_states(p_comp_states=transported_material)
-        self._add_component_states(p_comp_states=power_consumption)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS002_C002_Pump1.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2023-01-19  0.0.0     ML       Creation
+## -- 2023-03-28  1.0.0     ML/SY    Release of first version
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.0 (2023-03-28)
+
+This module provides a default implementation of a component of the Liquid Station, which is a Pump.
+This pump is located on the input side of the Liquid Station to fill liquid into the tank.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+import sys
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class PC1TransportedLiquid(SimState):
+    """
+    This class serves as a component state to calculate the transported liquid.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'PC1TransportedLiquid'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_Pump(p_name='TF_Pump',
+                        p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                        p_dt=0.05,
+                        coef=[0.464, 0.0332]
+                        )
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_Pump(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.coef = p_args['coef']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the transported material.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Turn-on duration
+            [1] = Status of the actuator
+        p_range : float
+            period of measuring the transported material in seconds.
+
+        Returns
+        -------
+        float
+            The transported material.
+        """
+        if p_input[1]:
+            if p_range is None:
+                mass_transport = (2*self.coef[1])+self.coef[0]
+            else:
+                if p_input[0] <= p_range:
+                    mass_transport = ((2*self.coef[1])+self.coef[0])*p_input[0]
+                else:
+                    mass_transport = ((2*self.coef[1])+self.coef[0])*p_range
+            return mass_transport
+        else:
+            return 0
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class PC1PowerConsumption(SimState):
+    """
+    This class serves as a component state to calculate the power consumption of a pump.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'PC1PowerConsumption'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_PowerPump(p_name='TF_PowerPump',
+                                   p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                   p_dt=0.05,
+                                   min_power = 0,
+                                   max_power = 305,
+                                   min_duration = 0.567,
+                                   max_duration = 4.575)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_PowerPump(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.min_power = p_args['min_power']
+                self.max_power = p_args['max_power']
+                self.min_duration = p_args['min_duration']
+                self.max_duration = p_args['max_duration']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the power consumption.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Turn-on duration
+            [1] = Status of the actuator
+        p_range : float
+            period of measuring the power consumption in seconds.
+
+        Returns
+        -------
+        float
+            The power consumption in kW.
+        """
+        if p_input[1]:
+            if p_range is None:
+                power = self.max_power
+            else:
+                if p_input[0] <= p_range:
+                    power = self.max_power*p_input[0]
+                else:
+                    power = self.max_power*p_range
+            return power/1000.0
+        else:
+            return 0
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class Pump1(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A pump consists of an actuator and two states components.
+        """
+        timer = SimActuator(p_name_short='Timer1',
+                            p_base_set=Dimension.C_BASE_SET_R,
+                            p_unit='s',
+                            p_boundaries=[0.567, 4.575])
+        
+        transported_liquid = PC1TransportedLiquid(p_name_short='PC1TransportedMaterial',
+                                                  p_base_set=Dimension.C_BASE_SET_R,
+                                                  p_unit='L',
+                                                  p_boundaries=[0,sys.maxsize]
+                                                  )
+        
+        power_consumption = PC1PowerConsumption(p_name_short='PC1PowerConsumption',
+                                                p_base_set=Dimension.C_BASE_SET_R,
+                                                p_unit='kW',
+                                                p_boundaries=[0,sys.maxsize]
+                                                )
+        
+        self._add_actuator(p_actuator=timer)
+        self._add_component_states(p_comp_states=transported_liquid)
+        self._add_component_states(p_comp_states=power_consumption)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C007_VacuumPump2.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C007_VacuumPump2.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C007_VacuumPump2.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-18  1.0.2     SY       Update because TransferFunction is shifted to MLPro.bf.systems
-## -- 2023-02-01  1.0.3     SY       Refactoring
-## -- 2023-02-06  1.0.4     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.4 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Vacuum Pump.
-This vacuum pump is located on Module 3 of the BGLP to transport materials from Hopper B to Silo C.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-from mlpro_mpps.pool.comps.PS001_C006_VacuumPump1 import *
-import sys
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VC2TransportedMaterial(SimState):
-    """
-    This class serves as a component state to calculate the transported material.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'VC2TransportedMaterial'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_VacuumPump(p_name='TF_VacuumPump',
-                              p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                              p_dt=0.05,
-                              coef=[0.3535, 0.0096])
-        return _func
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VC2PowerConsumption(SimState):
-    """
-    This class serves as a component state to calculate the power consumption.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'VC2PowerConsumption'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_PowerVacuumPump(p_name='TF_PowerVacuumPump',
-                                   p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                   p_dt=0.05,
-                                   min_power = 0,
-                                   max_power = 456,
-                                   min_duration = 0.979,
-                                   max_duration = 9.5)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VacuumPump2(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A vacuum pump consists of an actuator and two states components.
-        """
-        timer = SimActuator(p_name_short='Timer',
-                            p_base_set=Dimension.C_BASE_SET_R,
-                            p_unit='s',
-                            p_boundaries=[0.979, 9.5])
-        transported_material = VC2TransportedMaterial(p_name_short='VC2TransportedMaterial',
-                                                      p_base_set=Dimension.C_BASE_SET_R,
-                                                      p_unit='L',
-                                                      p_boundaries=[0,sys.maxsize])
-        power_consumption = VC2PowerConsumption(p_name_short='VC2PowerConsumption',
-                                                p_base_set=Dimension.C_BASE_SET_R,
-                                                p_unit='kW',
-                                                p_boundaries=[0,sys.maxsize])
-        
-        self._add_actuator(p_actuator=timer)
-        self._add_component_states(p_comp_states=transported_material)
-        self._add_component_states(p_comp_states=power_consumption)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C007_VacuumPump2.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-29  0.0.0     SY       Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
+## -- 2023-01-18  1.0.2     SY       Update because TransferFunction is shifted to MLPro.bf.systems
+## -- 2023-02-01  1.0.3     SY       Refactoring
+## -- 2023-02-06  1.0.4     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.4 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a Vacuum Pump.
+This vacuum pump is located on Module 3 of the BGLP to transport materials from Hopper B to Silo C.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+from mlpro_mpps.pool.comps.PS001_C006_VacuumPump1 import *
+import sys
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VC2TransportedMaterial(SimState):
+    """
+    This class serves as a component state to calculate the transported material.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'VC2TransportedMaterial'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_VacuumPump(p_name='TF_VacuumPump',
+                              p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                              p_dt=0.05,
+                              coef=[0.3535, 0.0096])
+        return _func
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VC2PowerConsumption(SimState):
+    """
+    This class serves as a component state to calculate the power consumption.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'VC2PowerConsumption'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_PowerVacuumPump(p_name='TF_PowerVacuumPump',
+                                   p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                   p_dt=0.05,
+                                   min_power = 0,
+                                   max_power = 456,
+                                   min_duration = 0.979,
+                                   max_duration = 9.5)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VacuumPump2(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A vacuum pump consists of an actuator and two states components.
+        """
+        timer = SimActuator(p_name_short='Timer',
+                            p_base_set=Dimension.C_BASE_SET_R,
+                            p_unit='s',
+                            p_boundaries=[0.979, 9.5])
+        transported_material = VC2TransportedMaterial(p_name_short='VC2TransportedMaterial',
+                                                      p_base_set=Dimension.C_BASE_SET_R,
+                                                      p_unit='L',
+                                                      p_boundaries=[0,sys.maxsize])
+        power_consumption = VC2PowerConsumption(p_name_short='VC2PowerConsumption',
+                                                p_base_set=Dimension.C_BASE_SET_R,
+                                                p_unit='kW',
+                                                p_boundaries=[0,sys.maxsize])
+        
+        self._add_actuator(p_actuator=timer)
+        self._add_component_states(p_comp_states=transported_material)
+        self._add_component_states(p_comp_states=power_consumption)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C008_VacuumPump3.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C008_VacuumPump3.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C008_VacuumPump3.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-30  0.0.0     SY       Creation
-## -- 2022-12-30  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-15  1.0.2     SY       Debugging
-## -- 2023-01-18  1.0.3     SY       - Update because TransferFunction is shifted to MLPro.bf.systems
-## --                                - Update transported material function
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-06  1.0.5     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Vacuum Pump.
-This vacuum pump is located on Module 4 of the BGLP to transport materials from Hopper C to
-finished good inventory with a constant outflow.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-import sys
-
-
-
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VC3TransportedMaterial(SimState):
-    """
-    This class serves as a component state to calculate the transported material.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'VC3TransportedMaterial'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_ConstVacuumPump(p_name='TF_ConstVacuumPump',
-                                   p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                   p_dt=0.05,
-                                   prod_target=0.1)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_ConstVacuumPump(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.prod_target = p_args['prod_target']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the transported material.
-
-        Parameters
-        ----------
-        p_input : boolean
-            [0] Status of the actuator
-            [1] Fill-level of the previous buffer
-        p_range : float
-            period of measuring the transported material in seconds.
-
-        Returns
-        -------
-        float
-            The transported material.
-        """
-        if p_input:
-            if p_range is None:
-                mass_transport = self.prod_target
-            else:
-                mass_transport = self.prod_target*p_range
-        
-            if mass_transport > p_input[1]:
-                return p_input[1]
-            else:
-                return mass_transport
-        else:
-            return 0
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class VacuumPump3(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A vacuum pump consists of an actuator and two states components.
-        """
-        switch = SimActuator(p_name_short='Switch',
-                             p_base_set=Dimension.C_BASE_SET_Z,
-                             p_unit='s',
-                             p_boundaries=[0, 1])
-        transported_material = VC3TransportedMaterial(p_name_short='VC1TransportedMaterial',
-                                                      p_base_set=Dimension.C_BASE_SET_R,
-                                                      p_unit='L',
-                                                      p_boundaries=[0,sys.maxsize])
-        
-        self._add_actuator(p_actuator=switch)
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C008_VacuumPump3.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-30  0.0.0     SY       Creation
+## -- 2022-12-30  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
+## -- 2023-01-15  1.0.2     SY       Debugging
+## -- 2023-01-18  1.0.3     SY       - Update because TransferFunction is shifted to MLPro.bf.systems
+## --                                - Update transported material function
+## -- 2023-02-01  1.0.4     SY       Refactoring
+## -- 2023-02-06  1.0.5     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.5 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a Vacuum Pump.
+This vacuum pump is located on Module 4 of the BGLP to transport materials from Hopper C to
+finished good inventory with a constant outflow.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+import sys
+
+
+
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VC3TransportedMaterial(SimState):
+    """
+    This class serves as a component state to calculate the transported material.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'VC3TransportedMaterial'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_ConstVacuumPump(p_name='TF_ConstVacuumPump',
+                                   p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                   p_dt=0.05,
+                                   prod_target=0.1)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_ConstVacuumPump(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.prod_target = p_args['prod_target']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the transported material.
+
+        Parameters
+        ----------
+        p_input : boolean
+            [0] Status of the actuator
+            [1] Fill-level of the previous buffer
+        p_range : float
+            period of measuring the transported material in seconds.
+
+        Returns
+        -------
+        float
+            The transported material.
+        """
+        if p_input:
+            if p_range is None:
+                mass_transport = self.prod_target
+            else:
+                mass_transport = self.prod_target*p_range
+        
+            if mass_transport > p_input[1]:
+                return p_input[1]
+            else:
+                return mass_transport
+        else:
+            return 0
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class VacuumPump3(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A vacuum pump consists of an actuator and two states components.
+        """
+        switch = SimActuator(p_name_short='Switch',
+                             p_base_set=Dimension.C_BASE_SET_Z,
+                             p_unit='s',
+                             p_boundaries=[0, 1])
+        transported_material = VC3TransportedMaterial(p_name_short='VC1TransportedMaterial',
+                                                      p_base_set=Dimension.C_BASE_SET_R,
+                                                      p_unit='L',
+                                                      p_boundaries=[0,sys.maxsize])
+        
+        self._add_actuator(p_actuator=switch)
         self._add_component_states(p_comp_states=transported_material)
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C009_Inventory.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C009_Inventory.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C009_Inventory.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-30  0.0.0     SY       Creation
-## -- 2022-12-30  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-18  1.0.2     SY       Update because TransferFunction is shifted to MLPro.bf.systems
-## -- 2023-02-01  1.0.3     SY       Refactoring
-## -- 2023-02-06  1.0.4     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.4 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a finished goods
-inventory.
-A finished good inventory is a component to store the finished goods before being sent to the
-next process or packaged.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-import sys
-
-
-         
-            
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class InventoryLevel(SimState):
-    """
-    This class serves as a component state to calculate the actual level of the inventory.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'InventoryLevel'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_InventoryLevel(p_name='TF_InventoryLevel',
-                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                  p_dt=0)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_InventoryLevel(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            pass          
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the current level.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Current level
-            [1] = Volume in
-
-        Returns
-        -------
-        float
-            Actual level.
-        """
-        return p_input[0]+p_input[1]
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class FinishedGoodsInventory(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A silo consists of two sensors and two states components.
-        """
-        inventory_level = InventoryLevel(p_name_short='InventoryLevel',
-                                        p_base_set=Dimension.C_BASE_SET_R,
-                                        p_unit='L',
-                                        p_boundaries=[0,sys.maxsize])
-        
-        self._add_component_states(p_comp_states=inventory_level)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C009_Inventory.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-30  0.0.0     SY       Creation
+## -- 2022-12-30  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
+## -- 2023-01-18  1.0.2     SY       Update because TransferFunction is shifted to MLPro.bf.systems
+## -- 2023-02-01  1.0.3     SY       Refactoring
+## -- 2023-02-06  1.0.4     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.4 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a finished goods
+inventory.
+A finished good inventory is a component to store the finished goods before being sent to the
+next process or packaged.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+import sys
+
+
+         
+            
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class InventoryLevel(SimState):
+    """
+    This class serves as a component state to calculate the actual level of the inventory.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'InventoryLevel'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_InventoryLevel(p_name='TF_InventoryLevel',
+                                  p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                  p_dt=0)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_InventoryLevel(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            pass          
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the current level.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Current level
+            [1] = Volume in
+
+        Returns
+        -------
+        float
+            Actual level.
+        """
+        return p_input[0]+p_input[1]
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class FinishedGoodsInventory(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A silo consists of two sensors and two states components.
+        """
+        inventory_level = InventoryLevel(p_name_short='InventoryLevel',
+                                        p_base_set=Dimension.C_BASE_SET_R,
+                                        p_unit='L',
+                                        p_boundaries=[0,sys.maxsize])
+        
+        self._add_component_states(p_comp_states=inventory_level)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/comps/PS001_C010_SiloLoading.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/comps/PS001_C010_SiloLoading.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.comps
-## -- Module  : PS001_C010_SiloLoading.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-30  0.0.0     SY       Creation
-## -- 2022-12-30  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
-## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
-## -- 2023-01-18  1.0.3     SY       Update because TransferFunction is shifted to MLPro.bf.systems
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-06  1.0.5     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-06)
-
-This module provides a default implementation of a component of the BGLP, which is a Silo in a
-Loading station with special mechanism.
-A silo is a component to temporary store materials that consists of two sensors.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro.bf.physics import TransferFunction
-from mlpro.bf.math import *
-from mlpro_mpps.pool.comps.PS001_C001_Silo import *
-import sys
-
-
-
-
-
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloLoadingFillLevel(SimState):
-    """
-    This class serves as a component state to calculate the actual fill-level of the silo.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'SiloLoadingFillLevel'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_FillLevel_Loading(p_name='TF_FillLevel_Loading',
-                                     p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                     p_dt=0,
-                                     max_vol = 17.42,
-                                     min_vol = 0,
-                                     theta_loading = 0.3*17.42)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_FillLevel_Loading(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.max_vol = p_args['max_vol']
-                self.min_vol = p_args['min_vol']
-                self.theta_loading = p_args['theta_loading']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the current fill-level.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Actual fill-level
-            [1] = Volume out
-
-        Returns
-        -------
-        float
-            Actual fill-level.
-        """
-        output = p_input[0]-p_input[1]
-        
-        if output >= self.max_vol:
-            return self.max_vol
-        elif output <= self.theta_loading:
-            return self.theta_loading
-        elif output <= self.min_vol:
-            return self.min_vol
-        else:
-            return output
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloLoadingOverflow(SimState):
-    """
-    This class serves as a component state to calculate the overflow level of the silo.
-    """
-
-    C_TYPE = 'SimState'
-    C_NAME = 'SiloLoadingOverflow'
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _setup_function(self) -> TransferFunction:
-        _func = TF_Overflow_Loading(p_name='TF_Overflow_Loading',
-                                    p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
-                                    p_dt=0,
-                                    max_vol = 17.42,
-                                    theta_loading = 0.3*17.42)
-        return _func
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class TF_Overflow_Loading(TransferFunction):
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _set_function_parameters(self, p_args) -> bool:
-        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
-            try:
-                self.max_vol = p_args['max_vol']
-                self.theta_loading = p_args['theta_loading']
-            except:
-                raise NotImplementedError('One/More parameters for this function is missing.')           
-        return True
-  
-    
-## -------------------------------------------------------------------------------------------------      
-    def _custom_function(self, p_input, p_range=None):
-        """
-        To measure the current overflow level.
-
-        Parameters
-        ----------
-        p_input : list
-            [0] = Actual fill-level
-            [1] = Volume out
-
-        Returns
-        -------
-        float
-            Actual fill-level.
-        """
-        cur_level = p_input[0]-p_input[1]
-        
-        if cur_level > self.max_vol:
-            return cur_level-self.max_vol
-        else:
-            return 0
-
-
-                 
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class SiloLoading(Component):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_component(self):
-        """
-        A silo consists of two sensors and two states components.
-        """
-        silo_sensor_1 = SiloSensor1(p_name_short='SiloSensor1',
-                                    p_base_set=Dimension.C_BASE_SET_Z,
-                                    p_boundaries=[0,1])
-        silo_sensor_2 = SiloSensor2(p_name_short='SiloSensor2',
-                                    p_base_set=Dimension.C_BASE_SET_Z,
-                                    p_boundaries=[0,1])
-        silo_fill_level = SiloLoadingFillLevel(p_name_short='SiloLoadingFillLevel',
-                                               p_base_set=Dimension.C_BASE_SET_R,
-                                               p_unit='L',
-                                               p_boundaries=[0,17.42])
-        silo_overflow = SiloLoadingOverflow(p_name_short='SiloLoadingOverflow',
-                                            p_base_set=Dimension.C_BASE_SET_R,
-                                            p_unit='L',
-                                            p_boundaries=[0,sys.maxsize])
-        
-        self._add_sensor(p_sensor=silo_sensor_1)
-        self._add_sensor(p_sensor=silo_sensor_2)
-        self._add_component_states(p_comp_states=silo_overflow)
-        self._add_component_states(p_comp_states=silo_fill_level)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.comps
+## -- Module  : PS001_C010_SiloLoading.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-30  0.0.0     SY       Creation
+## -- 2022-12-30  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging (sys.maxsize related issue)
+## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
+## -- 2023-01-18  1.0.3     SY       Update because TransferFunction is shifted to MLPro.bf.systems
+## -- 2023-02-01  1.0.4     SY       Refactoring
+## -- 2023-02-06  1.0.5     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.5 (2023-02-06)
+
+This module provides a default implementation of a component of the BGLP, which is a Silo in a
+Loading station with special mechanism.
+A silo is a component to temporary store materials that consists of two sensors.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro.bf.physics import TransferFunction
+from mlpro.bf.math import *
+from mlpro_mpps.pool.comps.PS001_C001_Silo import *
+import sys
+
+
+
+
+
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SiloLoadingFillLevel(SimState):
+    """
+    This class serves as a component state to calculate the actual fill-level of the silo.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'SiloLoadingFillLevel'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_FillLevel_Loading(p_name='TF_FillLevel_Loading',
+                                     p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                     p_dt=0,
+                                     max_vol = 17.42,
+                                     min_vol = 0,
+                                     theta_loading = 0.3*17.42)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_FillLevel_Loading(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.max_vol = p_args['max_vol']
+                self.min_vol = p_args['min_vol']
+                self.theta_loading = p_args['theta_loading']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the current fill-level.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Actual fill-level
+            [1] = Volume out
+
+        Returns
+        -------
+        float
+            Actual fill-level.
+        """
+        output = p_input[0]-p_input[1]
+        
+        if output >= self.max_vol:
+            return self.max_vol
+        elif output <= self.theta_loading:
+            return self.theta_loading
+        elif output <= self.min_vol:
+            return self.min_vol
+        else:
+            return output
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SiloLoadingOverflow(SimState):
+    """
+    This class serves as a component state to calculate the overflow level of the silo.
+    """
+
+    C_TYPE = 'SimState'
+    C_NAME = 'SiloLoadingOverflow'
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _setup_function(self) -> TransferFunction:
+        _func = TF_Overflow_Loading(p_name='TF_Overflow_Loading',
+                                    p_type=TransferFunction.C_TRF_FUNC_CUSTOM,
+                                    p_dt=0,
+                                    max_vol = 17.42,
+                                    theta_loading = 0.3*17.42)
+        return _func
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class TF_Overflow_Loading(TransferFunction):
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _set_function_parameters(self, p_args) -> bool:
+        if self.get_type() == self.C_TRF_FUNC_CUSTOM:
+            try:
+                self.max_vol = p_args['max_vol']
+                self.theta_loading = p_args['theta_loading']
+            except:
+                raise NotImplementedError('One/More parameters for this function is missing.')           
+        return True
+  
+    
+## -------------------------------------------------------------------------------------------------      
+    def _custom_function(self, p_input, p_range=None):
+        """
+        To measure the current overflow level.
+
+        Parameters
+        ----------
+        p_input : list
+            [0] = Actual fill-level
+            [1] = Volume out
+
+        Returns
+        -------
+        float
+            Actual fill-level.
+        """
+        cur_level = p_input[0]-p_input[1]
+        
+        if cur_level > self.max_vol:
+            return cur_level-self.max_vol
+        else:
+            return 0
+
+
+                 
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class SiloLoading(Component):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_component(self):
+        """
+        A silo consists of two sensors and two states components.
+        """
+        silo_sensor_1 = SiloSensor1(p_name_short='SiloSensor1',
+                                    p_base_set=Dimension.C_BASE_SET_Z,
+                                    p_boundaries=[0,1])
+        silo_sensor_2 = SiloSensor2(p_name_short='SiloSensor2',
+                                    p_base_set=Dimension.C_BASE_SET_Z,
+                                    p_boundaries=[0,1])
+        silo_fill_level = SiloLoadingFillLevel(p_name_short='SiloLoadingFillLevel',
+                                               p_base_set=Dimension.C_BASE_SET_R,
+                                               p_unit='L',
+                                               p_boundaries=[0,17.42])
+        silo_overflow = SiloLoadingOverflow(p_name_short='SiloLoadingOverflow',
+                                            p_base_set=Dimension.C_BASE_SET_R,
+                                            p_unit='L',
+                                            p_boundaries=[0,sys.maxsize])
+        
+        self._add_sensor(p_sensor=silo_sensor_1)
+        self._add_sensor(p_sensor=silo_sensor_2)
+        self._add_component_states(p_comp_states=silo_overflow)
+        self._add_component_states(p_comp_states=silo_fill_level)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M001_Loading.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M001_Loading.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.mods
-## -- Module  : PS001_M001_Loading.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2022-12-30  1.0.1     SY       Update Silo A component with SiloLoading
-## -- 2023-02-01  1.0.2     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.2 (2023-02-01)
-
-This module provides a default implementation of a module of the BGLP, which is a Loading station
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro_mpps.pool.comps.PS001_C010_SiloLoading import *
-from mlpro_mpps.pool.comps.PS001_C002_Hopper import *
-from mlpro_mpps.pool.comps.PS001_C003_ConveyorBelt import *
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class LoadingStation(Module):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_module(self):
-        """
-        Loading station consists of a silo, a hopper, and a conveyor belt.
-        """
-        silo = SiloLoading(p_name='SiloA')
-        hopper = Hopper(p_name='HopperA')
-        belt = ConveyorBelt(p_name='BeltA')
-        
-        self._add_component(p_component=silo)
-        self._add_component(p_component=hopper)
-        self._add_component(p_component=belt)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.mods
+## -- Module  : PS001_M001_Loading.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-29  0.0.0     SY       Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2022-12-30  1.0.1     SY       Update Silo A component with SiloLoading
+## -- 2023-02-01  1.0.2     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.2 (2023-02-01)
+
+This module provides a default implementation of a module of the BGLP, which is a Loading station
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro_mpps.pool.comps.PS001_C010_SiloLoading import *
+from mlpro_mpps.pool.comps.PS001_C002_Hopper import *
+from mlpro_mpps.pool.comps.PS001_C003_ConveyorBelt import *
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class LoadingStation(Module):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_module(self):
+        """
+        Loading station consists of a silo, a hopper, and a conveyor belt.
+        """
+        silo = SiloLoading(p_name='SiloA')
+        hopper = Hopper(p_name='HopperA')
+        belt = ConveyorBelt(p_name='BeltA')
+        
+        self._add_component(p_component=silo)
+        self._add_component(p_component=hopper)
+        self._add_component(p_component=belt)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M002_Storing.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M003_Weighing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.mods
-## -- Module  : PS001_M002_Storing.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-02-01  1.0.1     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.1 (2023-02-01)
-
-This module provides a default implementation of a module of the BGLP, which is a Storing station
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro_mpps.pool.comps.PS001_C001_Silo import *
-from mlpro_mpps.pool.comps.PS001_C002_Hopper import *
-from mlpro_mpps.pool.comps.PS001_C004_VibratoryConveyor import *
-from mlpro_mpps.pool.comps.PS001_C006_VacuumPump1 import *
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class StoringStation(Module):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_module(self):
-        """
-        Storing station consists of a silo, a hopper, a vibratory conveyor, and a vacuum pump.
-        """
-        hopper = Hopper(p_name='HopperB')
-        silo = Silo(p_name='SiloB')
-        vac = VacuumPump1(p_name='VacB')
-        belt = VibratoryConveyor(p_name='BeltB')
-        
-        self._add_component(p_component=silo)
-        self._add_component(p_component=hopper)
-        self._add_component(p_component=vac)
-        self._add_component(p_component=belt)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.mods
+## -- Module  : PS001_M003_Weighing.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-29  0.0.0     SY       Creation
+## -- 2022-12-29  1.0.0     SY       Release of first version
+## -- 2023-02-01  1.0.1     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.1 (2023-02-01)
+
+This module provides a default implementation of a module of the BGLP, which is a Weighing station
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro_mpps.pool.comps.PS001_C001_Silo import *
+from mlpro_mpps.pool.comps.PS001_C002_Hopper import *
+from mlpro_mpps.pool.comps.PS001_C005_RotaryFeeder import *
+from mlpro_mpps.pool.comps.PS001_C007_VacuumPump2 import *
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class WeighingStation(Module):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_module(self):
+        """
+        Storing station consists of a silo, a hopper, a rotary feeder, and a vacuum pump.
+        """
+        hopper = Hopper(p_name='HopperC')
+        silo = Silo(p_name='SiloC')
+        vac = VacuumPump2(p_name='VacC')
+        belt = RotaryFeeder(p_name='BeltC')
+        
+        self._add_component(p_component=silo)
+        self._add_component(p_component=hopper)
+        self._add_component(p_component=vac)
+        self._add_component(p_component=belt)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mods/PS001_M003_Weighing.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mods/PS001_M004_Filling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.mods
-## -- Module  : PS001_M003_Weighing.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-29  0.0.0     SY       Creation
-## -- 2022-12-29  1.0.0     SY       Release of first version
-## -- 2023-02-01  1.0.1     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.1 (2023-02-01)
-
-This module provides a default implementation of a module of the BGLP, which is a Weighing station
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro_mpps.pool.comps.PS001_C001_Silo import *
-from mlpro_mpps.pool.comps.PS001_C002_Hopper import *
-from mlpro_mpps.pool.comps.PS001_C005_RotaryFeeder import *
-from mlpro_mpps.pool.comps.PS001_C007_VacuumPump2 import *
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class WeighingStation(Module):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_module(self):
-        """
-        Storing station consists of a silo, a hopper, a rotary feeder, and a vacuum pump.
-        """
-        hopper = Hopper(p_name='HopperC')
-        silo = Silo(p_name='SiloC')
-        vac = VacuumPump2(p_name='VacC')
-        belt = RotaryFeeder(p_name='BeltC')
-        
-        self._add_component(p_component=silo)
-        self._add_component(p_component=hopper)
-        self._add_component(p_component=vac)
-        self._add_component(p_component=belt)
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.mods
+## -- Module  : PS001_M004_Filling.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-30  0.0.0     SY       Creation
+## -- 2022-12-30  1.0.0     SY       Release of first version
+## -- 2023-02-01  1.0.1     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.1 (2023-02-01)
+
+This module provides a default implementation of a module of the BGLP, which is a Filling station
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro_mpps.pool.comps.PS001_C008_VacuumPump3 import *
+from mlpro_mpps.pool.comps.PS001_C009_Inventory import *
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class FillingStation(Module):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_module(self):
+        """
+        Storing station consists of a silo, a hopper, a rotary feeder, and a vacuum pump.
+        """
+        inv = FinishedGoodsInventory(p_name='Inventory')
+        vac = VacuumPump3(p_name='VacD')
+        
+        self._add_component(p_component=inv)
+        self._add_component(p_component=vac)
+
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/mpps/PS001_bglp.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/mpps/PS001_BGLP.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,309 +1,308 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.mpps
-## -- Module  : PS001_BGLP.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2022-12-30  0.0.0     SY       Creation
-## -- 2022-12-30  1.0.0     SY       Release of first version
-## -- 2023-01-11  1.0.1     SY       Debugging on setup_mpps, adjusting sensors' indices
-## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
-## -- 2023-01-18  1.0.3     SY       Adjustment due to updated transported material functions
-## -- 2023-02-01  1.0.4     SY       Refactoring
-## -- 2023-02-02  1.0.5     SY       Refactoring
-## -- 2023-02-27  1.0.6     SY       Refactoring
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.6 (2023-02-27)
-
-This module provides a default implementation of the BGLP in MLPro-MPPS.
-"""
-
-
-from mlpro_mpps.mpps import *
-from mlpro_mpps.pool.mods.PS001_M001_Loading import *
-from mlpro_mpps.pool.mods.PS001_M002_Storing import *
-from mlpro_mpps.pool.mods.PS001_M003_Weighing import *
-from mlpro_mpps.pool.mods.PS001_M004_Filling import *
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class BGLP(SimMPPS):
-
-
-## -------------------------------------------------------------------------------------------------
-    def _setup_mpps(self, p_auto_adjust_names=True):
-        
-        # 0. Add reference
-        self.C_SCIREF_TYPE    = self.C_SCIREF_TYPE_ARTICLE
-        self.C_SCIREF_AUTHOR  = "Dorothea Schwung, Steve Yuwono, Andreas Schwung, Steven X. Ding"
-        self.C_SCIREF_TITLE   = "Decentralized learning of energy optimal production policies using PLC-informed reinforcement learning"
-        self.C_SCIREF_JOURNAL = "Computers & Chemical Engineering"
-        self.C_SCIREF_YEAR    = "2021"
-        self.C_SCIREF_MONTH   = "05"
-        self.C_SCIREF_DAY     = "28"
-        self.C_SCIREF_VOLUME  = "152"
-        self.C_SCIREF_DOI     = "10.1016/j.compchemeng.2021.107382"
-        
-        # 1. Add elements
-        loading = LoadingStation(p_name='LoadingStation')
-        storing = StoringStation(p_name='StoringStation')
-        weighing = WeighingStation(p_name='WeighingStation')
-        filling = FillingStation(p_name='FillingStation')
-        
-        self._add_element(p_elem=loading)
-        self._add_element(p_elem=storing)
-        self._add_element(p_elem=weighing)
-        self._add_element(p_elem=filling)
-        
-        # 2. Check duplications of the elements names
-        while not self._elements_names_checker():
-            if p_auto_adjust_names:
-                self._elements_names_auto_adjust()
-            else:
-                raise NameError('There are duplications of the elements names. You can just simply set p_auto_adjust_names to True.')
-
-        # 3. Setup which actions connected to which actuators
-        self._actions_in_order = False
-
-        # 4. Setup input signals for updating sensors or component states values
-        _sens = self.get_sensors()
-        _acts = self.get_actuators()
-        _sts = self.get_component_states()
-        
-        # 4.1. Actuators-related states
-        self._add_signal(
-            _sts['CBTransportedMaterial'],              # p_updated_elem
-            _acts['Motor'].get_value,                   # p_input_fcts[0]
-            _acts['Motor'].get_status,                  # p_input_fcts[1]
-            _sts['SiloLoadingFillLevel'].get_value      # p_input_fcts[2]
-            )
-        
-        self._add_signal(
-            _sts['CBPowerConsumption'],
-            _acts['Motor'].get_value, 
-            _acts['Motor'].get_status
-            )
-        
-        self._add_signal(
-            _sts['VC1TransportedMaterial'],
-            _acts['Timer'].get_value, 
-            _acts['Timer'].get_status, 
-            _sts['HopperFillLevel'].get_value
-            )
-        
-        self._add_signal(
-            _sts['VC1PowerConsumption'],
-            _acts['Timer'].get_value, 
-            _acts['Timer'].get_status
-            )
-        
-        self._add_signal(
-            _sts['VCTransportedMaterial'],
-            _acts['Switch'].get_status,
-            _sts['SiloFillLevel'].get_value
-            )
-        
-        self._add_signal(
-            _sts['VCPowerConsumption'],
-            _acts['Switch'].get_status
-            )
-        
-        self._add_signal(
-            _sts['VC2TransportedMaterial'],
-            _acts['Timer_1'].get_value, 
-            _acts['Timer_1'].get_status, 
-            _sts['HopperFillLevel_1'].get_value
-            )
-        
-        self._add_signal(
-            _sts['VC2PowerConsumption'],
-            _acts['Timer_1'].get_value,
-            _acts['Timer_1'].get_status
-            )
-        
-        self._add_signal(
-            _sts['RFTransportedMaterial'],
-            _acts['Motor_1'].get_value, 
-            _acts['Motor_1'].get_status, 
-            _sts['SiloFillLevel_1'].get_value
-            )
-        
-        self._add_signal(
-            _sts['RFPowerConsumption'],
-            _acts['Motor_1'].get_value, 
-            _acts['Motor_1'].get_status
-            )
-        
-        self._add_signal(
-            _sts['VC1TransportedMaterial_1'],
-            _acts['Switch_1'].get_status,
-            _sts['HopperFillLevel_2'].get_value
-            )
-        
-        # 4.2. Buffers-related states
-        self._add_signal(
-            _sts['SiloLoadingOverflow'],
-            _sts['SiloLoadingFillLevel'].get_value, 
-            _sts['CBTransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['SiloLoadingFillLevel'],
-            _sts['SiloLoadingFillLevel'].get_value, 
-            _sts['CBTransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['HopperOverflow'], 
-            _sts['HopperFillLevel'].get_value, 
-            _sts['CBTransportedMaterial'].get_value,
-            _sts['VC1TransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['HopperFillLevel'],
-            _sts['HopperFillLevel'].get_value,
-            _sts['CBTransportedMaterial'].get_value, 
-            _sts['VC1TransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['SiloOverflow'], 
-            _sts['SiloFillLevel'].get_value, 
-            _sts['VC1TransportedMaterial'].get_value, 
-            _sts['VCTransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['SiloFillLevel'], 
-            _sts['SiloFillLevel'].get_value, 
-            _sts['VC1TransportedMaterial'].get_value, 
-            _sts['VCTransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['HopperOverflow_1'], 
-            _sts['HopperFillLevel_1'].get_value, 
-            _sts['VCTransportedMaterial'].get_value, 
-            _sts['VC2TransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['HopperFillLevel_1'], 
-            _sts['HopperFillLevel_1'].get_value, 
-            _sts['VCTransportedMaterial'].get_value, 
-            _sts['VC2TransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['SiloOverflow_1'], 
-            _sts['SiloFillLevel_1'].get_value, 
-            _sts['VC2TransportedMaterial'].get_value, 
-            _sts['RFTransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['SiloFillLevel_1'], 
-            _sts['SiloFillLevel_1'].get_value, 
-            _sts['VC2TransportedMaterial'].get_value, 
-            _sts['RFTransportedMaterial'].get_value
-            )
-        
-        self._add_signal(
-            _sts['HopperOverflow_2'], 
-            _sts['HopperFillLevel_2'].get_value, 
-            _sts['RFTransportedMaterial'].get_value, 
-            _sts['VC1TransportedMaterial_1'].get_value
-            )
-        
-        self._add_signal(
-            _sts['HopperFillLevel_2'], 
-            _sts['HopperFillLevel_2'].get_value, 
-            _sts['RFTransportedMaterial'].get_value, 
-            _sts['VC1TransportedMaterial_1'].get_value
-            )
-        
-        self._add_signal(
-            _sts['InventoryLevel'], 
-            _sts['InventoryLevel'].get_value, 
-            _sts['VC1TransportedMaterial_1'].get_value
-            )        
-                
-        # 4.3. Buffers-related sensor
-        self._add_signal(
-            _sens['SiloSensor1'],
-            _sts['SiloLoadingFillLevel'].get_value
-            )
-        
-        self._add_signal(
-            _sens['SiloSensor2'], 
-            _sts['SiloLoadingFillLevel'].get_value
-            )
-        
-        self._add_signal(
-            _sens['SiloSensor1_1'], 
-            _sts['HopperFillLevel'].get_value
-            )
-   
-        self._add_signal(
-            _sens['SiloSensor1_2'], 
-            _sts['SiloFillLevel'].get_value
-            )
-   
-        self._add_signal(
-            _sens['SiloSensor2_1'], 
-            _sts['SiloFillLevel'].get_value
-            )
-        
-        self._add_signal(
-            _sens['SiloSensor1_3'], 
-            _sts['HopperFillLevel_1'].get_value
-            )
-        
-        self._add_signal(
-            _sens['SiloSensor1_4'], 
-            _sts['SiloFillLevel_1'].get_value
-            )
-   
-        self._add_signal(
-            _sens['SiloSensor2_2'], 
-            _sts['SiloFillLevel_1'].get_value
-            )
-   
-        self._add_signal(
-            _sens['SiloSensor1_5'], 
-            _sts['HopperFillLevel_2'].get_value
-            )
-
-
-
-## -------------------------------------------------------------------------------------------------
-    def _simulate_reaction(self, p_state: State, p_action: Action) -> State:
-        
-        # 1. Set values to actuators
-        if self._actions_in_order:
-            actions = Action.get_sorted_values()
-            for idx, (_, acts) in enumerate(self.get_actuators().items()):
-                acts.set_value(actions[idx])
-        else:
-            raise NotImplementedError
-        
-        # 2. Update values of the sensors and component states
-        for sig in self._signals:
-            if len(sig[1:]) == 1:
-                input = sig[1]()
-            else:
-                input = []
-                for x in range(len(sig[1:])):
-                    input.append(sig[x+1]())
-            sig[0].simulate(input, p_range=None)
-
-        # 3. Return the resulted states in the form of State object
-        raise NotImplementedError
-    
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.mpps
+## -- Module  : PS001_BGLP.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2022-12-30  0.0.0     SY       Creation
+## -- 2022-12-30  1.0.0     SY       Release of first version
+## -- 2023-01-11  1.0.1     SY       Debugging on setup_mpps, adjusting sensors' indices
+## -- 2023-01-16  1.0.2     SY       Change order between fill-level and overflow as comp. states
+## -- 2023-01-18  1.0.3     SY       Adjustment due to updated transported material functions
+## -- 2023-02-01  1.0.4     SY       Refactoring
+## -- 2023-02-02  1.0.5     SY       Refactoring
+## -- 2023-02-27  1.0.6     SY       Refactoring
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.6 (2023-02-27)
+
+This module provides a default implementation of the BGLP in MLPro-MPPS.
+"""
+
+
+from mlpro_mpps.mpps import *
+from mlpro_mpps.pool.mods.PS001_M001_Loading import *
+from mlpro_mpps.pool.mods.PS001_M002_Storing import *
+from mlpro_mpps.pool.mods.PS001_M003_Weighing import *
+from mlpro_mpps.pool.mods.PS001_M004_Filling import *
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class BGLP(SimMPPS):
+
+
+## -------------------------------------------------------------------------------------------------
+    def _setup_mpps(self, p_auto_adjust_names=True):
+        
+        # 0. Add reference
+        self.C_SCIREF_TYPE    = self.C_SCIREF_TYPE_ARTICLE
+        self.C_SCIREF_AUTHOR  = "Dorothea Schwung, Steve Yuwono, Andreas Schwung, Steven X. Ding"
+        self.C_SCIREF_TITLE   = "Decentralized learning of energy optimal production policies using PLC-informed reinforcement learning"
+        self.C_SCIREF_JOURNAL = "Computers & Chemical Engineering"
+        self.C_SCIREF_YEAR    = "2021"
+        self.C_SCIREF_MONTH   = "05"
+        self.C_SCIREF_DAY     = "28"
+        self.C_SCIREF_VOLUME  = "152"
+        self.C_SCIREF_DOI     = "10.1016/j.compchemeng.2021.107382"
+        
+        # 1. Add elements
+        loading = LoadingStation(p_name='LoadingStation')
+        storing = StoringStation(p_name='StoringStation')
+        weighing = WeighingStation(p_name='WeighingStation')
+        filling = FillingStation(p_name='FillingStation')
+        
+        self._add_element(p_elem=loading)
+        self._add_element(p_elem=storing)
+        self._add_element(p_elem=weighing)
+        self._add_element(p_elem=filling)
+        
+        # 2. Check duplications of the elements names
+        while not self._elements_names_checker():
+            if p_auto_adjust_names:
+                self._elements_names_auto_adjust()
+            else:
+                raise NameError('There are duplications of the elements names. You can just simply set p_auto_adjust_names to True.')
+
+        # 3. Setup which actions connected to which actuators
+        self._actions_in_order = False
+
+        # 4. Setup input signals for updating sensors or component states values
+        _sens = self.get_sensors()
+        _acts = self.get_actuators()
+        _sts = self.get_component_states()
+        
+        # 4.1. Actuators-related states
+        self._add_signal(
+            _sts['CBTransportedMaterial'],              # p_updated_elem
+            _acts['Motor'].get_value,                   # p_input_fcts[0]
+            _acts['Motor'].get_status,                  # p_input_fcts[1]
+            _sts['SiloLoadingFillLevel'].get_value      # p_input_fcts[2]
+            )
+        
+        self._add_signal(
+            _sts['CBPowerConsumption'],
+            _acts['Motor'].get_value, 
+            _acts['Motor'].get_status
+            )
+        
+        self._add_signal(
+            _sts['VC1TransportedMaterial'],
+            _acts['Timer'].get_value, 
+            _acts['Timer'].get_status, 
+            _sts['HopperFillLevel'].get_value
+            )
+        
+        self._add_signal(
+            _sts['VC1PowerConsumption'],
+            _acts['Timer'].get_value, 
+            _acts['Timer'].get_status
+            )
+        
+        self._add_signal(
+            _sts['VCTransportedMaterial'],
+            _acts['Switch'].get_status,
+            _sts['SiloFillLevel'].get_value
+            )
+        
+        self._add_signal(
+            _sts['VCPowerConsumption'],
+            _acts['Switch'].get_status
+            )
+        
+        self._add_signal(
+            _sts['VC2TransportedMaterial'],
+            _acts['Timer_1'].get_value, 
+            _acts['Timer_1'].get_status, 
+            _sts['HopperFillLevel_1'].get_value
+            )
+        
+        self._add_signal(
+            _sts['VC2PowerConsumption'],
+            _acts['Timer_1'].get_value,
+            _acts['Timer_1'].get_status
+            )
+        
+        self._add_signal(
+            _sts['RFTransportedMaterial'],
+            _acts['Motor_1'].get_value, 
+            _acts['Motor_1'].get_status, 
+            _sts['SiloFillLevel_1'].get_value
+            )
+        
+        self._add_signal(
+            _sts['RFPowerConsumption'],
+            _acts['Motor_1'].get_value, 
+            _acts['Motor_1'].get_status
+            )
+        
+        self._add_signal(
+            _sts['VC1TransportedMaterial_1'],
+            _acts['Switch_1'].get_status,
+            _sts['HopperFillLevel_2'].get_value
+            )
+        
+        # 4.2. Buffers-related states
+        self._add_signal(
+            _sts['SiloLoadingOverflow'],
+            _sts['SiloLoadingFillLevel'].get_value, 
+            _sts['CBTransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['SiloLoadingFillLevel'],
+            _sts['SiloLoadingFillLevel'].get_value, 
+            _sts['CBTransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['HopperOverflow'], 
+            _sts['HopperFillLevel'].get_value, 
+            _sts['CBTransportedMaterial'].get_value,
+            _sts['VC1TransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['HopperFillLevel'],
+            _sts['HopperFillLevel'].get_value,
+            _sts['CBTransportedMaterial'].get_value, 
+            _sts['VC1TransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['SiloOverflow'], 
+            _sts['SiloFillLevel'].get_value, 
+            _sts['VC1TransportedMaterial'].get_value, 
+            _sts['VCTransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['SiloFillLevel'], 
+            _sts['SiloFillLevel'].get_value, 
+            _sts['VC1TransportedMaterial'].get_value, 
+            _sts['VCTransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['HopperOverflow_1'], 
+            _sts['HopperFillLevel_1'].get_value, 
+            _sts['VCTransportedMaterial'].get_value, 
+            _sts['VC2TransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['HopperFillLevel_1'], 
+            _sts['HopperFillLevel_1'].get_value, 
+            _sts['VCTransportedMaterial'].get_value, 
+            _sts['VC2TransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['SiloOverflow_1'], 
+            _sts['SiloFillLevel_1'].get_value, 
+            _sts['VC2TransportedMaterial'].get_value, 
+            _sts['RFTransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['SiloFillLevel_1'], 
+            _sts['SiloFillLevel_1'].get_value, 
+            _sts['VC2TransportedMaterial'].get_value, 
+            _sts['RFTransportedMaterial'].get_value
+            )
+        
+        self._add_signal(
+            _sts['HopperOverflow_2'], 
+            _sts['HopperFillLevel_2'].get_value, 
+            _sts['RFTransportedMaterial'].get_value, 
+            _sts['VC1TransportedMaterial_1'].get_value
+            )
+        
+        self._add_signal(
+            _sts['HopperFillLevel_2'], 
+            _sts['HopperFillLevel_2'].get_value, 
+            _sts['RFTransportedMaterial'].get_value, 
+            _sts['VC1TransportedMaterial_1'].get_value
+            )
+        
+        self._add_signal(
+            _sts['InventoryLevel'], 
+            _sts['InventoryLevel'].get_value, 
+            _sts['VC1TransportedMaterial_1'].get_value
+            )        
+                
+        # 4.3. Buffers-related sensor
+        self._add_signal(
+            _sens['SiloSensor1'],
+            _sts['SiloLoadingFillLevel'].get_value
+            )
+        
+        self._add_signal(
+            _sens['SiloSensor2'], 
+            _sts['SiloLoadingFillLevel'].get_value
+            )
+        
+        self._add_signal(
+            _sens['SiloSensor1_1'], 
+            _sts['HopperFillLevel'].get_value
+            )
+   
+        self._add_signal(
+            _sens['SiloSensor1_2'], 
+            _sts['SiloFillLevel'].get_value
+            )
+   
+        self._add_signal(
+            _sens['SiloSensor2_1'], 
+            _sts['SiloFillLevel'].get_value
+            )
+        
+        self._add_signal(
+            _sens['SiloSensor1_3'], 
+            _sts['HopperFillLevel_1'].get_value
+            )
+        
+        self._add_signal(
+            _sens['SiloSensor1_4'], 
+            _sts['SiloFillLevel_1'].get_value
+            )
+   
+        self._add_signal(
+            _sens['SiloSensor2_2'], 
+            _sts['SiloFillLevel_1'].get_value
+            )
+   
+        self._add_signal(
+            _sens['SiloSensor1_5'], 
+            _sts['HopperFillLevel_2'].get_value
+            )
+
+
+
+## -------------------------------------------------------------------------------------------------
+    def _simulate_reaction(self, p_state: State, p_action: Action) -> State:
+        
+        # 1. Set values to actuators
+        if self._actions_in_order:
+            actions = Action.get_sorted_values()
+            for idx, (_, acts) in enumerate(self.get_actuators().items()):
+                acts.set_value(actions[idx])
+        else:
+            raise NotImplementedError
+        
+        # 2. Update values of the sensors and component states
+        for sig in self._signals:
+            if len(sig[1:]) == 1:
+                input = sig[1]()
+            else:
+                input = []
+                for x in range(len(sig[1:])):
+                    input.append(sig[x+1]())
+            sig[0].simulate(input, p_range=None)
+
+        # 3. Return the resulted states in the form of State object
+        raise NotImplementedError
```

### Comparing `mlpro_mpps-1.0.1/src/mlpro_mpps/pool/rl_environment/RL001_bglp.py` & `mlpro_mpps-1.1.0/src/mlpro_mpps/pool/ml/rl_environment/RL001_BGLP.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,360 +1,362 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps.pool.rl_environment
-## -- Module  : RL001_BGLP.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2023-02-17  0.0.0     SY       Creation
-## -- 2023-02-17  1.0.0     SY       Release of first version
-## -------------------------------------------------------------------------------------------------
-
-"""
-Ver. 1.0.5 (2023-02-02)
-
-This module provides a default implementation of the BGLP in MLPro-MPPS as RL Environment.
-"""
-
-
-from mlpro_mpps.pool.mpps.PS001_bglp import BGLP
-from mlpro.bf.math import *
-from mlpro.rl.models import *
-
-
-                     
-
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class BGLP4RL(BGLP):
-
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self, p_name:str, p_id:int=None, p_logging=Log.C_LOG_ALL, **p_kwargs):
-        super().__init__(p_name=p_name, p_id=p_id, p_logging=p_logging, p_kwargs=p_kwargs)
-        try:
-            self.parent = p_kwargs['p_parent']
-        except:
-            raise NotImplementedError('Please input the parent class of this class as p_parent')
-            
-
-
-## -------------------------------------------------------------------------------------------------
-    def _simulate_reaction(self, p_state: State, p_action: Action) -> State:
-        
-        # 1. Set values to actuators
-        action = []
-        for agent_id in p_action.get_agent_ids():
-            action_elem = p_action.get_elem(agent_id)
-            for action_id in action_elem.get_dim_ids():
-                action.append(action_elem.get_value(action_id))
-                
-        for idx, (_, acts) in enumerate(self.get_actuators().items()):
-            if idx != len(self.get_actuators())-1:
-                boundaries = acts.get_boundaries()
-                final_action = action[idx]*(boundaries[1]-boundaries[0])+boundaries[0]
-                acts.set_value(final_action)
-            else:
-                acts.set_value(True)
-        
-        # 2. Update values of the sensors and component states
-        init_inventory_level = self.get_component_states()['InventoryLevel'].get_value()
-        for sig in self._signals:
-            if len(sig[1:]) == 1:
-                input = sig[1]()
-            else:
-                input = []
-                for x in range(len(sig[1:])):
-                    input.append(sig[x+1]())
-            sig[0].simulate(input, p_range=self.parent.t_set)
-
-        # 3. Return the resulted states in the form of State object
-        self.parent._state = self.parent.get_states()
-        self.parent._state.set_success(False)
-        self.parent._state.set_broken(False)
-        
-        self.parent.t += self.parent.t_set
-        current_volume = self.get_component_states()['InventoryLevel'].get_value()
-        overlfow = sum(self.parent.get_overflow())
-        power = sum(self.parent.get_power())
-        self.parent.current_demand = self.parent.get_demand(init_inventory_level, current_volume)
-        self.parent.prod_reached += (current_volume-init_inventory_level)
-        
-        self.parent.data_storing.memorize("time",str(self.parent.data_frame), self.parent.t)
-        self.parent.data_storing.memorize("overflow",str(self.parent.data_frame), overlfow/self.parent.t_set)
-        self.parent.data_storing.memorize("power",str(self.parent.data_frame), power/self.parent.t_set)
-        self.parent.data_storing.memorize("demand",str(self.parent.data_frame), self.parent.current_demand/self.parent.t_set)
-        
-        return self.parent._state
-
-
-                     
-                        
-## -------------------------------------------------------------------------------------------------
-## -------------------------------------------------------------------------------------------------
-class BGLP_RLEnv(Environment):
-
-    C_TYPE = 'Environment'
-    C_NAME = 'MPPS-based BGLP - RL Environment'
-    C_CYCLE_LIMIT = 0  # Recommended cycle limit for training episodes
-
-
-## -------------------------------------------------------------------------------------------------
-    def __init__(self,
-                 p_reward_type=Reward.C_TYPE_EVERY_AGENT,
-                 p_logging=Log.C_LOG_ALL,
-                 t_set=10.0,
-                 demand=0.1,
-                 lr_margin=1.0,
-                 lr_demand=4.0,
-                 lr_power=0.0010, 
-                 margin_p=[0.2,0.8,4],
-                 prod_target=10000,
-                 prod_scenario='continuous',
-                 cycle_limit=0):
-
-        self.num_envs = 5                                                 # Number of internal sub-environments
-        self.reward_type = p_reward_type
-        
-        super().__init__(p_mode = Mode.C_MODE_SIM, 
-                         p_latency = None, 
-                         p_fct_strans = BGLP4RL(p_name='BGLP_RL',
-                                                p_logging=p_logging,
-                                                p_parent=self), 
-                         p_fct_reward = None, 
-                         p_fct_success = None, 
-                         p_fct_broken = None, 
-                         p_visualize = False, 
-                         p_logging = p_logging)
-        
-        self.C_SCIREF_TYPE    = self.C_SCIREF_TYPE_ARTICLE
-        self.C_SCIREF_AUTHOR  = "Dorothea Schwung, Steve Yuwono, Andreas Schwung, Steven X. Ding"
-        self.C_SCIREF_TITLE   = "Decentralized learning of energy optimal production policies using PLC-informed reinforcement learning"
-        self.C_SCIREF_JOURNAL = "Computers & Chemical Engineering"
-        self.C_SCIREF_YEAR    = "2021"
-        self.C_SCIREF_MONTH   = "05"
-        self.C_SCIREF_DAY     = "28"
-        self.C_SCIREF_VOLUME  = "152"
-        self.C_SCIREF_DOI     = "10.1016/j.compchemeng.2021.107382"
-        
-        self.C_CYCLE_LIMIT = cycle_limit
-        self.t = 0
-        self.t_set = t_set
-        self.demand = demand
-        self.lr_margin = lr_margin
-        self.lr_demand = lr_demand
-        self.lr_power = lr_power
-        self.prod_target = prod_target
-        self.prod_scenario = prod_scenario
-        self.margin_p = margin_p
-        
-        self.data_lists = ["time","overflow","power","demand"]
-        self.data_storing = DataStoring(self.data_lists)
-        self.data_frame = None
-        
-        self.set_overflow = ['SiloLoadingOverflow',
-                             'HopperOverflow',
-                             'SiloOverflow',
-                             'HopperOverflow_1',
-                             'SiloOverflow_1',
-                             'HopperOverflow_2']
-        self.set_fill_levels = ['SiloLoadingFillLevel',
-                                'HopperFillLevel',
-                                'SiloFillLevel',
-                                'HopperFillLevel_1',
-                                'SiloFillLevel_1',
-                                'HopperFillLevel_2']
-        self.set_power = ['CBPowerConsumption',
-                          'VC1PowerConsumption',
-                          'VCPowerConsumption',
-                          'VC2PowerConsumption',
-                          'RFPowerConsumption']
-        
-        self.reset()
-
-
-## -------------------------------------------------------------------------------------------------
-    @staticmethod
-    def setup_spaces():
-        state_space = ESpace()
-        action_space = ESpace()
-
-        state_space.add_dim(Dimension('R-1 LvlSiloA', 'R', 'Res-1 Level of Silo A', '', '', '', [0, 1]))
-        state_space.add_dim(Dimension('R-2 LvlHopperA', 'R', 'Res-2 Level of Hopper A', '', '', '', [0, 1]))
-        state_space.add_dim(Dimension('R-3 LvlSiloB', 'R', 'Res-3 Level of Silo B', '', '', '', [0, 1]))
-        state_space.add_dim(Dimension('R-4 LvlHopperB', 'R', 'Res-4 Level of Hopper B', '', '', '', [0, 1]))
-        state_space.add_dim(Dimension('R-5 LvlSiloC', 'R', 'Res-5 Level of Silo C', '', '', '', [0, 1]))
-        state_space.add_dim(Dimension('R-6 LvlHopperC', 'R', 'Res-6 Level of Hopper C', '', '', '', [0, 1]))
-        
-        action_space.add_dim(Dimension('A-1 Act', 'R', 'Act-1 Belt Conveyor A', '', '', '', [0, 1]))
-        action_space.add_dim(Dimension('A-2 Act', 'R', 'Act-2 Vacuum Pump B', '', '', '', [0, 1]))
-        action_space.add_dim(Dimension('A-3 Act', 'Z', 'Act-3 Vibratory Conveyor B', '', '', '', [0, 1]))
-        action_space.add_dim(Dimension('A-4 Act', 'R', 'Act-4 Vacuum Pump C', '', '', '', [0, 1]))
-        action_space.add_dim(Dimension('A-5 Act', 'R', 'Act-5 Rotary Feeder C', '', '', '', [0, 1]))
-
-        return state_space, action_space
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_states(self) -> State:
-        state = State(self._state_space)
-        ids = state.get_dim_ids()
-        
-        for x in range(len(ids)):
-            fill_level = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_value()
-            boundaries = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_boundaries()
-            norm_fill_level = (fill_level-boundaries[0])/(boundaries[1]-boundaries[0])
-            state.set_value(ids[x], norm_fill_level) 
-        return state
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_margin(self) -> list:
-        margin = []
-        
-        for x in range(len(self.set_fill_levels)):
-            fill_level = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_value()
-            boundaries = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_boundaries()
-            norm_fill_level = (fill_level-boundaries[0])/(boundaries[1]-boundaries[0])
-            if norm_fill_level < self.margin_p[0]:
-                m = (0-self.margin_p[2])/(self.margin_p[0])*(norm_fill_level-self.margin_p[0])*self.t_set
-            elif norm_fill_level > self.margin_p[1]:
-                m = self.margin_p[2]/(1-self.margin_p[1])*(norm_fill_level-self.margin_p[1])*self.t_set
-            else:
-                m = 0.0
-            margin.append(m)
-        return margin
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_overflow(self) -> list:
-        total_overflow = []
-        
-        for x in range(len(self.set_fill_levels)):
-            overflow = self._fct_strans.get_component_states()[self.set_overflow[x]].get_value()
-            total_overflow.append(overflow)
-        return total_overflow
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_power(self) -> list:
-        total_power = []
-        
-        for x in range(len(self.set_power)):
-            power = self._fct_strans.get_component_states()[self.set_power[x]].get_value()
-            total_power.append(power)
-        return total_power
-
-
-## -------------------------------------------------------------------------------------------------
-    def get_demand(self, init_volume, cur_volume) -> list:
-        delta = cur_volume-init_volume
-        
-        if (self.demand*self.t_set) > delta:
-            total_demand = delta-self.demand*self.t_set
-        else:
-            total_demand = 0
-        return total_demand
-
-
-## -------------------------------------------------------------------------------------------------
-    def _compute_reward(self, p_state_old: State = None, p_state_new: State = None) -> Reward:
-        reward = Reward(self.reward_type)
-
-        if self.reward_type == Reward.C_TYPE_OVERALL:
-            r_overall = 0
-            r_overall = r_overall + sum(self.calc_reward())
-            reward.set_overall_reward(r_overall)
-        
-        elif self.reward_type == Reward.C_TYPE_EVERY_AGENT:
-           for agent_id in self._last_action.get_agent_ids():
-               r_reward = self.calc_reward()
-               reward.add_agent_reward(agent_id, r_reward[int(agent_id)])
-               
-        else:
-           for agent_id in self._last_action.get_agent_ids():
-                agent_action_elem = self._last_action.get_elem(agent_id)
-                agent_action_ids = agent_action_elem.get_dim_ids()
-                r_reward = self.calc_reward()
-                action_idx = 0
-                for action_id in agent_action_ids:
-                    r_action = r_reward[action_idx]
-                    action_idx += 1
-                    reward.add_action_reward(agent_id, action_id, r_action)
-                    
-        return reward
-
-
-## -------------------------------------------------------------------------------------------------
-    def _compute_success(self, p_state: State) -> bool:        
-        if self.prod_scenario == 'continuous':
-            return False
-        else:
-            if self.prod_reached >= self.prod_target:
-                self._state.set_terminal(True)
-                return True
-            else:
-                return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _compute_broken(self, p_state: State) -> bool:
-        return False
-
-
-## -------------------------------------------------------------------------------------------------
-    def _reset(self, p_seed=None) -> None:
-        random.seed(p_seed)
-        self._fct_strans.get_component_states()['VC1TransportedMaterial_1']._function.prod_target = self.demand
-        
-        for acts in self._fct_strans.get_actuators():
-            self._fct_strans.get_actuators()[acts].deactivate()
-        for sens in self._fct_strans.get_sensors():
-            self._fct_strans.get_sensors()[sens].deactivate()
-            
-        for st in range(len(self.set_fill_levels)):
-            buffer = self._fct_strans.get_component_states()[self.set_fill_levels[st]]
-            boundaries = buffer.get_boundaries()
-            levels_init = random.uniform(0,1)
-            fill_level = levels_init*(boundaries[1]-boundaries[0])+boundaries[0]
-            buffer.set_value(fill_level)
-        self._fct_strans.get_component_states()['InventoryLevel'].set_value(0)
-        
-        self.t = 0
-        self.prod_reached = 0
-        self._state = self.get_states()
-        self._state.set_success(False)
-        self._state.set_broken(False)
-        
-        if self.data_frame == None:
-            self.data_frame = 0
-        else:
-            self.data_frame += 1
-        self.data_storing.add_frame(str(self.data_frame))
-            
-
-## -------------------------------------------------------------------------------------------------
-    def calc_reward(self):
-        reward = []
-        margin = self.get_margin()
-        power = self.get_power()
-        demand = self.current_demand/self.t_set
-        
-        for actnum, pwr in enumerate(self.set_power):
-            try:
-                power_max = self._fct_strans.get_component_states()[pwr]._function.max_power
-            except:
-                power_max = self._fct_strans.get_component_states()[pwr]._function.power
-                
-            reward.append(1/(1+self.lr_margin*margin[actnum]))
-            reward[actnum] += 1/(1+self.lr_power*power[actnum]/(power_max/1000.0))
-            if actnum == len(self.set_power)-1:
-                reward[actnum] += 1/(1-self.lr_demand*demand)
-            else:
-                reward[actnum] += 1/(1+self.lr_margin*margin[actnum+1])
-        return reward
-
-
-
-
-
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps.pool.rl_environment
+## -- Module  : RL001_BGLP.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2023-02-17  0.0.0     SY       Creation
+## -- 2023-02-17  1.0.0     SY       Release of first version
+## -- 2023-03-28  1.0.1     SY       Refactoring compute_reward
+## -------------------------------------------------------------------------------------------------
+
+"""
+Ver. 1.0.1 (2023-03-28)
+
+This module provides a default implementation of the BGLP in MLPro-MPPS as RL Environment.
+"""
+
+
+from mlpro_mpps.pool.mpps.PS001_BGLP import BGLP
+from mlpro.bf.math import *
+from mlpro.rl.models import *
+
+
+                     
+
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class BGLP4RL(BGLP):
+
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self, p_name:str, p_id:int=None, p_logging=Log.C_LOG_ALL, **p_kwargs):
+        super().__init__(p_name=p_name, p_id=p_id, p_logging=p_logging, p_kwargs=p_kwargs)
+        try:
+            self.parent = p_kwargs['p_parent']
+        except:
+            raise NotImplementedError('Please input the parent class of this class as p_parent')
+            
+
+
+## -------------------------------------------------------------------------------------------------
+    def _simulate_reaction(self, p_state: State, p_action: Action) -> State:
+        
+        # 1. Set values to actuators
+        action = []
+        for agent_id in p_action.get_agent_ids():
+            action_elem = p_action.get_elem(agent_id)
+            for action_id in action_elem.get_dim_ids():
+                action.append(action_elem.get_value(action_id))
+                
+        for idx, (_, acts) in enumerate(self.get_actuators().items()):
+            if idx != len(self.get_actuators())-1:
+                boundaries = acts.get_boundaries()
+                final_action = action[idx]*(boundaries[1]-boundaries[0])+boundaries[0]
+                acts.set_value(final_action)
+            else:
+                acts.set_value(True)
+        
+        # 2. Update values of the sensors and component states
+        init_inventory_level = self.get_component_states()['InventoryLevel'].get_value()
+        for sig in self._signals:
+            if len(sig[1:]) == 1:
+                input = sig[1]()
+            else:
+                input = []
+                for x in range(len(sig[1:])):
+                    input.append(sig[x+1]())
+            sig[0].simulate(input, p_range=self.parent.t_set)
+
+        # 3. Return the resulted states in the form of State object
+        self.parent._state = self.parent.get_states()
+        self.parent._state.set_success(False)
+        self.parent._state.set_broken(False)
+        
+        self.parent.t += self.parent.t_set
+        current_volume = self.get_component_states()['InventoryLevel'].get_value()
+        overlfow = sum(self.parent.get_overflow())
+        power = sum(self.parent.get_power())
+        self.parent.current_demand = self.parent.get_demand(init_inventory_level, current_volume)
+        self.parent.prod_reached += (current_volume-init_inventory_level)
+        
+        self.parent.data_storing.memorize("time",str(self.parent.data_frame), self.parent.t)
+        self.parent.data_storing.memorize("overflow",str(self.parent.data_frame), overlfow/self.parent.t_set)
+        self.parent.data_storing.memorize("power",str(self.parent.data_frame), power/self.parent.t_set)
+        self.parent.data_storing.memorize("demand",str(self.parent.data_frame), self.parent.current_demand/self.parent.t_set)
+        
+        return self.parent._state
+
+
+                     
+                        
+## -------------------------------------------------------------------------------------------------
+## -------------------------------------------------------------------------------------------------
+class BGLP_RLEnv(Environment):
+
+    C_TYPE = 'Environment'
+    C_NAME = 'MPPS-based BGLP - RL Environment'
+    C_CYCLE_LIMIT = 0  # Recommended cycle limit for training episodes
+
+
+## -------------------------------------------------------------------------------------------------
+    def __init__(self,
+                 p_reward_type=Reward.C_TYPE_EVERY_AGENT,
+                 p_logging=Log.C_LOG_ALL,
+                 t_set=10.0,
+                 demand=0.1,
+                 lr_margin=1.0,
+                 lr_demand=4.0,
+                 lr_power=0.0010, 
+                 margin_p=[0.2,0.8,4],
+                 prod_target=10000,
+                 prod_scenario='continuous',
+                 cycle_limit=0):
+
+        self.num_envs = 5                                                 # Number of internal sub-environments
+        self.reward_type = p_reward_type
+        
+        super().__init__(p_mode = Mode.C_MODE_SIM, 
+                         p_latency = None, 
+                         p_fct_strans = BGLP4RL(p_name='BGLP_RL',
+                                                p_logging=p_logging,
+                                                p_parent=self), 
+                         p_fct_reward = None, 
+                         p_fct_success = None, 
+                         p_fct_broken = None, 
+                         p_visualize = False, 
+                         p_logging = p_logging)
+        
+        self.C_SCIREF_TYPE    = self.C_SCIREF_TYPE_ARTICLE
+        self.C_SCIREF_AUTHOR  = "Dorothea Schwung, Steve Yuwono, Andreas Schwung, Steven X. Ding"
+        self.C_SCIREF_TITLE   = "Decentralized learning of energy optimal production policies using PLC-informed reinforcement learning"
+        self.C_SCIREF_JOURNAL = "Computers & Chemical Engineering"
+        self.C_SCIREF_YEAR    = "2021"
+        self.C_SCIREF_MONTH   = "05"
+        self.C_SCIREF_DAY     = "28"
+        self.C_SCIREF_VOLUME  = "152"
+        self.C_SCIREF_DOI     = "10.1016/j.compchemeng.2021.107382"
+        
+        self.C_CYCLE_LIMIT = cycle_limit
+        self.t = 0
+        self.t_set = t_set
+        self.demand = demand
+        self.lr_margin = lr_margin
+        self.lr_demand = lr_demand
+        self.lr_power = lr_power
+        self.prod_target = prod_target
+        self.prod_scenario = prod_scenario
+        self.margin_p = margin_p
+        
+        self.data_lists = ["time","overflow","power","demand"]
+        self.data_storing = DataStoring(self.data_lists)
+        self.data_frame = None
+        
+        self.set_overflow = ['SiloLoadingOverflow',
+                             'HopperOverflow',
+                             'SiloOverflow',
+                             'HopperOverflow_1',
+                             'SiloOverflow_1',
+                             'HopperOverflow_2']
+        self.set_fill_levels = ['SiloLoadingFillLevel',
+                                'HopperFillLevel',
+                                'SiloFillLevel',
+                                'HopperFillLevel_1',
+                                'SiloFillLevel_1',
+                                'HopperFillLevel_2']
+        self.set_power = ['CBPowerConsumption',
+                          'VC1PowerConsumption',
+                          'VCPowerConsumption',
+                          'VC2PowerConsumption',
+                          'RFPowerConsumption']
+        
+        self.reset()
+
+
+## -------------------------------------------------------------------------------------------------
+    @staticmethod
+    def setup_spaces():
+        state_space = ESpace()
+        action_space = ESpace()
+
+        state_space.add_dim(Dimension('R-1 LvlSiloA', 'R', 'Res-1 Level of Silo A', '', '', '', [0, 1]))
+        state_space.add_dim(Dimension('R-2 LvlHopperA', 'R', 'Res-2 Level of Hopper A', '', '', '', [0, 1]))
+        state_space.add_dim(Dimension('R-3 LvlSiloB', 'R', 'Res-3 Level of Silo B', '', '', '', [0, 1]))
+        state_space.add_dim(Dimension('R-4 LvlHopperB', 'R', 'Res-4 Level of Hopper B', '', '', '', [0, 1]))
+        state_space.add_dim(Dimension('R-5 LvlSiloC', 'R', 'Res-5 Level of Silo C', '', '', '', [0, 1]))
+        state_space.add_dim(Dimension('R-6 LvlHopperC', 'R', 'Res-6 Level of Hopper C', '', '', '', [0, 1]))
+        
+        action_space.add_dim(Dimension('A-1 Act', 'R', 'Act-1 Belt Conveyor A', '', '', '', [0, 1]))
+        action_space.add_dim(Dimension('A-2 Act', 'R', 'Act-2 Vacuum Pump B', '', '', '', [0, 1]))
+        action_space.add_dim(Dimension('A-3 Act', 'Z', 'Act-3 Vibratory Conveyor B', '', '', '', [0, 1]))
+        action_space.add_dim(Dimension('A-4 Act', 'R', 'Act-4 Vacuum Pump C', '', '', '', [0, 1]))
+        action_space.add_dim(Dimension('A-5 Act', 'R', 'Act-5 Rotary Feeder C', '', '', '', [0, 1]))
+
+        return state_space, action_space
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_states(self) -> State:
+        state = State(self._state_space)
+        ids = state.get_dim_ids()
+        
+        for x in range(len(ids)):
+            fill_level = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_value()
+            boundaries = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_boundaries()
+            norm_fill_level = (fill_level-boundaries[0])/(boundaries[1]-boundaries[0])
+            state.set_value(ids[x], norm_fill_level) 
+        return state
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_margin(self) -> list:
+        margin = []
+        
+        for x in range(len(self.set_fill_levels)):
+            fill_level = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_value()
+            boundaries = self._fct_strans.get_component_states()[self.set_fill_levels[x]].get_boundaries()
+            norm_fill_level = (fill_level-boundaries[0])/(boundaries[1]-boundaries[0])
+            if norm_fill_level < self.margin_p[0]:
+                m = (0-self.margin_p[2])/(self.margin_p[0])*(norm_fill_level-self.margin_p[0])*self.t_set
+            elif norm_fill_level > self.margin_p[1]:
+                m = self.margin_p[2]/(1-self.margin_p[1])*(norm_fill_level-self.margin_p[1])*self.t_set
+            else:
+                m = 0.0
+            margin.append(m)
+        return margin
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_overflow(self) -> list:
+        total_overflow = []
+        
+        for x in range(len(self.set_fill_levels)):
+            overflow = self._fct_strans.get_component_states()[self.set_overflow[x]].get_value()
+            total_overflow.append(overflow)
+        return total_overflow
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_power(self) -> list:
+        total_power = []
+        
+        for x in range(len(self.set_power)):
+            power = self._fct_strans.get_component_states()[self.set_power[x]].get_value()
+            total_power.append(power)
+        return total_power
+
+
+## -------------------------------------------------------------------------------------------------
+    def get_demand(self, init_volume, cur_volume) -> list:
+        delta = cur_volume-init_volume
+        
+        if (self.demand*self.t_set) > delta:
+            total_demand = delta-self.demand*self.t_set
+        else:
+            total_demand = 0
+        return total_demand
+
+
+## -------------------------------------------------------------------------------------------------
+    def _compute_reward(self, p_state_old: State = None, p_state_new: State = None) -> Reward:
+        reward = Reward(self.reward_type)
+
+        if self.reward_type == Reward.C_TYPE_OVERALL:
+            r_overall = 0
+            r_overall = r_overall + sum(self.calc_reward())
+            reward.set_overall_reward(r_overall)
+        
+        elif self.reward_type == Reward.C_TYPE_EVERY_AGENT:
+           for agent_id in self._last_action.get_agent_ids():
+               r_reward = self.calc_reward()
+               idx = self._last_action.get_agent_ids().index(agent_id)
+               reward.add_agent_reward(agent_id, r_reward[idx])
+               
+        else:
+           for agent_id in self._last_action.get_agent_ids():
+                agent_action_elem = self._last_action.get_elem(agent_id)
+                agent_action_ids = agent_action_elem.get_dim_ids()
+                r_reward = self.calc_reward()
+                action_idx = 0
+                for action_id in agent_action_ids:
+                    r_action = r_reward[action_idx]
+                    action_idx += 1
+                    reward.add_action_reward(agent_id, action_id, r_action)
+                    
+        return reward
+
+
+## -------------------------------------------------------------------------------------------------
+    def _compute_success(self, p_state: State) -> bool:        
+        if self.prod_scenario == 'continuous':
+            return False
+        else:
+            if self.prod_reached >= self.prod_target:
+                self._state.set_terminal(True)
+                return True
+            else:
+                return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _compute_broken(self, p_state: State) -> bool:
+        return False
+
+
+## -------------------------------------------------------------------------------------------------
+    def _reset(self, p_seed=None) -> None:
+        random.seed(p_seed)
+        self._fct_strans.get_component_states()['VC1TransportedMaterial_1']._function.prod_target = self.demand
+        
+        for acts in self._fct_strans.get_actuators():
+            self._fct_strans.get_actuators()[acts].deactivate()
+        for sens in self._fct_strans.get_sensors():
+            self._fct_strans.get_sensors()[sens].deactivate()
+            
+        for st in range(len(self.set_fill_levels)):
+            buffer = self._fct_strans.get_component_states()[self.set_fill_levels[st]]
+            boundaries = buffer.get_boundaries()
+            levels_init = random.uniform(0,1)
+            fill_level = levels_init*(boundaries[1]-boundaries[0])+boundaries[0]
+            buffer.set_value(fill_level)
+        self._fct_strans.get_component_states()['InventoryLevel'].set_value(0)
+        
+        self.t = 0
+        self.prod_reached = 0
+        self._state = self.get_states()
+        self._state.set_success(False)
+        self._state.set_broken(False)
+        
+        if self.data_frame == None:
+            self.data_frame = 0
+        else:
+            self.data_frame += 1
+        self.data_storing.add_frame(str(self.data_frame))
+            
+
+## -------------------------------------------------------------------------------------------------
+    def calc_reward(self):
+        reward = []
+        margin = self.get_margin()
+        power = self.get_power()
+        demand = self.current_demand/self.t_set
+        
+        for actnum, pwr in enumerate(self.set_power):
+            try:
+                power_max = self._fct_strans.get_component_states()[pwr]._function.max_power
+            except:
+                power_max = self._fct_strans.get_component_states()[pwr]._function.power
+                
+            reward.append(1/(1+self.lr_margin*margin[actnum]))
+            reward[actnum] += 1/(1+self.lr_power*power[actnum]/(power_max/1000.0))
+            if actnum == len(self.set_power)-1:
+                reward[actnum] += 1/(1-self.lr_demand*demand)
+            else:
+                reward[actnum] += 1/(1+self.lr_margin*margin[actnum+1])
+        return reward
+
+
+
+
+
```

### Comparing `mlpro_mpps-1.0.1/test/test_examples.py` & `mlpro_mpps-1.1.0/test/test_examples.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro_mpps
-## -- Module  : test_example.py
-## -------------------------------------------------------------------------------------------------
-## -- History :
-## -- yyyy-mm-dd  Ver.      Auth.    Description
-## -- 2023-02-27  0.0.0     SY/MRD   Creation
-## -- 2023-02-27  1.0.0     SY/MRD   Release First Version
-## -------------------------------------------------------------------------------------------------
-
-
-"""
-Ver. 1.0.0 (2023-02-27)
-
-Unit test for all examples available.
-"""
-
-
-import pytest
-import importlib
-
-
-howto_list = {
-
-# Basic Functions:
-
-    "ht_001": "mlpro_mpps.examples.howto_001_set_up_components_and_modules_in_MPPS",
-    "ht_002": "mlpro_mpps.examples.howto_002_set_up_MPPS",
-    "ht_003": "mlpro_mpps.examples.howto_003_run_RL_on_BGLP_using_MPPS",
-    "ht_004": "mlpro_mpps.examples.howto_004_run_GT_on_BGLP_using_MPPS",
-}
-
-
-@pytest.mark.parametrize("cls", list(howto_list.keys()))
-def test_howto(cls):
-    importlib.import_module(howto_list[cls])
+## -------------------------------------------------------------------------------------------------
+## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
+## -- Package : mlpro_mpps
+## -- Module  : test_example.py
+## -------------------------------------------------------------------------------------------------
+## -- History :
+## -- yyyy-mm-dd  Ver.      Auth.    Description
+## -- 2023-02-27  0.0.0     SY/MRD   Creation
+## -- 2023-02-27  1.0.0     SY/MRD   Release First Version
+## -- 2023-03-28  1.0.1     SY/MRD   Replacing importlib with runpy, add howtos
+## -------------------------------------------------------------------------------------------------
+
+
+"""
+Ver. 1.0.1 (2023-03-28)
+
+Unit test for all examples available.
+"""
+
+
+import pytest
+import runpy
+
+
+howto_list = {
+
+# Basic Functions:
+
+    "ht_001": "mlpro_mpps.examples.howto_001_set_up_components_and_modules_in_MPPS",
+    "ht_002": "mlpro_mpps.examples.howto_002_set_up_MPPS",
+    "ht_003": "mlpro_mpps.examples.howto_003_run_RL_on_BGLP_using_MPPS",
+    "ht_004": "mlpro_mpps.examples.howto_004_run_GT_on_BGLP_using_MPPS",
+    "ht_005": "mlpro_mpps.examples.howto_005_run_RL_on_LS_using_MPPS",
+    "ht_006": "mlpro_mpps.examples.howto_006_run_EA_on_LS_using_MPPS",
+    "ht_007": "mlpro_mpps.examples.howto_007_run_using_LS_MPPS_data_generation",
+}
+
+
+
+@pytest.mark.parametrize("cls", list(howto_list.keys()))
+def test_howto(cls):
+    runpy.run_path("src/"+howto_list[cls].replace(".","/")+".py")
```

