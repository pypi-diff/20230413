# Comparing `tmp/wis-s3api-0.0.7.tar.gz` & `tmp/wis-s3api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wis-s3api-0.0.7.tar", last modified: Thu Feb  9 13:20:03 2023, max compression
+gzip compressed data, was "wis-s3api-0.0.8.tar", last modified: Thu Apr 13 12:00:24 2023, max compression
```

## Comparing `wis-s3api-0.0.7.tar` & `wis-s3api-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-02-09 13:20:03.218447 wis-s3api-0.0.7/
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1071 2022-12-27 09:09:38.000000 wis-s3api-0.0.7/LICENSE
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      122 2022-12-27 09:09:38.000000 wis-s3api-0.0.7/MANIFEST.in
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-02-09 13:20:03.218447 wis-s3api-0.0.7/PKG-INFO
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1611 2023-01-13 04:30:25.000000 wis-s3api-0.0.7/README.md
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       35 2023-02-09 12:38:16.000000 wis-s3api-0.0.7/requirements.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      392 2023-02-09 13:20:03.218447 wis-s3api-0.0.7/setup.cfg
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1715 2023-02-09 13:19:51.000000 wis-s3api-0.0.7/setup.py
-drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-02-09 13:20:03.214447 wis-s3api-0.0.7/wis_s3api/
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1250 2022-12-29 11:19:29.000000 wis-s3api-0.0.7/wis_s3api/__init__.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)    12455 2023-02-09 13:07:41.000000 wis-s3api-0.0.7/wis_s3api/era5.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2338 2023-01-13 03:20:01.000000 wis-s3api-0.0.7/wis_s3api/gpm.py
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      216 2023-02-09 12:56:31.000000 wis-s3api-0.0.7/wis_s3api/wis_s3api.py
-drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-02-09 13:20:03.218447 wis-s3api-0.0.7/wis_s3api.egg-info/
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-02-09 13:20:02.000000 wis-s3api-0.0.7/wis_s3api.egg-info/PKG-INFO
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      341 2023-02-09 13:20:03.000000 wis-s3api-0.0.7/wis_s3api.egg-info/SOURCES.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       36 2023-02-09 13:20:02.000000 wis-s3api-0.0.7/wis_s3api.egg-info/dependency_links.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)        1 2022-12-29 10:07:02.000000 wis-s3api-0.0.7/wis_s3api.egg-info/not-zip-safe
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       36 2023-02-09 13:20:02.000000 wis-s3api-0.0.7/wis_s3api.egg-info/requires.txt
--rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       10 2023-02-09 13:20:02.000000 wis-s3api-0.0.7/wis_s3api.egg-info/top_level.txt
+drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:00:24.323988 wis-s3api-0.0.8/
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1071 2022-12-27 09:09:38.000000 wis-s3api-0.0.8/LICENSE
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      122 2022-12-27 09:09:38.000000 wis-s3api-0.0.8/MANIFEST.in
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-04-13 12:00:24.323988 wis-s3api-0.0.8/PKG-INFO
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1611 2023-01-13 04:30:25.000000 wis-s3api-0.0.8/README.md
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       48 2023-04-13 11:55:13.000000 wis-s3api-0.0.8/requirements.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      392 2023-04-13 12:00:24.327988 wis-s3api-0.0.8/setup.cfg
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1715 2023-02-22 06:10:50.000000 wis-s3api-0.0.8/setup.py
+drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:00:24.307988 wis-s3api-0.0.8/wis_s3api/
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     1277 2023-04-13 11:58:09.000000 wis-s3api-0.0.8/wis_s3api/__init__.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)    13066 2023-04-13 11:56:37.000000 wis-s3api-0.0.8/wis_s3api/era5.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     4610 2023-04-13 11:56:38.000000 wis-s3api-0.0.8/wis_s3api/gfs.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     5505 2023-04-13 11:56:37.000000 wis-s3api-0.0.8/wis_s3api/gpm.py
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      266 2023-04-13 11:57:52.000000 wis-s3api-0.0.8/wis_s3api/wis_s3api.py
+drwxr-xr-x   0 zhujianfeng  (1013) zhujianfeng  (1013)        0 2023-04-13 12:00:24.323988 wis-s3api-0.0.8/wis_s3api.egg-info/
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)     2345 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/PKG-INFO
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)      358 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/SOURCES.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       49 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/dependency_links.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)        1 2022-12-29 10:07:02.000000 wis-s3api-0.0.8/wis_s3api.egg-info/not-zip-safe
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       49 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/requires.txt
+-rw-r--r--   0 zhujianfeng  (1013) zhujianfeng  (1013)       10 2023-04-13 12:00:24.000000 wis-s3api-0.0.8/wis_s3api.egg-info/top_level.txt
```

### Comparing `wis-s3api-0.0.7/LICENSE` & `wis-s3api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wis-s3api-0.0.7/PKG-INFO` & `wis-s3api-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wis-s3api
-Version: 0.0.7
+Version: 0.0.8
 Summary: minio/s3 api
 Home-page: https://github.com/zjf014/wis-s3api
 Author: Jianfeng Zhu
 Author-email: zjf014@gmail.com
 License: MIT license
 Keywords: wis_s3api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `wis-s3api-0.0.7/README.md` & `wis-s3api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wis-s3api-0.0.7/setup.py` & `wis-s3api-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='wis_s3api',
     name='wis-s3api',
     packages=find_packages(include=['wis_s3api', 'wis_s3api.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zjf014/wis-s3api',
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

### Comparing `wis-s3api-0.0.7/wis_s3api/__init__.py` & `wis-s3api-0.0.8/wis_s3api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """Top-level package for wis-s3api."""
-import wis_s3api as main
+from .wis_s3api import paras
 
 __author__ = """Jianfeng Zhu"""
 __email__ = 'zjf014@gmail.com'
