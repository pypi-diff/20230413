# Comparing `tmp/pygoogalytics-0.2.6.tar.gz` & `tmp/pygoogalytics-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoogalytics-0.2.6.tar", last modified: Tue Apr 11 08:53:11 2023, max compression
+gzip compressed data, was "pygoogalytics-0.2.7.tar", last modified: Thu Apr 13 06:43:59 2023, max compression
```

## Comparing `pygoogalytics-0.2.6.tar` & `pygoogalytics-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.050288 pygoogalytics-0.2.6/
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.6/LICENCE.txt
--rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.6/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-11 08:53:11.050143 pygoogalytics-0.2.6/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.6/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.048104 pygoogalytics-0.2.6/pygoogalytics/
--rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-11 08:52:41.000000 pygoogalytics-0.2.6/pygoogalytics/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)     5729 2023-03-08 12:36:25.000000 pygoogalytics-0.2.6/pygoogalytics/client.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.049730 pygoogalytics-0.2.6/pygoogalytics/data/
--rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.6/pygoogalytics/data/country_iso_codes.csv
--rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.6/pygoogalytics/data/google_ads_location_ids.csv
--rw-r--r--   0 joshua     (501) staff       (20)    36524 2023-04-11 08:51:56.000000 pygoogalytics-0.2.6/pygoogalytics/googalytics_wrapper.py
--rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.6/pygoogalytics/googlepandas.py
--rw-r--r--   0 joshua     (501) staff       (20)    40628 2023-03-07 20:05:15.000000 pygoogalytics-0.2.6/pygoogalytics/kwp_wrappers.py
--rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.6/pygoogalytics/resource_utils.py
--rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.6/pygoogalytics/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-11 08:53:11.048898 pygoogalytics-0.2.6/pygoogalytics.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-11 08:53:11.000000 pygoogalytics-0.2.6/pygoogalytics.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-11 08:53:11.050333 pygoogalytics-0.2.6/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-11 08:52:31.000000 pygoogalytics-0.2.6/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.011377 pygoogalytics-0.2.7/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-22 09:57:18.000000 pygoogalytics-0.2.7/LICENCE.txt
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2023-02-16 19:07:57.000000 pygoogalytics-0.2.7/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 06:43:59.011195 pygoogalytics-0.2.7/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     4882 2023-02-23 08:04:27.000000 pygoogalytics-0.2.7/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.009319 pygoogalytics-0.2.7/pygoogalytics/
+-rw-r--r--   0 joshua     (501) staff       (20)     1212 2023-04-13 06:43:23.000000 pygoogalytics-0.2.7/pygoogalytics/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5729 2023-03-08 12:36:25.000000 pygoogalytics-0.2.7/pygoogalytics/client.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.010711 pygoogalytics-0.2.7/pygoogalytics/data/
+-rw-r--r--   0 joshua     (501) staff       (20)     6027 2022-02-02 23:47:01.000000 pygoogalytics-0.2.7/pygoogalytics/data/country_iso_codes.csv
+-rw-r--r--   0 joshua     (501) staff       (20)     4301 2022-04-20 14:13:44.000000 pygoogalytics-0.2.7/pygoogalytics/data/google_ads_location_ids.csv
+-rw-r--r--   0 joshua     (501) staff       (20)    36581 2023-04-13 06:41:42.000000 pygoogalytics-0.2.7/pygoogalytics/googalytics_wrapper.py
+-rw-r--r--   0 joshua     (501) staff       (20)    32322 2023-02-21 11:27:36.000000 pygoogalytics-0.2.7/pygoogalytics/googlepandas.py
+-rw-r--r--   0 joshua     (501) staff       (20)    41468 2023-04-12 13:27:23.000000 pygoogalytics-0.2.7/pygoogalytics/kwp_wrappers.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2409 2023-03-07 19:50:49.000000 pygoogalytics-0.2.7/pygoogalytics/resource_utils.py
+-rw-r--r--   0 joshua     (501) staff       (20)     2064 2023-02-20 08:31:45.000000 pygoogalytics-0.2.7/pygoogalytics/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-04-13 06:43:59.010269 pygoogalytics-0.2.7/pygoogalytics.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     5626 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      512 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)      113 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       14 2023-04-13 06:43:58.000000 pygoogalytics-0.2.7/pygoogalytics.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-04-13 06:43:59.011428 pygoogalytics-0.2.7/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1274 2023-04-13 06:43:53.000000 pygoogalytics-0.2.7/setup.py
```

### Comparing `pygoogalytics-0.2.6/LICENCE.txt` & `pygoogalytics-0.2.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/LICENSE` & `pygoogalytics-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/PKG-INFO` & `pygoogalytics-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.6
+Version: 0.2.7
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.6/README.md` & `pygoogalytics-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics/__init__.py` & `pygoogalytics-0.2.7/pygoogalytics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   sc_domain='<search-console-domain>',
   view_id='<ga3-view-id>',
   ga4_property_id='<ga4-property-id>'
 )
 ```
 """
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = 'Joshua Prettyman'
 __credits__ = 'Blink SEO'
 
 import os
 import csv
 import logging
```

