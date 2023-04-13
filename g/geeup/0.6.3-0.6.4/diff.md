# Comparing `tmp/geeup-0.6.3.tar.gz` & `tmp/geeup-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\geeup-0.6.3.tar", last modified: Tue Feb  7 15:39:20 2023, max compression
+gzip compressed data, was "dist\geeup-0.6.4.tar", last modified: Thu Apr 13 02:38:19 2023, max compression
```

## Comparing `geeup-0.6.3.tar` & `geeup-0.6.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 15:39:20.886381 geeup-0.6.3/
--rw-rw-rw-   0        0        0    30962 2023-02-07 15:39:20.885383 geeup-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0    25264 2023-02-04 18:59:09.000000 geeup-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 15:39:20.875380 geeup-0.6.3/geeup/
--rw-rw-rw-   0        0        0      119 2023-02-07 15:37:57.000000 geeup-0.6.3/geeup/__init__.py
--rw-rw-rw-   0        0        0       69 2020-06-18 02:06:06.000000 geeup-0.6.3/geeup/__main__.py
--rw-rw-rw-   0        0        0    17567 2023-02-04 18:34:10.000000 geeup-0.6.3/geeup/batch_uploader.py
--rw-rw-rw-   0        0        0    21857 2023-02-07 15:37:16.000000 geeup-0.6.3/geeup/geeup.py
--rw-rw-rw-   0        0        0     1504 2022-09-03 22:53:54.000000 geeup-0.6.3/geeup/getmeta.py
--rw-rw-rw-   0        0        0     3707 2021-04-16 00:02:09.000000 geeup-0.6.3/geeup/metadata_loader.py
--rw-rw-rw-   0        0        0    15888 2023-02-04 18:45:53.000000 geeup-0.6.3/geeup/tuploader.py
--rw-rw-rw-   0        0        0     2074 2022-05-26 04:04:00.000000 geeup-0.6.3/geeup/zipfiles.py
-drwxrwxrwx   0        0        0        0 2023-02-07 15:39:20.883390 geeup-0.6.3/geeup.egg-info/
--rw-rw-rw-   0        0        0    30962 2023-02-07 15:39:20.000000 geeup-0.6.3/geeup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-02-07 15:39:20.000000 geeup-0.6.3/geeup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 15:39:20.000000 geeup-0.6.3/geeup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-07 15:39:20.000000 geeup-0.6.3/geeup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      253 2023-02-07 15:39:20.000000 geeup-0.6.3/geeup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-07 15:39:20.000000 geeup-0.6.3/geeup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-07 15:39:20.886381 geeup-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1884 2023-02-07 15:37:42.000000 geeup-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:38:19.607045 geeup-0.6.4/
+-rw-rw-rw-   0        0        0    31128 2023-04-13 02:38:19.589545 geeup-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0    25398 2023-04-13 02:37:01.000000 geeup-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:38:19.522635 geeup-0.6.4/geeup/
+-rw-rw-rw-   0        0        0      119 2023-04-13 02:33:00.000000 geeup-0.6.4/geeup/__init__.py
+-rw-rw-rw-   0        0        0       69 2020-06-18 02:06:06.000000 geeup-0.6.4/geeup/__main__.py
+-rw-rw-rw-   0        0        0    17773 2023-04-13 02:23:25.000000 geeup-0.6.4/geeup/batch_uploader.py
+-rw-rw-rw-   0        0        0    22030 2023-04-13 02:22:21.000000 geeup-0.6.4/geeup/geeup.py
+-rw-rw-rw-   0        0        0     1504 2022-09-03 22:53:54.000000 geeup-0.6.4/geeup/getmeta.py
+-rw-rw-rw-   0        0        0     3707 2021-04-16 00:02:09.000000 geeup-0.6.4/geeup/metadata_loader.py
+-rw-rw-rw-   0        0        0    15888 2023-02-04 18:45:53.000000 geeup-0.6.4/geeup/tuploader.py
+-rw-rw-rw-   0        0        0     2074 2022-05-26 04:04:00.000000 geeup-0.6.4/geeup/zipfiles.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:38:19.582545 geeup-0.6.4/geeup.egg-info/
+-rw-rw-rw-   0        0        0    31128 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      253 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 02:38:18.000000 geeup-0.6.4/geeup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 02:38:19.607878 geeup-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1884 2023-04-13 02:33:22.000000 geeup-0.6.4/setup.py
```

### Comparing `geeup-0.6.3/PKG-INFO` & `geeup-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeup
-Version: 0.6.3
+Version: 0.6.4
 Summary: Simple Client for Earth Engine Uploads
 Home-page: https://github.com/samapriya/geeup
 Author: Samapriya Roy
 Author-email: samapriya.roy@gmail.com
 License: Apache 2.0
 Description: # geeup: Simple CLI for Earth Engine Uploads
         