-__version__ = '0.0.1'
+__version__ = '0.0.8'
 
 # endpoint_url = 'http://minio.waterism.com:9000'
 # access_key = 'JKhbLNL0jNKqbjn4'
 # secret_key = '0RDubDRBIrC2WOHAP4nHtYP28TXtVj8H'
 # bucket_path = 'test/geodata/'
 
 import os
 
 home_path = os.environ['HOME']
 
 if os.path.exists(os.path.join(home_path,'.wiss3api')):
-    rows = 0
-    for line in open(os.path.join(home_path,'.wiss3api')):
-        key = line.split('=')[0].strip()
-        value = line.split('=')[1].strip()
-        # print(key,value)
-        if key == 'endpoint_url':
-            main.endpoint_url = value
-        elif key == 'access_key':
-            main.access_key = value
-        elif key == 'secret_key':
-            main.secret_key = value
-        elif key == 'bucket_path':
-            main.bucket_path = value
+    pass
+    # rows = 0
+    # for line in open(os.path.join(home_path,'.wiss3api')):
+    #     key = line.split('=')[0].strip()
+    #     value = line.split('=')[1].strip()
+    #     # print(key,value)
+    #     if key == 'endpoint_url':
+    #         main.endpoint_url = value
+    #     elif key == 'access_key':
+    #         main.access_key = value
+    #     elif key == 'secret_key':
+    #         main.secret_key = value
+    #     elif key == 'bucket_path':
+    #         main.bucket_path = value
 else:
     
-    main.access_key = input('access_key:')
-    main.secret_key = input('access_key:')
+    access_key = input('access_key:')
+    secret_key = input('secret_key:')
 
     f = open(os.path.join(home_path,'.wiss3api'),'w')
-    f.write('endpoint_url = ' + main.endpoint_url)
-    f.write('\naccess_key = ' + main.access_key)
-    f.write('\nsecret_key = ' + main.secret_key)
-    f.write('\nbucket_path = ' + main.bucket_path)
+    f.write('endpoint_url = ' + paras['endpoint_url'])
+    f.write('\naccess_key = ' + access_key)
+    f.write('\nsecret_key = ' + secret_key)
+    f.write('\nbucket_path = ' + paras['bucket_path'])
     f.close()
```

### Comparing `wis-s3api-0.0.7/wis_s3api/era5.py` & `wis-s3api-0.0.8/wis_s3api/era5.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,37 @@
 import xarray as xr
 
 endpoint_url = paras['endpoint_url']
 access_key = paras['access_key']
 secret_key = paras['secret_key']
 bucket_path = paras['bucket_path']
 
+home_path = os.environ['HOME']
+
+if os.path.exists(os.path.join(home_path,'.wiss3api')):
+    for line in open(os.path.join(home_path,'.wiss3api')):
+        key = line.split('=')[0].strip()
+        value = line.split('=')[1].strip()
+        # print(key,value)
+        if key == 'endpoint_url':
+            endpoint_url = value
+        elif key == 'access_key':
+            access_key = value
+        elif key == 'secret_key':
+            secret_key = value
+        elif key == 'bucket_path':
+            bucket_path = value
+
+
 fs = s3fs.S3FileSystem(
     client_kwargs={"endpoint_url": endpoint_url}, 
     key=access_key, 
     secret=secret_key
 )
 
