# Comparing `tmp/dask-geomodeling-2.3.9.tar.gz` & `tmp/dask-geomodeling-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-geomodeling-2.3.9.tar", last modified: Mon Mar  7 12:08:05 2022, max compression
+gzip compressed data, was "dask-geomodeling-2.4.0.tar", last modified: Thu Apr 13 13:02:34 2023, max compression
```

## Comparing `dask-geomodeling-2.3.9.tar` & `dask-geomodeling-2.4.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    17987 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/CHANGES.rst
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1503 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/LICENSE
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       59 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/MANIFEST.in
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    25642 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/PKG-INFO
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1392 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/README.rst
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/dask_geomodeling/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      228 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/__init__.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      318 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/config.py
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/dask_geomodeling/core/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       30 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/core/__init__.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    11015 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/core/graphs.py
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/dask_geomodeling/geometry/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      337 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/__init__.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    18646 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/aggregate.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    10953 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/base.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     5056 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/constructive.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    24495 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/field_operations.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1492 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/geom_operations.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     5351 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/merge.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     3458 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/parallelize.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     4978 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/set_operations.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    10587 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/sinks.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     9148 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/sources.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     4138 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/geometry/text.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     4987 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/ipyleaflet_plugin.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     4796 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/measurements.py
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/dask_geomodeling/raster/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      291 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/__init__.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     4952 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/base.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    17119 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/combine.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    25151 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/elemwise.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    26150 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/misc.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     4450 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/parallelize.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     8276 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/reduction.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    17844 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/sources.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    26849 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/spatial.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    32375 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/raster/temporal.py
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    30671 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling/utils.py
-drwxrwxr-x   0 arjan     (1000) arjan     (1000)        0 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/
--rw-rw-r--   0 arjan     (1000) arjan     (1000)    25642 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/PKG-INFO
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1384 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/SOURCES.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)        1 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/dependency_links.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       20 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/entry_points.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)        1 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/not-zip-safe
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      112 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/requires.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)       17 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/dask_geomodeling.egg-info/top_level.txt
--rw-rw-r--   0 arjan     (1000) arjan     (1000)      324 2022-03-07 12:08:05.696123 dask-geomodeling-2.3.9/setup.cfg
--rw-rw-r--   0 arjan     (1000) arjan     (1000)     1670 2022-03-07 12:08:05.000000 dask-geomodeling-2.3.9/setup.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    18932 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/CHANGES.rst
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1503 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/LICENSE
+-rw-rw-r--   0 casper    (1000) casper    (1000)       59 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/MANIFEST.in
+-rw-rw-r--   0 casper    (1000) casper    (1000)    20802 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1240 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/README.rst
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      228 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)      318 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/config.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling/core/
+-rw-rw-r--   0 casper    (1000) casper    (1000)       30 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/core/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    11147 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/core/graphs.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling/geometry/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      337 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    22769 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/aggregate.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10953 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/constructive.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    24495 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/field_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1492 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/geom_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     5351 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/merge.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     3458 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4978 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/set_operations.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    10587 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/sinks.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     9096 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4138 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/geometry/text.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4987 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/ipyleaflet_plugin.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4796 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/measurements.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/dask_geomodeling/raster/
+-rw-rw-r--   0 casper    (1000) casper    (1000)      291 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/__init__.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4952 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/base.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    16996 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/combine.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    25032 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/elemwise.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26079 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/misc.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     4450 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/parallelize.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)     8124 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/reduction.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    17971 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/sources.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    26435 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/spatial.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    32375 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/raster/temporal.py
+-rw-rw-r--   0 casper    (1000) casper    (1000)    31545 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/dask_geomodeling/utils.py
+drwxrwxr-x   0 casper    (1000) casper    (1000)        0 2023-04-13 13:02:34.247781 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/
+-rw-rw-r--   0 casper    (1000) casper    (1000)    20802 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/PKG-INFO
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1341 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)        1 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/not-zip-safe
+-rw-rw-r--   0 casper    (1000) casper    (1000)      112 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/requires.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)       17 2023-04-13 13:02:34.000000 dask-geomodeling-2.4.0/dask_geomodeling.egg-info/top_level.txt
+-rw-rw-r--   0 casper    (1000) casper    (1000)      324 2023-04-13 13:02:34.251781 dask-geomodeling-2.4.0/setup.cfg
+-rw-rw-r--   0 casper    (1000) casper    (1000)     1670 2023-04-13 13:02:33.000000 dask-geomodeling-2.4.0/setup.py
```

### Comparing `dask-geomodeling-2.3.9/CHANGES.rst` & `dask-geomodeling-2.4.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,50 @@
 Changelog of dask-geomodeling
 ===================================================
 
+2.4.0 (2023-04-13)
+------------------
+
+- Change Block.get_data; instead of always computing in the main thread, use
+  the scheduler that is setup via dask.config.
+
+
+2.3.13 (2023-04-04)
+-------------------
+
+- Expand AggregateRaster for usage on points (and other geometries that are
+  smaller than a cell).
+
+
+2.3.12 (2022-11-28)
+-------------------
+
+- Perform more geometry transformations via pyproj (see 2.3.11 notes).
+
+- The .geometry property of elementwise, reduction and combine RasterBlocks is
+  now computed through the extents of the arguments (and will always be a box). 
+
+
+2.3.11 (2022-11-22)
+-------------------
+
+- Perform geometry transformations via pyproj instead of GDAL SWIG bindings to circumvent
+  a performance degradation in GDAL >=3 (PROJ >=6).
+
+- Drop support for Python 3.6 and GDAL 2.
+
+
+2.3.10 (2022-08-22)
+-------------------
+
+- Fixed compatibility with GDAL 3.4.
+
+- Fixed compatibility with shapely 2 (PyGEOS merge).
+
+
 2.3.9 (2022-03-07)
 ------------------
 
 - TemporalAggregate now correctly incorporates time resolution in retrieval of timekeys.
 
 
 2.3.8 (2022-02-18)
```

### Comparing `dask-geomodeling-2.3.9/LICENSE` & `dask-geomodeling-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/README.rst` & `dask-geomodeling-2.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 
 .. image:: https://readthedocs.org/projects/dask-geomodeling/badge/?version=latest
      :target: https://dask-geomodeling.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://github.com/nens/dask-geomodeling/actions/workflows/test.yml/badge.svg
     :target: https://github.com/nens/dask-geomodeling/actions/workflows/test.yml
 