@@ -266,14 +266,15 @@
           --dest DEST           Destination. Full path for upload to Google Earth Engine image collection, e.g. users/pinkiepie/myponycollection
           -m METADATA, --metadata METADATA
                                 Path to CSV with metadata.
           -u USER, --user USER  Google account name (gmail address).
         
         Optional named arguments:
           --nodata NODATA       The value to burn into the raster as NoData (missing data)
+          --mask MASK           Binary to use last band for mask True or False
           --pyramids PYRAMIDS   Pyramiding Policy, MEAN, MODE, MIN, MAX, SAMPLE
         ```
         
         Example setup would be
         
         ![gee_upload](https://user-images.githubusercontent.com/6677629/147895638-3d542ea5-2c72-43b7-8052-c5edef0ab717.gif)
         
@@ -343,14 +344,17 @@
         
         optional arguments:
           -h, --help  show this help message and exit
         ```
         
         # Changelog
         
+        ### 0.6.4
+        - Added masking option to use last band as mask
+        
         ### 0.6.2
         - Removed call to shell
         - Now prints status of task at task creation
         - Overwrite option for both images and tables
         
         ### 0.6.1
         - Removed dependency on pipwin uses pipgeo instead
```

### Comparing `geeup-0.6.3/README.md` & `geeup-0.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
   --dest DEST           Destination. Full path for upload to Google Earth Engine image collection, e.g. users/pinkiepie/myponycollection
   -m METADATA, --metadata METADATA
                         Path to CSV with metadata.
   -u USER, --user USER  Google account name (gmail address).
 
 Optional named arguments:
   --nodata NODATA       The value to burn into the raster as NoData (missing data)
+  --mask MASK           Binary to use last band for mask True or False
   --pyramids PYRAMIDS   Pyramiding Policy, MEAN, MODE, MIN, MAX, SAMPLE
 ```
 
 Example setup would be
 
 ![gee_upload](https://user-images.githubusercontent.com/6677629/147895638-3d542ea5-2c72-43b7-8052-c5edef0ab717.gif)
 
@@ -335,14 +336,17 @@
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 
 # Changelog
 
+### 0.6.4
+- Added masking option to use last band as mask
+
 ### 0.6.2
 - Removed call to shell
 - Now prints status of task at task creation
 - Overwrite option for both images and tables
 
 ### 0.6.1
 - Removed dependency on pipwin uses pipgeo instead
```

### Comparing `geeup-0.6.3/geeup/batch_uploader.py` & `geeup-0.6.4/geeup/batch_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         return "GEE file name & path cannot have spaces & can only have letters, numbers, hyphens and underscores"
 
 
 def upload(
     user,
     source_path,
     pyramiding,
+    mask,
     destination_path,
     metadata_path=None,
     nodata_value=None,
     overwrite=None,
 ):
     schema = {"collection_path": {
         "type": "string", "regex": "^[a-zA-Z0-9/_-]+$"}}
@@ -212,26 +213,30 @@
                             "name": asset_full_path,
                             "pyramidingPolicy": pyramidingPolicy,
                             "tilesets": [{"sources": [{"uris": gsid}]}],
                             "start_time": {"seconds": ""},
                             "end_time": {"seconds": ""},
                             "properties": j,
                             "missing_data": {"values": [nodata_value]},
+                            "maskBands": {"bandIds": [], "tilesetId": ''}
                         }
                         if start is not None:
                             main_payload["start_time"]["seconds"] = start
                         else:
                             main_payload.pop("start_time")
                         if end is not None:
                             main_payload["end_time"]["seconds"] = end
                         else:
                             main_payload.pop("end_time")
                         if nodata_value is None:
                             main_payload.pop("missing_data")
