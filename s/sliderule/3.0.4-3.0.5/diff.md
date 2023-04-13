# Comparing `tmp/sliderule-3.0.4.tar.gz` & `tmp/sliderule-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.0.4.tar", last modified: Wed Apr 12 11:52:04 2023, max compression
+gzip compressed data, was "sliderule-3.0.5.tar", last modified: Thu Apr 13 12:49:31 2023, max compression
```

## Comparing `sliderule-3.0.4.tar` & `sliderule-3.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:52:04.736271 sliderule-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-12 11:51:49.000000 sliderule-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-12 11:51:49.000000 sliderule-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-12 11:52:04.736271 sliderule-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-12 11:51:49.000000 sliderule-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-12 11:51:49.000000 sliderule-3.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 11:52:04.736271 sliderule-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-12 11:51:49.000000 sliderule-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:52:04.732271 sliderule-3.0.4/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24891 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    35898 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-12 11:51:49.000000 sliderule-3.0.4/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:52:04.732271 sliderule-3.0.4/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-12 11:52:04.000000 sliderule-3.0.4/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-12 11:52:04.000000 sliderule-3.0.4/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 11:52:04.000000 sliderule-3.0.4/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-12 11:52:04.000000 sliderule-3.0.4/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 11:52:04.000000 sliderule-3.0.4/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 11:52:04.736271 sliderule-3.0.4/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/hls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-12 11:51:49.000000 sliderule-3.0.4/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-12 11:51:49.000000 sliderule-3.0.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.270126 sliderule-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-13 12:49:11.000000 sliderule-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-13 12:49:11.000000 sliderule-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-13 12:49:31.270126 sliderule-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-13 12:49:11.000000 sliderule-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-13 12:49:11.000000 sliderule-3.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 12:49:31.270126 sliderule-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-13 12:49:11.000000 sliderule-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.262126 sliderule-3.0.5/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36103 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.262126 sliderule-3.0.5/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-13 12:49:31.000000 sliderule-3.0.5/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.270126 sliderule-3.0.5/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/hls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-13 12:49:11.000000 sliderule-3.0.5/version.txt
```

### Comparing `sliderule-3.0.4/LICENSE` & `sliderule-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/PKG-INFO` & `sliderule-3.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.4/README.md` & `sliderule-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/setup.py` & `sliderule-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/arcticdem.py` & `sliderule-3.0.5/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/earthdata.py` & `sliderule-3.0.5/sliderule/earthdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,17 +161,15 @@
             # generate multipolygon from list of polygons
             geometry = MultiPolygon(polygons)
         else:
             geometry, = geopandas.points_from_xy([None], [None])
         # Build GeoDataFrame (default geometry is crs=EPSG_MERCATOR)
         gdf = geopandas.GeoDataFrame(df, geometry=[geometry], crs=sliderule.EPSG_MERCATOR)
         # append to combined GeoDataFrame and catch warnings
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            granule_metadata = granule_metadata.append(gdf)
+        granule_metadata = geopandas.pd.concat([granule_metadata, gdf])
     # return granule metadata
     # - time start and time end
     # - time granule was updated
     # - granule size in bits
     # - polygons as geodataframe geometry
     return granule_metadata
 
@@ -220,19 +218,17 @@
         if not url_scroll_results:
             break
         urls += url_scroll_results
         # query for granule metadata and polygons
         if kwargs['return_metadata']:
             metadata_results = __cmr_granule_metadata(search_page)
         else:
-            metadata_results = [None for _ in url_scroll_results]
-        # append granule metadata and catch warnings
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            metadata = metadata.append(metadata_results)
+            metadata_results = geopandas.pd.DataFrame([None for _ in url_scroll_results])
+        # append granule metadata
+        metadata = geopandas.pd.concat([metadata, metadata_results])
 
     return (urls,metadata)
 
 ###############################################################################
 # CMR UTILITIES
 ###############################################################################
```

### Comparing `sliderule-3.0.4/sliderule/gedi.py` & `sliderule-3.0.5/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/h5.py` & `sliderule-3.0.5/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/icesat2.py` & `sliderule-3.0.5/sliderule/icesat2.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,18 +211,18 @@
             elif 'extrec' == rsp['__rectype']:
                 field_name = parm['atl03_geo_fields'][rsp['field_index']]
                 if field_name not in field_dictionary:
                     field_dictionary[field_name] = {'extent_id': [], field_name: []}
                 # Parse Ancillary Data
                 data = sliderule.getvalues(rsp['data'], rsp['datatype'], len(rsp['data']))
                 # Add Left Pair Track Entry
