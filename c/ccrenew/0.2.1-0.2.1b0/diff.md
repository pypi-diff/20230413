# Comparing `tmp/ccrenew-0.2.1.tar.gz` & `tmp/ccrenew-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccrenew-0.2.1.tar", last modified: Wed Apr 12 16:26:02 2023, max compression
+gzip compressed data, was "ccrenew-0.2.1b0.tar", last modified: Thu Apr 13 17:31:20 2023, max compression
```

## Comparing `ccrenew-0.2.1.tar` & `ccrenew-0.2.1b0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.681366 ccrenew-0.2.1/
--rw-rw-rw-   0        0        0     1100 2022-11-09 21:01:48.000000 ccrenew-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      349 2023-04-12 16:26:02.680365 ccrenew-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      615 2022-11-11 15:45:04.000000 ccrenew-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 16:26:02.681366 ccrenew-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      437 2023-02-14 20:58:01.000000 ccrenew-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.610365 ccrenew-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.629367 ccrenew-0.2.1/src/ccrenew/
--rw-rw-rw-   0        0        0     1120 2023-04-12 16:25:08.000000 ccrenew-0.2.1/src/ccrenew/__init__.py
--rw-rw-rw-   0        0        0     6869 2023-03-30 20:00:56.000000 ccrenew-0.2.1/src/ccrenew/ccr.py
--rw-rw-rw-   0        0        0     8021 2023-04-05 21:36:13.000000 ccrenew-0.2.1/src/ccrenew/cloud_data.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.648368 ccrenew-0.2.1/src/ccrenew/dashboard/
--rw-rw-rw-   0        0        0     2463 2023-03-30 18:52:35.000000 ccrenew-0.2.1/src/ccrenew/dashboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.667365 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/
--rw-rw-rw-   0        0        0     1783 2023-03-30 17:14:14.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/BV_pp_deg.py
--rw-rw-rw-   0        0        0    18089 2023-03-17 12:55:19.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py
--rw-rw-rw-   0        0        0    15346 2023-03-17 13:06:23.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py
--rw-rw-rw-   0        0        0    15095 2023-03-17 13:06:04.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py
--rw-rw-rw-   0        0        0    13086 2023-03-30 17:22:42.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py
--rw-rw-rw-   0        0        0    18643 2023-04-11 19:13:49.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py
--rw-rw-rw-   0        0        0    16011 2023-03-30 17:25:57.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py
--rw-rw-rw-   0        0        0     4195 2023-03-17 13:10:53.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py
--rw-rw-rw-   0        0        0        0 2022-10-27 20:52:08.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/__init__.py
--rw-rw-rw-   0        0        0       46 2023-03-13 14:27:41.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/_project_processing.py
--rw-rw-rw-   0        0        0     6645 2023-03-31 19:10:24.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/batch_process.py
--rw-rw-rw-   0        0        0     8608 2023-03-17 13:08:51.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/battery_deg.py
--rw-rw-rw-   0        0        0     6026 2023-03-17 13:11:08.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py
--rw-rw-rw-   0        0        0     3668 2023-03-16 14:56:45.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/solcats_API.py
--rw-rw-rw-   0        0        0    10948 2023-03-17 13:13:01.000000 ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.669366 ccrenew-0.2.1/src/ccrenew/dashboard/plotting/
--rw-rw-rw-   0        0        0        0 2022-10-27 20:51:43.000000 ccrenew-0.2.1/src/ccrenew/dashboard/plotting/__init__.py
--rw-rw-rw-   0        0        0    60141 2023-04-12 12:56:15.000000 ccrenew-0.2.1/src/ccrenew/dashboard/plotting/plots.py
--rw-rw-rw-   0        0        0   176836 2023-04-11 21:18:09.000000 ccrenew-0.2.1/src/ccrenew/dashboard/project.py
--rw-rw-rw-   0        0        0    65313 2023-04-11 18:39:34.000000 ccrenew-0.2.1/src/ccrenew/dashboard/session.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.676380 ccrenew-0.2.1/src/ccrenew/dashboard/utils/
--rw-rw-rw-   0        0        0        0 2022-10-27 20:52:31.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/__init__.py
--rw-rw-rw-   0        0        0     5468 2023-03-30 17:24:26.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/dashboard_utils.py
--rw-rw-rw-   0        0        0     1623 2023-02-01 16:17:23.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/df_tools.py
--rw-rw-rw-   0        0        0     1265 2022-09-22 19:52:54.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/logging_conf.py
--rw-rw-rw-   0        0        0     7281 2023-03-16 14:57:33.000000 ccrenew-0.2.1/src/ccrenew/dashboard/utils/project_neighbors.py
--rw-rw-rw-   0        0        0    12778 2023-04-11 17:07:28.000000 ccrenew-0.2.1/src/ccrenew/data_determination.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.679366 ccrenew-0.2.1/src/ccrenew/pvmodel/
--rw-rw-rw-   0        0        0       54 2023-03-09 21:59:00.000000 ccrenew-0.2.1/src/ccrenew/pvmodel/__init__.py
--rw-rw-rw-   0        0        0    11379 2023-04-12 15:52:36.000000 ccrenew-0.2.1/src/ccrenew/pvmodel/project_model.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:26:02.644366 ccrenew-0.2.1/src/ccrenew.egg-info/
--rw-rw-rw-   0        0        0      349 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1688 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 16:26:02.000000 ccrenew-0.2.1/src/ccrenew.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/
+-rw-rw-rw-   0        0        0     1100 2022-11-09 21:01:48.000000 ccrenew-0.2.1b0/LICENSE
+-rw-rw-rw-   0        0        0      351 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2022-11-11 15:45:04.000000 ccrenew-0.2.1b0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-02-14 20:58:01.000000 ccrenew-0.2.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.742975 ccrenew-0.2.1b0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.758599 ccrenew-0.2.1b0/src/ccrenew/
+-rw-rw-rw-   0        0        0     1181 2023-04-13 17:30:35.000000 ccrenew-0.2.1b0/src/ccrenew/__init__.py
+-rw-rw-rw-   0        0        0     6869 2023-03-30 20:00:56.000000 ccrenew-0.2.1b0/src/ccrenew/ccr.py
+-rw-rw-rw-   0        0        0     8021 2023-04-05 21:36:13.000000 ccrenew-0.2.1b0/src/ccrenew/cloud_data.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.789852 ccrenew-0.2.1b0/src/ccrenew/dashboard/
+-rw-rw-rw-   0        0        0     2467 2023-04-13 17:05:41.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.796362 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/
+-rw-rw-rw-   0        0        0     1783 2023-03-30 17:14:14.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/BV_pp_deg.py
+-rw-rw-rw-   0        0        0    18089 2023-03-17 12:55:19.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py
+-rw-rw-rw-   0        0        0    15346 2023-03-17 13:06:23.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py
+-rw-rw-rw-   0        0        0    15095 2023-03-17 13:06:04.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py
+-rw-rw-rw-   0        0        0    13082 2023-04-13 17:05:22.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py
+-rw-rw-rw-   0        0        0    18643 2023-04-11 19:13:49.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py
+-rw-rw-rw-   0        0        0    16007 2023-04-13 17:04:44.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py
+-rw-rw-rw-   0        0        0     4195 2023-03-17 13:10:53.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py
+-rw-rw-rw-   0        0        0        0 2022-10-27 20:52:08.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-03-13 14:27:41.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/_project_processing.py
+-rw-rw-rw-   0        0        0     6645 2023-03-31 19:10:24.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/batch_process.py
+-rw-rw-rw-   0        0        0     8608 2023-03-17 13:08:51.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/battery_deg.py
+-rw-rw-rw-   0        0        0     6026 2023-03-17 13:11:08.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py
+-rw-rw-rw-   0        0        0     3668 2023-03-16 14:56:45.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/solcats_API.py
+-rw-rw-rw-   0        0        0    10948 2023-03-17 13:13:01.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/src/ccrenew/dashboard/plotting/
+-rw-rw-rw-   0        0        0        0 2022-10-27 20:51:43.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/plotting/__init__.py
+-rw-rw-rw-   0        0        0    61442 2023-04-13 15:13:36.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/plotting/plots.py
+-rw-rw-rw-   0        0        0   177466 2023-04-13 17:18:26.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/project.py
+-rw-rw-rw-   0        0        0    65258 2023-04-13 16:57:01.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/session.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-27 20:52:31.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-04-13 16:55:48.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/dashboard_utils.py
+-rw-rw-rw-   0        0        0     1623 2023-02-01 16:17:23.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/df_tools.py
+-rw-rw-rw-   0        0        0     1265 2022-09-22 19:52:54.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/logging_conf.py
+-rw-rw-rw-   0        0        0     7281 2023-03-16 14:57:33.000000 ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/project_neighbors.py
+-rw-rw-rw-   0        0        0    12778 2023-04-11 17:07:28.000000 ccrenew-0.2.1b0/src/ccrenew/data_determination.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/src/ccrenew/pvmodel/
+-rw-rw-rw-   0        0        0       54 2023-03-09 21:59:00.000000 ccrenew-0.2.1b0/src/ccrenew/pvmodel/__init__.py
+-rw-rw-rw-   0        0        0    11379 2023-04-12 15:52:36.000000 ccrenew-0.2.1b0/src/ccrenew/pvmodel/project_model.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.811999 ccrenew-0.2.1b0/src/ccrenew/tst_pkg/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:27:25.000000 ccrenew-0.2.1b0/src/ccrenew/tst_pkg/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-13 17:28:19.000000 ccrenew-0.2.1b0/src/ccrenew/tst_pkg/tst.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:31:20.774247 ccrenew-0.2.1b0/src/ccrenew.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-04-13 17:31:20.000000 ccrenew-0.2.1b0/src/ccrenew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2023-04-13 17:31:20.000000 ccrenew-0.2.1b0/src/ccrenew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:31:20.000000 ccrenew-0.2.1b0/src/ccrenew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 17:31:20.000000 ccrenew-0.2.1b0/src/ccrenew.egg-info/top_level.txt
```

### Comparing `ccrenew-0.2.1/LICENSE` & `ccrenew-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/README.md` & `ccrenew-0.2.1b0/README.md`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/__init__.py` & `ccrenew-0.2.1b0/src/ccrenew/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base package for Cypress Creek Renewables Utilities
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.1b0"
 
 from collections import namedtuple
 from datetime import (
     date,
     datetime
 )
 import numpy as np
@@ -19,14 +19,18 @@
 Numeric = int|float
 
 # Custom data structures
 DaylightParams = namedtuple('DaylightParams', ['lat', 'lon', 'tz'])
 ProjectModelParams = namedtuple('ProjectModelParams', ['project_name', 'ccr_id', 'folder', 'tz', 'lat', 'lon',
                                              'elevation', 'mwdc', 'racking', 'tilt_gcr', 'max_angle',
                                              'temp_coef', 'a_module', 'b_module', 'delta_tcnd'])
+utility_map = {
+    'DEC': 'duke',
+    'DEP': 'duke'
+}
 
 from ccrenew import (
     ccr,
     data_determination
 )
 
 # Custom exceptions
```

