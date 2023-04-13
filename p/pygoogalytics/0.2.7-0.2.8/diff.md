# Comparing `tmp/pygoogalytics-0.2.7.tar.gz` & `tmp/pygoogalytics-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.2.7.tar", last modified: Thu Apr 13 06:43:59 2023, max compression
+gzip compressed data, was "pygoogalytics-0.2.8.tar", last modified: Thu Apr 13 10:58:45 2023, max compression
```

## Comparing `pygoogalytics-0.2.7.tar` & `pygoogalytics-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.011377 pygoogalytics-0.2.7/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.7/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.7/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 06:43:59.011195 pygoogalytics-0.2.7/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.7/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.009319 pygoogalytics-0.2.7/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-13 06:43:23.000000 pygoogalytics-0.2.7/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5729 2023-03-08 12:36:25.000000 pygoogalytics-0.2.7/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.010711 pygoogalytics-0.2.7/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.7/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.7/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    36581 2023-04-13 06:41:42.000000 pygoogalytics-0.2.7/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.7/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    41468 2023-04-12 13:27:23.000000 pygoogalytics-0.2.7/pygoogalytics/kwp_wrappers.py
--rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.7/pygoogalytics/resource_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.7/pygoogalytics/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.010269 pygoogalytics-0.2.7/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-13 06:43:59.011428 pygoogalytics-0.2.7/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-13 06:43:53.000000 pygoogalytics-0.2.7/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.685303 pygoogalytics-0.2.8/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.8/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.8/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 10:58:45.685149 pygoogalytics-0.2.8/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.8/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.683525 pygoogalytics-0.2.8/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-13 10:58:25.000000 pygoogalytics-0.2.8/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5911 2023-04-13 08:54:19.000000 pygoogalytics-0.2.8/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.684742 pygoogalytics-0.2.8/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.8/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.8/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    36784 2023-04-13 07:30:02.000000 pygoogalytics-0.2.8/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.8/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    42080 2023-04-13 10:54:44.000000 pygoogalytics-0.2.8/pygoogalytics/kwp_wrappers.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.8/pygoogalytics/resource_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.8/pygoogalytics/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 10:58:45.684227 pygoogalytics-0.2.8/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-13 10:58:45.000000 pygoogalytics-0.2.8/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-13 10:58:45.685344 pygoogalytics-0.2.8/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-13 10:58:25.000000 pygoogalytics-0.2.8/setup.py
```

### Comparing `pygoogalytics-0.2.7/LICENCE.txt` & `pygoogalytics-0.2.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/LICENSE` & `pygoogalytics-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/PKG-INFO` & `pygoogalytics-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.7
+Version: 0.2.8
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.7/README.md` & `pygoogalytics-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/pygoogalytics/__init__.py` & `pygoogalytics-0.2.8/pygoogalytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.2.7/pygoogalytics/client.py` & `pygoogalytics-0.2.8/pygoogalytics/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,28 +114,34 @@
     def __bool__(self):
         if self.googleads_client is not None:
             return True
         else:
             return False
 
     def plan_service(self,
-                     customer_id: str,
+                     customer_id: str = None,
                      location_codes: List[str] = None,
                      language_id: str = None
                      ):
+        if customer_id is None:
+            customer_id = self.default_customer_id
+
         return KeywordPlanService(googleads_client=self.googleads_client,
                                   customer_id=customer_id,
                                   location_codes=location_codes,
                                   language_id=language_id)
 
     def ideas_service(self,
-                      customer_id: str,
+                      customer_id: str = None,
                       site_url: str = None,
                       location_codes: List[str] = None,
                       language_id: str = None
                       ):
+        if customer_id is None:
+            customer_id = self.default_customer_id
+
         return KeywordPlanIdeaService(googleads_client=self.googleads_client,
                                       customer_id=customer_id,
                                       site_url=site_url,
                                       location_codes=location_codes,
                                       language_id=language_id)
