# Comparing `tmp/OpenDSSDirect.py-0.8.1.tar.gz` & `tmp/OpenDSSDirect.py-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenDSSDirect.py-0.8.1.tar", last modified: Sun Apr  2 04:46:41 2023, max compression
+gzip compressed data, was "OpenDSSDirect.py-0.8.2.tar", last modified: Thu Apr 13 12:26:03 2023, max compression
```

## Comparing `OpenDSSDirect.py-0.8.1.tar` & `OpenDSSDirect.py-0.8.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/
--rw-r--r--   0 meira     (1000) users      (100)     2442 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/LICENSE
--rw-r--r--   0 meira     (1000) users      (100)      197 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/MANIFEST.in
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.784689 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/
--rw-r--r--   0 meira     (1000) users      (100)     4375 2023-04-02 04:46:41.000000 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/PKG-INFO
--rw-r--r--   0 meira     (1000) users      (100)     2006 2023-04-02 04:46:41.000000 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/SOURCES.txt
--rw-r--r--   0 meira     (1000) users      (100)        1 2023-04-02 04:46:41.000000 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/dependency_links.txt
--rw-r--r--   0 meira     (1000) users      (100)        1 2023-04-02 04:46:37.000000 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/not-zip-safe
--rw-r--r--   0 meira     (1000) users      (100)      124 2023-04-02 04:46:41.000000 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/requires.txt
--rw-r--r--   0 meira     (1000) users      (100)       14 2023-04-02 04:46:41.000000 OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/top_level.txt
--rw-r--r--   0 meira     (1000) users      (100)     4375 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/PKG-INFO
--rw-r--r--   0 meira     (1000) users      (100)     3035 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/README.md
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.788689 OpenDSSDirect.py-0.8.1/docs/
--rw-r--r--   0 meira     (1000) users      (100)      909 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/docs/Makefile
--rw-r--r--   0 meira     (1000) users      (100)     5331 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/docs/conf.py
--rw-r--r--   0 meira     (1000) users      (100)      534 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/docs/index.rst
--rw-r--r--   0 meira     (1000) users      (100)      819 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/docs/make.bat
--rw-r--r--   0 meira     (1000) users      (100)     6968 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/docs/opendssdirect.rst
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/opendssdirect/
--rw-r--r--   0 meira     (1000) users      (100)     2417 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/ActiveClass.py
--rw-r--r--   0 meira     (1000) users      (100)     6913 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Basic.py
--rw-r--r--   0 meira     (1000) users      (100)     6752 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Bus.py
--rw-r--r--   0 meira     (1000) users      (100)     5352 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/CNData.py
--rw-r--r--   0 meira     (1000) users      (100)     5846 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/CapControls.py
--rw-r--r--   0 meira     (1000) users      (100)     3527 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Capacitors.py
--rw-r--r--   0 meira     (1000) users      (100)     8072 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Circuit.py
--rw-r--r--   0 meira     (1000) users      (100)    11293 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/CktElement.py
--rw-r--r--   0 meira     (1000) users      (100)     1595 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/CmathLib.py
--rw-r--r--   0 meira     (1000) users      (100)     2173 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/CtrlQueue.py
--rw-r--r--   0 meira     (1000) users      (100)       88 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/DSSCore.py
--rw-r--r--   0 meira     (1000) users      (100)       28 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/DSSEvents.py
--rw-r--r--   0 meira     (1000) users      (100)      323 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/DSSimComs.py
--rw-r--r--   0 meira     (1000) users      (100)     1053 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Element.py
--rw-r--r--   0 meira     (1000) users      (100)     1855 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Error.py
--rw-r--r--   0 meira     (1000) users      (100)     1209 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Executive.py
--rw-r--r--   0 meira     (1000) users      (100)     4306 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Fuses.py
--rw-r--r--   0 meira     (1000) users      (100)     7672 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Generators.py
--rw-r--r--   0 meira     (1000) users      (100)     2082 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Isource.py
--rw-r--r--   0 meira     (1000) users      (100)     5241 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/LineCodes.py
--rw-r--r--   0 meira     (1000) users      (100)     5039 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/LineGeometries.py
--rw-r--r--   0 meira     (1000) users      (100)     2870 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/LineSpacings.py
--rw-r--r--   0 meira     (1000) users      (100)     9279 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Lines.py
--rw-r--r--   0 meira     (1000) users      (100)     4751 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/LoadShape.py
--rw-r--r--   0 meira     (1000) users      (100)    12260 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Loads.py
--rw-r--r--   0 meira     (1000) users      (100)     9461 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Meters.py
--rw-r--r--   0 meira     (1000) users      (100)     5656 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Monitors.py
--rw-r--r--   0 meira     (1000) users      (100)     8426 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/PDElements.py
--rw-r--r--   0 meira     (1000) users      (100)     7270 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/PVsystems.py
--rw-r--r--   0 meira     (1000) users      (100)     2290 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Parallel.py
--rw-r--r--   0 meira     (1000) users      (100)     4475 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Parser.py
--rw-r--r--   0 meira     (1000) users      (100)      601 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Progress.py
--rw-r--r--   0 meira     (1000) users      (100)     1616 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Properties.py
--rw-r--r--   0 meira     (1000) users      (100)     9553 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Reactors.py
--rw-r--r--   0 meira     (1000) users      (100)     4925 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Reclosers.py
--rw-r--r--   0 meira     (1000) users      (100)     2936 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/ReduceCkt.py
--rw-r--r--   0 meira     (1000) users      (100)     8295 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/RegControls.py
--rw-r--r--   0 meira     (1000) users      (100)     2713 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Relays.py
--rw-r--r--   0 meira     (1000) users      (100)     5351 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Sensors.py
--rw-r--r--   0 meira     (1000) users      (100)     7573 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Settings.py
--rw-r--r--   0 meira     (1000) users      (100)    13553 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Solution.py
--rw-r--r--   0 meira     (1000) users      (100)     2271 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Storages.py
--rw-r--r--   0 meira     (1000) users      (100)     3823 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/SwtControls.py
--rw-r--r--   0 meira     (1000) users      (100)     5175 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/TSData.py
--rw-r--r--   0 meira     (1000) users      (100)      569 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Text.py
--rw-r--r--   0 meira     (1000) users      (100)     3816 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Topology.py
--rw-r--r--   0 meira     (1000) users      (100)     8186 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Transformers.py
--rw-r--r--   0 meira     (1000) users      (100)     2555 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/Vsources.py
--rw-r--r--   0 meira     (1000) users      (100)     3665 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/WireData.py
--rw-r--r--   0 meira     (1000) users      (100)     4036 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/XYCurves.py
--rw-r--r--   0 meira     (1000) users      (100)     3087 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/YMatrix.py
--rw-r--r--   0 meira     (1000) users      (100)     2570 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/ZIP.py
--rw-r--r--   0 meira     (1000) users      (100)      883 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/__init__.py
--rw-r--r--   0 meira     (1000) users      (100)      938 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/_utils.py
--rw-r--r--   0 meira     (1000) users      (100)       46 2023-04-02 04:46:23.000000 OpenDSSDirect.py-0.8.1/opendssdirect/_version.py
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/opendssdirect/dss/
--rw-r--r--   0 meira     (1000) users      (100)     1388 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/dss/__init__.py
--rw-r--r--   0 meira     (1000) users      (100)     8286 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/opendssdirect/utils.py
--rw-r--r--   0 meira     (1000) users      (100)       38 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/setup.cfg
--rw-r--r--   0 meira     (1000) users      (100)     2658 2023-04-02 04:46:23.000000 OpenDSSDirect.py-0.8.1/setup.py
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/tests/
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.784689 OpenDSSDirect.py-0.8.1/tests/data/
-drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-02 04:46:41.792689 OpenDSSDirect.py-0.8.1/tests/data/13Bus/
--rw-r--r--   0 meira     (1000) users      (100)      243 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/tests/data/13Bus/IEEE13Node_BusXY.csv
--rw-r--r--   0 meira     (1000) users      (100)     8205 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/tests/data/13Bus/IEEE13Nodeckt.dss
--rw-r--r--   0 meira     (1000) users      (100)    11851 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/tests/data/13Bus/IEEELineCodes.dss
--rw-r--r--   0 meira     (1000) users      (100)      455 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/tests/test_evaluate_expression.py
--rw-r--r--   0 meira     (1000) users      (100)   175831 2023-04-02 04:46:13.000000 OpenDSSDirect.py-0.8.1/tests/test_opendssdirect.py
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/
+-rw-r--r--   0 meira     (1000) users      (100)     2442 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/LICENSE
+-rw-r--r--   0 meira     (1000) users      (100)      197 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/MANIFEST.in
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.593876 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/
+-rw-r--r--   0 meira     (1000) users      (100)     4022 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/PKG-INFO
+-rw-r--r--   0 meira     (1000) users      (100)     2006 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/SOURCES.txt
+-rw-r--r--   0 meira     (1000) users      (100)        1 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/dependency_links.txt
+-rw-r--r--   0 meira     (1000) users      (100)        1 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/not-zip-safe
+-rw-r--r--   0 meira     (1000) users      (100)      124 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/requires.txt
+-rw-r--r--   0 meira     (1000) users      (100)       14 2023-04-13 12:26:03.000000 OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/top_level.txt
+-rw-r--r--   0 meira     (1000) users      (100)     4022 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/PKG-INFO
+-rw-r--r--   0 meira     (1000) users      (100)     3035 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/README.md
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.593876 OpenDSSDirect.py-0.8.2/docs/
+-rw-r--r--   0 meira     (1000) users      (100)      909 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/Makefile
+-rw-r--r--   0 meira     (1000) users      (100)     5331 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/conf.py
+-rw-r--r--   0 meira     (1000) users      (100)      534 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/index.rst
+-rw-r--r--   0 meira     (1000) users      (100)      819 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/make.bat
+-rw-r--r--   0 meira     (1000) users      (100)     6968 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/docs/opendssdirect.rst
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/opendssdirect/
+-rw-r--r--   0 meira     (1000) users      (100)     2417 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/ActiveClass.py
+-rw-r--r--   0 meira     (1000) users      (100)     6913 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Basic.py
+-rw-r--r--   0 meira     (1000) users      (100)     6752 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Bus.py
+-rw-r--r--   0 meira     (1000) users      (100)     5352 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CNData.py
+-rw-r--r--   0 meira     (1000) users      (100)     5846 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CapControls.py
+-rw-r--r--   0 meira     (1000) users      (100)     3527 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Capacitors.py
+-rw-r--r--   0 meira     (1000) users      (100)     8072 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Circuit.py
+-rw-r--r--   0 meira     (1000) users      (100)    11293 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CktElement.py
+-rw-r--r--   0 meira     (1000) users      (100)     1595 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CmathLib.py
+-rw-r--r--   0 meira     (1000) users      (100)     2173 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/CtrlQueue.py
+-rw-r--r--   0 meira     (1000) users      (100)       88 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/DSSCore.py
+-rw-r--r--   0 meira     (1000) users      (100)       28 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/DSSEvents.py
+-rw-r--r--   0 meira     (1000) users      (100)      323 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/DSSimComs.py
+-rw-r--r--   0 meira     (1000) users      (100)     1053 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Element.py
+-rw-r--r--   0 meira     (1000) users      (100)     1855 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Error.py
+-rw-r--r--   0 meira     (1000) users      (100)     1209 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Executive.py
+-rw-r--r--   0 meira     (1000) users      (100)     4306 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Fuses.py
+-rw-r--r--   0 meira     (1000) users      (100)     7672 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Generators.py
+-rw-r--r--   0 meira     (1000) users      (100)     2082 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Isource.py
+-rw-r--r--   0 meira     (1000) users      (100)     5241 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LineCodes.py
+-rw-r--r--   0 meira     (1000) users      (100)     5039 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LineGeometries.py
+-rw-r--r--   0 meira     (1000) users      (100)     2870 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LineSpacings.py
+-rw-r--r--   0 meira     (1000) users      (100)     9279 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Lines.py
+-rw-r--r--   0 meira     (1000) users      (100)     4751 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/LoadShape.py
+-rw-r--r--   0 meira     (1000) users      (100)    12260 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Loads.py
+-rw-r--r--   0 meira     (1000) users      (100)     9461 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Meters.py
+-rw-r--r--   0 meira     (1000) users      (100)     5656 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Monitors.py
+-rw-r--r--   0 meira     (1000) users      (100)     8426 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/PDElements.py
+-rw-r--r--   0 meira     (1000) users      (100)     7270 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/PVsystems.py
+-rw-r--r--   0 meira     (1000) users      (100)     2290 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Parallel.py
+-rw-r--r--   0 meira     (1000) users      (100)     4475 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Parser.py
+-rw-r--r--   0 meira     (1000) users      (100)      601 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Progress.py
+-rw-r--r--   0 meira     (1000) users      (100)     1616 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Properties.py
+-rw-r--r--   0 meira     (1000) users      (100)     9553 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Reactors.py
+-rw-r--r--   0 meira     (1000) users      (100)     4925 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Reclosers.py
+-rw-r--r--   0 meira     (1000) users      (100)     2936 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/ReduceCkt.py
+-rw-r--r--   0 meira     (1000) users      (100)     8295 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/RegControls.py
+-rw-r--r--   0 meira     (1000) users      (100)     2713 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Relays.py
+-rw-r--r--   0 meira     (1000) users      (100)     5351 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Sensors.py
+-rw-r--r--   0 meira     (1000) users      (100)     7573 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Settings.py
+-rw-r--r--   0 meira     (1000) users      (100)    13553 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Solution.py
+-rw-r--r--   0 meira     (1000) users      (100)     2271 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Storages.py
+-rw-r--r--   0 meira     (1000) users      (100)     3823 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/SwtControls.py
+-rw-r--r--   0 meira     (1000) users      (100)     5175 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/TSData.py
+-rw-r--r--   0 meira     (1000) users      (100)      569 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Text.py
+-rw-r--r--   0 meira     (1000) users      (100)     3816 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Topology.py
+-rw-r--r--   0 meira     (1000) users      (100)     8186 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Transformers.py
+-rw-r--r--   0 meira     (1000) users      (100)     2555 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/Vsources.py
+-rw-r--r--   0 meira     (1000) users      (100)     3665 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/WireData.py
+-rw-r--r--   0 meira     (1000) users      (100)     4036 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/XYCurves.py
+-rw-r--r--   0 meira     (1000) users      (100)     3087 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/YMatrix.py
+-rw-r--r--   0 meira     (1000) users      (100)     2570 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/ZIP.py
+-rw-r--r--   0 meira     (1000) users      (100)      883 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/__init__.py
+-rw-r--r--   0 meira     (1000) users      (100)      938 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/_utils.py
+-rw-r--r--   0 meira     (1000) users      (100)       46 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/_version.py
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/opendssdirect/dss/
+-rw-r--r--   0 meira     (1000) users      (100)     1388 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/dss/__init__.py
+-rw-r--r--   0 meira     (1000) users      (100)     8286 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/opendssdirect/utils.py
+-rw-r--r--   0 meira     (1000) users      (100)       38 2023-04-13 12:26:03.605877 OpenDSSDirect.py-0.8.2/setup.cfg
+-rw-r--r--   0 meira     (1000) users      (100)     2658 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/setup.py
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/tests/
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.593876 OpenDSSDirect.py-0.8.2/tests/data/
+drwxr-xr-x   0 meira     (1000) users      (100)        0 2023-04-13 12:26:03.601876 OpenDSSDirect.py-0.8.2/tests/data/13Bus/
+-rw-r--r--   0 meira     (1000) users      (100)      243 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEE13Node_BusXY.csv
+-rw-r--r--   0 meira     (1000) users      (100)     8205 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEE13Nodeckt.dss
+-rw-r--r--   0 meira     (1000) users      (100)    11851 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEELineCodes.dss
+-rw-r--r--   0 meira     (1000) users      (100)      455 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/test_evaluate_expression.py
+-rw-r--r--   0 meira     (1000) users      (100)   175831 2023-04-13 12:25:45.000000 OpenDSSDirect.py-0.8.2/tests/test_opendssdirect.py
```

### Comparing `OpenDSSDirect.py-0.8.1/LICENSE` & `OpenDSSDirect.py-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/PKG-INFO` & `OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: OpenDSSDirect.py
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python direct-mode interface to OpenDSS
 Home-page: https://github.com/dss-extensions/OpenDSSDirect.py
