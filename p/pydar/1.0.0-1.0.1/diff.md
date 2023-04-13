# Comparing `tmp/pydar-1.0.0.tar.gz` & `tmp/pydar-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydar-1.0.0.tar", last modified: Tue Apr 11 21:00:05 2023, max compression
+gzip compressed data, was "dist/pydar-1.0.1.tar", last modified: Thu Apr 13 21:16:43 2023, max compression
```

## Comparing `pydar-1.0.0.tar` & `pydar-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.238731 pydar-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-01-04 06:11:53.000000 pydar-1.0.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    49553 2023-04-11 21:00:05.238731 pydar-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    42653 2023-04-11 20:30:20.000000 pydar-1.0.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.222731 pydar-1.0.0/pydar/
--rw-rw-r--   0 user      (1000) user      (1000)     2345 2023-03-25 01:17:08.000000 pydar-1.0.0/pydar/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.226731 pydar-1.0.0/pydar/data/
--rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-01-01 06:47:05.000000 pydar-1.0.0/pydar/data/cassini_flyby.csv
--rw-rw-r--   0 user      (1000) user      (1000)    15662 2023-02-19 01:03:57.000000 pydar-1.0.0/pydar/data/coradr_jpl_options.csv
--rw-rw-r--   0 user      (1000) user      (1000)    30062 2023-02-19 01:20:45.000000 pydar-1.0.0/pydar/data/feature_name_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)    36144 2023-01-13 02:14:43.000000 pydar-1.0.0/pydar/data/sar_swath_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)   545452 2023-02-19 01:17:22.000000 pydar-1.0.0/pydar/data/swath_coverage_by_time_position.csv
--rw-rw-r--   0 user      (1000) user      (1000)     1774 2023-03-29 19:49:01.000000 pydar-1.0.0/pydar/display_image.py
--rw-rw-r--   0 user      (1000) user      (1000)    19293 2023-03-29 05:23:48.000000 pydar-1.0.0/pydar/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    15941 2023-04-11 20:17:28.000000 pydar-1.0.0/pydar/extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-03-29 22:21:31.000000 pydar-1.0.0/pydar/pydar_testing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.238731 pydar-1.0.0/pydar/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     1425 2023-04-11 20:25:57.000000 pydar-1.0.0/pydar/pytests/test_extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)    12401 2023-03-25 01:33:08.000000 pydar-1.0.0/pydar/read_readme.py
--rw-rw-r--   0 user      (1000) user      (1000)    14316 2023-03-21 20:58:40.000000 pydar-1.0.0/pydar/retrieve_ids_by_time_position.py
--rw-rw-r--   0 user      (1000) user      (1000)     4081 2023-03-18 07:53:32.000000 pydar-1.0.0/pydar/retrieve_supplementary_backplanes.py
--rw-rw-r--   0 user      (1000) user      (1000)    12251 2023-02-25 05:04:59.000000 pydar-1.0.0/pydar/sbdr_make_shapefile.py
--rw-rw-r--   0 user      (1000) user      (1000)      969 2023-02-18 06:42:56.000000 pydar-1.0.0/pydar/test_bearing_correction.py
--rw-rw-r--   0 user      (1000) user      (1000)     3021 2023-03-21 20:49:44.000000 pydar-1.0.0/pydar/updateCsvCORADARJPLOptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     4075 2023-03-21 20:49:20.000000 pydar-1.0.0/pydar/updateCsvFeatureNameDetails.py
--rw-rw-r--   0 user      (1000) user      (1000)     5609 2023-03-21 20:48:33.000000 pydar-1.0.0/pydar/updateCsvSwathCoverage.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.222731 pydar-1.0.0/pydar.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    49553 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      792 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      132 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-11 21:00:05.238731 pydar-1.0.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1669 2023-03-29 20:59:27.000000 pydar-1.0.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.188861 pydar-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2023-01-04 06:11:53.000000 pydar-1.0.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    49602 2023-04-13 21:16:43.188861 pydar-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    42710 2023-04-13 21:12:32.000000 pydar-1.0.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.180862 pydar-1.0.1/pydar/
+-rw-rw-r--   0 user      (1000) user      (1000)     2345 2023-03-25 01:17:08.000000 pydar-1.0.1/pydar/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.188861 pydar-1.0.1/pydar/data/
+-rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-01-01 06:47:05.000000 pydar-1.0.1/pydar/data/cassini_flyby.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    15662 2023-02-19 01:03:57.000000 pydar-1.0.1/pydar/data/coradr_jpl_options.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    30062 2023-02-19 01:20:45.000000 pydar-1.0.1/pydar/data/feature_name_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    36144 2023-01-13 02:14:43.000000 pydar-1.0.1/pydar/data/sar_swath_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)   545452 2023-02-19 01:17:22.000000 pydar-1.0.1/pydar/data/swath_coverage_by_time_position.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2023-03-29 19:49:01.000000 pydar-1.0.1/pydar/display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20504 2023-04-13 20:28:45.000000 pydar-1.0.1/pydar/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15942 2023-04-12 19:20:45.000000 pydar-1.0.1/pydar/extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2023-03-29 22:21:31.000000 pydar-1.0.1/pydar/pydar_testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.188861 pydar-1.0.1/pydar/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     4488 2023-04-13 20:31:01.000000 pydar-1.0.1/pydar/pytests/test_display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14238 2023-04-13 20:14:27.000000 pydar-1.0.1/pydar/pytests/test_extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9129 2023-04-13 21:00:32.000000 pydar-1.0.1/pydar/pytests/test_read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32985 2023-04-13 21:11:44.000000 pydar-1.0.1/pydar/pytests/test_retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12401 2023-04-13 01:01:16.000000 pydar-1.0.1/pydar/read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14306 2023-04-13 03:32:41.000000 pydar-1.0.1/pydar/retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4081 2023-03-18 07:53:32.000000 pydar-1.0.1/pydar/retrieve_supplementary_backplanes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12251 2023-02-25 05:04:59.000000 pydar-1.0.1/pydar/sbdr_make_shapefile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      969 2023-02-18 06:42:56.000000 pydar-1.0.1/pydar/test_bearing_correction.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3021 2023-03-21 20:49:44.000000 pydar-1.0.1/pydar/updateCsvCORADARJPLOptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4075 2023-03-21 20:49:20.000000 pydar-1.0.1/pydar/updateCsvFeatureNameDetails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5609 2023-03-21 20:48:33.000000 pydar-1.0.1/pydar/updateCsvSwathCoverage.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-13 21:16:43.184862 pydar-1.0.1/pydar.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    49602 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      914 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-13 21:16:43.000000 pydar-1.0.1/pydar.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-13 21:16:43.188861 pydar-1.0.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1669 2023-04-13 20:45:18.000000 pydar-1.0.1/setup.py
```

### Comparing `pydar-1.0.0/PKG-INFO` & `pydar-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.1.tar.gz
 Description: # PYDAR
          <p align="center">
           <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/pydar)
         ![license](https://img.shields.io/pypi/l/pydar)
@@ -408,15 +408,14 @@
         * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be less than or equal to the max_latitude, range from -90° to 90°
         * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be greater than or equal to the min_latitude, range from -90° to 90°
         * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
         * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude must be greater than or equal to the min_longitude, range from 0° to 360°
         
         ```python
         import pydar
-        
         pydar.retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=-82,
         						max_latitude=-72,
         						min_longitude=183,
         						max_longitude=190)
         ```
         Output = `['Crveno Lacus', 'Ontario Lacus', 'Romo Planitia', 'Rossak Planitia', 'Saraswati Flumen']`
         
@@ -685,15 +684,15 @@
         
         ## Developer Notes TODO:
         ### TODO Code:
         * add a colored outline around a feature when displaying as a 2D image
         * save image pixel to an array
         * extract pdr functionality to reduce overhead
         * displayImages() bug fix: 87 displays invalid integer
-        * segments will be less than 99 (default to 1 - 01 is the primary imaging)
+        * segments will be less than 99 (default to 1 - 01 is the primary imaging) (requires segment_options = ['S01', 'S02', 'S03', 'S04'])
         * progress bars print to command line (still downloading...)
         * save .IMG as .SHP for ArcGIS
         
         ### TODO Questions:
         * add details for what a segment_num is
         * associate burst ID from SBDR data to BIDR data for metadata
         * save .IMG as an array of pixel values
```

### Comparing `pydar-1.0.0/README.md` & `pydar-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,14 @@
 * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be less than or equal to the max_latitude, range from -90° to 90°
 * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be greater than or equal to the min_latitude, range from -90° to 90°
 * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
 * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude must be greater than or equal to the min_longitude, range from 0° to 360°
 
 ```python
 import pydar
-
 pydar.retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=-82,
 						max_latitude=-72,
 						min_longitude=183,
 						max_longitude=190)
 ```
 Output = `['Crveno Lacus', 'Ontario Lacus', 'Romo Planitia', 'Rossak Planitia', 'Saraswati Flumen']`
 
@@ -677,15 +676,15 @@
 
 ## Developer Notes TODO:
 ### TODO Code:
 * add a colored outline around a feature when displaying as a 2D image
 * save image pixel to an array
 * extract pdr functionality to reduce overhead
 * displayImages() bug fix: 87 displays invalid integer
-* segments will be less than 99 (default to 1 - 01 is the primary imaging)
+* segments will be less than 99 (default to 1 - 01 is the primary imaging) (requires segment_options = ['S01', 'S02', 'S03', 'S04'])
 * progress bars print to command line (still downloading...)
 * save .IMG as .SHP for ArcGIS
 
 ### TODO Questions:
 * add details for what a segment_num is
 * associate burst ID from SBDR data to BIDR data for metadata
 * save .IMG as an array of pixel values
```

### Comparing `pydar-1.0.0/pydar/__init__.py` & `pydar-1.0.1/pydar/__init__.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/data/cassini_flyby.csv` & `pydar-1.0.1/pydar/data/cassini_flyby.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/data/coradr_jpl_options.csv` & `pydar-1.0.1/pydar/data/coradr_jpl_options.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/data/feature_name_details.csv` & `pydar-1.0.1/pydar/data/feature_name_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/data/sar_swath_details.csv` & `pydar-1.0.1/pydar/data/sar_swath_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/data/swath_coverage_by_time_position.csv` & `pydar-1.0.1/pydar/data/swath_coverage_by_time_position.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/display_image.py` & `pydar-1.0.1/pydar/display_image.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/error_handling.py` & `pydar-1.0.1/pydar/error_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 	if flyby_observation_num is not None and flyby_id is not None:
 		logger.critical("\nCRITICAL ERROR: Requires either a flyby_observation_num OR flyby_id, not both.")
 		exit()
 
 	if flyby_id is not None:
 		if type(flyby_id) != str:
-			logger.critical("\nCRITICAL ERROR, [flyby_observation_num]: Must be a str, current type = '{0}'".format(type(flyby_id)))
+			logger.critical("\nCRITICAL ERROR, [flyby_id]: Must be a str, current type = '{0}'".format(type(flyby_id)))
 			exit()
 		if flyby_id not in available_flyby_id:
 			logger.critical("\nCRITICAL ERROR, [flyby_id]: '{0}' not in available ids options '{1}'".format(flyby_id, available_flyby_id))
 			exit()
 
 	if flyby_observation_num is not None:
 		if type(flyby_observation_num) != str:
@@ -61,14 +61,15 @@
 		exit()
 	if segment_num not in segment_options:
 		logger.critical("\nCRITICAL ERROR, [segment_num]: '{0}' not an available segment option '{1}'".format(segment_num, segment_options))
 		exit()
 
 	if len(additional_data_types_to_download) != 0:
 		logger.critical("\nINFO [additional_data_types_to_download]: Current v1 behavior does not support additional_data_types_to_download, so no additional files will be included in the download")
+		"""
 		if type(additional_data_types_to_download) != list:
 			logger.critical("\nCRITICAL ERROR [additional_data_types_to_download]: Must be a list, current type = '{0}'".format(type(additional_data_types_to_download)))
 			exit()
 		for data_type in additional_data_types_to_download:
 			if type(data_type) != str:
 				logger.critical("\nCRITICAL ERROR [additional_data_types_to_download]: All data types should be strings, but '{0}' current type = '{0}'".format(data_type, type(data_type)))
 
@@ -91,18 +92,15 @@
 			if row_bool is True:
 				coradr_data_types.append(pydar.datafile_types_columns[i])
 
 		for data_type in additional_data_types_to_download:
 			if data_type not in coradr_data_types:
 				logger.critical("\nCRITICAL ERROR [additional_data_types_to_download]: Data type '{0}' not available in {1}".format(data_type, coradr_data_types))
 				exit()
-
-	if resolution is not None and top_x_resolutions is not None:
-		logger.critical("\nCRITICAL ERROR: Requires either a resolution OR a top_x_resolutions, not both")
-		exit()
+		"""
 
 	if resolution is not None :
 		if type(resolution) != str:
 			logger.critical("\nCRITICAL ERROR, [resolution]: Must be a str, current type = '{0}'".format(type(resolution)))
 			exit()
 		if resolution not in pydar.resolution_types:
 			logger.critical("\nCRITICAL ERROR, [resolution]: resolution '{0}' must be a valid resolution type in {1}".format(resolution, pydar.resolution_types))
@@ -170,94 +168,134 @@
 		exit()
 	else:
 		if type(image_directory) != str:
 			logger.critical("\nCRITICAL ERROR, [image_directory]: Must be a str, current type = '{0}'".format(type(image_directory)))
 			exit()
 
 	if fig_title is not None and type(fig_title) != str:
-		logger.critical("\nCRITICAL ERROR, [fig_title]: Must be a int, current type = '{0}'".format(type(fig_title)))
+		logger.critical("\nCRITICAL ERROR, [fig_title]: Must be a str, current type = '{0}'".format(type(fig_title)))
 		exit()
 
 	if type(figsize_n) != int:
 		logger.critical("\nCRITICAL ERROR, [figsize_n]: Must be a int, current type = '{0}'".format(type(figsize_n)))
 		exit()
+	else:
+		if figsize_n < 1:
+			logger.critical("\nCRITICAL ERROR, [figsize_n]: figsize_n must be greater than 1, current value = '{0}'".format(figsize_n))
+			exit()
 
 	if type(fig_dpi) != int:
 		logger.critical("\nCRITICAL ERROR, [fig_dpi]: Must be a int, current type = '{0}'".format(type(fig_dpi)))
 		exit()
+	else:
+		if fig_dpi < 1:
+			logger.critical("\nCRITICAL ERROR, [fig_dpi]: fig_dpi must be greater than 1, current value = '{0}'".format(fig_dpi))
+			exit()
 
 def errorHandlingREADME(coradr_results_directory=None,
 						section_to_print=None,
 						print_to_console=True):
 	# Error Handling for README options: read_readme
-	if type(coradr_results_directory) != str:
-		logger.critical("\nCRITICAL ERROR, [coradr_results_directory]: Must be a str, current type = '{0}'".format(type(coradr_results_directory)))
+	if coradr_results_directory is None:
+		logger.critical("\nCRITICAL ERROR, [coradr_results_directory]: coradr_results_directory is required")
 		exit()
+	else:
+		if type(coradr_results_directory) != str:
+			logger.critical("\nCRITICAL ERROR, [coradr_results_directory]: Must be a str, current type = '{0}'".format(type(coradr_results_directory)))
+			exit()
 
-	if type(section_to_print) != str:
+	if section_to_print is not None and type(section_to_print) != str:
 		logger.critical("\nCRITICAL ERROR, [section_to_print]: Must be a str, current type = '{0}'".format(type(section_to_print)))
 		exit()
 
 	if type(print_to_console) != bool:
 		logger.critical("\nCRITICAL ERROR, [print_to_console]: Must be a bool, current type = '{0}'".format(type(print_to_console)))
 		exit()
 
 def errorHandlingRetrieveIDSByFeature(feature_name=None):
 	# Error Handling for retrieving the IDs for a specific feature name: retrieveIDSByFeature()
-	if type(feature_name) != str:
-		logger.critical("\nCRITICAL ERROR, [feature_name]: Must be a str, current type = '{0}'".format(type(feature_name)))
+	if feature_name is None:
+		logger.critical("\nCRITICAL ERROR, [feature_name]: feature_name is required")
 		exit()
+	else:
+		if type(feature_name) != str:
+			logger.critical("\nCRITICAL ERROR, [feature_name]: Must be a str, current type = '{0}'".format(type(feature_name)))
+			exit()
 
 def errorHandlingRetrieveIDSByLatitudeLongitude(latitude=None,
 												longitude=None):
 	# Error Handling for retrieving IDs based on latitude and longitude
+
+	if latitude is None:
+		logger.critical("\nCRITICAL ERROR, [latitude]: latitude is required")
+		exit()
+
 	if type(latitude) != float and type(latitude) != int:
 		logger.critical("\nCRITICAL ERROR, [latitude]: Must be a float or int, current type = '{0}'".format(type(latitude)))
 		exit()
 
 	if latitude > 90 or latitude < -90:
 		logger.critical("\nCRITICAL ERROR, [latitude]: Latitude must be between 90 and -90, current value = '{0}'".format(latitude))
 		exit()
 
+	if longitude is None:
+		logger.critical("\nCRITICAL ERROR, [longitude]: longitude is required")
+		exit()
 	if type(longitude) != float and type(longitude) != int:
 		logger.critical("\nCRITICAL ERROR, [longitude]: Must be a float or int, current type = '{0}'".format(type(longitude)))
 		exit()
 
 	if longitude < 0 or longitude > 360:
 		logger.critical("\nCRITICAL ERROR, [longitude]: Longitude must be between 0 and 360, current value = '{0}'".format(longitude))
 		exit()
 
 def errorHandlingRetrieveIDSByLatitudeLongitudeRange(min_latitude=None,
-												max_latitude=None,
-												min_longitude=None,
-												max_longitude=None):
+													max_latitude=None,
+													min_longitude=None,
+													max_longitude=None):
 	# Error Handling for retrieving IDs based on a range of latitude and longitudes