### Comparing `ccrenew-0.2.1/src/ccrenew/ccr.py` & `ccrenew-0.2.1b0/src/ccrenew/ccr.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/cloud_data.py` & `ccrenew-0.2.1b0/src/ccrenew/cloud_data.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/__init__.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 # Create boto s3 client
 s3_client = boto3.client('s3')
 
 # Initilize custom mappings
 Colmap = namedtuple('Colmap', ['col_list', 'col_avg'])
-DataPlatformDirs = namedtuple('DataPlatformDirs', ['sharepoint', 's3'])
+DataSourceDirs = namedtuple('DataSourceDirs', ['s3_local', 's3', 'sharepoint'])
 S3FilePath = namedtuple('S3FilePath', ['bucket', 'key'])
 
 
 def make_s3_filepath(filepath:str|Path, obj_type:str) -> S3FilePath:
     filepath = Path(filepath)
     filepath_parts = filepath.parts
     bucket = filepath_parts[1]
@@ -33,16 +33,16 @@
     if obj_type == 'folder':
         key = key + '/'
 
     s3_filepath = S3FilePath(bucket, key)
 
     return s3_filepath
 
-def get_modified_time(filepath:str|Path, data_platform:str, obj_type:str='file'):
-    if data_platform == 's3':
+def get_modified_time(filepath:str|Path, data_source:str, obj_type:str='file'):
+    if data_source == 's3':
         s3_filepath = make_s3_filepath(filepath, obj_type=obj_type)
         s3_file = s3_client.get_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
         modified_time = s3_file['LastModified']
     else:
         modified_time = datetime.fromtimestamp(os.path.getmtime(filepath))
 
     return modified_time
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/BV_pp_deg.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/BV_pp_deg.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_IS6.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Correct_Meter_data_v08_smartercheck.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Correct_POI_data_v01.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Performance_Guarantees_v01.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,21 +194,21 @@
     df_perf['Guar_freq'] = 'Monthly'
     df_perf['Gaur_range'] = ['{} - {}'.format(s.strftime('%m/%d'), e.strftime('%m/%d')) for s,e in zip(month_start, result.index.tolist())]
     
     return df_perf, result.tolist()
 
 
 #added by SPA on 11/28/18
-def SCEG_performance_guarantee(project_name, df, df_Pvsyst, PIS_date, df_perf, data_platform):    
+def SCEG_performance_guarantee(project_name, df, df_Pvsyst, PIS_date, df_perf, data_source):    
     
     #read in Net Energy and REC Delivery Requirements - One large Excel file for all the SCEG sites taking different tabs
     #df_attachement = pd.read_excel(r'D:\Box Sync\Cypress Creek Renewables\Asset Management\8) Production Data\_Dashboard_Project\Python_Functions\Other Scripts\Testing - SCEG Performance Guarantees\SCEG_Perf Gaur_Contract_Quantity.xlsx', sheet_name=project_name) #NEED TO PUT THIS EXCEL FILE IN CENTRAL LOCATION AND RENAME
         
     filepath = Path(file_project) / 'Python_Functions\Other Scripts\Performance Guarantee Inputs\SCEG\SCEG_Perf Gaur_Contract_Quantity.xlsx'
-    if data_platform == 's3':
+    if data_source == 's3':
         filepath = filepath.as_posix().replace('s3:/', 's3://')
 
     df_attachment = pd.read_excel(filepath, sheet_name=project_name) #NEED TO PUT THIS EXCEL FILE IN CENTRAL LOCATION AND RENAME
 
     #get start year to test if we are in year 2 or not
     perf_guar_start_year = PIS_date.year
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Plant_Availability_v16_bbsc.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Rate_Structure_Python_with_DST_v07.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     
     aux = pd.DataFrame(np.zeros([len(df),len(filler)]), index = df.index, columns = filler)
     
     export = pd.concat([aux,df], axis = 1)
     
     return export
 
-def generate_Rate_column (project_name, file_input, shift_DST, year, data_platform):
+def generate_Rate_column (project_name, file_input, shift_DST, year, data_source):
 
     def generate_rate(df_t1, df_t2, normal_rate_flag, year, shift_DST):
         #  Create DataFrame with Columns of Interest
         #
         #   Read all variables defined on Table 1
         #
         # year =  df_t1[df_t1['Name'] == 'Current Year']['Value'].values[0]
