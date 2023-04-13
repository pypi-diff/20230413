# Comparing `tmp/bcdata-0.7.6.tar.gz` & `tmp/bcdata-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.7.6.tar", last modified: Wed Feb  1 22:54:21 2023, max compression
+gzip compressed data, was "bcdata-0.7.7.tar", last modified: Thu Apr 13 19:52:21 2023, max compression
```

## Comparing `bcdata-0.7.6.tar` & `bcdata-0.7.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-02-01 22:54:21.271067 bcdata-0.7.6/
--rw-r--r--   0 snorris    (501) staff       (20)     6209 2023-02-01 22:52:54.000000 bcdata-0.7.6/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.6/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16269 2023-02-01 22:54:21.270907 bcdata-0.7.6/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15449 2022-11-18 23:36:23.000000 bcdata-0.7.6/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-02-01 22:54:21.268554 bcdata-0.7.6/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      349 2023-02-01 22:53:09.000000 bcdata-0.7.6/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.6/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.6/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     9553 2022-09-28 20:59:30.000000 bcdata-0.7.6/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.6/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.6/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    10936 2022-12-07 02:00:22.000000 bcdata-0.7.6/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-02-01 22:54:21.269793 bcdata-0.7.6/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16269 2023-02-01 22:54:21.000000 bcdata-0.7.6/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-02-01 22:54:21.000000 bcdata-0.7.6/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-02-01 22:54:21.000000 bcdata-0.7.6/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-02-01 22:54:21.000000 bcdata-0.7.6/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.6/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      123 2023-02-01 22:54:21.000000 bcdata-0.7.6/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-02-01 22:54:21.000000 bcdata-0.7.6/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.6/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      104 2023-02-01 22:20:34.000000 bcdata-0.7.6/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-02-01 22:54:21.271100 bcdata-0.7.6/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.6/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-02-01 22:54:21.270617 bcdata-0.7.6/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.6/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     5887 2022-11-18 22:56:31.000000 bcdata-0.7.6/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.6/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.6/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.462252 bcdata-0.7.7/
+-rw-r--r--   0 snorris    (501) staff       (20)     6314 2023-04-13 19:45:00.000000 bcdata-0.7.7/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.7/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16421 2023-04-13 19:52:21.462130 bcdata-0.7.7/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    15601 2023-04-13 19:41:37.000000 bcdata-0.7.7/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.460509 bcdata-0.7.7/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      349 2023-04-13 19:42:43.000000 bcdata-0.7.7/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.7/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.7/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     9795 2023-04-13 19:45:53.000000 bcdata-0.7.7/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.7/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.7/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11387 2023-04-13 19:45:53.000000 bcdata-0.7.7/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.461455 bcdata-0.7.7/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16421 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      474 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.7/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      123 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.7/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      104 2023-02-01 22:20:34.000000 bcdata-0.7.7/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-04-13 19:52:21.462284 bcdata-0.7.7/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.7/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.461974 bcdata-0.7.7/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.7/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6049 2023-04-13 19:25:05.000000 bcdata-0.7.7/tests/test_bcdata.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.7/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.7/tests/test_cli.py
```

### Comparing `bcdata-0.7.6/CHANGES.txt` & `bcdata-0.7.7/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 =======
 