-	if type(min_latitude) != float and type(min_latitude) != int:
-		logger.critical("\nCRITICAL ERROR, [min_latitude]: Must be a float or int, current type = '{0}'".format(type(min_latitude)))
+	if min_latitude is None:
+		logger.critical("\nCRITICAL ERROR, [min_latitude]: min_latitude is required")
 		exit()
+	else:
+		if type(min_latitude) != float and type(min_latitude) != int:
+			logger.critical("\nCRITICAL ERROR, [min_latitude]: Must be a float or int, current type = '{0}'".format(type(min_latitude)))
+			exit()
 
-	if type(max_latitude) != float and type(max_latitude) != int:
-		logger.critical("\nCRITICAL ERROR, [max_latitude]: Must be a float or int, current type = '{0}'".format(type(max_latitude)))
+	if max_latitude is None:
+		logger.critical("\nCRITICAL ERROR, [max_latitude]: max_latitude is required")
 		exit()
+	else:
+		if type(max_latitude) != float and type(max_latitude) != int:
+			logger.critical("\nCRITICAL ERROR, [max_latitude]: Must be a float or int, current type = '{0}'".format(type(max_latitude)))
+			exit()
 
 	if min_latitude > 90 or min_latitude < -90:
 		logger.critical("\nCRITICAL ERROR, [min_latitude]: Latitude must be between 90 and -90, current value = '{0}'".format(min_latitude))
 		exit()
 
 	if max_latitude > 90 or max_latitude < -90:
 		logger.critical("\nCRITICAL ERROR, [max_latitude]: Latitude must be between 90 and -90, current value = '{0}'".format(max_latitude))
 		exit()
 