### Comparing `pygoogalytics-0.2.6/pygoogalytics/client.py` & `pygoogalytics-0.2.7/pygoogalytics/client.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics/data/country_iso_codes.csv` & `pygoogalytics-0.2.7/pygoogalytics/data/country_iso_codes.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics/data/google_ads_location_ids.csv` & `pygoogalytics-0.2.7/pygoogalytics/data/google_ads_location_ids.csv`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics/googalytics_wrapper.py` & `pygoogalytics-0.2.7/pygoogalytics/googalytics_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,26 +245,29 @@
                          start_date: Union[str, datetime.date],
                          end_date: Optional[Union[str, datetime.date]] = None,
                          ga_dimensions: Optional[Union[List[str], str]] = None,
                          ga_metrics: Optional[Union[List[str], str]] = None,
                          ga_filters: Optional[dict] = None,
                          raise_http_error: bool = False,
                          filter_google_organic: bool = False,
-                         _print_log: bool = False) -> dict:
+                         _print_log: bool = False) -> Optional[dict]:
 
         r = self._ga3_response_raw(
             start_date=start_date,
             end_date=end_date,
             ga_dimensions=ga_dimensions,
             ga_metrics=ga_metrics,
             ga_filters=ga_filters,
             filter_google_organic=filter_google_organic,
             raise_http_error=raise_http_error,
             page_token=None
         )
