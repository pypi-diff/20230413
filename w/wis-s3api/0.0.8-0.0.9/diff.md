# Comparing `tmp/wis-s3api-0.0.8.tar.gz` & `tmp/wis-s3api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wis-s3api-0.0.8.tar", last modified: Thu Apr 13 12:00:24 2023, max compression
+gzip compressed data, was "wis-s3api-0.0.9.tar", last modified: Thu Apr 13 12:12:14 2023, max compression
```

## Comparing `wis-s3api-0.0.8.tar` & `wis-s3api-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:00:24.323988 wis-s3api-0.0.8/
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1071 2022-12-27 09:09:38.000000 wis-s3api-0.0.8/LICENSE
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      122 2022-12-27 09:09:38.000000 wis-s3api-0.0.8/MANIFEST.in
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-04-13 12:00:24.323988 wis-s3api-0.0.8/PKG-INFO
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1611 2023-01-13 04:30:25.000000 wis-s3api-0.0.8/README.md
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       48 2023-04-13 11:55:13.000000 wis-s3api-0.0.8/requirements.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      392 2023-04-13 12:00:24.327988 wis-s3api-0.0.8/setup.cfg
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1715 2023-02-22 06:10:50.000000 wis-s3api-0.0.8/setup.py
-drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:00:24.307988 wis-s3api-0.0.8/wis_s3api/
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1277 2023-04-13 11:58:09.000000 wis-s3api-0.0.8/wis_s3api/__init__.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)    13066 2023-04-13 11:56:37.000000 wis-s3api-0.0.8/wis_s3api/era5.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     4610 2023-04-13 11:56:38.000000 wis-s3api-0.0.8/wis_s3api/gfs.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     5505 2023-04-13 11:56:37.000000 wis-s3api-0.0.8/wis_s3api/gpm.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      266 2023-04-13 11:57:52.000000 wis-s3api-0.0.8/wis_s3api/wis_s3api.py
-drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:00:24.323988 wis-s3api-0.0.8/wis_s3api.egg-info/
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/PKG-INFO
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      358 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/SOURCES.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       49 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/dependency_links.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)        1 2022-12-29 10:07:02.000000 wis-s3api-0.0.8/wis_s3api.egg-info/not-zip-safe
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       49 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/requires.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       10 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/top_level.txt
+drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:12:14.437017 wis-s3api-0.0.9/
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1071 2022-12-27 09:09:38.000000 wis-s3api-0.0.9/LICENSE
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      122 2022-12-27 09:09:38.000000 wis-s3api-0.0.9/MANIFEST.in
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-04-13 12:12:14.437017 wis-s3api-0.0.9/PKG-INFO
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1611 2023-01-13 04:30:25.000000 wis-s3api-0.0.9/README.md
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       48 2023-04-13 11:55:13.000000 wis-s3api-0.0.9/requirements.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      392 2023-04-13 12:12:14.441017 wis-s3api-0.0.9/setup.cfg
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1715 2023-04-13 12:11:33.000000 wis-s3api-0.0.9/setup.py
+drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:12:14.437017 wis-s3api-0.0.9/wis_s3api/
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1277 2023-04-13 12:11:55.000000 wis-s3api-0.0.9/wis_s3api/__init__.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)    13066 2023-04-13 12:10:11.000000 wis-s3api-0.0.9/wis_s3api/era5.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     4610 2023-04-13 12:10:30.000000 wis-s3api-0.0.9/wis_s3api/gfs.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     5505 2023-04-13 12:10:55.000000 wis-s3api-0.0.9/wis_s3api/gpm.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      266 2023-04-13 11:57:52.000000 wis-s3api-0.0.9/wis_s3api/wis_s3api.py
+drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:12:14.437017 wis-s3api-0.0.9/wis_s3api.egg-info/
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-04-13 12:12:13.000000 wis-s3api-0.0.9/wis_s3api.egg-info/PKG-INFO
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      358 2023-04-13 12:12:13.000000 wis-s3api-0.0.9/wis_s3api.egg-info/SOURCES.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       49 2023-04-13 12:12:13.000000 wis-s3api-0.0.9/wis_s3api.egg-info/dependency_links.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)        1 2022-12-29 10:07:02.000000 wis-s3api-0.0.9/wis_s3api.egg-info/not-zip-safe
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       49 2023-04-13 12:12:13.000000 wis-s3api-0.0.9/wis_s3api.egg-info/requires.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       10 2023-04-13 12:12:13.000000 wis-s3api-0.0.9/wis_s3api.egg-info/top_level.txt
```

### Comparing `wis-s3api-0.0.8/LICENSE` & `wis-s3api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wis-s3api-0.0.8/PKG-INFO` & `wis-s3api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wis-s3api
-Version: 0.0.8
+Version: 0.0.9
 Summary: minio/s3 api
 Home-page: https://github.com/zjf014/wis-s3api
 Author: Jianfeng Zhu
 Author-email: zjf014@gmail.com
 License: MIT license
 Keywords: wis_s3api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `wis-s3api-0.0.8/README.md` & `wis-s3api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wis-s3api-0.0.8/setup.py` & `wis-s3api-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='wis_s3api',
     name='wis-s3api',
     packages=find_packages(include=['wis_s3api', 'wis_s3api.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zjf014/wis-s3api',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

### Comparing `wis-s3api-0.0.8/wis_s3api/__init__.py` & `wis-s3api-0.0.9/wis_s3api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Top-level package for wis-s3api."""
 from .wis_s3api import paras
 
 __author__ = """Jianfeng Zhu"""
 __email__ = 'zjf014@gmail.com'
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 # endpoint_url = 'http://minio.waterism.com:9000'
 # access_key = 'JKhbLNL0jNKqbjn4'
 # secret_key = '0RDubDRBIrC2WOHAP4nHtYP28TXtVj8H'
 # bucket_path = 'test/geodata/'
 
 import os
```

### Comparing `wis-s3api-0.0.8/wis_s3api/era5.py` & `wis-s3api-0.0.9/wis_s3api/era5.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
 def from_shp(data_variables=variables, start_time=start, end_time=end, shp=None, time_chunks=24):
 
     gdf = gpd.GeoDataFrame.from_file(shp)
     b = gdf.bounds
     bbox = _bbox((b.loc[0]['minx'],b.loc[0]['miny'],b.loc[0]['maxx'],b.loc[0]['maxy']), 0.1, 0)
 
-    ds = open(data_variables, start_time, end_time, bbox, time_chunks)
+    ds = Open(data_variables, start_time, end_time, bbox, time_chunks)
     
     return ds
 
 
 from netCDF4 import Dataset,date2num,num2date
 import time
 from datetime import datetime, timedelta
@@ -307,15 +307,15 @@
     
     gdf = gpd.GeoDataFrame.from_file(shp)
     b = gdf.bounds
     bbox = _bbox((b.loc[0]['minx'],b.loc[0]['miny'],b.loc[0]['maxx'],b.loc[0]['maxy']), 0.1, 0)
     
     if resolution == 'hourly':
         
-        ds = open(data_variables, start_time, end_time, bbox, time_chunks)
+        ds = Open(data_variables, start_time, end_time, bbox, time_chunks)
     
         if ds.to_netcdf(save_file) == None:
             print(save_file, '已生成')
             ds = xr.open_dataset(save_file)
             return ds
 
     if resolution == 'daily':
@@ -364,15 +364,15 @@
     
     if resolution == '6-hourly':
         
         start_time = np.datetime64(f'{str(start_time)[:10]}T01:00:00.000000000')        
         end_time = np.datetime64(str(end_time)[:10])+1
         end_time = np.datetime64(f'{str(end_time)}T00:00:00.000000000')
     
-        ds = open(data_variables, start_time, end_time, bbox, time_chunks)
+        ds = Open(data_variables, start_time, end_time, bbox, time_chunks)
         
         days = ds['time'].size // 6
         
         data_vars = {}
         for k,v in ds.data_vars.items():
             data_vars[k] = v.attrs
```

### Comparing `wis-s3api-0.0.8/wis_s3api/gfs.py` & `wis-s3api-0.0.9/wis_s3api/gfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,10 @@
 
 def from_shp(data_variables=variables, creation_date=create_date, creation_time='00', valid_time=range(1,121), shp=None, time_chunks=24):
 
     gdf = gpd.GeoDataFrame.from_file(shp)
     b = gdf.bounds
     bbox = _bbox((b.loc[0]['minx'],b.loc[0]['miny'],b.loc[0]['maxx'],b.loc[0]['maxy']), 0.1, 0)
 
-    ds = open(data_variables, creation_date, creation_time, valid_time, bbox, time_chunks)
+    ds = Open(data_variables, creation_date, creation_time, valid_time, bbox, time_chunks)
     
     return ds
```

### Comparing `wis-s3api-0.0.8/wis_s3api/gpm.py` & `wis-s3api-0.0.9/wis_s3api/gpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,10 +169,10 @@
 
 def from_shp(start_time=start, end_time=end, shp=None, time_chunks=24):
 
     gdf = gpd.GeoDataFrame.from_file(shp)
     b = gdf.bounds
     bbox = _bbox((b.loc[0]['minx'],b.loc[0]['miny'],b.loc[0]['maxx'],b.loc[0]['maxy']), 0.1, 0.05)
 
-    ds = open(start_time, end_time, bbox, time_chunks)
+    ds = Open(start_time, end_time, bbox, time_chunks)
     
     return ds
```

### Comparing `wis-s3api-0.0.8/wis_s3api.egg-info/PKG-INFO` & `wis-s3api-0.0.9/wis_s3api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wis-s3api
-Version: 0.0.8
+Version: 0.0.9
 Summary: minio/s3 api
 Home-page: https://github.com/zjf014/wis-s3api
 Author: Jianfeng Zhu
 Author-email: zjf014@gmail.com
 License: MIT license
 Keywords: wis_s3api
 Classifier: Development Status :: 2 - Pre-Alpha
```

