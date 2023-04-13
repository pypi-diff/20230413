# Comparing `tmp/saeonobspy-0.1.0.tar.gz` & `tmp/saeonobspy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saeonobspy-0.1.0.tar", last modified: Tue Mar 28 22:47:41 2023, max compression
+gzip compressed data, was "saeonobspy-0.2.0.tar", last modified: Thu Apr 13 13:53:26 2023, max compression
```

## Comparing `saeonobspy-0.1.0.tar` & `saeonobspy-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/saeonobspy/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/saeonobspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/saeonobspy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/saeonobspy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/saeonobspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-28 22:47:41.000000 saeonobspy-0.1.0/saeonobspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-28 22:47:41.000000 saeonobspy-0.1.0/saeonobspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 22:47:41.000000 saeonobspy-0.1.0/saeonobspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 22:47:41.000000 saeonobspy-0.1.0/saeonobspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 22:47:41.000000 saeonobspy-0.1.0/saeonobspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:47:41.702839 saeonobspy-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-03-28 22:47:38.000000 saeonobspy-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/saeonobspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/saeonobspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/saeonobspy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/saeonobspy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/saeonobspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-13 13:53:26.000000 saeonobspy-0.2.0/saeonobspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 13:53:26.000000 saeonobspy-0.2.0/saeonobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:53:26.000000 saeonobspy-0.2.0/saeonobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 13:53:26.000000 saeonobspy-0.2.0/saeonobspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 13:53:26.000000 saeonobspy-0.2.0/saeonobspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:53:26.175106 saeonobspy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17551 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-04-13 13:53:22.000000 saeonobspy-0.2.0/versioneer.py
```

### Comparing `saeonobspy-0.1.0/LICENSE` & `saeonobspy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saeonobspy-0.1.0/PKG-INFO` & `saeonobspy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saeonobspy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to interact with the SAEON Observation Database API
 Home-page: https://github.com/GMoncrieff/saeonobspy
 Author: Glenn Moncrieff
 Author-email: glenn@saeon.ac.za
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `saeonobspy-0.1.0/README.md` & `saeonobspy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `saeonobspy-0.1.0/saeonobspy/api.py` & `saeonobspy-0.2.0/saeonobspy/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
-import requests
 import pandas as pd
 import geopandas as gpd
 from shapely.geometry import Point
 from typing import Union
 
+import asyncio
+import aiohttp
+
 
 class SAEONObsAPI:
     def __init__(self):
         """
         Initialize the SAEONObsAPI class to access the South African Environmental Observation Network (SAEON) Observation Database API.
 
         Example:
@@ -51,17 +53,15 @@
         # Without extent and spatial set to False (default)
         datasets_df = saeon_api.view_datasets()
 
         # With extent and spatial set to True
         extent_gdf = geopandas.read_file('path/to/extent/shapefile.shp')
         spatial_datasets_gdf = saeon_api.view_datasets(extent=extent_gdf, spatial=True)
         """
-        response = requests.get(self.BASE_URL, headers=self.HEADERS)
-        response.raise_for_status()
-        data = response.json()
+        data = asyncio.run(self._view_datasets(extent, spatial))
         df = pd.DataFrame(data)
 
         # Extract relevant columns and clean up the DataFrame
         df = df[
             [
                 "id",
                 "siteName",
@@ -135,36 +135,61 @@
         # Filter the datasets DataFrame based on your criteria
         filtered_datasets_df = datasets_df[datasets_df['siteName'] == 'Constantiaberg']
         filtered_datasets_df = filtered_datasets_df[filtered_datasets_df['description'] == 'Air Temperature - Daily Minimum - Degrees Celsius']
 
         #download data
         obs_data = saeon_api.get_datasets(filtered_datasets_df, start_date='2020-01-01', end_date='2020-12-31')
         """
+        datasets = asyncio.run(self._get_datasets(df, start_date, end_date))
+        result = pd.concat([pd.DataFrame(data) for data in datasets], ignore_index=True)
+        return result
 
+    async def _view_datasets(
+        self, extent: gpd.GeoDataFrame = None, spatial: bool = False
+    ) -> pd.DataFrame:
+        async with aiohttp.ClientSession(headers=self.HEADERS) as session:
+            async with session.get(self.BASE_URL) as response:
+                response.raise_for_status()
+                data = await response.json()
+
+        return data
+
+    async def _get_datasets(
+        self,
+        df: Union[pd.DataFrame, gpd.GeoDataFrame],
+        start_date: str = None,
+        end_date: str = None,
+    ) -> pd.DataFrame:
         if (
             not (isinstance(df, pd.DataFrame) or isinstance(df, gpd.GeoDataFrame))
             or "id" not in df.columns
         ):
             raise ValueError("Input must be a DataFrame containing an 'id' column.")
 
         if start_date:
             start_date = pd.to_datetime(start_date).strftime("%Y-%m-%dT%H:%M:%S")
         if end_date:
             end_date = pd.to_datetime(end_date).strftime("%Y-%m-%dT%H:%M:%S")
 
-        datasets = []
-
-        for dataset_id in df["id"]:
+        async def fetch_dataset(session, dataset_id, start_date, end_date):
             url_obs = f"{self.BASE_URL}/{dataset_id}/Observations"
             payload = {}
             if start_date and end_date:
                 payload = {"startDate": start_date, "endDate": end_date}
 
-            response = requests.post(url_obs, headers=self.HEADERS, json=payload)
-            response.raise_for_status()
-
-            data = response.json()
-            temp_df = pd.DataFrame(data)
-            datasets.append(temp_df)
+            async with session.post(url_obs, json=payload) as response:
+                response.raise_for_status()
+                data = await response.json()
+                return data
+
+        async def fetch_all_datasets():
+            async with aiohttp.ClientSession(headers=self.HEADERS) as session:
+                tasks = []
+                for dataset_id in df["id"]:
+                    task = asyncio.create_task(
+                        fetch_dataset(session, dataset_id, start_date, end_date)
+                    )
+                    tasks.append(task)
+                return await asyncio.gather(*tasks)
 
-        result = pd.concat(datasets, ignore_index=True)
-        return result
+        datasets = await fetch_all_datasets()
+        return datasets
```

### Comparing `saeonobspy-0.1.0/saeonobspy.egg-info/PKG-INFO` & `saeonobspy-0.2.0/saeonobspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saeonobspy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to interact with the SAEON Observation Database API
 Home-page: https://github.com/GMoncrieff/saeonobspy
 Author: Glenn Moncrieff
 Author-email: glenn@saeon.ac.za
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `saeonobspy-0.1.0/setup.py` & `saeonobspy-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 setup(
     name="saeonobspy",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     packages=find_packages(),
-    install_requires=["pandas", "geopandas", "requests", "shapely"],
+    install_requires=["pandas", "geopandas", "requests", "shapely", "aiohttp"],
     url="https://github.com/GMoncrieff/saeonobspy",
     author="Glenn Moncrieff",
     author_email="glenn@saeon.ac.za",
     description="Python package to interact with the SAEON Observation Database API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `saeonobspy-0.1.0/versioneer.py` & `saeonobspy-0.2.0/versioneer.py`

 * *Files identical despite different names*