-.. image:: https://ci.appveyor.com/api/projects/status/aopxohgl23llkeq8?svg=true
-    :target: https://ci.appveyor.com/project/reinout/dask-geomodeling
-
 .. image:: https://badge.fury.io/py/dask-geomodeling.svg
     :target: https://badge.fury.io/py/dask-geomodeling
 
 .. image:: https://anaconda.org/conda-forge/dask-geomodeling/badges/version.svg
     :target: https://anaconda.org/conda-forge/dask-geomodeling
 
 Dask-geomodeling is a collection of classes that are to be stacked together to
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/core/graphs.py` & `dask-geomodeling-2.4.0/dask_geomodeling/core/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module containing the core graphs.
 """
 import inspect
 import sys
 import json
 import logging
 
-from dask.base import tokenize, normalize_token
+from dask.base import get_scheduler, tokenize, normalize_token
 from dask.local import get_sync
 
 from shapely.geometry.base import BaseGeometry
 from datetime import datetime
 from datetime import timedelta
 
 logger = logging.getLogger(__name__)
@@ -36,17 +36,21 @@
         int(token, 16)
     except ValueError:
         return None
     return token.lower()
 
 
 def compute(graph, name, *args, **kwargs):
-    """Compute a graph ({name: [func, arg1, arg2, ...]}) using dask.get_sync
+    """Compute a graph ({name: [func, arg1, arg2, ...]}) using the configured
+    scheduler. See dask.config.
     """