@@ -351,15 +351,15 @@
         normal_rate_flag = False
 
         #read new file - only use specific year's worth of data
         filedir = Path(file_input).parent
         filename = project_name + '_YearlyRates.csv'
         filepath = filedir / filename
 
-        if data_platform == 's3':
+        if data_source == 's3':
             filepath = filepath.as_posix().replace('s3:/', 's3://')
 
         df = pd.read_csv(filepath, index_col = 'IND', usecols= ['IND', np.str(year)])
 
         if not shift_DST:
             df_1 = yearly8760(df.copy(), project_name, year, shift_DST=True)
             df_2 = yearly8760(df.copy(), project_name, year, shift_DST=False)
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/Table_by_Rate_Schedule_v01.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/batch_process.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/batch_process.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/battery_deg.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/battery_deg.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/snow_loss_functions_v3.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/solcats_API.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/solcats_API.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/data_processing/weather_adjusted_functions_v03.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/plotting/plots.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/plotting/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1114,14 +1114,44 @@
 
                 on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
                 fig.canvas.mpl_connect('pick_event', on_pick)
 
                 fig_list.append(fig)
 
 
+        elif plot_name.replace(' ', '_').lower() == 'utility':
+            utility_data = kwargs.get('utility_data', pd.DataFrame())
+            if utility_data.empty:
+                print(f"No utility data to plot for {self.project.project_name}. Please check that utility data exists for this project.")
+            
+            y_meter = self.project.df['Meter_Corrected_2']
+            y_meter.name = 'CCR Meter'
+            y_utility = utility_data.iloc[:,0]
+            y_utility.name = 'Utility Meter'
+
+            fig, ax = plt.subplots(num=f"Utility Data - {self.project.project_name}")
+            fig.suptitle(self.project.project_name)
+            ax.set_title('Utility Meter vs CCR Meter')
+
+            y_meter.plot(ax=ax)
+            y_utility.plot(ax=ax, linestyle='--')
+            ax.set_xlim(left=min_date, right=max_date)
+
+            # Create interactive legend
+            legend = ax.legend()
+            legend.set_draggable(True)
+            plot_paths = {line._label: {'lines': [line]} for line in ax.get_lines()}
+
+            for legend_handle in legend.legendHandles:
+                legend_handle.set_picker(5)
+
+            on_pick = partial(picker, fig=fig, plot_paths=plot_paths)
+            fig.canvas.mpl_connect('pick_event', on_pick)
+
+
         elif plot_name.replace(' ', '_').lower() == 'snow':
             # Snow Plots
             y_snow_data = self.project.snow_data['snow']
             y_snow_coverage = self.project.snow_coverage
 
             fig, ax = plt.subplots(num='Snow Data - {}'.format(self.project.project_name))
             fig.suptitle(self.project.project_name)
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/project.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import xlsxwriter.utility
 
 from ccrenew import (
     __version__,
     ccr,
     DateLike,
     Numeric,
+    utility_map,
     FileNotFoundError,
     FileOpenError
 )
 from ccrenew.dashboard import (
     Colmap,
     S3FilePath,
     func_timer,
@@ -75,14 +76,16 @@
 # suppress warnings about "A value is trying to be set on a copy of a slice from a DataFrame."
 pd.set_option('mode.chained_assignment', None)
 
 # Create logger
 # logger = logging.getLogger(__name__)
 # logger = logging.getLogger(__name__)
 
+S3_PERFDATADEV = 'perfdatadev.ccrenew.com'
+
 
 class PowertrackFileException(Exception):
     pass
 
 class Project:
     """An object representing a project (i.e. site). This should never be initialized\
         outside of a [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance,
@@ -124,28 +127,25 @@
         self.config_neighbor_sensors = set()
         
         # Project properties passed from DashboardSession
         self.df_proj_keys = proj_init_dict['df_proj_keys']
         self.df_proj_ss_comments = proj_init_dict['df_proj_ss_comments']
         self.dashboard_dir = proj_init_dict['dashboard_dir']
         self.data_cutoff_date = proj_init_dict['data_cutoff_date']
-        self.data_platform = proj_init_dict['data_platform']
-        self.data_platform_dirs = proj_init_dict['data_platform_dirs']
+        self.year = proj_init_dict['year']
         self.data_source = proj_init_dict['data_source']
+        self.data_source_dirs = proj_init_dict['data_source_dirs']
         self.report_type = proj_init_dict['report_type']
         self.Battery_AC_site = proj_init_dict['Battery_AC_site']
         self.Battery_DC_site = proj_init_dict['Battery_DC_site']
         self.Tracker_site = proj_init_dict['Tracker_site']
         self.raw_snow_df = proj_init_dict['raw_snow_df']
         self.snow_file = proj_init_dict['snow_file']
         self.neighbor_list = proj_init_dict['neighbor_list']
 
-        # Project year based on `data_source`
-        self.year = int(self.data_source.split('_')[0])
-
         # Get information for the project from DF keys
         # `self.df_proj_keys` is the appropriate row from `df_keys` as a dictionary
         self.project_directory = self.df_proj_keys['Folder']
         self.lat = self.df_proj_keys['GPS_Lat']
         self.lon = self.df_proj_keys['GPS_Long']
         self.tz = f"US/{self.df_proj_keys['Timezone']}"
         self.MWAC = self.df_proj_keys['MWAC']
@@ -311,15 +311,15 @@
         return f'{self.report_type_map[self.report_type]} Project object for {self.project_name}'
 
 
     def _parse_config_file(self):
         """Reads data from config file & parses each sheet into a dataframe"""
         # Read variables from Plant Configuration File
         # `self.config_sheets` will store all the sheets from the config file as a dictionary
-        if self.last_update_config == get_modified_time(self.config_filepath, self.data_platform, 'file'):
+        if self.last_update_config == get_modified_time(self.config_filepath, self.data_source, 'file'):
             return
 
         try:
             print("Loading config file for {}".format(self.project_name))
             self.config_sheets = pd.read_excel(self.config_filepath, sheet_name=None)
         except Exception:
             error_num = sys.exc_info()[1].errno # type: ignore
@@ -385,22 +385,22 @@
         # Get capacity & neighbor sensor params
         self.OFF_PEAK = self.config_dict['OFF_PEAK']
         self.CAPACITY_ON_PEAK_SUMMER = self.config_dict['CAPACITY_ON_PEAK_SUMMER']
         self.CAPACITY_ON_PEAK_NON_SUMMER = self.config_dict['CAPACITY_ON_PEAK_NON_SUMMER']
         self.Get_Sensor = self.df_config.loc[(self.df_config['Name'].str.lower() == 'get_sensor'), :]
         
         # Update last config update timestamp
-        self.last_update_config = get_modified_time(self.config_filepath, self.data_platform, 'file')
+        self.last_update_config = get_modified_time(self.config_filepath, self.data_source, 'file')
 
 
     def _load_bool_file(self):
         try:
-            if self.last_update_bool != get_modified_time(self.bool_filepath, self.data_platform, 'file'):
+            if self.last_update_bool != get_modified_time(self.bool_filepath, self.data_source, 'file'):
                 self.df_bool = pd.read_csv(self.bool_filepath, index_col=0, parse_dates=True)
-                self.last_update_bool = get_modified_time(self.bool_filepath, self.data_platform, 'file')
+                self.last_update_bool = get_modified_time(self.bool_filepath, self.data_source, 'file')
         except:
             pass
 
 
     def _map_columns(self):
 
         def get_colnames(df_cols, colref):
@@ -547,15 +547,15 @@
                                         self.project_directory,
                                         self.project_name,
                                        'Plant_Config_File',
                                         config_filename)
 
         config_filepath = Path(config_filepath)
 
-        if self.data_platform == 's3':
+        if self.data_source == 's3':
             # Convert Windows-type filepath to use forwards slashes like a normal
             config_filepath = config_filepath.as_posix().replace('s3:/', 's3://')
             s3_filepath = make_s3_filepath(config_filepath, obj_type='file')
             try:
                 s3_client.get_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
             except:
                 error_msg = f"*** No config file on S3 found for {self.project_name}, skipping project. Check that filepath exists: {config_filepath}"
@@ -578,48 +578,48 @@
                                      self.project_directory,
                                      self.project_name,
                                      'Plant_Config_File',
                                      bool_filename)
 
         bool_filepath = Path(bool_filepath)
 
-        if self.data_platform == 's3':
+        if self.data_source == 's3':
             # Convert Windows-type filepath to use forwards slashes like a normal
             bool_filepath = bool_filepath.as_posix().replace('s3:/', 's3://')
         else:
             bool_filepath = str(bool_filepath)
 
         return bool_filepath
 
 
     def _find_powertrack_file(self):
         # Find Powertrack folder
-        self.data_AE_dir = os.path.join(self.dashboard_dir,
-                                        self.project_directory,
-                                        self.project_name,
-                                        'Powertrack_data')
+        self.powertrack_dir = os.path.join(self.dashboard_dir,
+                                           self.project_directory,
+                                           self.project_name,
+                                           'Powertrack_data')
         
-        if self.data_platform == 's3':
-            s3_filepath = make_s3_filepath(self.data_AE_dir, obj_type='folder')
+        if self.data_source == 's3':
+            s3_filepath = make_s3_filepath(self.powertrack_dir, obj_type='folder')
             all_pt_files = s3_client.list_objects(Bucket=s3_filepath.bucket, Prefix=s3_filepath.key)
-            powertrack_filename = [f['Key'] for f in all_pt_files['Contents'] if self.data_source in f['Key']][0]
+            powertrack_filename = [f['Key'] for f in all_pt_files['Contents'] if self.year in f['Key']][0]
             powertrack_filename = Path(powertrack_filename).name
         else:
-            self.data_AE_all_files = [f for f in os.listdir(self.data_AE_dir) if os.path.isfile(os.path.join(self.data_AE_dir, f))]
-            powertrack_filename = [s for s in self.data_AE_all_files if self.data_source in s][0]
+            self.powertrack_all_files = [f for f in os.listdir(self.powertrack_dir) if os.path.isfile(os.path.join(self.powertrack_dir, f))]
+            powertrack_filename = [s for s in self.powertrack_all_files if str(self.year) in s][0]
 
         # TODO: check on error handling here if we can't find the Powertrack file
         if len(powertrack_filename) == 0:
             raise PowertrackFileException("*** No Powertrack file found for {}, skipping project".format(self.project_name))
 
         # Build filename for Powertrack file
         powertrack_filepath = Path(self.dashboard_dir) / self.project_directory / self.project_name / 'Powertrack_data' / powertrack_filename
         powertrack_csv = Path(powertrack_filepath).parent / f"{self.year}_hourly_{self.project_name}.csv"
 
-        if self.data_platform == 's3':
+        if self.data_source == 's3':
             # Convert Windows-type filepath to use forwards slashes like a normal
             powertrack_filepath = powertrack_filepath.as_posix().replace('s3:/', 's3://')
             powertrack_csv = powertrack_csv.as_posix().replace('s3:/', 's3://')
         else:
             powertrack_filepath = str(powertrack_filepath)
             powertrack_csv = str(powertrack_csv)
         
@@ -631,15 +631,15 @@
         pickle_jar = os.path.join(self.dashboard_dir,
                                        self.project_directory,
                                        self.project_name,
                                        'Pickle_Jar')
 
         pickle_jar = Path(pickle_jar)
 
-        if self.data_platform == 's3':
+        if self.data_source == 's3':
             # Check that Pickle Jar exists & create folder if not
             s3_filepath = make_s3_filepath(pickle_jar, obj_type='folder')
             try:
                 s3_client.get_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
             except:
                 s3_client.put_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
 
@@ -663,18 +663,18 @@
         """
 
         # Read Powertrack data
         # If the powertrack file has been updated since we last loaded production
         # we'll read the data from Excel & store a copy in df_powertrack
         # If it hasn't been updated we'll just use the powertrack copy we loaded previously
         try:
-            last_update_powertrack_file = get_modified_time(self.powertrack_filepath, self.data_platform, 'file')
+            last_update_powertrack_file = get_modified_time(self.powertrack_filepath, self.data_source, 'file')
         except:
             self.powertrack_filepath, self.powertrack_csv = self._find_powertrack_file()
-            last_update_powertrack_file = get_modified_time(self.powertrack_filepath, self.data_platform, 'file')
+            last_update_powertrack_file = get_modified_time(self.powertrack_filepath, self.data_source, 'file')
         
         if self.last_update_powertrack != last_update_powertrack_file:
             self.__load_from_source(self.powertrack_filepath)
         else:
             # If we try to load from `df_powertrack` and it doesn't exist we'll need to load from source
             try:
                 self.df = self.df_powertrack.copy()
@@ -756,54 +756,32 @@
         # Locate columns
         self._locate_column_positions()
 
         # Perform any unit conversions needed
         self._convert_sensor_units()
 
         # Update the last updated date for the powertrack file
-        self.last_update_powertrack = get_modified_time(self.powertrack_filepath, self.data_platform, 'file')
+        self.last_update_powertrack = get_modified_time(self.powertrack_filepath, self.data_source, 'file')
         self.df_powertrack = self.df.copy()
 
         # Write to csv
         self.df.to_csv(self.powertrack_csv)
 
 
     def _fetch_bluesky_data(self):
         # If solcast data hasn't been loaded from AWS or the indexes of the main df & df_bluesky don't match - load data
         if self.df_bluesky.empty or self.df_bluesky.index[0] != self.df.index[0] or self.df_bluesky.index[-1] != self.df.index[-1]:
             start_date = self.df.index[0]
             end_date = self.df.index[-1]
 
+            # We will only pull GHI data if the project has a GHI column
             fetch_ghi = False
             if self.pos_GHI:
                 fetch_ghi = True
             df_bluesky = self.pv_model.run_bluesky(start_date, end_date, resample=True, fetch_ghi=fetch_ghi) # type: ignore
-            # df_bluesky = df_bluesky.fillna(0)
-
-            # # (the filter returns True where there are daylight zeroes so we need to invert it)
-            # proj_ghi_poa = df_project_ghi.join(project_poa['poa_global'])
-            # proj_ghi_bool = ~det.daylight_zeroes(df=proj_ghi_poa, pv_model=self)
-
-            # # Convert all False values (bad data) to np.inf so we can replace with NaN after reindexing in the next step
-            # proj_ghi_bool = proj_ghi_bool.replace(False, np.inf)
-
-            # # Reindex to add nighttime rows back in & set them to False so they don't change the data in the original df
-            # proj_ghi_bool = proj_ghi_bool.reindex(index=proj_ghi_poa.index).fillna(False)
-
-            # # Replace np.inf with np.nan (we used np.inf to demarcate bad data so it wouldn't be overwritten in the step above)
-            # proj_ghi_bool = proj_ghi_bool.replace(np.inf, np.nan)
-
-            # # Filter out bad data
-            # proj_ghi_poa = (proj_ghi_poa*proj_ghi_bool).astype(float)
-
-            # # Fill in any NaNs with satellite data
-            # proj_ghi_poa = proj_ghi_poa.fillna({'proj_ghi': df_bluesky['sat_ghi'], 'poa_global': df_bluesky['sat_poa']})
-
-            # # Rename & drop column `sites_ghi_poa` column to match sites with no GHI
-            # df_bluesky[['ghi', 'poa']] = proj_ghi_poa[['proj_ghi', 'poa_global']]
 
             # Rename to match sensor avg columns & replace NaNs
             self.df_bluesky = df_bluesky.rename(columns={'Tamb': 'Tamb_avg', 'Tmod': 'Tmod_avg',
                                                          'poa': 'POA_avg', 'ghi': 'GHI_avg'})
 
   
     def _locate_column_positions(self):
@@ -1082,50 +1060,94 @@
                 break
             
         print('\n')
         print('Power data successfully generated for {}'.format(self.project_name))
         print('\n')
         return power_data
 
+    
+    def get_utility_data(self, resample:bool = True) -> pd.DataFrame:
+        """
+        Pulls utility meter data from S3 for the Project.
+
+        Args:
+            resample: Option to resample the data to hourly.
+        Returns:
+            df_utility: A 1-column dataframe containing the metered energy from the utility.
+        """
+        utility_code = self.df_proj_keys['Utility']
+        utility = utility_map[utility_code]
+        ccr_id = self.df_proj_keys['CCR_ID']
+        object_key = f"5min_archive/Utility_Data/{ccr_id}/{str(self.year)}_Utility_Data.csv"
+        df_utility = pd.read_csv(f"s3://{S3_PERFDATADEV}/{object_key}", index_col=0, parse_dates=True)
+        df_utility = df_utility.loc[~df_utility.index.duplicated(), :]
+        if utility == 'duke':
+            df_utility.index = df_utility.index+pd.Timedelta("-15min")
+            meter_col = df_utility.filter(regex='kWh', axis=1).sum().idxmax()
+            df_utility = df_utility[[meter_col]].rename(columns={meter_col: 'utility_meter'})
+
+        if resample:
+            df_utility = df_utility.resample('H').sum()
+
+        return df_utility
+    
+
+    def plot_utility_data(self, resample:bool = True, **kwargs) -> None:
+        """
+        Plots the utility meter data alongside the CCR meter for the Project
+        
+        Args:
+            resample: Option to resample the data to hourly
+        """
+        # We'll check if the project is processed & process it if not.
+        # We won't flip the processed flag because we don't have neighbor data from a session
+        if not self.processed:
+            self._load_bool_file()
+            self.load_production_data()
+            self._process_data(neighbor_sensor_data={}, datasub=False, use_bluesky=False)
+            self.last_update_powertrack = datetime.fromtimestamp(0)
+        df_utility = self.get_utility_data(resample=resample)
+        self.plotter.draw_plots(plot_order='utility', utility_data=df_utility, close_plots=False, **kwargs)
+
 
-    def plot_meters(self):
+    def plot_meters(self) -> None:
         """Plots all meters for the Project"""
         # We'll check if the project is processed & process it if not.
         # We won't flip the processed flag because we don't have neighbor data from a session
         if not self.processed:
             self._load_bool_file()
             self.load_production_data()
             self._process_data(neighbor_sensor_data={}, datasub=False, use_bluesky=False)
             self.last_update_powertrack = datetime.fromtimestamp(0)
         self.plotter.draw_plots(plot_order='meters', close_plots=False)
 
 
-    def plot_snow(self):
+    def plot_snow(self) -> None:
         """Plots snow data for the Project"""
         # We'll check if the project is processed & process it if not.
         # We won't flip the processed flag because we don't have neighbor data from a session
         if not self.processed:
             self._load_bool_file()
             self.load_production_data()
             self._process_data(neighbor_sensor_data={}, datasub=False, use_bluesky=False)
             self.last_update_powertrack = datetime.fromtimestamp(0)
         self.plotter.draw_plots(plot_order='snow', close_plots=False)
 
 
-    def save_pickle(self, store_plots=False):
+    def save_pickle(self, store_plots=False) -> None:
         """Saves the Project object to a pickle in the
         [project_directory][ccrenew.dashboard.project.Project.project_directory].
         """
         if not store_plots and self.plotter:
             self.plotter.plot_list = {}
         year = self.year
         pickle_name = utils.picklefy_project_name(self.project_name)
         pickle_file = str(year) + "_" + pickle_name + ".pickle"
-        pickle_path_sharepoint = Path(self.data_platform_dirs.sharepoint) / self.project_directory / self.project_name / 'Pickle_Jar' / pickle_file
-        pickle_path_s3 = Path(self.data_platform_dirs.s3) / self.project_directory / self.project_name / 'Pickle_Jar' / pickle_file
+        pickle_path_sharepoint = Path(self.data_source_dirs.sharepoint) / self.project_directory / self.project_name / 'Pickle_Jar' / pickle_file
+        pickle_path_s3 = Path(self.data_source_dirs.s3) / self.project_directory / self.project_name / 'Pickle_Jar' / pickle_file
         pickle_path_s3 = pickle_path_s3.as_posix().replace('s3:/', 's3://')
         
         with open(pickle_path_sharepoint, 'wb') as f:
             pickle.dump(self, f)
         
         fs = s3fs.S3FileSystem()
         with fs.open(pickle_path_s3, 'wb') as f:
@@ -1297,30 +1319,30 @@
             sharepoint_filename = sharepoint_filename.replace('.xlsx', '_UL.xlsx')
 
         if server.lower() != 'prod':
             s3_filename = s3_filename.replace('.xlsx', '_COPY.xlsx')
             sharepoint_filename = sharepoint_filename.replace('.xlsx', '_COPY.xlsx')
 
         # Create a copy of template in sharepoint
-        dashboard_root_dir = Path(self.data_platform_dirs.sharepoint)
+        dashboard_root_dir = Path(self.data_source_dirs.sharepoint)
         template_filepath = dashboard_root_dir / 'Python_Functions' / 'Dashboard_Template' / template_filename
         output_dir = dashboard_root_dir / self.project_directory / self.project_name
         output_template = shutil.copy(template_filepath, output_dir)
         output_filepath = output_dir / sharepoint_filename
         try:
             os.rename(output_template, output_filepath)
         except FileExistsError:
             os.remove(output_filepath)
             os.rename(output_template, output_filepath)
 
         # Write data to file on sharepoint
         df_tools.dfs_to_excel(output_filepath, df_dict)
 
         # Store copy on S3 with export timestamp
-        s3_filepath = Path(self.data_platform_dirs.s3) / self.project_directory / self.project_name / s3_filename
+        s3_filepath = Path(self.data_source_dirs.s3) / self.project_directory / self.project_name / s3_filename
         s3_filepath = make_s3_filepath(s3_filepath, obj_type='file')
         bucket = s3_filepath.bucket
         key = s3_filepath.key
         s3_client.upload_file(output_filepath, Bucket=bucket, Key=key)
 
         if server != 'prod':
             os.remove(output_filepath)
@@ -1342,15 +1364,15 @@
 
         # PostgreSQL initialization
         engine = ccr.get_sql_engine()
         metadata = MetaData()
 
         #  Save to Dataframes folder on S3
         df_filename = self.data_source + self.project_name + '.csv'
-        df_filepath = Path(self.data_platform_dirs.s3) / self.project_directory / self.project_name / 'Dataframes' / df_filename
+        df_filepath = Path(self.data_source_dirs.s3) / self.project_directory / self.project_name / 'Dataframes' / df_filename
         df_filepath = df_filepath.as_posix().replace('s3:/', 's3://')
         
         if report_type.lower() == 'ul':
             df_filepath = df_filepath.replace('.csv', '_UL_.csv')
 
         if server != 'prod':
             df_filepath = df_filepath.replace('.csv', '_COPY.csv')
@@ -1618,15 +1640,15 @@
                                'Meter_&_ava_&_grid', 'Meter_losses&snow', 'Weather_KWh',
                                'NREL_Weather_Adj_%', 'Inv_Ava_%', 'Grid_Ava_%', 'Snow_Adj_%', 'Plant_Perf_%']]
 
         # Build filepath
         week_folder = os.path.join(self.dashboard_dir, 'Python_Functions', 'Other Scripts', 'Weekly reporting', 'results', self.project_name)
         weekly_filepath = os.path.join(week_folder, self.data_source + '.csv')
 