+0.7.7 (2023-04-13)
+------------------
+- add option to lowercasify properties keys / column names (#126)
+
 0.7.6 (2023-02-01)
 ------------------
 - better handling of connection errors (#118)
 - correctly handle empty geodataframes (#121)
 - pin sqlalchemy to <2.0               (#124)
 
 0.7.4 (2022-09-28)
```

### Comparing `bcdata-0.7.6/LICENSE.txt` & `bcdata-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/PKG-INFO` & `bcdata-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -171,14 +171,15 @@
   --compact / --not-compact       Use compact separators (',', ':').
   --dst-crs, --dst_crs TEXT       Destination CRS
   -p, --pagesize INTEGER          Maximum request size
   -s, --sortby TEXT               Name of sort field
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
   -w, --max_workers INTEGER       Max number of concurrent requests
+  -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### dem 
 
@@ -214,25 +215,26 @@
 
   Write DataBC features to stdout as GeoJSON feature collection.
 
     $ bcdata dump bc-airports
     $ bcdata dump bc-airports --query "AIRPORT_NAME='Victoria Harbour (Shoal Point) Heliport'"
     $ bcdata dump bc-airports --bounds xmin ymin xmax ymax
 
-   It can also be combined to read bounds of a feature dataset using Fiona: 
+   It can also be combined to read bounds of a feature dataset using Fiona:
    $ bcdata dump bc-airports --bounds $(fio info aoi.shp --bounds)
 
 Options:
   --query TEXT                    A valid CQL or ECQL query
   -o, --out_file TEXT             Output file
   --bounds TEXT                   Bounds: "left bottom right top" or "[left,
                                   bottom, right, top]". Coordinates are BC
                                   Albers (default) or --bounds_crs
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
+  -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### info
```

### Comparing `bcdata-0.7.6/README.md` & `bcdata-0.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
   --compact / --not-compact       Use compact separators (',', ':').
   --dst-crs, --dst_crs TEXT       Destination CRS
   -p, --pagesize INTEGER          Maximum request size
   -s, --sortby TEXT               Name of sort field
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
   -w, --max_workers INTEGER       Max number of concurrent requests
+  -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### dem 
 
@@ -192,25 +193,26 @@
 
   Write DataBC features to stdout as GeoJSON feature collection.
 
     $ bcdata dump bc-airports
     $ bcdata dump bc-airports --query "AIRPORT_NAME='Victoria Harbour (Shoal Point) Heliport'"
     $ bcdata dump bc-airports --bounds xmin ymin xmax ymax
 
-   It can also be combined to read bounds of a feature dataset using Fiona: 
+   It can also be combined to read bounds of a feature dataset using Fiona:
    $ bcdata dump bc-airports --bounds $(fio info aoi.shp --bounds)
 
 Options:
   --query TEXT                    A valid CQL or ECQL query
   -o, --out_file TEXT             Output file
   --bounds TEXT                   Bounds: "left bottom right top" or "[left,
                                   bottom, right, top]". Coordinates are BC
                                   Albers (default) or --bounds_crs
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
+  -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### info
```

### Comparing `bcdata-0.7.6/bcdata/bc2pg.py` & `bcdata-0.7.7/bcdata/bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/bcdata/bcdc.py` & `bcdata-0.7.7/bcdata/bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/bcdata/cli.py` & `bcdata-0.7.7/bcdata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,18 @@
     help='Bounds: "left bottom right top" or "[left, bottom, right, top]". Coordinates are BC Albers (default) or --bounds_crs',
 )
 
 dst_crs_opt = click.option(
     "--dst-crs", "--dst_crs", default="epsg:4326", help="Destination CRS"
 )
 
+lowercase_opt = click.option(
+    "--lowercase", "-l", is_flag=True, help="Write column/properties names as lowercase"
+)
+
 
 @click.group()
 @click.version_option(version=bcdata.__version__, message="%(version)s")
 def cli():
     pass
 
 
@@ -187,17 +191,18 @@
 @bounds_opt
 @click.option(
     "--bounds-crs",
     "--bounds_crs",
     help="CRS of provided bounds",
     default="EPSG:3005",
 )
+@lowercase_opt
 @verbose_opt
 @quiet_opt
-def dump(dataset, query, out_file, bounds, bounds_crs, verbose, quiet):
+def dump(dataset, query, out_file, bounds, bounds_crs, lowercase, verbose, quiet):
     """Write DataBC features to stdout as GeoJSON feature collection.
 
     \b
       $ bcdata dump bc-airports
       $ bcdata dump bc-airports --query "AIRPORT_NAME='Victoria Harbour (Shoal Point) Heliport'"
       $ bcdata dump bc-airports --bounds xmin ymin xmax ymax
 
@@ -205,15 +210,17 @@
     \b
       $ bcdata dump bc-airports --bounds $(fio info aoi.shp --bounds)
 
     """
     verbosity = verbose - quiet
     configure_logging(verbosity)
     table = bcdata.validate_name(dataset)
-    data = bcdata.get_data(table, query=query, bounds=bounds, bounds_crs=bounds_crs)
+    data = bcdata.get_data(
+        table, query=query, bounds=bounds, bounds_crs=bounds_crs, lowercase=lowercase
+    )
     if out_file:
         with open(out_file, "w") as sink:
             sink.write(json.dumps(data))
     else:
         sink = click.get_text_stream("stdout")
         sink.write(json.dumps(data))
 
@@ -235,27 +242,29 @@
     "--bounds_crs",
     help="CRS of provided bounds",
     default="EPSG:3005",
 )
 @click.option(
     "--max_workers", "-w", default=2, help="Max number of concurrent requests"
 )
+@lowercase_opt
 @verbose_opt
 @quiet_opt
 def cat(
     dataset,
     query,
     bounds,
     bounds_crs,
     indent,
     compact,
     dst_crs,
     pagesize,
     sortby,
     max_workers,
+    lowercase,
     verbose,
     quiet,
 ):
     """Write DataBC features to stdout as GeoJSON feature objects."""
     # Note that cat does not concatenate!
     verbosity = verbose - quiet
     configure_logging(verbosity)
@@ -272,14 +281,15 @@
         query=query,
         bounds=bounds,
         bounds_crs=bounds_crs,
         sortby=sortby,
         crs=dst_crs,
         pagesize=pagesize,
         max_workers=max_workers,