```

### Comparing `pygoogalytics-0.2.7/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.2.8/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.2.8/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.2.8/pygoogalytics/googalytics_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         """test GA API"""
         pga_logger.debug(f"{self.__class__.__name__}.api_test() :: testing GA api")
         _api_error = None
         if not self.view_id:
             _api_status = "No view id"
         try:
             _ = self.get_ga3_response(start_date=datetime.date.today() + datetime.timedelta(days=-7),
-                                      raise_http_error=True)
+                                      raise_http_error=True, log_error=False)
             _api_status = "Success"
             pga_logger.debug(f"{self.__class__.__name__}.api_test() :: GA api successful")
         except GoogleApiHttpError as http_e:
             _api_status = "HttpError"
             _api_error = repr(http_e)
             pga_logger.debug(f"{self.__class__.__name__}.api_test() :: GA api failed")
         except Exception as http_e:
@@ -244,25 +244,27 @@
     def get_ga3_response(self,
                          start_date: Union[str, datetime.date],
                          end_date: Optional[Union[str, datetime.date]] = None,
                          ga_dimensions: Optional[Union[List[str], str]] = None,
                          ga_metrics: Optional[Union[List[str], str]] = None,
                          ga_filters: Optional[dict] = None,
                          raise_http_error: bool = False,
+                         log_error: bool = True,
                          filter_google_organic: bool = False,
                          _print_log: bool = False) -> Optional[dict]:
 
         r = self._ga3_response_raw(
             start_date=start_date,
             end_date=end_date,
             ga_dimensions=ga_dimensions,
             ga_metrics=ga_metrics,
             ga_filters=ga_filters,
             filter_google_organic=filter_google_organic,
             raise_http_error=raise_http_error,
+            log_error=log_error,
             page_token=None
         )
         if r is None:
             return None
 
         data = r.get('reports', [{}])[0].get('data', {}).get('rows', [])
         column_header = r.get('reports', [{}])[0].get('columnHeader')
@@ -298,14 +300,15 @@
                           start_date: Union[str, datetime.date],
                           end_date: Optional[Union[str, datetime.date]] = None,
                           ga_dimensions: Optional[Union[List[str], str]] = None,
                           ga_metrics: Optional[Union[List[str], str]] = None,
                           ga_filters: Optional[dict] = None,
                           filter_google_organic: bool = False,
                           raise_http_error: bool = False,
+                          log_error: bool = True,
                           return_raw_response: bool = False,
                           page_token: str = None,
                           _print_log: bool = False):
 
         if not self.view_id:
             # If there is no view_id we stop here and return None,
             # unless raise_http_error is True, in which case we continue to the execution and see what errors come up
@@ -385,19 +388,22 @@
 
         try:
             ga3_response = self.ga3_resource.reports().batchGet(body=ga3_request).execute()
             if return_raw_response:
                 pga_logger.info(f"{self.__class__.__name__}.get_ga3_response() :: returning raw response")
                 return ga3_response
         except GoogleApiHttpError as http_error:
+            _msg = ''
             if re.match(".*user does not have sufficient permissions", repr(http_error).lower()):
-                pga_logger.error(
-                    f"{self.__class__.__name__}.get_ga3_response() :: user does not have sufficient permissions")
+                _msg = f"{self.__class__.__name__}.get_ga3_response() :: user does not have sufficient permissions"
             if re.match(".*viewid must be set", repr(http_error).lower()):
-                pga_logger.error(f"{self.__class__.__name__}.get_ga3_response() :: view id is not set")
+                _msg = f"{self.__class__.__name__}.get_ga3_response() :: view id is not set"
+
+            if log_error and _msg:
+                pga_logger.error(_msg)
 
             if raise_http_error:
                 raise http_error
             else:
                 return None
 
         try:
```

### Comparing `pygoogalytics-0.2.7/pygoogalytics/googlepandas.py` & `pygoogalytics-0.2.8/pygoogalytics/googlepandas.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.2.8/pygoogalytics/kwp_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,29 +340,37 @@
         metrics_df: pd.DataFrame = _df.drop(columns=['volume_trend_tuples'])
 
         monthly_volume_df: pd.DataFrame = _df[['date_obtained',
                                                'query',
                                                'keyword',
                                                'status',
                                                'volume_trend_tuples']].explode('volume_trend_tuples')