-        if self.data_platform == 's3':
+        if self.data_source == 's3':
             weekly_filepath = Path(weekly_filepath).as_posix().replace('s3:/', 's3://')
         
         if server != 'prod':
             weekly_filepath = weekly_filepath.replace('.csv', '_COPY.csv')
             df_weekly.to_csv(weekly_filepath)
             s3_filepath = make_s3_filepath(weekly_filepath, obj_type='file')
             s3_client.delete_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
@@ -1664,15 +1686,15 @@
         """
         server = kwargs.get('server')
 
         # Update bool file
         self._update_bool()
 
         if server != 'prod':
-            if self.data_platform == 's3':
+            if self.data_source == 's3':
                 filepath = self.bool_filepath.replace('.csv', '_COPY.csv')
                 s3_filepath = make_s3_filepath(filepath, obj_type='file')
                 self.df_bool.to_csv(filepath)
                 s3_client.delete_object(Bucket=s3_filepath.bucket, Key=s3_filepath.key)
             else:
                 dev_filepath = self.bool_filepath.replace('.csv', '_COPY.csv')
                 self.df_bool.to_csv(dev_filepath)
@@ -1889,15 +1911,15 @@
         # For PVsyst we need to shift the columns to adjust for DST.
         # It also deletes the last value. It is from the following year
         (self.df_Pvsyst_2, _,
         self.rates_year, self.normal_rate_flag) = rates.generate_Rate_column(self.project_name,
                                                                              self.config_filepath,
                                                                              shift_DST=None,
                                                                              year=self.year,
-                                                                             data_platform=self.data_platform)
+                                                                             data_source=self.data_source)
         self.df_Pvsyst_2 = self.df_Pvsyst_2.iloc[:-1, :]
         self.rates_year = self.rates_year.iloc[:-1, :]
 
         # Also need to remove Feb 29, to match PVsyst file.
         self.df_Pvsyst_2 = self.df_Pvsyst_2[~((self.df_Pvsyst_2.index.month == 2) & (self.df_Pvsyst_2.index.day == 29))]
 
         # Adjust df_Pvsyst index to match the year that we're running
@@ -2579,25 +2601,25 @@
         self.losses.loc[:, 'Inv_losses'] = self.df.loc[:, 'Meter_&_ava'] - self.df.loc[:, 'Meter_Corrected_2']
         self.losses.loc[:, 'Grid_losses'] = self.df.loc[:, 'Meter_&_ava_&_grid'] - self.df.loc[:, 'Meter_&_ava']
         self.losses.loc[:, 'Snow_losses'] = self.df.loc[:, 'Meter_losses&snow'] - self.df.loc[:, 'Meter_&_ava_&_grid']
 
 
     def __calculate_revenue(self, method):
         def initial_hourly():
-            self.rates_year_i = self.rates_year['Rates'][self.df.index[0]:self.df.index[-1]]
-            flat_year_i = self.rates_year['Flat'][self.df.index[0]:self.df.index[-1]]
-            self.df['Rates'] = self.rates_year_i
+            rates_ytd = self.rates_year['Rates'][self.df.index[0]:self.df.index[-1]]
+            flat_ytd = self.rates_year['Flat'][self.df.index[0]:self.df.index[-1]]
+            self.df['Rates'] = rates_ytd
             self.df['Energy_Peak'] = self.rates_year['Energy_Peak']
             self.df['Capacity_Peak'] = self.rates_year['Capacity_Peak']
-            self.df['Meter_Corrected_2_rev'] = (self.rates_year_i * self.df['Meter_Corrected_2']) + flat_year_i
-            self.df['Meter_&_ava_rev'] = (self.rates_year_i * self.df['Meter_&_ava']) + flat_year_i
-            self.df['Meter_&_ava_&_grid_rev'] = (self.rates_year_i * self.df['Meter_&_ava_&_grid']) + flat_year_i
-            self.df['Meter_losses&snow_rev'] = (self.rates_year_i * self.df['Meter_losses&snow']) + flat_year_i
-            self.df['POI_Corrected_2_rev'] = (self.rates_year_i * self.df['POI_Corrected_2']) + flat_year_i
-            self.df['POI_modeled_rev'] = (self.rates_year_i * self.df['POI_modeled']) + flat_year_i
+            self.df['Meter_Corrected_2_rev'] = (rates_ytd * self.df['Meter_Corrected_2']) + flat_ytd
+            self.df['Meter_&_ava_rev'] = (rates_ytd * self.df['Meter_&_ava']) + flat_ytd
+            self.df['Meter_&_ava_&_grid_rev'] = (rates_ytd * self.df['Meter_&_ava_&_grid']) + flat_ytd
+            self.df['Meter_losses&snow_rev'] = (rates_ytd * self.df['Meter_losses&snow']) + flat_ytd
+            self.df['POI_Corrected_2_rev'] = (rates_ytd * self.df['POI_Corrected_2']) + flat_ytd
+            self.df['POI_modeled_rev'] = (rates_ytd * self.df['POI_modeled']) + flat_ytd
 
         def weather_adjusted_monthly():
             #  Calculate Revenue.
             #  With the NREL method, Revenue due to Weather is calculated with monthly %
             #
             self.df_Pvsyst_2_month['Revenue_IE_P50_days_adj'] = \
                 self.df_Pvsyst_2_month['Revenue_IE_POI'].multiply(self.df_Pvsyst_2_month['%_days_month'], axis="index")
@@ -2874,15 +2896,15 @@
                                                                        self.df_perf)
             elif guarantee_id == 'SCEG':
                 self.df_perf, guarantee_result = perf.SCEG_performance_guarantee(self.project_name,
                                                                        self.df,
                                                                        self.df_Pvsyst,
                                                                        self.PIS_date,
                                                                        self.df_perf,
-                                                                       data_platform=self.data_platform)
+                                                                       data_source=self.data_source)
             elif guarantee_id == "Regions_OPR":
                 guarantee_input = pd.to_datetime(self.df_proj_keys['Guarantee_input'])
                 self.df_perf, guarantee_result = perf.Regions_performance_guarantee(self.df,
                                                                           self.df_month_2,
                                                                           self.df_Pvsyst,
                                                                           self.df_Pvsyst_2_month,
                                                                           guarantee_input,
@@ -2991,26 +3013,27 @@
         self.df_Pvsyst_2['NREL_Weather_Adj_Kwh'] = self.df_Pvsyst_2['NREL_Weather_Adj_days_%'].multiply(
             self.df_Pvsyst_2['Year 0 Actual Production (kWh)'])
 
         # Added flat payments/fees
         self.df_Pvsyst_2['NREL_Weather_Adj_Kwh_$'] = \
             self.df_Pvsyst_2['NREL_Weather_Adj_Kwh'].multiply(self.df_Pvsyst_2['Rates'], axis="index") + self.df_Pvsyst_2['Flat']
 
+        rates_ytd = self.rates_year['Rates'][self.df.index[0]:self.df.index[-1]]
         if self.normal_rate_flag:  # are you using normal 3 price rate, or custom 8760 rate?
             self.table_gen = \
-                rate_table.generate_table_variable_by_rev_schedule_v02(self.rates_year_i,
+                rate_table.generate_table_variable_by_rev_schedule_v02(rates_ytd,
                                                             self.df,
                                                             'POI_kWH',
                                                             self.df_Pvsyst_2,
                                                             'NREL_Weather_Adj_Kwh',
                                                             self.df_config,
                                                             self.df_month_2,
                                                             self.df_Pvsyst_2_month)
             self.table_rev = \
-                rate_table.generate_table_variable_by_rev_schedule_v02(self.rates_year_i,
+                rate_table.generate_table_variable_by_rev_schedule_v02(rates_ytd,
                                                             self.df,
                                                             'POI_rev',
                                                             self.df_Pvsyst_2,
                                                             'NREL_Weather_Adj_Kwh_$',
                                                             self.df_config,
                                                             self.df_month_2,
                                                             self.df_Pvsyst_2_month)
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/session.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,17 @@
 from ccrenew import (
     __version__,
     ccr,
     all_df_keys,
     ListLike
 )
 from ccrenew.dashboard import (
-    DataPlatformDirs,
+    DataSourceDirs,
     func_timer,
-    get_modified_time,
-    make_s3_filepath
+    get_modified_time
 )
 from ccrenew.dashboard import Plotter
 from ccrenew.dashboard.project import Project
 from ccrenew.dashboard.utils.df_tools import df_update_join
 import ccrenew.dashboard.utils.dashboard_utils as utils
 import ccrenew.dashboard.utils.project_neighbors as neighbs
 
@@ -52,15 +51,14 @@
 
 # suppress warnings about "A value is trying to be set on a copy of a slice from a DataFrame."
 pd.set_option('mode.chained_assignment', None)
 
 # Initialize logger
 # Get logging configuration from the logging.conf file in the same directory as this file
 username = os.getenv('username')
-dashboard_folder = ccr.file_project
 # log_filename = '{}_dashboard-{}.log'.format(datetime.now().strftime('%Y-%m-%d_%H-%M-%S'), username)
 # log_config = os.path.join(dashboard_folder, 'Python_Functions', 'logging.conf')
 # log_file = os.path.join(dashboard_folder, 'Python_Functions', '_old', 'logs', log_filename)
 # LOGGING_CONFIG = get_logging_config(log_file)
 # logging.config.dictConfig(LOGGING_CONFIG)
 
 # Create logger
@@ -82,26 +80,26 @@
 
     
 class DashboardSession:
     """Main orchestrator for processing, plotting, and exporting data for projects (i.e. sites).
 
     Args:
         project_list (str or list): List of [Projects][ccrenew.dashboard.project.Project] to initialize when initializing the session.