-                field_dictionary[field_name]['extent_id'] += rsp['extent_id'] | 0x2,
+                field_dictionary[field_name]['extent_id'] += numpy.uint64(rsp['extent_id']) | numpy.uint64(0x2),
                 field_dictionary[field_name][field_name] += data[LEFT_PAIR],
                 # Add Right Pair Track Entry
-                field_dictionary[field_name]['extent_id'] += rsp['extent_id'] | 0x3,
+                field_dictionary[field_name]['extent_id'] += numpy.uint64(rsp['extent_id']) | numpy.uint64(0x3),
                 field_dictionary[field_name][field_name] += data[RIGHT_PAIR],
             elif 'rsrec' == rsp['__rectype'] or 'zsrec' == rsp['__rectype']:
                 if rsp["num_samples"] <= 0:
                     continue
                 # Get field names and set
                 sample = rsp["samples"][0]
                 field_names = list(sample.keys())
@@ -233,15 +233,15 @@
                     as_numpy_array = True
                 # On first time, build empty dictionary for field set associated with raster
                 if field_set not in field_dictionary:
                     field_dictionary[field_set] = {'extent_id': []}
                     for field in field_names:
                         field_dictionary[field_set][field_set + "." + field] = []
                 # Populate dictionary for field set
-                field_dictionary[field_set]['extent_id'] += rsp['index'],
+                field_dictionary[field_set]['extent_id'] += numpy.uint64(rsp['index']),
                 for field in field_names:
                     if as_numpy_array:
                         data = []
                         for s in rsp["samples"]:
                             data += s[field],
                         field_dictionary[field_set][field_set + "." + field] += numpy.array(data),
                     else:
@@ -253,14 +253,16 @@
                 if field_set not in field_dictionary:
                     field_dictionary[field_set] = {'extent_id': []}
                     for field in field_names:
                         field_dictionary[field_set][field] = []
                 for field in field_names:
                     if type(rsp[field]) == tuple:
                         field_dictionary[field_set][field] += numpy.array(rsp[field]),
+                    elif field == 'extent_id':
+                        field_dictionary[field_set][field] += numpy.uint64(rsp[field]),
                     else:
                         field_dictionary[field_set][field] += rsp[field],
             elif 'fileidrec' == rsp['__rectype']:
                 file_dictionary[rsp["file_id"]] = rsp["file_name"]
 
         # Build Columns
         if num_records > 0:
@@ -286,15 +288,15 @@
     # Build Initial GeoDataFrame
     gdf = __todataframe(columns)
 
     # Merge Ancillary Fields
     tstart_merge = time.perf_counter()
     for field_set in field_dictionary:
         df = geopandas.pd.DataFrame(field_dictionary[field_set])
-        gdf = geopandas.pd.merge(gdf, df, on='extent_id', how='left').set_axis(gdf.index)
+        gdf = geopandas.pd.merge(gdf, df, how='left', on='extent_id').set_axis(gdf.index)
     profiles["merge"] = time.perf_counter() - tstart_merge
 
     # Delete Extent ID Column
     if len(gdf) > 0 and not keep_id:
         del gdf["extent_id"]
 
     # Attach Metadata
```

### Comparing `sliderule-3.0.4/sliderule/io.py` & `sliderule-3.0.5/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/ipxapi.py` & `sliderule-3.0.5/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/ipysliderule.py` & `sliderule-3.0.5/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule/sliderule.py` & `sliderule-3.0.5/sliderule/sliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/sliderule.egg-info/PKG-INFO` & `sliderule-3.0.5/sliderule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.4/sliderule.egg-info/SOURCES.txt` & `sliderule-3.0.5/sliderule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/_landsat.py` & `sliderule-3.0.5/utils/_landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/big_query.py` & `sliderule-3.0.5/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.0.5/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.0.5/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.0.5/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/extract_h5_dataset.py` & `sliderule-3.0.5/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/hls.py` & `sliderule-3.0.5/utils/hls.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/icepyx_region.py` & `sliderule-3.0.5/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/landsat.py` & `sliderule-3.0.5/utils/landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/monitor.py` & `sliderule-3.0.5/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/query_cmr.py` & `sliderule-3.0.5/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/query_elevations.py` & `sliderule-3.0.5/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/query_metrics.py` & `sliderule-3.0.5/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/query_photons.py` & `sliderule-3.0.5/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/query_stac.py` & `sliderule-3.0.5/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/query_version.py` & `sliderule-3.0.5/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/region_of_interest.py` & `sliderule-3.0.5/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/results_to_s3.py` & `sliderule-3.0.5/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/stac.py` & `sliderule-3.0.5/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/stream_events.py` & `sliderule-3.0.5/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/tail_events.py` & `sliderule-3.0.5/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.4/utils/utils.py` & `sliderule-3.0.5/utils/utils.py`

 * *Files identical despite different names*

