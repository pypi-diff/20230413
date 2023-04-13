# Comparing `tmp/reverse-geocode-bd-1.0.6.tar.gz` & `tmp/reverse-geocode-bd-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/aci/ACI Projects/PyPi Packages/reverse_geocode_bd/dist/.tmp-n5h_ryyn/reverse-geocode-bd-1.0.6.tar", last modified: Tue Mar  7 03:48:38 2023, max compression
+gzip compressed data, was "/home/aci/ACI Projects/PyPi Packages/reverse_geocode_bd/dist/.tmp-87pv8kqx/reverse-geocode-bd-1.0.7.tar", last modified: Thu Apr 13 16:37:10 2023, max compression
```

## Comparing `reverse-geocode-bd-1.0.6.tar` & `reverse-geocode-bd-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 aci       (1000) aci       (1000)        0 2023-03-07 03:48:37.998316 reverse-geocode-bd-1.0.6/
--rw-rw-r--   0 aci       (1000) aci       (1000)     1074 2023-03-06 17:58:00.000000 reverse-geocode-bd-1.0.6/LICENSE
--rw-rw-r--   0 aci       (1000) aci       (1000)       33 2023-03-06 17:48:03.000000 reverse-geocode-bd-1.0.6/MANIFEST.in
--rw-rw-r--   0 aci       (1000) aci       (1000)     1378 2023-03-07 03:48:37.998316 reverse-geocode-bd-1.0.6/PKG-INFO
--rw-rw-r--   0 aci       (1000) aci       (1000)      922 2023-03-07 03:39:01.000000 reverse-geocode-bd-1.0.6/README.md
--rw-rw-r--   0 aci       (1000) aci       (1000)      103 2023-03-06 17:37:15.000000 reverse-geocode-bd-1.0.6/pyproject.toml
-drwxrwxr-x   0 aci       (1000) aci       (1000)        0 2023-03-07 03:48:37.994316 reverse-geocode-bd-1.0.6/reverse_geocode_bd/
--rw-rw-r--   0 aci       (1000) aci       (1000)     4102 2023-03-06 18:07:03.000000 reverse-geocode-bd-1.0.6/reverse_geocode_bd/__init__.py
--rw-rw-r--   0 aci       (1000) aci       (1000)  4464856 2021-02-07 16:46:52.000000 reverse-geocode-bd-1.0.6/reverse_geocode_bd/small_bangladesh_geojson_adm4_5160_unions_thanas.json
-drwxrwxr-x   0 aci       (1000) aci       (1000)        0 2023-03-07 03:48:37.998316 reverse-geocode-bd-1.0.6/reverse_geocode_bd.egg-info/
--rw-rw-r--   0 aci       (1000) aci       (1000)     1378 2023-03-07 03:48:37.000000 reverse-geocode-bd-1.0.6/reverse_geocode_bd.egg-info/PKG-INFO
--rw-rw-r--   0 aci       (1000) aci       (1000)      326 2023-03-07 03:48:37.000000 reverse-geocode-bd-1.0.6/reverse_geocode_bd.egg-info/SOURCES.txt
--rw-rw-r--   0 aci       (1000) aci       (1000)        1 2023-03-07 03:48:37.000000 reverse-geocode-bd-1.0.6/reverse_geocode_bd.egg-info/dependency_links.txt
--rw-rw-r--   0 aci       (1000) aci       (1000)       19 2023-03-07 03:48:37.000000 reverse-geocode-bd-1.0.6/reverse_geocode_bd.egg-info/top_level.txt
--rw-rw-r--   0 aci       (1000) aci       (1000)      544 2023-03-07 03:48:37.998316 reverse-geocode-bd-1.0.6/setup.cfg
+drwxrwxr-x   0 aci       (1000) aci       (1000)        0 2023-04-13 16:37:10.645987 reverse-geocode-bd-1.0.7/
+-rw-rw-r--   0 aci       (1000) aci       (1000)     1074 2023-03-06 17:58:00.000000 reverse-geocode-bd-1.0.7/LICENSE
+-rw-rw-r--   0 aci       (1000) aci       (1000)       33 2023-03-06 17:48:03.000000 reverse-geocode-bd-1.0.7/MANIFEST.in
+-rw-rw-r--   0 aci       (1000) aci       (1000)     1378 2023-04-13 16:37:10.645987 reverse-geocode-bd-1.0.7/PKG-INFO
+-rw-rw-r--   0 aci       (1000) aci       (1000)      922 2023-04-06 06:58:35.000000 reverse-geocode-bd-1.0.7/README.md
+-rw-rw-r--   0 aci       (1000) aci       (1000)      103 2023-03-06 17:37:15.000000 reverse-geocode-bd-1.0.7/pyproject.toml
+drwxrwxr-x   0 aci       (1000) aci       (1000)        0 2023-04-13 16:37:10.645987 reverse-geocode-bd-1.0.7/reverse_geocode_bd/
+-rw-rw-r--   0 aci       (1000) aci       (1000)     4102 2023-03-06 18:07:03.000000 reverse-geocode-bd-1.0.7/reverse_geocode_bd/__init__.py
+-rw-rw-r--   0 aci       (1000) aci       (1000)  4464856 2021-02-07 16:46:52.000000 reverse-geocode-bd-1.0.7/reverse_geocode_bd/small_bangladesh_geojson_adm4_5160_unions_thanas.json
+drwxrwxr-x   0 aci       (1000) aci       (1000)        0 2023-04-13 16:37:10.645987 reverse-geocode-bd-1.0.7/reverse_geocode_bd.egg-info/
+-rw-rw-r--   0 aci       (1000) aci       (1000)     1378 2023-04-13 16:37:10.000000 reverse-geocode-bd-1.0.7/reverse_geocode_bd.egg-info/PKG-INFO
+-rw-rw-r--   0 aci       (1000) aci       (1000)      326 2023-04-13 16:37:10.000000 reverse-geocode-bd-1.0.7/reverse_geocode_bd.egg-info/SOURCES.txt
+-rw-rw-r--   0 aci       (1000) aci       (1000)        1 2023-04-13 16:37:10.000000 reverse-geocode-bd-1.0.7/reverse_geocode_bd.egg-info/dependency_links.txt
+-rw-rw-r--   0 aci       (1000) aci       (1000)       19 2023-04-13 16:37:10.000000 reverse-geocode-bd-1.0.7/reverse_geocode_bd.egg-info/top_level.txt
+-rw-rw-r--   0 aci       (1000) aci       (1000)      544 2023-04-13 16:37:10.645987 reverse-geocode-bd-1.0.7/setup.cfg
```

### Comparing `reverse-geocode-bd-1.0.6/LICENSE` & `reverse-geocode-bd-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reverse-geocode-bd-1.0.6/PKG-INFO` & `reverse-geocode-bd-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: reverse-geocode-bd
-Version: 1.0.6
+Version: 1.0.7
 Summary: Offline reverse geocoder for Bangladesh Map
 Home-page: https://github.com/ShakhrulSiam268/reverse_geocode_bd
 Author: Shakhrul Iman Siam
 Author-email: shakhrulsiam268@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Reverse GeoCode BD
 