-        data_cutoff_date (str or datetime, optional): The last date you want to analyze. Defaults to the current date the dashboard is being run.
-        data_source (str, optional): The location where project data is stored.
-            Default is current year Sharepoint data. To pull S3 data add 's3' to the input. See below for examples.
+        data_cutoff_date (str or datetime): The last date you want to analyze. Defaults to the current date the dashboard is being run.
+        year (int or None): The production year for the Project. Defaults to current year.
+        data_source (str or None): Location of source data files.
         
     `data_source` examples:
     
-    | data_source      | Explanation                  |
-    |------------------|------------------------------|
-    | `None`           | Current year Sharepoint data |
-    | `'s3'`           | Current year S3 data         |
-    | `'2022_data_'`   | 2022 Sharepoint data         |
-    | `'2022_data_s3'` | 2022 S3 data                 |
+    | data_source      | Explanation                                                           |
+    |------------------|-----------------------------------------------------------------------|
+    | `None`           | S3 data mounted to local machine's D: drive                           |
+    | `'local'`        | S3 data mounted to local machine's D: drive                           |
+    | `'s3'`           | S3 data remote connection                                             |
+    | `'sharepoint'`   | Sharepoint data located in each user's `_Dashboard_Project` directory |
     """
 
     # Instantiate globals as class variables
     df_keys = all_df_keys.copy()
     __version__ = __version__
 
     print('Pulling diagnostic comments from Smartsheets...')
@@ -131,15 +129,15 @@
     """Projects with AC batteries."""
     battery_dc_sites: list
     """Projects with DC batteries."""
     tracker_sites: list
     """Projects with tracker-type racking."""
 
     def __init__(self, project_list:str|ListLike|None=None, data_cutoff_date:str|datetime|None=None,
-                 data_source:str|None=None, **kwargs):
+                 year:int|None=None, data_source:str='local', **kwargs):
 
         print('Initializing DashboardSession...')
         
         # Initialize a dict to store projects - key = project name; value = project object
         # utils.project_dict() overrides the __repr__ method of dict to pretty print the projects when you call it
         self.project_list = utils.project_dict()
 
@@ -155,51 +153,51 @@
             try:
                 self.data_cutoff_date = parser.parse(data_cutoff_date) # type: ignore
             except:
                 self.data_cutoff_date = datetime.today()
         else:
             self.data_cutoff_date = datetime.today()
 
-        def set_data_source(data_source:str|None) -> None:
-            if data_source:
-                self.data_source = data_source
-            else:
-                self.data_source = f"{datetime.now().year}_data_"
-
-        self.data_platform_dirs = DataPlatformDirs(ccr.file_project,
-                                                   's3://cypress-perfeng-datalake-dev-us-west-2/Raw/HourlyResolution/')
+        # Set the year
+        if year:
+            self.year = year
+        else:
+            self.year = datetime.today().year
 
-        set_data_source(data_source)
-        if 's3' in self.data_source.lower():
-            data_source = self.data_source.replace(' ', '').replace('s3', '')
-            set_data_source(data_source)
-            self.dashboard_dir = self.data_platform_dirs.s3
-            self.data_platform = 's3'
+        # Set data source & dashboard directory for the session
+        if data_source:
+            self.data_source = data_source
         else:
-            self.dashboard_dir = self.data_platform_dirs.sharepoint
-            self.data_platform = 'sharepoint'
+            self.data_source = 'local'
+
+        self.data_source_dirs = {'local': 'D:\\Raw\\HourlyResolution',
+                                 's3': 's3://cypress-perfeng-datalake-dev-us-west-2/Raw/HourlyResolution/',
+                                 'sharepoint': ccr.file_project}
+
+        self.dashboard_dir = self.data_source_dirs[self.data_source]
 
         # Get snow dataframe
-        self.raw_snow_df, self.snow_file = utils.get_snow_df(dashboard_folder, self.data_source, file_format='csv', data_platform=self.data_platform)
+        self.raw_snow_df, self.snow_file = utils.get_snow_df(dashboard_dir=self.dashboard_dir, year=self.year,
+                                                             file_format='csv', data_source=self.data_source)
 
         # Create list for projects that have errored out
         self.errored_projects = {}
 
         # List of plotter objects for different projects
         self.plotters = {}
 
         # Type annotations & docstrings for documentation
         self.project_list: dict
         """List of [Projects][ccrenew.dashboard.project.Project] that
         have been initialized & added to the
         [DashboardSession][ccrenew.dashboard.session.DashboardSession] instance."""
-        self.data_platform: str
-        """Backend architecture of the source data for a project. Either `s3` or `sharepoint`."""
+        self.year: int
+        """Production year to analyze."""
         self.data_source: str
-        """Location of the source data for projects based on production year."""
+        """Location of the source data for projects."""
         self.raw_snow_df: pd.DataFrame
         """Snow data."""
         self.data_cutoff_date: datetime
         """Last day to process data."""
         self.errored_projects: dict
         """List of [Projects][ccrenew.dashboard.project.Project] that have encountered
         errors while processing & their error messages."""
@@ -329,16 +327,17 @@
         
         proj_init_dict = {}
         proj_init_dict['project_name'] = project_name
         proj_init_dict['df_proj_keys'] = df_proj_keys
         proj_init_dict['df_proj_ss_comments'] = df_proj_ss_comments
         proj_init_dict['dashboard_dir'] = self.dashboard_dir
         proj_init_dict['data_cutoff_date'] = self.data_cutoff_date
-        proj_init_dict['data_platform'] = self.data_platform
-        proj_init_dict['data_platform_dirs'] = self.data_platform_dirs
+        proj_init_dict['year'] = self.year
+        proj_init_dict['data_source'] = self.data_source
+        proj_init_dict['data_source_dirs'] = self.data_source_dirs
         proj_init_dict['data_source'] = self.data_source
         proj_init_dict['report_type'] = report_type
         proj_init_dict['Battery_AC_site'] = Battery_AC_site
         proj_init_dict['Battery_DC_site'] = Battery_DC_site
         proj_init_dict['Tracker_site'] = Tracker_site
         proj_init_dict['raw_snow_df'] = self.raw_snow_df
         proj_init_dict['snow_file'] = self.snow_file
@@ -387,22 +386,22 @@
         
         return neighbor_list
 
 
     def _source_file_updates(self, project:Project, reprocess:bool) -> bool:
         # Pull the last updated dates from the filesystem for the config, bool, & Powertrack files
         try:
-            last_update_config_file = get_modified_time(project.config_filepath, self.data_platform, 'file')
-            last_update_bool_file = get_modified_time(project.bool_filepath, self.data_platform, 'file')
-            last_update_powertrack_file = get_modified_time(project.powertrack_filepath, self.data_platform, 'file')
+            last_update_config_file = get_modified_time(project.config_filepath, self.data_source, 'file')
+            last_update_bool_file = get_modified_time(project.bool_filepath, self.data_source, 'file')
+            last_update_powertrack_file = get_modified_time(project.powertrack_filepath, self.data_source, 'file')
         except:
             self.__update_project_filepaths(project)
-            last_update_config_file = get_modified_time(project.config_filepath, self.data_platform, 'file')
-            last_update_bool_file = get_modified_time(project.bool_filepath, self.data_platform, 'file')
-            last_update_powertrack_file = get_modified_time(project.powertrack_filepath, self.data_platform, 'file')
+            last_update_config_file = get_modified_time(project.config_filepath, self.data_source, 'file')
+            last_update_bool_file = get_modified_time(project.bool_filepath, self.data_source, 'file')
+            last_update_powertrack_file = get_modified_time(project.powertrack_filepath, self.data_source, 'file')
 
         # Check if the config, bool, or Powertrack files have been updated.
         # If not we don't need to process.
         if reprocess:
             project.last_update_config = datetime.fromtimestamp(0)
             project.last_update_bool = datetime.fromtimestamp(0)
             project.last_update_powertrack = datetime.fromtimestamp(0)
@@ -573,15 +572,15 @@
                     # We'll use half of the available processors for the machine to not completely bog it down.
                     max_workers = int(os.cpu_count()/2) # type: ignore
                     print(f"Processing {len(project_list)} projects with {min(max_workers, len(project_list))} workers.")
                     print("Progress messages from workers will be suppressed in an interactive session.")
                     print("Projects will report success upon completion and may not complete in the order in which they were submitted.")
 
                     # Construct a dict of kwargs for each project to pass to `process_pool`
-                    if self.data_platform == 's3':
+                    if self.data_source == 's3':
                         data_source = self.data_source + 's3'
                     else:
                         data_source = self.data_source
 
                     kwargslist =  [{"project_name": project_name,
                                     "session": DashboardSession,
                                     "data_source": data_source,
@@ -766,15 +765,15 @@
                     # We'll use half of the available processors for the machine to not completely bog it down.
                     max_workers = int(os.cpu_count()/2) # type: ignore
                     print(f"Exporting {len(project_list)} projects with {min(max_workers, len(project_list))} workers.")
                     print("Progress messages from workers will be suppressed in an interactive session.")
                     print("Projects will report success upon completion and may not complete in the order in which they were submitted.")
 
                     # Construct a dict of kwargs for each project to pass to `process_pool`
-                    if self.data_platform == 's3':
+                    if self.data_source == 's3':
                         data_source = self.data_source + 's3'
                     else:
                         data_source = self.data_source
 
                     kwargslist =  [{"project_name": project_name,
                                     "session": DashboardSession,
                                     "data_source": data_source,
@@ -925,15 +924,15 @@
                                   project_name,
                                   'Pickle_Jar')
         
         pickle_name = utils.picklefy_project_name(project_name)
         pickle_file = year + "_" + pickle_name + ".pickle"
         pickle_path = os.path.join(pickle_jar, pickle_file)
         
-        if self.data_platform == 's3':
+        if self.data_source == 's3':
             pickle_path = Path(pickle_path).as_posix().replace('s3:/', 's3://')
             fs = s3fs.S3FileSystem()
             open = fs.open
         else:
             open = builtins.open
 
         with open(pickle_path, 'rb') as f:
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/utils/dashboard_utils.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/dashboard_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,29 +69,31 @@
         str: The picklefied project name.
     """
     project_name = re.sub(r"(,\s)|[,\s]", "_", project_name)
     project_name = re.sub(r"[']", "", project_name)
 
     return project_name
 
