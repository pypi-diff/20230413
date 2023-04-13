# Comparing `tmp/pygmtsar-2023.4.1.tar.gz` & `tmp/pygmtsar-2023.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2023.4.1.tar", last modified: Sat Apr  1 13:50:18 2023, max compression
+gzip compressed data, was "pygmtsar-2023.4.12.tar", last modified: Thu Apr 13 09:44:23 2023, max compression
```

## Comparing `pygmtsar-2023.4.1.tar` & `pygmtsar-2023.4.12.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-01 13:50:18.826285 pygmtsar-2023.4.1/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2023.4.1/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    10037 2023-04-01 13:50:18.826125 pygmtsar-2023.4.1/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     9313 2023-03-12 07:12:55.000000 pygmtsar-2023.4.1/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-01 13:50:18.825188 pygmtsar-2023.4.1/pygmtsar/
--rwxr-xr-x   0 mbg        (501) staff       (20)    25114 2023-03-31 14:50:35.000000 pygmtsar-2023.4.1/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    21884 2023-03-07 05:42:58.000000 pygmtsar-2023.4.1/pygmtsar/PRM_gmtsar.py
--rwxr-xr-x   0 mbg        (501) staff       (20)    11684 2023-03-30 13:07:17.000000 pygmtsar-2023.4.1/pygmtsar/SBAS.py
--rw-r--r--   0 mbg        (501) staff       (20)    17137 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     2161 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)     7320 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_dem_gmt_gdal.py
--rw-r--r--   0 mbg        (501) staff       (20)     8753 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    12213 2023-03-31 14:51:14.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)     4791 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     2504 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_intf.py
--rw-r--r--   0 mbg        (501) staff       (20)     1488 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)     1799 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_landmask_gmt.py
--rw-r--r--   0 mbg        (501) staff       (20)     4993 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_merge_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)      821 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)     9743 2023-03-07 05:42:58.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     5518 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    13311 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     5448 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_sbas_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    10429 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_stack.py
--rw-r--r--   0 mbg        (501) staff       (20)     5630 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_topo_ra.py
--rw-r--r--   0 mbg        (501) staff       (20)     8644 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)     1219 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     5856 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/SBAS_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)      257 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    10812 2023-03-31 15:15:54.000000 pygmtsar-2023.4.1/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     1820 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)      992 2023-02-25 05:08:30.000000 pygmtsar-2023.4.1/pygmtsar/tqdm_joblib.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-01 13:50:18.825940 pygmtsar-2023.4.1/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    10037 2023-04-01 13:50:18.000000 pygmtsar-2023.4.1/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)      872 2023-04-01 13:50:18.000000 pygmtsar-2023.4.1/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2023-04-01 13:50:18.000000 pygmtsar-2023.4.1/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      255 2023-04-01 13:50:18.000000 pygmtsar-2023.4.1/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2023-04-01 13:50:18.000000 pygmtsar-2023.4.1/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2023-04-01 13:50:18.826328 pygmtsar-2023.4.1/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     1847 2023-04-01 13:49:54.000000 pygmtsar-2023.4.1/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-13 09:44:23.660218 pygmtsar-2023.4.12/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2023.4.12/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-13 09:44:23.659787 pygmtsar-2023.4.12/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     9313 2023-03-12 07:12:55.000000 pygmtsar-2023.4.12/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-13 09:44:23.656524 pygmtsar-2023.4.12/pygmtsar/
+-rwxr-xr-x   0 mbg        (501) staff       (20)    25116 2023-04-09 08:43:45.000000 pygmtsar-2023.4.12/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    21884 2023-03-07 05:42:58.000000 pygmtsar-2023.4.12/pygmtsar/PRM_gmtsar.py
+-rwxr-xr-x   0 mbg        (501) staff       (20)    11684 2023-03-30 13:07:17.000000 pygmtsar-2023.4.12/pygmtsar/SBAS.py
+-rw-r--r--   0 mbg        (501) staff       (20)    17137 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2161 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7320 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_dem_gmt_gdal.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8780 2023-04-05 05:10:27.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    12220 2023-04-12 18:26:43.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4791 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2693 2023-04-12 07:30:31.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_intf.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1488 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1799 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_landmask_gmt.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4993 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_merge_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)      821 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9743 2023-03-07 05:42:58.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5518 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13303 2023-04-09 14:02:35.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5448 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_sbas_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10429 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5630 2023-04-11 17:42:45.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_topo_ra.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8644 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1219 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5856 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)      257 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10812 2023-03-31 15:15:54.000000 pygmtsar-2023.4.12/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1820 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)      992 2023-02-25 05:08:30.000000 pygmtsar-2023.4.12/pygmtsar/tqdm_joblib.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-13 09:44:23.659052 pygmtsar-2023.4.12/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)      872 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      259 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2023-04-13 09:44:23.000000 pygmtsar-2023.4.12/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2023-04-13 09:44:23.660270 pygmtsar-2023.4.12/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     1900 2023-04-12 15:02:17.000000 pygmtsar-2023.4.12/setup.py
```

### Comparing `pygmtsar-2023.4.1/LICENSE.txt` & `pygmtsar-2023.4.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/PKG-INFO` & `pygmtsar-2023.4.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2023.4.1
+Version: 2023.4.12
 Summary: PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone
 Home-page: https://github.com/mobigroup/gmtsar
 Author: Alexey Pechnikov
 Author-email: pechnikov@mobigroup.ru
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![MacOS tests](https://github.com/mobigroup/gmtsar/actions/workflows/macos.yml/badge.svg)](https://github.com/mobigroup/gmtsar/actions/workflows/macos.yml)
 [![Ubuntu tests](https://github.com/mobigroup/gmtsar/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/mobigroup/gmtsar/actions/workflows/ubuntu.yml)
 [![PyPI tests](https://github.com/mobigroup/gmtsar/actions/workflows/pypi.yml/badge.svg)](https://github.com/mobigroup/gmtsar/actions/workflows/pypi.yml)
 [![Available on pypi](https://img.shields.io/pypi/v/pygmtsar.svg)](https://pypi.python.org/pypi/pygmtsar/)
```

### Comparing `pygmtsar-2023.4.1/README.md` & `pygmtsar-2023.4.12/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/PRM.py` & `pygmtsar-2023.4.12/pygmtsar/PRM.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,15 @@
         NLOOKSRANGE    1
         NLOOKSAZ       1
         TILEDIR        {tiledir}_snaphu_tiledir
         NPROC          {n_jobs}
         """
         conf_custom = '# custom config\n'
         # defomax can be None
-        keyvalues = [('DEFOMAX_CYCLE', defomax)] if defomax is not None else [] + list(kwargs.items())
+        keyvalues = ([('DEFOMAX_CYCLE', defomax)] if defomax is not None else []) + list(kwargs.items())
         for key, value in keyvalues:
             if isinstance(value, bool):
                 value = 'TRUE' if value else 'FALSE'
             conf_custom += f'        {key} {value}\n'
         return conf_basic + conf_custom
 
 def main():
```

### Comparing `pygmtsar-2023.4.1/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2023.4.12/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_base.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_dem.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_dem_gmt_gdal.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_dem_gmt_gdal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_detrend.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_detrend.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,16 @@
         Returns filtered dataarray with the same coordinates as input one.
         Fast approximate calculation silently skipped when sigma is less than 64 so the result is always exact for small filters.
         """
         import xarray as xr
         import numpy as np
 
         if wavelength is None:
-            print ('NOTE: Gaussian filter cut-off wavelength is not defined, function does nothing')
+            if debug:
+                print ('DEBUG: Gaussian filter cut-off wavelength is not defined, function does nothing')
             return dataarray
 
         # input grid can be too large
         decimator = self.pixel_decimator(resolution_meters=resolution_meters, grid=dataarray, debug=debug)
         # decimate
         dataarray_dec = decimator(dataarray)
         # ground pixel size
```

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_geocode.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_geocode.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
         """
         Inverse geocoding function based on interferogram geocode matrix to call from open_grids(inverse_geocode=True)
         """
         import xarray as xr
         import numpy as np
 
         # helper check
-        if not 'y' in grids.dims and 'x' in grid.dims:
-            print ('NOTE: the grid is not in geograpphic coordinates, miss geocoding')
+        if not 'y' in grids.dims or not 'x' in grids.dims:
+            print ('NOTE: the input grid is not in radar coordinates, miss geocoding')
             return grids
 
         # unify the input grids for transform matrix defined on the intf grid (y, x)
         source_grid = self.get_intf_ll2ra()
         grids = grids.interp_like(source_grid, method='nearest')
 
         # target grid is tranform matrix
@@ -235,16 +235,16 @@
         """
         Inverse geocoding function based on interferogram geocode matrix to call from open_grids(inverse_geocode=True)
         """
         import xarray as xr
         import numpy as np
 
         # helper check
-        if not 'lat' in grids.dims and 'lon' in grid.dims:
-            print ('NOTE: the grid is not in geograpphic coordinates, miss geocoding')
+        if not 'lat' in grids.dims or not 'lon' in grids.dims:
+            print ('NOTE: the grid is not in geographic coordinates, miss geocoding')
             return grids
 
         # unify the input grids for transform matrix defined on the trans_dat grid (lat, lon)
         source_grid = self.get_trans_dat().ll
         grids = grids.interp_like(source_grid, method='nearest')
         # target grid is tranform matrix
         matrix_ll2ra = self.get_intf_ll2ra()
```

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_incidence.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_landmask.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_landmask_gmt.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_landmask_gmt.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_merge.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_merge_gmtsar.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_merge_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_orbits.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_reframe.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_reframe_gmtsar.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_sbas.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_sbas.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,22 @@
                 self.make_s1a_tops(subswath, date, debug=debug)
 
         # generate PRM, LED if needed
         #for (date, dt) in datetimes.iteritems():
         #    #print (dt, date)
         #    ondemand(dt)
         with self.tqdm_joblib(tqdm(desc='PRM generation', total=len(datetimes))) as progress_bar:
-            joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(ondemand)(date, dt) for (date, dt) in datetimes.iteritems())
+            joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(ondemand)(date, dt) for (date, dt) in datetimes.items())
     
         # after merging use unmerged subswath PRM files
         # calc_dop_orb() required for SAT_baseline
         master_dt = datetimes[self.master]
         prm_ref = PRM().from_file(get_filename(master_dt)).calc_dop_orb(inplace=True)
         data = []
-        for (date, dt) in datetimes.iteritems():
+        for (date, dt) in datetimes.items():
             # after merging use unmerged subswath PRM files
             prm_rep = PRM().from_file(get_filename(dt))
             ST0 = prm_rep.get('SC_clock_start')
             DAY = int(ST0 % 1000)
             YR = int(ST0/1000) - 2014
             YDAY = YR * 365 + DAY
             #print (f'YR={YR}, DAY={DAY}')
```

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_sbas_gmtsar.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_sbas_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_stack.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_topo_ra.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_topo_ra.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_trans.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_unwrap.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/SBAS_unwrap_snaphu.py` & `pygmtsar-2023.4.12/pygmtsar/SBAS_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/datagrid.py` & `pygmtsar-2023.4.12/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/tqdm_dask.py` & `pygmtsar-2023.4.12/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar/tqdm_joblib.py` & `pygmtsar-2023.4.12/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2023.4.12/pygmtsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2023.4.1
+Version: 2023.4.12
 Summary: PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone
 Home-page: https://github.com/mobigroup/gmtsar
 Author: Alexey Pechnikov
 Author-email: pechnikov@mobigroup.ru
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![MacOS tests](https://github.com/mobigroup/gmtsar/actions/workflows/macos.yml/badge.svg)](https://github.com/mobigroup/gmtsar/actions/workflows/macos.yml)
 [![Ubuntu tests](https://github.com/mobigroup/gmtsar/actions/workflows/ubuntu.yml/badge.svg)](https://github.com/mobigroup/gmtsar/actions/workflows/ubuntu.yml)
 [![PyPI tests](https://github.com/mobigroup/gmtsar/actions/workflows/pypi.yml/badge.svg)](https://github.com/mobigroup/gmtsar/actions/workflows/pypi.yml)
 [![Available on pypi](https://img.shields.io/pypi/v/pygmtsar.svg)](https://pypi.python.org/pypi/pygmtsar/)
```

### Comparing `pygmtsar-2023.4.1/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2023.4.12/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.1/setup.py` & `pygmtsar-2023.4.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!/usr/bin/env python
+# TODO: xarray 2023.3.0 requires pandas<2,>=1.4
 
 from setuptools import setup
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pygmtsar',
-    version='2023.4.1',
+    version='2023.4.12',
     description='PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mobigroup/gmtsar',
     author='Alexey Pechnikov',
     author_email='pechnikov@mobigroup.ru',
     license='BSD-3-Clause',
     packages=['pygmtsar'],
     install_requires=['xarray>=0.19.0',
-                      'importlib-metadata<=4.12.0',
+                      'importlib-metadata',
                       'numpy>=1.22.4',
-                      'pandas',
+                      'pandas>=1.4',
                       'geopandas',
                       'distributed>=2022.11.1',
                       'dask[complete]',
                       'dask_image',
                       'joblib',
                       'tqdm',
                       'sentineleof',
                       'scipy>=1.9.1',
-                      'shapely',
+                      'shapely>=2.0.1',
                       'scikit-learn',
                       'elevation',
                       'xmltodict',
                       'rioxarray',
                       'ipywidgets',
                       'h5netcdf==1.0.2',
                       'h5py',
@@ -47,9 +48,9 @@
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8'
     ],
-    python_requires='>=3.7'
+    python_requires='>=3.8'
 )
```