-
 start = np.datetime64('2015-01-01T00:00:00.000000000')
 end = np.datetime64('2021-12-31T23:00:00.000000000')
 box = (115,38,136,54)
 variables = [
     '10 metre U wind component',
     '10 metre V wind component',
     '2 metre dewpoint temperature',
@@ -120,15 +136,32 @@
     'Total precipitation'
     # 'Volumetric soil water layer 1',
     # 'Volumetric soil water layer 2',
     # 'Volumetric soil water layer 3',
     # 'Volumetric soil water layer 4'
 ]
 
-def open(data_variables=variables, start_time=start, end_time=end, bbox=box, time_chunks=24):
+def _bbox(bbox, resolution, offset):
+    
+    lx = bbox[0]
+    rx = bbox[2]
+    LLON = round(int(lx) + resolution * int((lx - int(lx)) / resolution + 0.5) + offset * (int(lx * 10) / 10 + offset - lx) / abs(int(lx * 10) // 10 + offset - lx + 0.0000001), 3)
+    RLON = round(int(rx) + resolution * int((rx - int(rx)) / resolution + 0.5) - offset * (int(rx * 10) / 10 + offset - rx) / abs(int(rx * 10) // 10 + offset - rx + 0.0000001), 3)
+    
+    by = bbox[1]
+    ty = bbox[3]
+    BLAT = round(int(by) + resolution * int((by - int(by)) / resolution + 0.5) + offset * (int(by * 10) / 10 + offset - by) / abs(int(by * 10) // 10 + offset - by + 0.0000001), 3)
+    TLAT = round(int(ty) + resolution * int((ty - int(ty)) / resolution + 0.5) - offset * (int(ty * 10) / 10 + offset - ty) / abs(int(ty * 10) // 10 + offset - ty + 0.0000001), 3)
+    
+    # print(LLON,BLAT,RLON,TLAT)
+    
+    return LLON,BLAT,RLON,TLAT
+
+
+def Open(data_variables=variables, start_time=start, end_time=end, bbox=box, time_chunks=24):
 
     chunks = {"time": time_chunks}
     ds = xr.open_dataset(
         "reference://", 
         engine="zarr", 
         chunks=chunks,
         backend_kwargs={
@@ -153,14 +186,16 @@
     
     if end_time > end:
         end_time = end
     
     times = slice(start_time, end_time)
     ds = ds.sel(time=times)
     
+    bbox = _bbox(bbox, 0.1, 0)
+    
     if bbox[0] < box[0]:
         left = box[0]
     else:
         left = bbox[0]
         
     if bbox[1] < box[1]:
         bottom = box[1]
@@ -182,31 +217,14 @@
     
     ds = ds.sortby('lat', ascending=True)
     ds = ds.sel(lon=longitudes, lat=latitudes)
     
     return ds
 
 
-def _bbox(bbox, resolution, offset):
-    
-    lx = bbox[0]
-    rx = bbox[2]
-    LLON = round(int(lx) + resolution * int((lx - int(lx)) / resolution + 0.5) + offset * (int(lx * 10) / 10 + offset - lx) / abs(int(lx * 10) / 10 + offset - lx), 3)
-    RLON = round(int(rx) + resolution * int((rx - int(rx)) / resolution + 0.5) - offset * (int(rx * 10) / 10 + offset - rx) / abs(int(rx * 10) / 10 + offset - rx), 3)
-    
-    by = bbox[1]
-    ty = bbox[3]
-    BLAT = round(int(by) + resolution * int((by - int(by)) / resolution + 0.5) + offset * (int(by * 10) / 10 + offset - by) / abs(int(by * 10) / 10 + offset - by), 3)
-    TLAT = round(int(ty) + resolution * int((ty - int(ty)) / resolution + 0.5) - offset * (int(ty * 10) / 10 + offset - ty) / abs(int(ty * 10) / 10 + offset - ty), 3)
-    
-    # print(LLON,BLAT,RLON,TLAT)
-    
-    return LLON,BLAT,RLON,TLAT
-
-
 import geopandas as gpd
 
 def from_shp(data_variables=variables, start_time=start, end_time=end, shp=None, time_chunks=24):
 
     gdf = gpd.GeoDataFrame.from_file(shp)
     b = gdf.bounds
     bbox = _bbox((b.loc[0]['minx'],b.loc[0]['miny'],b.loc[0]['maxx'],b.loc[0]['maxy']), 0.1, 0)
```

### Comparing `wis-s3api-0.0.7/wis_s3api.egg-info/PKG-INFO` & `wis-s3api-0.0.8/wis_s3api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wis-s3api
-Version: 0.0.7
+Version: 0.0.8
 Summary: minio/s3 api
 Home-page: https://github.com/zjf014/wis-s3api
 Author: Jianfeng Zhu
 Author-email: zjf014@gmail.com
 License: MIT license
 Keywords: wis_s3api
 Classifier: Development Status :: 2 - Pre-Alpha
```