-    return get_sync(graph, [name])[0]
+    dask_get = get_scheduler()
+    if dask_get is None:
+        dask_get = get_sync
+    return dask_get(graph, [name])[0]
 
 
 def construct(graph, name, validate=True):
     """Construct a Block with dependent Blocks from a graph and endpoint name.
     """
     return construct_multiple(graph, [name], validate)[0]
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/aggregate.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/aggregate.py`

 * *Files 20% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     integer level.  Level 0 corresponds to the unit cell. Each doubling of the
     cellsize level increase corresponds to a doubling of the cellsize of the
     previous level.
     """
     x1, y1, x2, y2 = bbox
     level = -ceil(log(max(x2 - x1, y2 - y1), 2))
 
-    width = 0.5 ** level
-    height = 0.5 ** level
+    width = 0.5**level
+    height = 0.5**level
 
     j1 = floor(x1 / width)
     j2 = floor(x2 / width)
     i1 = floor(y1 / height)
     i2 = floor(y2 / height)
 
     return level, {(i1, j1), (i1, j2), (i2, j1), (i2, j2)}
@@ -106,21 +106,172 @@
         bucket.add(index=index, cells=cells)
 
     return [
         bucket.indices for bucket_list in bucket_dict.values() for bucket in bucket_list
     ]
 
 
+def aggregate_polygons(
+    geometries,
+    values,
+    no_data_value,
+    agg_bbox,
+    agg_srs,
+    threshold_values,
+    statistic,
+    percentile,
+):
+    """Compute aggregates for given geometries.
+
+    Geometries are rasterized using gdal_rasterize (without the ALL_TOUCHED option).
+    
+    Args:
+      geometries (GeoSeries): The geometries to aggregate the raster in.
+      values (ndarray): A three-dimensional raster ``(t, y, x)`` to aggregate.
+      no_data_value (number): The value in ``values`` that denotes missing data.
+      agg_bbox (tuple of 4 numbers): The bbox of ``values``.
+      agg_srs (str): The projection of ``values``.
+      threshold_values (ndarray, optional): A threshold value per geometry.
+      statistic (str): A key in ``AggregateRaster.STATISTICS``.
+      percentile (float, optional): Required if ``statistic == "percentile"``
+
+    Returns:
+      - ndarray of dtype float32 and with shape ``(t, len(geometries))``
+      - list of geometry indexes that didn't cover any cell
+    """
+    # Select the aggregation function
+    agg_func = AggregateRaster.STATISTICS[statistic]["func"]
+    if statistic == "percentile":
+        agg_func = partial(agg_func, qval=percentile)
+
+    # Append NaN to the threshold values for later usage
+    if threshold_values is not None:
+        threshold_values = np.concatenate(
+            [threshold_values, np.array([np.nan], dtype=threshold_values.dtype)]
+        )
+    depth, height, width = values.shape
+    geometries_no_cells = set()
+
+    agg = np.full((depth, len(geometries)), np.nan, dtype="f4")
+    for select in bucketize(geometries.bounds.values):
+        rasterize_result = utils.rasterize_geoseries(
+            geometries.iloc[select],
+            agg_bbox,
+            agg_srs,
+            height,
+            width,
+            values=np.asarray(select, dtype=np.int32),  # GDAL needs int32
+        )
+        labels = rasterize_result["values"][0]
+        unique_labels = set(np.unique(labels[labels != rasterize_result["no_data_value"]]).tolist())
+        geometries_no_cells |= (set(select) - unique_labels)
+        if not unique_labels:
+            continue
+
+        # if there is a threshold, generate a raster with thresholds
+        if threshold_values is not None:
+            # mode="clip" ensures that unlabeled cells use the appended NaN
+            thresholds = np.take(threshold_values, labels, mode="clip")
+        else:
+            thresholds = None
+
+        for frame_no, frame in enumerate(values):
+            # limit statistics to active pixels
+            active = frame != no_data_value
+            # if there is a threshold, mask the frame
+            if threshold_values is not None:
+                valid = ~np.isnan(thresholds)  # to suppress warnings
+                active[~valid] = False  # no threshold -> no aggregation
+                active[valid] &= frame[valid] >= thresholds[valid]
+
+            # if there is no single active value: do not aggregate
+            if not active.any():
+                continue
+
+            # select features that actually have data
+            # (min, max, median, and percentile cannot handle it otherwise)
+            active_labels = labels[active]
+            select_and_active = list(set(np.unique(active_labels)) & set(select))
+
+            if not select_and_active:
+                continue
+
+            agg[frame_no][select_and_active] = agg_func(
+                1 if statistic == "count" else frame[active],
+                labels=active_labels,
+                index=select_and_active,
+            )
+    return agg, list(geometries_no_cells)
+
+
+def aggregate_points(
+    points,
+    values,
+    no_data_value,
+    agg_bbox,
+    threshold_values,
+    statistic,
+):
+    """Compute aggregates for given point geometries.
+
+    The values of the raster is taken at the point coordinates.
+    
+    Args:
+      points (GeoSeries): The geometries (points) to aggregate the raster in.
+      values (ndarray): A three-dimensional raster ``(t, y, x)`` to aggregate.
+      no_data_value (number): The value in ``values`` that denotes missing data.
+      agg_bbox (tuple of 4 numbers): The bbox of ``values``.
+      threshold_values (ndarray): A threshold value per geometry.
+      statistic (str): A key in ``AggregateRaster.STATISTICS``.
+
+    Returns:
+      ndarray of dtype float32 and with shape ``(t, len(n_geometries))``
+    """
+    # Transform the points to indices
+    _, height, width = values.shape
+    gt = utils.GeoTransform.from_bbox(agg_bbox, height, width)
+    i_y, i_x = gt.get_indices(np.array([points.x.values, points.y.values]).T)
+    point_values = values[:, np.clip(i_y, 0, height - 1), np.clip(i_x, 0, width - 1)]
+
+    # if there is a threshold, mask the point values
+    active = point_values != no_data_value
+    if threshold_values is not None:
+        threshold_values = threshold_values[np.newaxis, :]  # broadcast over t
+        valid = ~np.isnan(threshold_values)  # to suppress warnings
+        active[~valid] = False  # no threshold -> no aggregation
+        active[valid] &= point_values[valid] >= threshold_values[valid]
+
+    # Convert nodata to NaN
+    agg = point_values.astype("f4")
+    agg[~active] = np.nan
+
+    # For all statistics the aggregated value equals the pixel value
+    # (if there is only one pixel), with the exception of "count":
+    if statistic == "count":
+        agg[active] = 1.0
+
+    return agg
+
+
 class AggregateRaster(GeometryBlock):
     """
     Compute statistics of a raster for each geometry in a geometry source.
 
-    A statistic is computed in a specific projection and with a specified cell
-    size. If ``projection`` or ``pixel_size`` are not given, these default to
-    the native projection of the provided raster source.
+    A statistic is computed in a specific projection and with a specified raster 
+    cell size. If ``projection`` or ``pixel_size`` are not given, these default to
+    the native projection of the provided raster source. The following cells are
+    selected to perform the statistic (e.g. mean) on:
+
+    - Polygons: all raster cells whose center is inside the polygon
+    - Points: the raster cell (singular) that contains the point
+    - Linestrings: Bresenham's line algorithm is used
+
+    If this assignment leads to the situation that a geometry covers no raster
+    cells (for instance with a polygon much smaller than the raster cell size),
+    the geometry is reduced to a point by taking its centroid.    
 
     Should the combination of the requested pixel_size and the extent of the
     source geometry cause the required raster size to exceed ``max_pixels``,
     the ``pixel_size`` can be adjusted automatically if ``auto_pixel_size`` is
     set to ``True``, else (the default) a RuntimeError is raised.
 
     Please note that for any field operation on the result of this block
@@ -180,16 +331,15 @@
     ):
         if not isinstance(source, GeometryBlock):
             raise TypeError("'{}' object is not allowed".format(type(source)))
         if not isinstance(raster, RasterBlock):
             raise TypeError("'{}' object is not allowed".format(type(raster)))
         if not isinstance(statistic, str):
             raise TypeError("'{}' object is not allowed".format(type(statistic)))
-        statistic = statistic.lower()
-        percentile = utils.parse_percentile_statistic(statistic)
+        statistic, percentile = utils.parse_percentile_statistic(statistic.lower())
         if percentile:
             statistic = "p{0}".format(percentile)
         elif statistic not in self.STATISTICS or statistic == "percentile":
             raise ValueError("Unknown statistic '{}'".format(statistic))
 
         if projection is None:
             projection = raster.projection
@@ -277,18 +427,18 @@
             return [
                 (None, None),
                 (None, None),
                 ({"empty": True, "projection": req_srs}, None),
             ]
 
         # transform the extent into the projection in which we aggregate
-        x1, y1, x2, y2 = utils.transform_extent(extent, req_srs, agg_srs)
+        x1, y1, x2, y2 = utils.Extent(extent, req_srs).transformed(agg_srs).bbox
 
         # estimate the amount of required pixels
-        required_pixels = int(((x2 - x1) * (y2 - y1)) / (self.pixel_size ** 2))
+        required_pixels = int(((x2 - x1) * (y2 - y1)) / (self.pixel_size**2))
 
         # in case this request is too large, we adapt pixel size
         max_pixels = self.max_pixels
         if max_pixels is None:
             max_pixels = config.get("geomodeling.raster-limit")
         pixel_size = self.pixel_size
 
@@ -315,15 +465,15 @@
             "mode": "vals",
             "projection": agg_srs,
             "start": request.get("start"),
             "stop": request.get("stop"),
             "aggregation": None,  # TODO
             "bbox": (x1, y1, x2, y2),
             "width": width,
-            "height": height
+            "height": height,
         }
 
         # only propagate if provided
         if "time_resolution" in request:
             raster_request["time_resolution"] = request["time_resolution"]
 
         process_kwargs = {
@@ -363,107 +513,71 @@
         req_srs = process_kwargs["req_srs"]
         agg_srs = process_kwargs["agg_srs"]
 
         agg_geometries = utils.geoseries_transform(
             features["geometry"], req_srs, agg_srs
         )
 
-        statistic = process_kwargs["statistic"]
-        percentile = utils.parse_percentile_statistic(statistic)
-        if percentile:
-            statistic = "percentile"
-            agg_func = partial(
-                AggregateRaster.STATISTICS[statistic]["func"], qval=percentile
-            )
-        else:
-            agg_func = AggregateRaster.STATISTICS[statistic]["func"]
-
+        statistic, percentile = utils.parse_percentile_statistic(process_kwargs["statistic"])
         extensive = AggregateRaster.STATISTICS[statistic]["extensive"]
         result_column = process_kwargs["result_column"]
 
         # this is only there for the AggregateRasterAboveThreshold
         threshold_name = process_kwargs.get("threshold_name")
         if threshold_name:
-            # get the threshold, appending NaN for unlabeled pixels
-            threshold_values = np.empty((len(features) + 1,), dtype="f4")
-            threshold_values[:-1] = features[threshold_name].values
-            threshold_values[-1] = np.nan
+            threshold_values = features[threshold_name].values.astype("f4")
         else:
             threshold_values = None
 
         # investigate the raster data
+        agg_bbox = process_kwargs["agg_bbox"]
         if raster_data is None:
             values = no_data_value = None
         else:
             values = raster_data["values"]
             no_data_value = raster_data["no_data_value"]
         if values is None or np.all(values == no_data_value):  # skip the rest
             result[result_column] = 0 if extensive else np.nan
             return {"features": result, "projection": req_srs}
-        depth, height, width = values.shape
 
         pixel_size = process_kwargs["pixel_size"]
         actual_pixel_size = process_kwargs["actual_pixel_size"]
 
-        # process in groups of disjoint subsets of the features
-        agg = np.full((depth, len(features)), np.nan, dtype="f4")
-        for select in bucketize(features.bounds.values):
-            rasterize_result = utils.rasterize_geoseries(
-                agg_geometries.iloc[select],
-                process_kwargs["agg_bbox"],
-                agg_srs,
-                height,
-                width,
-                values=np.asarray(select, dtype=np.int32),  # GDAL needs int32
-            )
-            labels = rasterize_result["values"][0]
+        agg, geometries_no_cells = aggregate_polygons(
+            agg_geometries,
+            values,
+            no_data_value,
+            agg_bbox,
+            agg_srs,
+            threshold_values,
+            statistic,
+            percentile,
+        )
 
-            # if there is a threshold, generate a raster with thresholds
-            if threshold_name:
-                # mode="clip" ensures that unlabeled cells use the appended NaN
-                thresholds = np.take(threshold_values, labels, mode="clip")
-            else:
-                thresholds = None
-
-            for frame_no, frame in enumerate(values):
-                # limit statistics to active pixels
-                active = frame != no_data_value
-                # if there is a threshold, mask the frame
-                if threshold_name:
-                    valid = ~np.isnan(thresholds)  # to suppress warnings
-                    active[~valid] = False  # no threshold -> no aggregation
-                    active[valid] &= frame[valid] >= thresholds[valid]
-
-                # if there is no single active value: do not aggregate
-                if not active.any():
-                    continue
-
-                # select features that actually have data
-                # (min, max, median, and percentile cannot handle it otherwise)
-                active_labels = labels[active]
-                select_and_active = list(set(np.unique(active_labels)) & set(select))
-
-                if not select_and_active:
-                    continue
-
-                agg[frame_no][select_and_active] = agg_func(
-                    1 if statistic == "count" else frame[active],
-                    labels=active_labels,
-                    index=select_and_active,
-                )
+        if geometries_no_cells:
+            # For points and polygons that don't touch a cell center,
+            # use the centroid.
+            agg[:, geometries_no_cells] = aggregate_points(
+                agg_geometries.iloc[geometries_no_cells].centroid,
+                values,
+                no_data_value,
+                agg_bbox,
+                None if threshold_values is None else threshold_values[geometries_no_cells],
+                statistic,
+            )
 
         if extensive:  # sum and count
             agg[~np.isfinite(agg)] = 0
             # extensive aggregations have to be scaled
             if actual_pixel_size != pixel_size:
                 agg *= (actual_pixel_size / pixel_size) ** 2
         else:
             agg[~np.isfinite(agg)] = np.nan  # replaces inf by nan
 
-        if depth == 1:
+        if values.shape[0] == 1:
             result[result_column] = agg[0]
         else:
             # store an array in a dataframe cell: set each cell with [np.array]
             result[result_column] = [[x] for x in agg.T]
 
         return {"features": result, "projection": req_srs}
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/base.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/constructive.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/constructive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module containing geometry block constructive operations
 """
 import numbers
 
-from dask_geomodeling.utils import Extent, shapely_transform, transform_extent
+from dask_geomodeling.utils import Extent, shapely_transform
 
 from .base import BaseSingle
 
 __all__ = ["Buffer", "Simplify"]
 
 
 class Buffer(BaseSingle):
@@ -79,18 +79,16 @@
             return {"features": features, "projection": req_srs}
         elif "extent" in data:
             if not data["extent"]:
                 return data
             req_srs = data["projection"]
             buf_srs = kwargs["buf_srs"]
             distance = kwargs["distance"]
-            extent = transform_extent(data["extent"], req_srs, buf_srs)
-            extent = Extent(extent, buf_srs).buffered(distance).bbox
-            extent = transform_extent(extent, buf_srs, req_srs)
-            return {"extent": extent, "projection": req_srs}
+            extent = Extent(data["extent"], req_srs).transformed(buf_srs).buffered(distance).transformed(req_srs)
+            return {"extent": extent.bbox, "projection": req_srs}
         else:
             raise NotImplementedError("Dunno this mode!")
 
 
 class Simplify(BaseSingle):
     """
     Simplify geometries, mainly to make them computationally more efficient.
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/field_operations.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/field_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/geom_operations.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/geom_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/merge.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/merge.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/parallelize.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/set_operations.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/set_operations.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/sinks.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/sinks.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/sources.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 import geopandas as gpd
 import warnings
 
 from dask import config
 from dask_geomodeling import utils
 from .base import GeometryBlock
 
-from shapely.errors import WKTReadingError
-from shapely.wkt import loads as load_wkt
-
 
 # this import is a copy from geopandas.io.files
 
 __all__ = ["GeometryFileSource", "GeometryWKTSource"]
 
 
 class GeometryFileSource(GeometryBlock):
@@ -171,16 +168,16 @@
 
     def __init__(self, wkt, projection):
         if not isinstance(wkt, str):
             raise TypeError("'{}' object is not allowed".format(type(wkt)))
         if not isinstance(projection, str):
             raise TypeError("'{}' object is not allowed".format(type(projection)))
         try:
-            load_wkt(wkt)
-        except WKTReadingError:
+            utils.shapely_from_wkt(wkt)
+        except utils.WKTReadingError:
             raise ValueError("The provided geometry is not a valid WKT")
         try:
             utils.get_sr(projection)
         except TypeError:
             raise ValueError("The provided projection is not a valid WKT")
         super().__init__(wkt, projection)
 
@@ -204,15 +201,15 @@
     def process(data, request):
 
         mode = request["mode"]
         if mode not in ("extent", "intersects", "centroid"):
             raise ValueError("Unknown mode '{}'".format(mode))
 
         # load the geometry and transform it into the requested projection
-        geometry = load_wkt(data["wkt"])
+        geometry = utils.shapely_from_wkt(data["wkt"])
         if data["projection"] != request["projection"]:
             geometry = utils.shapely_transform(
                 geometry, data["projection"], request["projection"]
             )
 
         f = gpd.GeoDataFrame(
             geometry=[geometry], crs=utils.get_crs(request["projection"])
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/geometry/text.py` & `dask-geomodeling-2.4.0/dask_geomodeling/geometry/text.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/ipyleaflet_plugin.py` & `dask-geomodeling-2.4.0/dask_geomodeling/ipyleaflet_plugin.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/measurements.py` & `dask-geomodeling-2.4.0/dask_geomodeling/measurements.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/base.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/base.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/combine.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module containing raster blocks that combine rasters.
 """
 import itertools
 from datetime import timedelta as Timedelta
 import numpy as np
 
 from dask_geomodeling.utils import filter_none, get_dtype_max, get_index
-from dask_geomodeling.utils import GeoTransform
+from dask_geomodeling.utils import GeoTransform, Extent
 
 from .base import RasterBlock
 
 __all__ = ["Group"]
 
 
 class BaseCombine(RasterBlock):
@@ -103,22 +103,18 @@
     def geometry(self):
         """Combined geometry in the projection of the first store geometry. """
         geometries = filter_none([x.geometry for x in self.args])
         if len(geometries) == 0:
             return
         elif len(geometries) == 1:
             return geometries[0]
-        result = geometries[0]
-        sr = result.GetSpatialReference()
+        extent = Extent.from_geometry(geometries[0])
         for geometry in geometries[1:]:
-            if not geometry.GetSpatialReference().IsSame(sr):
-                geometry = geometry.Clone()
-                geometry.TransformTo(sr)
-            result = result.Union(geometry)
-        return result
+            extent = extent.union(Extent.from_geometry(geometry))
+        return extent.as_geometry()
 
     @property
     def projection(self):
         """Projection of the data if they match, else None"""
         projection = self.args[0].projection
         if projection is None:
             return
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/elemwise.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/elemwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module containing elementwise raster blocks.
 """
 from functools import wraps
 
 import numpy as np
 
-from dask_geomodeling.utils import get_dtype_max, get_index, GeoTransform
+from dask_geomodeling.utils import get_dtype_max, get_index, GeoTransform, Extent
 
 from .base import RasterBlock, BaseSingle
 
 __all__ = [
     "Add",
     "Subtract",
     "Multiply",
@@ -152,24 +152,20 @@
         """Intersection of geometries in the projection of the first store
         geometry. """
         geometries = [x.geometry for x in self._sources]
         if any(x is None for x in geometries):
             return
         if len(geometries) == 1:
             return geometries[0]
-        result = geometries[0]
-        sr = result.GetSpatialReference()
+        extent = Extent.from_geometry(geometries[0])
         for geometry in geometries[1:]:
-            if not geometry.GetSpatialReference().IsSame(sr):
-                geometry = geometry.Clone()
-                geometry.TransformTo(sr)
-            result = result.Intersection(geometry)
-        if result.GetArea() == 0.0:
-            return
-        return result
+            extent = extent.intersection(Extent.from_geometry(geometry))
+            if extent is None:
+                return None
+        return extent.as_geometry()
 
     @property
     def projection(self):
         """Projection of the data if they match, else None"""
         projection = self._sources[0].projection
         if projection is None:
             return
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/misc.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
 from osgeo import ogr
 import numpy as np
 from geopandas import GeoSeries
 
 from shapely.geometry import box
 from shapely.geometry import Point
-from shapely.errors import WKTReadingError
-from shapely.wkt import loads as load_wkt
 
 from dask import config
 from dask_geomodeling.geometry import GeometryBlock
 from dask_geomodeling import utils
 
 from .base import RasterBlock, BaseSingle
 
@@ -124,22 +122,18 @@
 
     @property
     def geometry(self):
         """Intersection of geometries of 'store' and 'source'. """
         result, mask = [x.geometry for x in self.args]
         if result is None or mask is None:
             return
-        sr = result.GetSpatialReference()
-        if not mask.GetSpatialReference().IsSame(sr):
-            mask = mask.Clone()
-            mask.TransformTo(sr)
-        result = result.Intersection(mask)
-        if result.GetArea() == 0.0:
-            return
-        return result
+        extent = utils.Extent.from_geometry(result).intersection(utils.Extent.from_geometry(mask))
+        if extent is None:
+            return None
+        return extent.as_geometry()
 
     @property
     def period(self):
         """ Return period datetime tuple. """
         periods = [x.period for x in self.args]
         if any(period is None for period in periods):
             return None  # None precedes
@@ -678,15 +672,16 @@
             height=height,
             width=width,
         )
 
         values = result["values"]
 
         # cast to the expected dtype if necessary
-        cast_values = values.astype(process_kwargs["dtype"])
+        with np.errstate(over="ignore", under="ignore"):
+            cast_values = values.astype(process_kwargs["dtype"])
 
         # replace the nodata value if necessary
         if result["no_data_value"] != no_data_value:
             cast_values[values == result["no_data_value"]] = no_data_value
 
         return {"values": cast_values, "no_data_value": no_data_value}
 
@@ -704,16 +699,16 @@
 
     def __init__(self, wkt, projection):
         if not isinstance(wkt, str):
             raise TypeError("'{}' object is not allowed".format(type(wkt)))
         if not isinstance(projection, str):
             raise TypeError("'{}' object is not allowed".format(type(projection)))
         try:
-            load_wkt(wkt)
-        except WKTReadingError:
+            utils.shapely_from_wkt(wkt)
+        except utils.WKTReadingError:
             raise ValueError("The provided geometry is not a valid WKT")
         try:
             utils.get_sr(projection)
         except TypeError:
             raise ValueError("The provided projection is not a valid WKT")
         super().__init__(wkt, projection)
 
@@ -737,15 +732,15 @@
     def period(self):
         return (self.DEFAULT_ORIGIN,) * 2
 
     @property
     def extent(self):
         return tuple(
             utils.shapely_transform(
-                load_wkt(self.wkt), self.projection, "EPSG:4326"
+                utils.shapely_from_wkt(self.wkt), self.projection, "EPSG:4326"
             ).bounds
         )
 
     @property
     def timedelta(self):
         return None
 
@@ -774,15 +769,15 @@
     def process(data, request):
         mode = request["mode"]
         if mode == "time":
             return {"time": [data]}
         elif mode == "meta":
             return {"meta": [None]}
         # load the geometry and transform it into the requested projection
-        geometry = load_wkt(data["wkt"])
+        geometry = utils.shapely_from_wkt(data["wkt"])
         if data["projection"] != request["projection"]:
             geometry = utils.shapely_transform(
                 geometry, data["projection"], request["projection"]
             )
 
         # take a shortcut when the geometry does not intersect the bbox
         x1, y1, x2, y2 = request["bbox"]
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/parallelize.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/parallelize.py`

 * *Files identical despite different names*

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/reduction.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/reduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module containing reduction raster blocks.
 """
 import numpy as np
-from dask_geomodeling.utils import filter_none, get_index
+from dask_geomodeling.utils import filter_none, get_index, Extent
 from dask_geomodeling.utils import parse_percentile_statistic
 from .base import RasterBlock
 from .elemwise import BaseElementwise
 from functools import partial
 
 __all__ = ["Max"]
 
@@ -26,15 +26,15 @@
     "product": np.nanprod,
     # "p<number>" uses np.nanpercentile
 }
 
 
 def check_statistic(statistic):
     if statistic not in STATISTICS:
-        percentile = parse_percentile_statistic(statistic)
+        statistic, percentile = parse_percentile_statistic(statistic)
         if percentile is None:
             raise ValueError('Unknown statistic "{}"'.format(statistic))
 
 
 def reduce_rasters(stack, statistic, no_data_value=None, dtype=None):
     """Apply a statistic (e.g. "mean") to a stack of rasters, skipping
     'no data' values.