-	if type(min_longitude) != float and type(min_longitude) != int:
-		logger.critical("\nCRITICAL ERROR, [min_longitude]: Must be a float or int, current type = '{0}'".format(type(min_longitude)))
+	if min_longitude is None:
+		logger.critical("\nCRITICAL ERROR, [min_longitude]: min_longitude is required")
 		exit()
+	else:
+		if type(min_longitude) != float and type(min_longitude) != int:
+			logger.critical("\nCRITICAL ERROR, [min_longitude]: Must be a float or int, current type = '{0}'".format(type(min_longitude)))
+			exit()
 
-	if type(max_longitude) != float and type(max_longitude) != int:
-		logger.critical("\nCRITICAL ERROR, [max_longtiude]: Must be a float or int, current type = '{0}'".format(type(max_longitude)))
+	if max_longitude is None:
+		logger.critical("\nCRITICAL ERROR, [max_longitude]: max_longitude is required")
 		exit()
+	else:
+		if type(max_longitude) != float and type(max_longitude) != int:
+			logger.critical("\nCRITICAL ERROR, [max_longitude]: Must be a float or int, current type = '{0}'".format(type(max_longitude)))
+			exit()
 
 	if min_longitude < 0 or min_longitude > 360:
 		logger.critical("\nCRITICAL ERROR, [min_longitude]: Longitude must be between 0 and 360, current value = '{0}'".format(min_longitude))
 		exit()
 
 	if max_longitude < 0 or max_longitude > 360:
 		logger.critical("\nCRITICAL ERROR, [max_longitude]: Longitude must be between 0 and 360, current value = '{0}'".format(max_longitude))