+        lowercase=lowercase,
     ):
         click.echo(json.dumps(feat, **dump_kwds))
 
 
 @cli.command()
 @click.argument("dataset", type=click.STRING)
 @click.option(
```

### Comparing `bcdata-0.7.6/bcdata/database.py` & `bcdata-0.7.7/bcdata/database.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/bcdata/wcs.py` & `bcdata-0.7.7/bcdata/wcs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/bcdata/wfs.py` & `bcdata-0.7.7/bcdata/wfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
     max_workers=2,
     as_gdf=False,
+    lowercase=False,
 ):
     """Get GeoJSON featurecollection (or geodataframe) from DataBC WFS"""
     urls = define_requests(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
@@ -233,14 +234,20 @@
     )
     with ThreadPoolExecutor(max_workers=max_workers) as executor:
         results = executor.map(make_request, urls)
 
     outjson = dict(type="FeatureCollection", features=[])
     for result in results:
         outjson["features"] += result
+    # if specified, lowercasify all properties
+    if lowercase:
+        for feature in outjson["features"]:
+            feature["properties"] = {
+                k.lower(): v for k, v in feature["properties"].items()
+            }
     if not as_gdf:
         # If output crs is specified, include the crs object in the json
         # But as default, we prefer to default to 4326 and RFC7946 (no crs)
         if crs.lower() != "epsg:4326":
             crs_int = crs.split(":")[1]
             outjson[
                 "crs"
@@ -261,14 +268,15 @@
     crs="epsg:4326",
     bounds=None,
     bounds_crs="epsg:3005",
     count=None,
     sortby=None,
     pagesize=10000,
     max_workers=2,
+    lowercase=False,
 ):
     """Yield features from DataBC WFS"""
     urls = define_requests(
         dataset,
         query=query,
         crs=crs,
         bounds=bounds,
@@ -276,14 +284,18 @@
         count=count,
         sortby=sortby,
         pagesize=pagesize,
     )
     with ThreadPoolExecutor(max_workers=max_workers) as executor:
         for result in executor.map(make_request, urls):
             for feature in result:
+                if lowercase:
+                    feature["properties"] = {
+                        k.lower(): v for k, v in feature["properties"].items()
+                    }
                 yield feature
 
 
 def get_types(dataset, count=10):
     """Return distinct types within the first n features"""
     # validate the table name
     table = validate_name(dataset)
```

### Comparing `bcdata-0.7.6/bcdata.egg-info/PKG-INFO` & `bcdata-0.7.7/bcdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -171,14 +171,15 @@
   --compact / --not-compact       Use compact separators (',', ':').
   --dst-crs, --dst_crs TEXT       Destination CRS
   -p, --pagesize INTEGER          Maximum request size
   -s, --sortby TEXT               Name of sort field
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
   -w, --max_workers INTEGER       Max number of concurrent requests
+  -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### dem 
 
@@ -214,25 +215,26 @@
 
   Write DataBC features to stdout as GeoJSON feature collection.
 
     $ bcdata dump bc-airports
     $ bcdata dump bc-airports --query "AIRPORT_NAME='Victoria Harbour (Shoal Point) Heliport'"
     $ bcdata dump bc-airports --bounds xmin ymin xmax ymax
 
-   It can also be combined to read bounds of a feature dataset using Fiona: 
+   It can also be combined to read bounds of a feature dataset using Fiona:
    $ bcdata dump bc-airports --bounds $(fio info aoi.shp --bounds)
 
 Options:
   --query TEXT                    A valid CQL or ECQL query
   -o, --out_file TEXT             Output file
   --bounds TEXT                   Bounds: "left bottom right top" or "[left,
                                   bottom, right, top]". Coordinates are BC
                                   Albers (default) or --bounds_crs
   --bounds-crs, --bounds_crs TEXT
                                   CRS of provided bounds
+  -l, --lowercase                 Write column/properties names as lowercase
   -v, --verbose                   Increase verbosity.
   -q, --quiet                     Decrease verbosity.
   --help                          Show this message and exit.
 ```
 
 #### info
```

### Comparing `bcdata-0.7.6/setup.py` & `bcdata-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/tests/test_bc2pg.py` & `bcdata-0.7.7/tests/test_bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/tests/test_bcdata.py` & `bcdata-0.7.7/tests/test_bcdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 
 
 def test_get_data_small():
     data = bcdata.get_data(AIRPORTS_TABLE)
     assert data["type"] == "FeatureCollection"
 
 
+def test_get_data_lowercase():
+    data = bcdata.get_data(AIRPORTS_TABLE, lowercase=True)
+    assert "airport_name" in data["features"][0]["properties"].keys()
+
+
 def test_get_data_crs():
     data = bcdata.get_data(AIRPORTS_TABLE, crs="EPSG:3005")
     assert (
         data["crs"]
         == """{"type":"name","properties":{"name":"urn:ogc:def:crs:EPSG::3005"}}"""
     )
```

### Comparing `bcdata-0.7.6/tests/test_bcdc.py` & `bcdata-0.7.7/tests/test_bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.6/tests/test_cli.py` & `bcdata-0.7.7/tests/test_cli.py`

 * *Files identical despite different names*