@@ -55,19 +55,17 @@
         dtype of the first element in the stack. If the input
         data cannot be cast to this dtype, a ValueError is raised.
 
     Returns:
       dict with "values" and "no_data_value"
     """
     if statistic not in STATISTICS:
-        percentile = parse_percentile_statistic(statistic)
+        statistic, percentile = parse_percentile_statistic(statistic)
         if percentile is None:
             raise KeyError('Unknown statistic "{}"'.format(statistic))
-        else:
-            statistic = "percentile"
 
     if len(stack) == 0:
         raise ValueError("Cannot reduce a zero-length stack")
 
     # get the output array properties (dtype, no_data_value, shape)
     if dtype is None:
         dtype = stack[0]["values"].dtype
@@ -178,22 +176,18 @@
     def geometry(self):
         """Combined geometry in the projection of the first store geometry. """
         geometries = filter_none([x.geometry for x in self.args])
         if len(geometries) == 0:
             return
         elif len(geometries) == 1:
             return geometries[0]
-        result = geometries[0]
-        sr = result.GetSpatialReference()
+        extent = Extent.from_geometry(geometries[0])
         for geometry in geometries[1:]:
-            if not geometry.GetSpatialReference().IsSame(sr):
-                geometry = geometry.Clone()
-                geometry.TransformTo(sr)
-            result = result.Union(geometry)
-        return result
+            extent = extent.union(Extent.from_geometry(geometry))
+        return extent.as_geometry()
 
 
 def wrap_reduction_function(statistic):
     def reduction_function(process_kwargs, *args):
         stack = []
         for arg in args:
             if "time" in arg or "meta" in arg:
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/sources.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,19 @@
         projection,
         pixel_size,
         pixel_origin,
         time_first=0,
         time_delta=None,
         metadata=None,
     ):
-        data = np.atleast_3d(data)
+        data = np.asarray(data)
+        if data.ndim == 2:
+            data = data[np.newaxis]
+        if data.ndim != 3:
+            raise ValueError("data should be two- or three-dimensional.")
         no_data_value = data.dtype.type(no_data_value)
         projection = utils.get_epsg_or_wkt(projection)
         if not hasattr(pixel_size, "__iter__"):
             pixel_size = [pixel_size] * 2
         else:
             pixel_size = list(pixel_size)
             if len(pixel_size) != 2:
@@ -142,22 +146,22 @@
         a, d = self.pixel_size
         return utils.GeoTransform((p, a, 0, q, 0, -d))
 
     def _get_extent(self):
         if not self.data.size:
             return
         bbox = self.geo_transform.get_bbox((0, 0), self.data.shape[1:])
-        return utils.Extent(bbox, utils.get_sr(self.projection))
+        return utils.Extent(bbox, self.projection)
 
     @property
     def extent(self):
         extent = self._get_extent()
         if extent is None:
             return
-        return extent.transformed(utils.EPSG4326).bbox
+        return extent.transformed("EPSG:4326").bbox
 
     @property
     def geometry(self):
         extent = self._get_extent()
         if extent is None:
             return
         return extent.as_geometry()
@@ -366,19 +370,19 @@
     def geo_transform(self):
         return utils.GeoTransform(self.gdal_dataset.GetGeoTransform())
 
     def _get_extent(self):
         bbox = self.geo_transform.get_bbox(
             (0, 0), (self.gdal_dataset.RasterYSize, self.gdal_dataset.RasterXSize)
         )
-        return utils.Extent(bbox, utils.get_sr(self.projection))
+        return utils.Extent(bbox, self.projection)
 
     @property
     def extent(self):
-        extent_epsg4326 = self._get_extent().transformed(utils.EPSG4326)
+        extent_epsg4326 = self._get_extent().transformed("EPSG:4326")
         return extent_epsg4326.bbox
 
     @property
     def geometry(self):
         return self._get_extent().as_geometry()
 
     def __len__(self):
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/spatial.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import math
 
 from scipy import ndimage
 import numpy as np
 from osgeo import ogr
 
 from dask_geomodeling.utils import (
-    EPSG3857,
-    EPSG4326,
     POLYGON,
     get_sr,
     Extent,
     get_dtype_min,
     get_footprint,
     get_index,
     shapely_transform,
@@ -62,16 +60,16 @@
     sr = get_sr(request["projection"])
     bbox = request["bbox"]
 
     # throughout, variables in the projected unit ( = meters, mostly) are
     # suffixed by _m, in pixels by _px
     if sr.IsGeographic():
         # expand geographic bbox in EPSG3857
-        extent_geom = Extent(bbox, sr)
-        bbox = extent_geom.transformed(EPSG3857).bbox
+        extent_geom = Extent(bbox, request["projection"])
+        bbox = extent_geom.transformed("EPSG:3857").bbox
     else:
         # most Projected projections are in meters, but to be sure:
         radius_m /= sr.GetLinearUnits()
 
     # compute the initial zoom factors: how much to expand the bbox to obtain
     # margins of exactly 'radius' (in meters)
     x1, y1, x2, y2 = bbox
@@ -98,16 +96,16 @@
         x1 - margins_m[1],
         y1 - margins_m[0],
         x2 + margins_m[1],
         y2 + margins_m[0],
     )
     if sr.IsGeographic():
         # transform back to original projection
-        extent_proj = Extent(new_request["bbox"], EPSG3857)
-        new_request["bbox"] = extent_proj.transformed(sr).bbox
+        extent_proj = Extent(new_request["bbox"], "EPSG:3857")
+        new_request["bbox"] = extent_proj.transformed(request["projection"]).bbox
     new_request["height"] += 2 * margins_px[0]
     new_request["width"] += 2 * margins_px[1]
 
     return new_request, radius_px
 
 
 class Dilate(BaseSingle):
@@ -529,36 +527,29 @@
             return self.store.geo_transform
 
     @property
     def extent(self):
         geometry = self.geometry
         if geometry is None:
             return
-        if not geometry.GetSpatialReference().IsSame(EPSG4326):
-            geometry = geometry.Clone()
-            geometry.TransformTo(EPSG4326)
-        x1, x2, y1, y2 = geometry.GetEnvelope()
-        return x1, y1, x2, y2
+        return Extent.from_geometry(geometry).transformed("EPSG:4326").bbox
 
     @property
     def geometry(self):
         """Combined geometry in this block's native projection. """
         store_geometry = self.store.geometry
         if store_geometry is None:
             return