+        if r is None:
+            return None
+
         data = r.get('reports', [{}])[0].get('data', {}).get('rows', [])
         column_header = r.get('reports', [{}])[0].get('columnHeader')
         next_page_token = r.get('reports', [{}])[0].get('nextPageToken')
 
         while next_page_token:
             r = self._ga3_response_raw(
                 start_date=start_date,
```

### Comparing `pygoogalytics-0.2.6/pygoogalytics/googlepandas.py` & `pygoogalytics-0.2.7/pygoogalytics/googlepandas.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics/kwp_wrappers.py` & `pygoogalytics-0.2.7/pygoogalytics/kwp_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import logging
 import time
 
 import pandas as pd
 import numpy as np
 import uuid
 import re
 
@@ -54,15 +55,16 @@
 
     def get_campaigns(self) -> pd.DataFrame:
         query = """
             SELECT
               campaign.id,
               campaign.name
             FROM campaign
-            ORDER BY campaign.id"""
+            ORDER BY campaign.id
+        """
 
         # Issues a search request using streaming.
         stream = self.googleads_service.search_stream(customer_id=self.customer_id, query=query)
 
         _out = []
         for batch in stream:
             for row in batch.results:
@@ -296,30 +298,37 @@
         self.default_keyword_plan_campaign_cpc_bid_micros = DEFAULT_KEYWORD_PLAN_CAMPAIGN_CPC_BID
         self.default_keyword_plan_ad_group_cpc_bid_micros = DEFAULT_KEYWORD_PLAN_AD_GROUP_CPC_BID
 
     def get_keyword_metrics(self,
                             keywords: Union[List[str], str],
                             location_codes: List[str] = None,
                             language_id: str = None,
-                            print_progress: bool = False) -> Tuple[pd.DataFrame, pd.DataFrame]:
+                            print_progress: bool = False,
+                            calculated_fields: bool = True) -> Tuple[pd.DataFrame, pd.DataFrame]:
+
         if isinstance(keywords, str):
             keywords = [keywords]
 
         keyword_list_partition = _partition_list(_list=keywords, n=2_000)
         frames: List[pd.DataFrame] = []
         keyword_plans = []
 
         for _keyword_sublist in keyword_list_partition:
             try:
-                historical_metrics_df, _kwp = self.get_historical_metrics_df(keywords=_keyword_sublist,
-                                                                             location_codes=location_codes,
-                                                                             language_id=language_id)
-                keyword_plans.append(_kwp)
-                frames.append(historical_metrics_df)
-                self.remove_keyword_plan(keyword_plan_resource_name=_kwp)
+                historical_metrics_df, _kwp = self.get_historical_metrics_df(
+                    keywords=_keyword_sublist,
+                    location_codes=location_codes,
+                    language_id=language_id,
+                    calculated_fields=calculated_fields
+                )
+
+                if historical_metrics_df is not None:
+                    keyword_plans.append(_kwp)
+                    frames.append(historical_metrics_df)
+                    self.remove_keyword_plan(keyword_plan_resource_name=_kwp)
 
             except GoogleAdsException:
                 print(f"GoogleAdsException encountered after obtaining {len(frames)} frames")
                 break
 
             if print_progress:
                 print(f"{len(frames)} - obtained metrics for {len(frames[-1])} keywords")
@@ -331,15 +340,16 @@
         metrics_df: pd.DataFrame = _df.drop(columns=['volume_trend_tuples'])
 
         monthly_volume_df: pd.DataFrame = _df[['date_obtained',
                                                'query',
                                                'keyword',
                                                'status',
                                                'volume_trend_tuples']].explode('volume_trend_tuples')
-        monthly_volume_df['volume_trend_tuples'] = monthly_volume_df['volume_trend_tuples'].apply(_check_volume_trend_tuples)
+        monthly_volume_df['volume_trend_tuples'] = monthly_volume_df['volume_trend_tuples'].apply(
+            _check_volume_trend_tuples)
 
         monthly_volume_df['month_name'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[3])
         monthly_volume_df['month_enum'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[2])
         monthly_volume_df['month'] = monthly_volume_df['month_enum'].apply(_get_month_from_enum_value)
         monthly_volume_df['year'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[1])
 
         monthly_volume_df['volume'] = monthly_volume_df['volume_trend_tuples'].apply(lambda t: t[0])
@@ -371,42 +381,62 @@
         _df["keyword_id"] = _df["keyword_plan_ad_group_keyword"].apply(lambda s: int(s.split('/')[-1]))
         keywords_df["query"] = keywords_df["keyword_text"]
         _df = pd.merge(_df, keywords_df, how="left", on="keyword_id")
         _df = _df[['date_obtained', 'query', 'impressions', 'clicks', 'ctr', 'average_cpc', 'cost_micros']]
 
         return _df
 
-    def get_historical_metrics_df(self,
-                                  keywords: List[str],
-                                  location_codes: List[str] = None,
-                                  language_id: str = None) -> Tuple[pd.DataFrame, Any]:
-
-        try:
-            keyword_plan, stripped_keyword_dict = self.add_keyword_plan(keywords=keywords,
-                                                                        match_type="EXACT",
-                                                                        location_codes=location_codes,
-                                                                        language_id=language_id)
-            metrics = self.generate_historical_metrics(keyword_plan_resource_name=keyword_plan,
-                                                       stripped_keyword_dict=stripped_keyword_dict)
-            # self.remove_keyword_plan(keyword_plan_resource_name=keyword_plan)
-            _df = pd.DataFrame(metrics)
+    def _get_historical_metrics_df(self,
+                                   keywords: List[str],
+                                   location_codes: List[str] = None,
+                                   language_id: str = None,
+                                   calculated_fields: bool = True) -> Tuple[pd.DataFrame, Any]:
+        keyword_plan, stripped_keyword_dict = self.add_keyword_plan(keywords=keywords,
+                                                                    match_type="EXACT",
+                                                                    location_codes=location_codes,
+                                                                    language_id=language_id)
+        metrics = self.generate_historical_metrics(keyword_plan_resource_name=keyword_plan,
+                                                   stripped_keyword_dict=stripped_keyword_dict)
+        # self.remove_keyword_plan(keyword_plan_resource_name=keyword_plan)
+        _df = pd.DataFrame(metrics)
+        if calculated_fields:
             _df["volume_trend_coef"] = _df["volume_trend"].apply(_three_month_trend_coef)
             _df["volume"] = _df["volume_trend"].apply(_latest_volume)
             _df["volume_last_month"] = _df["volume_trend"].apply(_previous_volume)
             _df["volume_last_year"] = _df["volume_trend"].apply(_last_year_volume)
             _df["volume_3monthavg"] = _df["volume_trend"].apply(_volume_3monthavg)
             _df["volume_6monthavg"] = _df["volume_trend"].apply(_volume_6monthavg)
             _df["volume_12monthavg"] = _df["volume_trend"].apply(_volume_12monthavg)
-        except InternalServerError:
-            print("Keyword planner :: InternalServerError :: retrying after 2 seconds")
-            time.sleep(2)
-            _df, keyword_plan = self.get_historical_metrics_df(keywords=keywords,
-                                                               location_codes=location_codes,
-                                                               language_id=language_id
-                                                               )
+        return _df, keyword_plan
+
+    def get_historical_metrics_df(self,
+                                  keywords: List[str],
+                                  location_codes: List[str] = None,
+                                  language_id: str = None,
+                                  calculated_fields: bool = True,
+                                  max_retries: int = 5) -> Tuple[pd.DataFrame, Any]:
+
+        retries: int = 0
+        complete: bool = False
+        while retries < max_retries and complete is False:
+            try:
+                _df, keyword_plan = self._get_historical_metrics_df(
+                    keywords=keywords,
+                    location_codes=location_codes,
+                    language_id=language_id,
+                    calculated_fields=calculated_fields
+                )
+                complete = True
+            except InternalServerError:
+                logging.warning("Keyword planner :: InternalServerError :: retrying after 2 seconds")
+                time.sleep(2)
+                retries += 1
+
+        if complete is False:
+            return None, None
 
         return _df, keyword_plan
 
     def generate_forecast_metrics(self,
                                   keyword_plan_resource_name: str):
         response_forcast = self.keyword_plan_service.generate_forecast_metrics(
             keyword_plan=keyword_plan_resource_name,
@@ -930,16 +960,16 @@
 
 def strip_illegal_chars(s, language_id):
     # lower case obvs
     s = s.lower()
     # replace `‘’ with simple '
     s = re.sub(r"[`‘’]+", "'", s)
     # first remove any non-ascii characters, replace with a space
-    if language_id in ['1001']: # when german language_id don't replace one of [Ä, ä, Ö, ö, Ü, ü, ß]
-      s = re.sub(r"[^\x00-\x7F\xC4\xE4\xD6\xF6\xDC\xFC\xDF]+", " ", s)
+    if language_id in ['1001']:  # when german language_id don't replace one of [Ä, ä, Ö, ö, Ü, ü, ß]
+        s = re.sub(r"[^\x00-\x7F\xC4\xE4\xD6\xF6\xDC\xFC\xDF]+", " ", s)
     else:
-      s = re.sub(r"[^\x00-\x7F]+", " ", s)
+        s = re.sub(r"[^\x00-\x7F]+", " ", s)
     # then replace any punctuation with a space
     s = re.sub(r"""[!¡⁄@%^()={}:;,.+\-–—_±~“"#<>?/|*¶•ªº&\[\]\\]+""", " ", s)
     # finally, replace multiple spaces (r"\s+") with a single space
     s = re.sub(r"\s+", " ", s)
     return s.strip()
```

### Comparing `pygoogalytics-0.2.6/pygoogalytics/resource_utils.py` & `pygoogalytics-0.2.7/pygoogalytics/resource_utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics/utils.py` & `pygoogalytics-0.2.7/pygoogalytics/utils.py`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/pygoogalytics.egg-info/PKG-INFO` & `pygoogalytics-0.2.7/pygoogalytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygoogalytics
-Version: 0.2.6
+Version: 0.2.7
 Summary: PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 Home-page: https://github.com/Blink-SEO/pygoogalytics
 Author: Joshua Prettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygoogalytics-0.2.6/pygoogalytics.egg-info/SOURCES.txt` & `pygoogalytics-0.2.7/pygoogalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygoogalytics-0.2.6/setup.py` & `pygoogalytics-0.2.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # twine upload dist/*
 
 _desc = """PyGoogalytics allows a user to quickly and simply download Google Analytics and Google Search Console data
 in the form of a pandas dataframe."""
 
 setup(
     name='pygoogalytics',
-    version='0.2.6',
+    version='0.2.7',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Blink-SEO/pygoogalytics',
     author='Joshua Prettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