-[![PyPI Downloads](https://static.pepy.tech/personalized-badge/reverse-geocode-bd?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPi%20Downloads)](https://pepy.tech/project/reverse-geocode-bd)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/reverse-geocode-bd?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPi%20Downloads)](https://pepy.tech/project/reverse-geocode-bd)
 
 ## Installation
 ```shell
 $ pip install reverse-geocode-bd
 ```
 A Python library for offline reverse geocoding. Reverse Geocode BD takes a (latitude , longitude) coordinate and returns the Division, District, Upazila and Thana of any location in Bangladesh.
```

### Comparing `reverse-geocode-bd-1.0.6/README.md` & `reverse-geocode-bd-1.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Reverse GeoCode BD
 
-[![PyPI Downloads](https://static.pepy.tech/personalized-badge/reverse-geocode-bd?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPi%20Downloads)](https://pepy.tech/project/reverse-geocode-bd)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/reverse-geocode-bd?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPi%20Downloads)](https://pepy.tech/project/reverse-geocode-bd)
 
 ## Installation
 ```shell
 $ pip install reverse-geocode-bd
 ```
 A Python library for offline reverse geocoding. Reverse Geocode BD takes a (latitude , longitude) coordinate and returns the Division, District, Upazila and Thana of any location in Bangladesh.
```

### Comparing `reverse-geocode-bd-1.0.6/reverse_geocode_bd/__init__.py` & `reverse-geocode-bd-1.0.7/reverse_geocode_bd/__init__.py`

 * *Files identical despite different names*

### Comparing `reverse-geocode-bd-1.0.6/reverse_geocode_bd/small_bangladesh_geojson_adm4_5160_unions_thanas.json` & `reverse-geocode-bd-1.0.7/reverse_geocode_bd/small_bangladesh_geojson_adm4_5160_unions_thanas.json`

 * *Files identical despite different names*

### Comparing `reverse-geocode-bd-1.0.6/reverse_geocode_bd.egg-info/PKG-INFO` & `reverse-geocode-bd-1.0.7/reverse_geocode_bd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: reverse-geocode-bd
-Version: 1.0.6
+Version: 1.0.7
 Summary: Offline reverse geocoder for Bangladesh Map
 Home-page: https://github.com/ShakhrulSiam268/reverse_geocode_bd
 Author: Shakhrul Iman Siam
 Author-email: shakhrulsiam268@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Reverse GeoCode BD
 
-[![PyPI Downloads](https://static.pepy.tech/personalized-badge/reverse-geocode-bd?period=month&units=international_system&left_color=blue&right_color=orange&left_text=PyPi%20Downloads)](https://pepy.tech/project/reverse-geocode-bd)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/reverse-geocode-bd?period=total&units=international_system&left_color=blue&right_color=orange&left_text=PyPi%20Downloads)](https://pepy.tech/project/reverse-geocode-bd)
 
 ## Installation
 ```shell
 $ pip install reverse-geocode-bd
 ```
 A Python library for offline reverse geocoding. Reverse Geocode BD takes a (latitude , longitude) coordinate and returns the Division, District, Upazila and Thana of any location in Bangladesh.
```

### Comparing `reverse-geocode-bd-1.0.6/setup.cfg` & `reverse-geocode-bd-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reverse-geocode-bd
-version = 1.0.6
+version = 1.0.7
 author = Shakhrul Iman Siam
 author_email = shakhrulsiam268@gmail.com
 description = Offline reverse geocoder for Bangladesh Map
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ShakhrulSiam268/reverse_geocode_bd
 classifiers =
```