-        sr = get_sr(self.place_projection)
-        if not store_geometry.GetSpatialReference().IsSame(sr):
-            store_geometry = store_geometry.Clone()
-            store_geometry.TransformTo(sr)
-        _x1, _x2, _y1, _y2 = store_geometry.GetEnvelope()
+        extent = Extent.from_geometry(store_geometry).transformed(self.place_projection)
+        _x1, _y1, _x2, _y2 = extent.bbox
         p, q = self.anchor
         P, Q = zip(*self.coordinates)
         x1, x2 = _x1 + min(P) - p, _x2 + max(P) - p
         y1, y2 = _y1 + min(Q) - q, _y2 + max(Q) - q
-        return ogr.CreateGeometryFromWkt(POLYGON.format(x1, y1, x2, y2), sr)
+        return ogr.CreateGeometryFromWkt(POLYGON.format(x1, y1, x2, y2), extent.sr)
 
     def get_sources_and_requests(self, **request):
         if request["mode"] != "vals":
             return ({"mode": request["mode"]}, None), (self.store, request)
 
         # transform the anchor and coordinates into the requested projection
         anchor = shapely_transform(
@@ -572,19 +563,15 @@
         ]
 
         # transform the source's extent
         extent_geometry = self.store.geometry
         if extent_geometry is None:
             # no geometry means: no data
             return (({"mode": "null"}, None),)