@@ -270,33 +308,35 @@
 	if max_longitude < min_longitude:
 		logger.critical("\nCRITICAL ERROR, [longitude]: max_longitude must be greater than min_longtiude")
 		exit()
 
 
 def errorHandlingRetrieveIDSByTime(year=None, doy=None, hour=None, minute=None, second=None, millisecond=None):
 	# Error handling for retrieving IDs based on a specific time
-	if year == None:
+	if year is None:
 		logger.critical("\nCRITICAL ERROR, [year]: year is required")
 		exit()
-	if type(year) != int:
-		logger.critical("\nCRITICAL ERROR, [year]: Must be an int, current type = '{0}'".format(type(year)))
-		exit()
-	if year < 2004 or year > 2014:
-		logger.critical("\nCRITICAL ERROR, [year]: year must be between 2004-2014")
-		exit()
+	else:
+		if type(year) != int:
+			logger.critical("\nCRITICAL ERROR, [year]: Must be an int, current type = '{0}'".format(type(year)))
+			exit()
+		if year < 2004 or year > 2014:
+			logger.critical("\nCRITICAL ERROR, [year]: year must be between 2004-2014")
+			exit()
 
-	if doy == None:
+	if doy is None:
 		logger.critical("\nCRITICAL ERROR, [doy]: doy is required")
 		exit()