+
         monthly_volume_df['volume_trend_tuples'] = monthly_volume_df['volume_trend_tuples'].apply(
             _check_volume_trend_tuples)
 
         monthly_volume_df['month_name'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[3])
         monthly_volume_df['month_enum'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[2])
         monthly_volume_df['month'] = monthly_volume_df['month_enum'].apply(_get_month_from_enum_value)
         monthly_volume_df['year'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[1])
 
+        monthly_volume_df.dropna(axis='index', subset=['month'], inplace=True)
+
+        monthly_volume_df['record_date'] = monthly_volume_df.apply(
+            lambda df: _conv_date(df['year'], df['month'], 15)
+        )
         monthly_volume_df['volume'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[0])
 
-        monthly_volume_df.drop(columns=['month_enum', 'volume_trend_tuples'], inplace=True)
-        monthly_volume_df.dropna(axis='index', subset=['month'], inplace=True)
+        monthly_volume_df.drop(
+            columns=['month_enum', 'volume_trend_tuples', 'month', 'year' 'month_name'],
+            inplace=True
+        )
 
         metrics_df.drop_duplicates(subset=["query", "keyword"], keep="first", inplace=True)
-        monthly_volume_df.drop_duplicates(subset=["query", "keyword", "year", "month"], keep="first", inplace=True)
+        monthly_volume_df.drop_duplicates(subset=["query", "keyword", "record_date"], keep="first", inplace=True)
 
         metrics_df.reset_index(drop=True, inplace=True)
         monthly_volume_df.reset_index(drop=True, inplace=True)
 
         return metrics_df, monthly_volume_df
 
     def get_forcast_metrics_df(self,
@@ -770,22 +778,25 @@
         request.customer_id = self.customer_id
         request.language = language_rn
         request.geo_target_constants = location_resource_names
         request.include_adult_keywords = include_adult_keywords
         request.keyword_plan_network = self.keyword_plan_network
         # request.page_size = page_size
 
-        if RE_URL.match(url):
-            page_url = url
-        elif url == "/" or url == "":
-            page_url = self.site_url
-        elif url[0] == "/":
-            page_url = self.site_url + url[1:]
+        if url is not None:
+            if RE_URL.match(url):
+                page_url = url
+            elif url == "/" or url == "":
+                page_url = self.site_url
+            elif url[0] == "/":
+                page_url = self.site_url + url[1:]
+            else:
+                page_url = self.site_url + url
         else:
-            page_url = self.site_url + url
+            page_url = None
 
         # To generate keyword ideas with only a page_url and no keywords we need
         # to initialize a UrlSeed object with the page_url as the "url" field.
         if not phrases and page_url:
             request.url_seed.url = page_url
 
         # To generate keyword ideas with only a list of keywords and no page_url
@@ -903,14 +914,26 @@
     return np.mean(volume_trends[-12:])
 
 
 def _partition_list(_list, n):
     return [_list[n * i:n * i + n] for i in range(ceil(len(_list) / n))]
 
 
+def _conv_date(year, month, day):
+    if isinstance(year, float):
+        year = int(year)
+    if not isinstance(year, int):
+        return None
+    if isinstance(month, float):
+        month = int(month)
+    if not isinstance(month, int):
+        return None
+    return datetime.date(year, month, day)
+
+
 def _map_location_to_resource_names(client,
                                     location_codes: Union[str, List[str]]):
     if isinstance(location_codes, str):
         location_codes = [location_codes]
 
     location_ids = []
     for _code in location_codes:
```

### Comparing `pygoogalytics-0.2.7/pygoogalytics/resource_utils.py` & `pygoogalytics-0.2.8/pygoogalytics/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/pygoogalytics/utils.py` & `pygoogalytics-0.2.8/pygoogalytics/utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.2.8/pygoogalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.7
+Version: 0.2.8
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.7/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.2.8/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.7/setup.py` & `pygoogalytics-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.2.7',
+    version='0.2.8',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