-        sr = get_sr(request["projection"])
-        if not extent_geometry.GetSpatialReference().IsSame(sr):
-            extent_geometry = extent_geometry.Clone()
-            extent_geometry.TransformTo(sr)
-        xmin, xmax, ymin, ymax = extent_geometry.GetEnvelope()
+        xmin, xmax, ymin, ymax = Extent.from_geometry(extent_geometry).transformed(request["projection"]).bbox
 
         # compute the requested cellsize
         x1, y1, x2, y2 = request["bbox"]
         size_x = (x2 - x1) / request["width"]
         size_y = (y2 - y1) / request["height"]
 
         # point requests: never request the full source extent
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/raster/temporal.py` & `dask-geomodeling-2.4.0/dask_geomodeling/raster/temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         else:
             closed = None
             label = None
             timezone = None
         if not isinstance(statistic, str):
             raise TypeError("'{}' object is not allowed.".format(type(statistic)))
         # interpret percentile statistic
-        percentile = parse_percentile_statistic(statistic)
+        statistic, percentile = parse_percentile_statistic(statistic.lower())
         if percentile:
             statistic = "p{0}".format(percentile)
         elif statistic not in self.STATISTICS:
             raise ValueError("Unknown statistic '{}'".format(statistic))
         super(TemporalAggregate, self).__init__(
             source, frequency, statistic, closed, label, timezone
         )