-	if type(doy) != int:
-		logger.critical("\nCRITICAL ERROR, [doy]: Must be an int, current type = '{0}'".format(type(doy)))
-		exit()
-	if doy < 0 or doy > 365:
-		logger.critical("\nCRITICAL ERROR, [doy]: doy must be between 0-365")
-		exit()
+	else:
+		if type(doy) != int:
+			logger.critical("\nCRITICAL ERROR, [doy]: Must be an int, current type = '{0}'".format(type(doy)))
+			exit()
+		if doy < 0 or doy > 365:
+			logger.critical("\nCRITICAL ERROR, [doy]: doy must be between 0-365")
+			exit()
 
 	if hour is not None:
 		if type(hour) != int:
 			logger.critical("\nCRITICAL ERROR, [hour]: Must be an int, current type = '{0}'".format(type(hour)))
 			exit()
 		if hour < 0 or hour > 23:
 			logger.critical("\nCRITICAL ERROR, [hour]: hour must be within UTC range between 0 to 23")
```

### Comparing `pydar-1.0.0/pydar/extract_flyby_parameters.py` & `pydar-1.0.1/pydar/extract_flyby_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
 	if flyby_id is not None and type(flyby_id) == str:
 		flyby_id = flyby_id.upper() # ensure that observation number set to capitalized 'T'
 	if flyby_observation_num is not None and type(flyby_observation_num) == str:
 		while len(flyby_observation_num) < 4:
 			flyby_observation_num = "0" + flyby_observation_num # set all radar take numbers to be four digits long: 229 -> 0229
 	if top_x_resolutions is not None:
-		logger.info("\nINFO: [top_x_resolutions] in use, overriding resolution '{0}' to save the top {1} resolutions".format(resolution, top_x_resolutions))
+		#logger.info("\nINFO: [top_x_resolutions] in use, overriding resolution '{0}' to save the top {1} resolutions".format(resolution, top_x_resolutions))
 		resolution = None # set default resolution to None if selecting the top x resolutions
 
 	# Error handling:
 	pydar.errorHandlingExtractFlybyDataImages(flyby_observation_num=flyby_observation_num,
 											flyby_id=flyby_id,
 											segment_num=segment_num,
 											additional_data_types_to_download=additional_data_types_to_download,
```

### Comparing `pydar-1.0.0/pydar/read_readme.py` & `pydar-1.0.1/pydar/read_readme.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/retrieve_ids_by_time_position.py` & `pydar-1.0.1/pydar/retrieve_ids_by_time_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,18 @@
 				if flyby not in flyby_ids.keys():
 					flyby_ids[flyby] = []
 				segment_number = "S0" + str(row["SEGMENT NUMBER"])
 				if segment_number not in flyby_ids[flyby]:
 					flyby_ids[flyby].append(segment_number)
 
 	if len(flyby_ids) == 0:
-		logger.info("\n[WARNING]: No Features found at latitude from {0} to {1} and longitude from {2} to {3} \n".format(min_latitude,
-																														max_latitude,
-																														min_longitude,
-																														max_longitude))
+		logger.info("\n[WARNING]: No IDs found at latitude from {0} to {1} and longitude from {2} to {3}\n".format(min_latitude,
+																													max_latitude,
+																													min_longitude,
+																													max_longitude))
 
 	return flyby_ids
 
 ### RETURN FLYBY IDS FOR A SPECIFIC TIME ###############################
 def retrieveIDSByTime(year=None, doy=None, hour=None, minute=None, second=None, millisecond=None):
 	# Retrieve Flyby IDs based on a single Timestamp of YYYY-DOYThh:mm:ss.sss
 	#	Returns a Dictionary of Flyby IDs and a list of their segment numbers
@@ -280,13 +280,13 @@
 		if twoRangesIntersect(min_feature_latitude, max_feature_latitude, min_latitude, max_latitude):
 			min_feature_longitude = min([float(position_dict["Westernmost Longitude"]), float(position_dict["Easternmost Longitude"])])
 			max_feature_longitude = max([float(position_dict["Westernmost Longitude"]), float(position_dict["Easternmost Longitude"])])
 			if twoRangesIntersect(min_feature_longitude, max_feature_longitude, min_longitude, max_longitude):
 				feature_names_list.append(feature_name)
 
 	if len(feature_names_list) == 0:
-		logger.info("\n[WARNING]: No Features found at latitude from {0} to {1} and longitude from {2} to {3} \n".format(min_latitude,
+		logger.info("\n[WARNING]: No Features found at latitude from {0} to {1} and longitude from {2} to {3}\n".format(min_latitude,
 																														max_latitude,
 																														min_longitude,
 																														max_longitude))
 
 	return feature_names_list
```

### Comparing `pydar-1.0.0/pydar/retrieve_supplementary_backplanes.py` & `pydar-1.0.1/pydar/retrieve_supplementary_backplanes.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/sbdr_make_shapefile.py` & `pydar-1.0.1/pydar/sbdr_make_shapefile.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/test_bearing_correction.py` & `pydar-1.0.1/pydar/test_bearing_correction.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/updateCsvCORADARJPLOptions.py` & `pydar-1.0.1/pydar/updateCsvCORADARJPLOptions.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/updateCsvFeatureNameDetails.py` & `pydar-1.0.1/pydar/updateCsvFeatureNameDetails.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar/updateCsvSwathCoverage.py` & `pydar-1.0.1/pydar/updateCsvSwathCoverage.py`

 * *Files identical despite different names*

### Comparing `pydar-1.0.0/pydar.egg-info/PKG-INFO` & `pydar-1.0.1/pydar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.1.tar.gz
 Description: # PYDAR
          <p align="center">
           <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/pydar)
         ![license](https://img.shields.io/pypi/l/pydar)
@@ -408,15 +408,14 @@
         * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be less than or equal to the max_latitude, range from -90° to 90°
         * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be greater than or equal to the min_latitude, range from -90° to 90°
         * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
         * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude must be greater than or equal to the min_longitude, range from 0° to 360°
         
         ```python
         import pydar
-        
         pydar.retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=-82,
         						max_latitude=-72,
         						min_longitude=183,
         						max_longitude=190)
         ```
         Output = `['Crveno Lacus', 'Ontario Lacus', 'Romo Planitia', 'Rossak Planitia', 'Saraswati Flumen']`
         
@@ -685,15 +684,15 @@
         
         ## Developer Notes TODO:
         ### TODO Code:
         * add a colored outline around a feature when displaying as a 2D image
         * save image pixel to an array
         * extract pdr functionality to reduce overhead
         * displayImages() bug fix: 87 displays invalid integer
-        * segments will be less than 99 (default to 1 - 01 is the primary imaging)
+        * segments will be less than 99 (default to 1 - 01 is the primary imaging) (requires segment_options = ['S01', 'S02', 'S03', 'S04'])
         * progress bars print to command line (still downloading...)
         * save .IMG as .SHP for ArcGIS
         
         ### TODO Questions:
         * add details for what a segment_num is
         * associate burst ID from SBDR data to BIDR data for metadata
         * save .IMG as an array of pixel values
```

### Comparing `pydar-1.0.0/setup.py` & `pydar-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.0.0"
+VERSION="1.0.1"
 DESCRIPTION="A Python package to access, download, view, and manipulate Cassini RADAR images"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="pydar",
```