+Download-URL: https://github.com/dss-extensions/OpenDSSDirect.py
 Author: Dheepak Krishnamurthy
 Author-email: me@kdheepak.com
 License: BSD-compatible
-Download-URL: https://github.com/dss-extensions/OpenDSSDirect.py
-Description: # OpenDSSDirect.py
-        [![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/github/dss-extensions/OpenDSSDirect.py?branch=master&svg=true)](https://ci.appveyor.com/project/PMeira/opendssdirect-py)
-        [![codecov](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py/branch/master/graph/badge.svg)](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py)
-        [![PyPI](https://img.shields.io/pypi/v/OpenDSSDirect.py.svg)](https://pypi.python.org/pypi/OpenDSSDirect.py/)
-        [![Documentation](https://img.shields.io/badge/docs-ready-blue.svg)](http://dss-extensions.org/OpenDSSDirect.py)
-        
-        OpenDSSDirect.py is a cross-platform Python package implements a "direct" library interface [our customized implementation](https://github.com/dss-extensions/dss_capi) of [OpenDSS](http://smartgrid.epri.com/SimulationTool.aspx) using [DSS-Python](https://github.com/dss-extensions/dss_python/).
-        OpenDSS is an open-source distribution system simulator. See [OpenDSSDirect.jl](https://github.com/dss-extensions/OpenDSSDirect.jl) for a similar package in Julia, and for more context about this project and its components (including alternatives in MATLAB, C++ and C#/.NET), please check [https://dss-extensions.org/](https://dss-extensions.org/) and our hub repository at [dss-extensions/dss-extensions](https://github.com/dss-extensions/dss-extensions) for more documentation, discussions and the [FAQ](https://github.com/dss-extensions/dss-extensions#faq).
-        
-        *As a reminder, although very compatible, this project is not supported by EPRI.*
-        
-        **This package is available for Windows, Mac and Linux, including ARM and x86 variants.**
-        
-        ### Documentation
-        
-        The documentation for this package can be found [here](http://dss-extensions.org/OpenDSSDirect.py).
-        
-        ### Installation
-        
-        **Recommended**: Install Python using Miniconda or Anaconda
-        
-        Open a command line interface and type the following.
-        
-        ```bash
-        pip install 'OpenDSSDirect.py[extras]'
-        ```
-        
-        See [installation](https://dss-extensions.org/OpenDSSDirect.py/notebooks/Installation.html) instructions for more information.
-        
-        ### Troubleshooting
-        
-        It is recommended to use `conda` to install pandas, which is currently a dependency of this package.
-        This package interfaces with OpenDSS using the "direct" library interface, so a good understanding of OpenDSS will help troubleshooting.
-        There are plenty of useful resources located [here](https://sourceforge.net/p/electricdss/code/HEAD/tree/trunk/Doc/).
-        
-        If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
-        
-        ### Thanks
-        
-        Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
-        
-        See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
-        [DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
-        
 Keywords: OpenDSS,cffi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: dev
+License-File: LICENSE
+
+# OpenDSSDirect.py
+[![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/github/dss-extensions/OpenDSSDirect.py?branch=master&svg=true)](https://ci.appveyor.com/project/PMeira/opendssdirect-py)
+[![codecov](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py/branch/master/graph/badge.svg)](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py)
+[![PyPI](https://img.shields.io/pypi/v/OpenDSSDirect.py.svg)](https://pypi.python.org/pypi/OpenDSSDirect.py/)
+[![Documentation](https://img.shields.io/badge/docs-ready-blue.svg)](http://dss-extensions.org/OpenDSSDirect.py)
+
+OpenDSSDirect.py is a cross-platform Python package implements a "direct" library interface [our customized implementation](https://github.com/dss-extensions/dss_capi) of [OpenDSS](http://smartgrid.epri.com/SimulationTool.aspx) using [DSS-Python](https://github.com/dss-extensions/dss_python/).
+OpenDSS is an open-source distribution system simulator. See [OpenDSSDirect.jl](https://github.com/dss-extensions/OpenDSSDirect.jl) for a similar package in Julia, and for more context about this project and its components (including alternatives in MATLAB, C++ and C#/.NET), please check [https://dss-extensions.org/](https://dss-extensions.org/) and our hub repository at [dss-extensions/dss-extensions](https://github.com/dss-extensions/dss-extensions) for more documentation, discussions and the [FAQ](https://github.com/dss-extensions/dss-extensions#faq).
+
+*As a reminder, although very compatible, this project is not supported by EPRI.*
+
+**This package is available for Windows, Mac and Linux, including ARM and x86 variants.**
+
+### Documentation
+
+The documentation for this package can be found [here](http://dss-extensions.org/OpenDSSDirect.py).
+
+### Installation
+
+**Recommended**: Install Python using Miniconda or Anaconda
+
+Open a command line interface and type the following.
+
+```bash
+pip install 'OpenDSSDirect.py[extras]'
+```
+
+See [installation](https://dss-extensions.org/OpenDSSDirect.py/notebooks/Installation.html) instructions for more information.
+
+### Troubleshooting
+
+It is recommended to use `conda` to install pandas, which is currently a dependency of this package.
+This package interfaces with OpenDSS using the "direct" library interface, so a good understanding of OpenDSS will help troubleshooting.
+There are plenty of useful resources located [here](https://sourceforge.net/p/electricdss/code/HEAD/tree/trunk/Doc/).
+
+If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
+
+### Thanks
+
+Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
+
+See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
+[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
```

### Comparing `OpenDSSDirect.py-0.8.1/OpenDSSDirect.py.egg-info/SOURCES.txt` & `OpenDSSDirect.py-0.8.2/OpenDSSDirect.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/PKG-INFO` & `OpenDSSDirect.py-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: OpenDSSDirect.py
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python direct-mode interface to OpenDSS
 Home-page: https://github.com/dss-extensions/OpenDSSDirect.py
+Download-URL: https://github.com/dss-extensions/OpenDSSDirect.py
 Author: Dheepak Krishnamurthy
 Author-email: me@kdheepak.com
 License: BSD-compatible
-Download-URL: https://github.com/dss-extensions/OpenDSSDirect.py
-Description: # OpenDSSDirect.py
-        [![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/github/dss-extensions/OpenDSSDirect.py?branch=master&svg=true)](https://ci.appveyor.com/project/PMeira/opendssdirect-py)
-        [![codecov](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py/branch/master/graph/badge.svg)](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py)
-        [![PyPI](https://img.shields.io/pypi/v/OpenDSSDirect.py.svg)](https://pypi.python.org/pypi/OpenDSSDirect.py/)
-        [![Documentation](https://img.shields.io/badge/docs-ready-blue.svg)](http://dss-extensions.org/OpenDSSDirect.py)
-        
-        OpenDSSDirect.py is a cross-platform Python package implements a "direct" library interface [our customized implementation](https://github.com/dss-extensions/dss_capi) of [OpenDSS](http://smartgrid.epri.com/SimulationTool.aspx) using [DSS-Python](https://github.com/dss-extensions/dss_python/).
-        OpenDSS is an open-source distribution system simulator. See [OpenDSSDirect.jl](https://github.com/dss-extensions/OpenDSSDirect.jl) for a similar package in Julia, and for more context about this project and its components (including alternatives in MATLAB, C++ and C#/.NET), please check [https://dss-extensions.org/](https://dss-extensions.org/) and our hub repository at [dss-extensions/dss-extensions](https://github.com/dss-extensions/dss-extensions) for more documentation, discussions and the [FAQ](https://github.com/dss-extensions/dss-extensions#faq).
-        
-        *As a reminder, although very compatible, this project is not supported by EPRI.*
-        
-        **This package is available for Windows, Mac and Linux, including ARM and x86 variants.**
-        
-        ### Documentation
-        
-        The documentation for this package can be found [here](http://dss-extensions.org/OpenDSSDirect.py).
-        
-        ### Installation
-        
-        **Recommended**: Install Python using Miniconda or Anaconda
-        
-        Open a command line interface and type the following.
-        
-        ```bash
-        pip install 'OpenDSSDirect.py[extras]'
-        ```
-        
-        See [installation](https://dss-extensions.org/OpenDSSDirect.py/notebooks/Installation.html) instructions for more information.
-        
-        ### Troubleshooting
-        
-        It is recommended to use `conda` to install pandas, which is currently a dependency of this package.
-        This package interfaces with OpenDSS using the "direct" library interface, so a good understanding of OpenDSS will help troubleshooting.
-        There are plenty of useful resources located [here](https://sourceforge.net/p/electricdss/code/HEAD/tree/trunk/Doc/).
-        
-        If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
-        
-        ### Thanks
-        
-        Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
-        
-        See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
-        [DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
-        
 Keywords: OpenDSS,cffi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: dev
+License-File: LICENSE
+
+# OpenDSSDirect.py
+[![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/github/dss-extensions/OpenDSSDirect.py?branch=master&svg=true)](https://ci.appveyor.com/project/PMeira/opendssdirect-py)
+[![codecov](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py/branch/master/graph/badge.svg)](https://codecov.io/gh/dss-extensions/OpenDSSDirect.py)
+[![PyPI](https://img.shields.io/pypi/v/OpenDSSDirect.py.svg)](https://pypi.python.org/pypi/OpenDSSDirect.py/)
+[![Documentation](https://img.shields.io/badge/docs-ready-blue.svg)](http://dss-extensions.org/OpenDSSDirect.py)
+
+OpenDSSDirect.py is a cross-platform Python package implements a "direct" library interface [our customized implementation](https://github.com/dss-extensions/dss_capi) of [OpenDSS](http://smartgrid.epri.com/SimulationTool.aspx) using [DSS-Python](https://github.com/dss-extensions/dss_python/).
+OpenDSS is an open-source distribution system simulator. See [OpenDSSDirect.jl](https://github.com/dss-extensions/OpenDSSDirect.jl) for a similar package in Julia, and for more context about this project and its components (including alternatives in MATLAB, C++ and C#/.NET), please check [https://dss-extensions.org/](https://dss-extensions.org/) and our hub repository at [dss-extensions/dss-extensions](https://github.com/dss-extensions/dss-extensions) for more documentation, discussions and the [FAQ](https://github.com/dss-extensions/dss-extensions#faq).
+
+*As a reminder, although very compatible, this project is not supported by EPRI.*
+
+**This package is available for Windows, Mac and Linux, including ARM and x86 variants.**
+
+### Documentation
+
+The documentation for this package can be found [here](http://dss-extensions.org/OpenDSSDirect.py).
+
+### Installation
+
+**Recommended**: Install Python using Miniconda or Anaconda
+
+Open a command line interface and type the following.
+
+```bash
+pip install 'OpenDSSDirect.py[extras]'
+```
+
+See [installation](https://dss-extensions.org/OpenDSSDirect.py/notebooks/Installation.html) instructions for more information.
+
+### Troubleshooting
+
+It is recommended to use `conda` to install pandas, which is currently a dependency of this package.
+This package interfaces with OpenDSS using the "direct" library interface, so a good understanding of OpenDSS will help troubleshooting.
+There are plenty of useful resources located [here](https://sourceforge.net/p/electricdss/code/HEAD/tree/trunk/Doc/).
+
+If you are having issues using this Python interface, feel free to open an Issue on GitHub [here](https://github.com/dss-extensions/OpenDSSDirect.py/issues/new).
+
+### Thanks
+
+Thanks to @tshort, Davis, @temcdrm, @GordStephen, @Muxelmann and @PMeira for their contributions, as well as all the users for their valuable feedback.
+
+See also our repositories for [DSS-Python](https://github.com/dss-extensions/dss_python) for the underlying Python package used in this package, and 
+[DSS C-API](https://github.com/dss-extensions/dss_capi) for the modified and extended OpenDSS codebase used in DSS Extensions.
```

### Comparing `OpenDSSDirect.py-0.8.1/README.md` & `OpenDSSDirect.py-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/docs/Makefile` & `OpenDSSDirect.py-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/docs/conf.py` & `OpenDSSDirect.py-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/docs/index.rst` & `OpenDSSDirect.py-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/docs/make.bat` & `OpenDSSDirect.py-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/docs/opendssdirect.rst` & `OpenDSSDirect.py-0.8.2/docs/opendssdirect.rst`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/ActiveClass.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/ActiveClass.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Basic.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Basic.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Bus.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Bus.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/CNData.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/CNData.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/CapControls.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/CapControls.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Capacitors.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Capacitors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Circuit.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Circuit.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/CktElement.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/CktElement.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/CmathLib.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/CmathLib.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/CtrlQueue.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/CtrlQueue.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Element.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Element.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Error.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Error.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Executive.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Executive.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Fuses.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Fuses.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Generators.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Generators.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Isource.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Isource.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/LineCodes.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/LineCodes.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/LineGeometries.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/LineGeometries.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/LineSpacings.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/LineSpacings.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Lines.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Lines.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/LoadShape.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/LoadShape.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Loads.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Loads.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Meters.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Meters.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Monitors.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Monitors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/PDElements.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/PDElements.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/PVsystems.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/PVsystems.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Parallel.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Parallel.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Parser.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Parser.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Progress.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Progress.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Properties.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Properties.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Reactors.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Reactors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Reclosers.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Reclosers.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/ReduceCkt.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/ReduceCkt.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/RegControls.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/RegControls.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Relays.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Relays.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Sensors.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Sensors.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Settings.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Settings.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Solution.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Solution.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Storages.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Storages.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/SwtControls.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/SwtControls.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/TSData.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/TSData.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Text.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Text.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Topology.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Topology.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Transformers.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Transformers.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/Vsources.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/Vsources.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/WireData.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/WireData.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/XYCurves.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/XYCurves.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/YMatrix.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/YMatrix.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/ZIP.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/ZIP.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/__init__.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/_utils.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/_utils.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/dss/__init__.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/dss/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/opendssdirect/utils.py` & `OpenDSSDirect.py-0.8.2/opendssdirect/utils.py`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/setup.py` & `OpenDSSDirect.py-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     url="https://github.com/dss-extensions/OpenDSSDirect.py",
     download_url="https://github.com/dss-extensions/OpenDSSDirect.py",
     # Author details
     author="Dheepak Krishnamurthy",
     author_email="me@kdheepak.com",
     license="BSD-compatible",
     packages=find_packages(),
-    install_requires=["dss_python==0.13.1"],
+    install_requires=["dss_python==0.14.*"],
     extras_require={
         "extras": ["pandas", "matplotlib", "networkx"],
         "dev": [
             "pytest",
             "pytest-cov",
             "sphinx-rtd-theme",
             "nbsphinx",
```

### Comparing `OpenDSSDirect.py-0.8.1/tests/data/13Bus/IEEE13Nodeckt.dss` & `OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEE13Nodeckt.dss`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/tests/data/13Bus/IEEELineCodes.dss` & `OpenDSSDirect.py-0.8.2/tests/data/13Bus/IEEELineCodes.dss`

 * *Files identical despite different names*

### Comparing `OpenDSSDirect.py-0.8.1/tests/test_opendssdirect.py` & `OpenDSSDirect.py-0.8.2/tests/test_opendssdirect.py`

 * *Files identical despite different names*