@@ -616,16 +616,15 @@
         # mode == 'vals'
         if data is None or "values" not in data:
             return
 
         values = data["values"]
         if values.shape[0] != len(times):
             raise RuntimeError("Shape of raster does not match number of timestamps")
-        statistic = process_kwargs["statistic"]
-        percentile = parse_percentile_statistic(statistic)
+        statistic, percentile = parse_percentile_statistic(process_kwargs["statistic"])
         if percentile:
             extensive = False
             agg_func = partial(np.nanpercentile, q=percentile)
         else:
             extensive = TemporalAggregate.STATISTICS[statistic]["extensive"]
             agg_func = TemporalAggregate.STATISTICS[statistic]["func"]
 
@@ -702,15 +701,15 @@
 
     def __init__(self, source, statistic="sum", frequency=None, timezone="UTC"):
         if not isinstance(source, RasterBlock):
             raise TypeError("'{}' object is not allowed.".format(type(source)))
         if not isinstance(statistic, str):
             raise TypeError("'{}' object is not allowed.".format(type(statistic)))
         # interpret percentile statistic
-        percentile = parse_percentile_statistic(statistic)
+        statistic, percentile = parse_percentile_statistic(statistic.lower())
         if percentile:
             statistic = "p{0}".format(percentile)
         elif statistic not in self.STATISTICS:
             raise ValueError("Unknown statistic '{}'".format(statistic))
         if frequency is not None:
             if not isinstance(frequency, str):
                 raise TypeError("'{}' object is not allowed.".format(type(frequency)))
@@ -856,16 +855,15 @@
         # mode == 'vals'
         if data is None or "values" not in data:
             return
 
         values = data["values"]
         if values.shape[0] != len(times):
             raise RuntimeError("Shape of raster does not match number of timestamps")
-        statistic = process_kwargs["statistic"]
-        percentile = parse_percentile_statistic(statistic)
+        statistic, percentile = parse_percentile_statistic(process_kwargs["statistic"])
         if percentile:
             extensive = False
             agg_func = partial(np.nanpercentile, q=percentile)
         else:
             extensive = Cumulative.STATISTICS[statistic]["extensive"]
             agg_func = Cumulative.STATISTICS[statistic]["func"]
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling/utils.py` & `dask-geomodeling-2.4.0/dask_geomodeling/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import re
 import math
 import pytz
 import os
 import warnings
-from functools import lru_cache
+from functools import lru_cache, partial
 from itertools import repeat
 
 from math import floor, log10
 
 import numpy as np
 import pandas as pd
 from scipy import ndimage
 from dask import config
 
 from osgeo import gdal, ogr, osr, gdal_array
 from shapely.geometry import box, Point
-from shapely import wkb as shapely_wkb
-from pyproj import CRS
+from shapely.ops import transform as _shapely_transform
+
+try:  # shapely 2.*
+    from shapely import from_wkt, GEOSException
+except ImportError:  # shapely 1.*
+    from shapely.errors import ShapelyError as GEOSException
+    from shapely.wkt import loads as from_wkt
+
+
+from pyproj import CRS, Transformer
+from pyproj.exceptions import ProjError
 
 import fiona
 import fiona.crs
 
 POLYGON = "POLYGON (({0} {1},{2} {1},{2} {3},{0} {3},{0} {1}))"
 
 try:
@@ -100,20 +109,24 @@
 
 
 class Extent(object):
     """ Spatially aware extent. """
 
     def __init__(self, bbox, sr):
         self.bbox = bbox
-        self.sr = sr
+        self.srs = get_projection(sr)
+
+    @property
+    def sr(self):
+        return get_sr(self.srs)
 
     def __repr__(self):
         return "<{}: {} / {}>".format(
             self.__class__.__name__,
-            get_projection(self.sr),
+            self.srs,
             get_rounded_repr(self.bbox),
         )
 
     @property
     def width(self):
         return self.bbox[2] - self.bbox[0]
 
@@ -147,17 +160,36 @@
     def buffered(self, size):
         """ Return Extent instance. """
         x1, y1, x2, y2 = self.bbox
         buffered_bbox = x1 - size, y1 - size, x2 + size, y2 + size
         return self.__class__(bbox=buffered_bbox, sr=self.sr)
 
     def transformed(self, sr):