-                        # print(json.dumps(main_payload))
+                        if bool(mask) is False:
+                            main_payload.pop("maskBands")
+
+                        # print(json.dumps(main_payload, indent=2))
                         schema = {
                             "asset_path": {
                                 "type": "string",
                                 "regex": "^[a-zA-Z0-9/_-]+$",
                             }
                         }
                         asset_validate = {"asset_path": asset_full_path}
```

### Comparing `geeup-0.6.3/geeup/geeup.py` & `geeup-0.6.4/geeup/geeup.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
 def upload_from_parser(args):
     upload(
         user=args.user,
         source_path=args.source,
         destination_path=args.dest,
         metadata_path=args.metadata,
         nodata_value=args.nodata,
+        mask=args.mask,
         pyramiding=args.pyramids,
         overwrite=args.overwrite
     )
 
 
 def tabup_from_parser(args):
     tabup(
@@ -559,14 +560,19 @@
         "Optional named arguments")
     optional_named.add_argument(
         "--nodata",
         type=int,
         help="The value to burn into the raster as NoData (missing data)",
     )
     optional_named.add_argument(
+        "--mask",
+        default=False,
+        help="Binary to use last band for mask True or False",
+    )
+    optional_named.add_argument(
         "--pyramids",
         help="Pyramiding Policy, MEAN, MODE, MIN, MAX, SAMPLE",
     )
     optional_named.add_argument(
         "--overwrite",
         help="Default is No but you can pass yes or y",
     )
```

### Comparing `geeup-0.6.3/geeup/getmeta.py` & `geeup-0.6.4/geeup/getmeta.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.3/geeup/metadata_loader.py` & `geeup-0.6.4/geeup/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.3/geeup/tuploader.py` & `geeup-0.6.4/geeup/tuploader.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.3/geeup/zipfiles.py` & `geeup-0.6.4/geeup/zipfiles.py`

 * *Files identical despite different names*

### Comparing `geeup-0.6.3/geeup.egg-info/PKG-INFO` & `geeup-0.6.4/geeup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geeup
-Version: 0.6.3
+Version: 0.6.4
 Summary: Simple Client for Earth Engine Uploads
 Home-page: https://github.com/samapriya/geeup
 Author: Samapriya Roy
 Author-email: samapriya.roy@gmail.com
 License: Apache 2.0
 Description: # geeup: Simple CLI for Earth Engine Uploads
         
@@ -266,14 +266,15 @@
           --dest DEST           Destination. Full path for upload to Google Earth Engine image collection, e.g. users/pinkiepie/myponycollection
           -m METADATA, --metadata METADATA
                                 Path to CSV with metadata.
           -u USER, --user USER  Google account name (gmail address).
         
         Optional named arguments:
           --nodata NODATA       The value to burn into the raster as NoData (missing data)
+          --mask MASK           Binary to use last band for mask True or False
           --pyramids PYRAMIDS   Pyramiding Policy, MEAN, MODE, MIN, MAX, SAMPLE
         ```
         
         Example setup would be
         
         ![gee_upload](https://user-images.githubusercontent.com/6677629/147895638-3d542ea5-2c72-43b7-8052-c5edef0ab717.gif)
         
@@ -343,14 +344,17 @@
         
         optional arguments:
           -h, --help  show this help message and exit
         ```
         
         # Changelog
         
+        ### 0.6.4
+        - Added masking option to use last band as mask
+        
         ### 0.6.2
         - Removed call to shell
         - Now prints status of task at task creation
         - Overwrite option for both images and tables
         
         ### 0.6.1
         - Removed dependency on pipwin uses pipgeo instead
```

### Comparing `geeup-0.6.3/setup.py` & `geeup-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setuptools.setup(
     name="geeup",
-    version="0.6.3",
+    version="0.6.4",
     packages=find_packages(),
     url="https://github.com/samapriya/geeup",
     install_requires=[
         "wheel",
         "earthengine_api>=0.1.274",
         "logzero>=1.5.0",
         "requests >= 2.10.0",
```