-def get_snow_df(dashboard_folder, data_source, file_format, data_platform):
-    """Pulls snow data & returns a dataframe. Temporary fix for now, need to
+def get_snow_df(dashboard_dir, year, file_format, data_source):
+    """
+    Pulls snow data & returns a dataframe. Temporary fix for now, need to
     update path references
 
     Returns:
         DataFrame: Snow data
     """
+    file_prefix = f"{year}_data_"
     if file_format == 'xlsx':
-        snow_file = Path(dashboard_folder) / 'Python_Functions' / 'Snow Losses' / f'{data_source}Operating-States-snowfall.xlsx'
-        if data_platform == 's3':
+        snow_file = Path(dashboard_dir) / 'Python_Functions' / 'Snow Losses' / f'{file_prefix}Operating-States-snowfall.xlsx'
+        if data_source == 's3':
             snow_file = snow_file.as_posix().replace('s3:/', 's3://')
         raw_snow_df = read_excel(snow_file, index_col=0)
     else:
-        snow_file = Path(dashboard_folder) / 'Python_Functions' / 'Snow Losses' / f'{data_source}Operating-States-snowfall.csv'
-        if data_platform == 's3':
+        snow_file = Path(dashboard_dir) / 'Python_Functions' / 'Snow Losses' / f'{file_prefix}Operating-States-snowfall.csv'
+        if data_source == 's3':
             snow_file = snow_file.as_posix().replace('s3:/', 's3://')
         raw_snow_df = read_csv(snow_file, index_col=0)
 
     return raw_snow_df, snow_file
 
 def retrieve_s3_df(bucket, key):
 # helper function to get data from s3
```

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/utils/df_tools.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/df_tools.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/utils/logging_conf.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/logging_conf.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/dashboard/utils/project_neighbors.py` & `ccrenew-0.2.1b0/src/ccrenew/dashboard/utils/project_neighbors.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/data_determination.py` & `ccrenew-0.2.1b0/src/ccrenew/data_determination.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew/pvmodel/project_model.py` & `ccrenew-0.2.1b0/src/ccrenew/pvmodel/project_model.py`

 * *Files identical despite different names*

### Comparing `ccrenew-0.2.1/src/ccrenew.egg-info/SOURCES.txt` & `ccrenew-0.2.1b0/src/ccrenew.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 src/ccrenew/dashboard/plotting/plots.py
 src/ccrenew/dashboard/utils/__init__.py
 src/ccrenew/dashboard/utils/dashboard_utils.py
 src/ccrenew/dashboard/utils/df_tools.py
 src/ccrenew/dashboard/utils/logging_conf.py
 src/ccrenew/dashboard/utils/project_neighbors.py
 src/ccrenew/pvmodel/__init__.py
-src/ccrenew/pvmodel/project_model.py
+src/ccrenew/pvmodel/project_model.py
+src/ccrenew/tst_pkg/__init__.py
+src/ccrenew/tst_pkg/tst.py
```