-        geometry = self.as_geometry()
-        geometry.TransformTo(sr)
-        return Extent.from_geometry(geometry)
+        srs = get_projection(sr)
+        if self.srs.upper() == srs.upper():
+            return self  # avoids shapely geometry construction
+        geometry = shapely_transform(box(*self.bbox), self.srs, srs)
+        return Extent(bbox=geometry.bounds, sr=srs)
+
+    def union(self, other):
+        """Return the union of self and other, in the SRS of self"""
+        a = self.bbox
+        b = other.transformed(self.srs).bbox
+        return Extent(bbox=(min(a[0], b[0]), min(a[1], b[1]), max(a[2], b[2]), max(a[3], b[3])), sr=self.srs)
+
+    def intersection(self, other):
+        """Return the intersection of self and other, in the SRS of self
+
+        Returns None if the intersection has no area.
+        """
+        a = self.bbox
+        b = other.transformed(self.srs).bbox
+        result = Extent(bbox=(max(a[0], b[0]), max(a[1], b[1]), min(a[2], b[2]), min(a[3], b[3])), sr=self.srs)
+        if result.width > 0 and result.height > 0:
+            return result
 
 
 class GeoTransform(tuple):
     """
     Wrapper with handy methods for the GeoTransform tuple
     as used by the GDAL library.
 
@@ -391,56 +423,56 @@
 class TransformException(Exception):
     """Exception used for errors occuring while transforming between spatial
     reference systems"""
 
     pass
 
 
-def wkb_transform(wkb, src_sr, dst_sr):
-    """
-    Return a shapely geometry transformed from src_sr to dst_sr.
-
-    :param wkb: wkb bytes
-    :param src_sr: source osr SpatialReference
-    :param dst_sr: destination osr SpatialReference
-    """
-    result = ogr.CreateGeometryFromWkb(wkb, src_sr)
-    result.TransformTo(dst_sr)
-    return result.ExportToWkb()
+@lru_cache(maxsize=100)
+def get_transform_func(src_srs: str, dst_srs: str):
+    transformer = Transformer.from_crs(
+        CRS(src_srs), CRS(dst_srs), always_xy=True
+    )
+    return partial(transformer.transform, errcheck=True)
 
 
 def shapely_transform(geometry, src_srs, dst_srs):
     """
     Return a shapely geometry transformed from src_srs to dst_srs.
 
     :param geometry: shapely geometry
     :param src_srs: source projection string
     :param dst_srs: destination projection string
 
-    Note that we do not use geopandas for the transformation, because this is
-    much slower than OGR.
+    Note that we separately construct (and cache) the Transformer instance,
+    because of large overhead in constructing the instance since PROJ v6.
     """
-    transform_kwargs = {
-        "wkb": geometry.wkb,
-        "src_sr": get_sr(src_srs),
-        "dst_sr": get_sr(dst_srs),
-    }
+    if src_srs.upper() == dst_srs.upper():
+        return geometry
     try:
-        output_wkb = wkb_transform(**transform_kwargs)
-    except RuntimeError:
-        # include the geometry in the error message, truncated to 64 chars
-        wkt = geometry.wkt
-        if len(wkt) > 64:
-            wkt = wkt[:61] + "..."
+        func = get_transform_func(src_srs, dst_srs)
+        return _shapely_transform(func, geometry)
+    except ProjError:
         raise TransformException(
             "An error occured while transforming {} from {} to {}.".format(
-                wkt, src_srs, dst_srs
+                geometry.wkt, src_srs, dst_srs
             )
         )
-    return shapely_wkb.loads(output_wkb)
+
+
+def shapely_from_wkt(wkt):
+    """Return a shapely geometry from a WKT representation."""
+    try:
+        return from_wkt(wkt)
+    except GEOSException as e:
+        raise WKTReadingError(str(e))
+
+
+class WKTReadingError(Exception):
+    pass
 
 
 def geoseries_transform(df, src_srs, dst_srs):
     """
     Transform a GeoSeries to a different SRS. Returns a copy.
 
     :param df: GeoSeries to transform
@@ -488,37 +520,24 @@
         warnings.simplefilter("ignore")
         source = geometry.centroid.buffer(min_size / 2)
     target = shapely_transform(source, src_srs=src_srs, dst_srs=dst_srs)
     x1, y1, x2, y2 = target.bounds
     return max(x2 - x1, y2 - y1)
 
 
-def transform_extent(extent, src_srs, dst_srs):
-    """
-    Return extent tuple transformed from src_srs to dst_srs.
-
-    :param extent: xmin, ymin, xmax, ymax
-    :param src_srs: source projection string
-    :param dst_srs: destination projection string
-    """
-    source = box(*extent)
-    target = shapely_transform(source, src_srs=src_srs, dst_srs=dst_srs)
-    return target.bounds
-
-
-EPSG3857 = get_sr("EPSG:3857")
-EPSG4326 = get_sr("EPSG:4326")
-
-
 def get_projection(sr):
     """ Return simple userinput string for spatial reference, if any. """
+    if isinstance(sr, str):
+        return sr
     key = str("GEOGCS") if sr.IsGeographic() else str("PROJCS")
-    return "{name}:{code}".format(
-        name=sr.GetAuthorityName(key), code=sr.GetAuthorityCode(key)
-    )
+    name = sr.GetAuthorityName(key)
+    if name is None:
+        return sr.ExportToWkt()
+    code = sr.GetAuthorityCode(key)
+    return "{name}:{code}".format(name=name, code=code)
 
 
 def get_epsg_or_wkt(text):
     """
     Return EPSG:<code> where possible, and WKT otherwise.
 
     :param text: Textual representation of a spatial reference system.
@@ -814,15 +833,17 @@
     """Parses p<float> to a float, or None if it does not match."""
     # interpret percentile statistic
     percentile_match = PERCENTILE_REGEX.findall(statistic)
     if percentile_match:
         percentile = float(percentile_match[0])
         if not 0 <= percentile <= 100:
             raise ValueError("Percentiles must be in the range [0, 100]")
-        return percentile
+        return "percentile", percentile
+    else:
+        return statistic, None
 
 
 def dtype_for_statistic(dtype, statistic):
     """Return the result dtype of given statistic function"""
     # the dtype depends on the statistic
     if statistic in ("min", "max"):
         return dtype
```

### Comparing `dask-geomodeling-2.3.9/dask_geomodeling.egg-info/SOURCES.txt` & `dask-geomodeling-2.4.0/dask_geomodeling.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 dask_geomodeling/config.py
 dask_geomodeling/ipyleaflet_plugin.py
 dask_geomodeling/measurements.py
 dask_geomodeling/utils.py
 dask_geomodeling.egg-info/PKG-INFO
 dask_geomodeling.egg-info/SOURCES.txt
 dask_geomodeling.egg-info/dependency_links.txt
-dask_geomodeling.egg-info/entry_points.txt
 dask_geomodeling.egg-info/not-zip-safe
 dask_geomodeling.egg-info/requires.txt
 dask_geomodeling.egg-info/top_level.txt
 dask_geomodeling/core/__init__.py
 dask_geomodeling/core/graphs.py
 dask_geomodeling/geometry/__init__.py
 dask_geomodeling/geometry/aggregate.py
```

### Comparing `dask-geomodeling-2.3.9/setup.py` & `dask-geomodeling-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = '2.3.9'
+version = '2.4.0'
 
 long_description = "\n\n".join([open("README.rst").read(), open("CHANGES.rst").read()])
 
 install_requires = (
     [
         "dask[delayed]>=0.20",
         "pandas>=0.23",
@@ -48,11 +48,11 @@
         "dask_geomodeling.geometry",
         "dask_geomodeling.raster",
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=install_requires,
     tests_require=tests_require,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     extras_require={"test": tests_require, "cityhash": ["cityhash"]},
     entry_points={"console_scripts": []},
 )
```

