# Comparing `tmp/simfin-0.9.0.tar.gz` & `tmp/simfin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfin-0.9.0.tar", last modified: Wed Feb 22 13:22:05 2023, max compression
+gzip compressed data, was "simfin-0.9.1.tar", last modified: Thu Apr 13 14:14:22 2023, max compression
```

## Comparing `simfin-0.9.0.tar` & `simfin-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-02-22 13:22:05.498882 simfin-0.9.0/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1259 2023-02-22 12:33:47.000000 simfin-0.9.0/LICENSE.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-02-22 13:22:05.498719 simfin-0.9.0/PKG-INFO
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7352 2023-02-22 12:33:47.000000 simfin-0.9.0/README.md
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)       38 2023-02-22 13:22:05.498923 simfin-0.9.0/setup.cfg
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1008 2023-02-22 13:21:56.000000 simfin-0.9.0/setup.py
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-02-22 13:22:05.497889 simfin-0.9.0/simfin/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1621 2023-02-22 13:21:56.000000 simfin-0.9.0/simfin/__init__.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11769 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/cache.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     4917 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/config.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    10036 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/datasets.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     6944 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/derived.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11022 2023-02-22 13:21:56.000000 simfin-0.9.0/simfin/download.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      743 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/exceptions.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    31133 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/hubs.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     8872 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/info.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11568 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/load.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     2925 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/load_info.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    19450 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/names.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7990 2023-02-22 13:21:56.000000 simfin-0.9.0/simfin/names_extra.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     3830 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/paths.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    17189 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/rel_change.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14284 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/resample.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    37350 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/signals.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14331 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/transform.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    13979 2023-02-22 12:33:47.000000 simfin-0.9.0/simfin/utils.py
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-02-22 13:22:05.498549 simfin-0.9.0/simfin.egg-info/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-02-22 13:22:05.000000 simfin-0.9.0/simfin.egg-info/PKG-INFO
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      521 2023-02-22 13:22:05.000000 simfin-0.9.0/simfin.egg-info/SOURCES.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)        1 2023-02-22 13:22:05.000000 simfin-0.9.0/simfin.egg-info/dependency_links.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)       22 2023-02-22 13:22:05.000000 simfin-0.9.0/simfin.egg-info/requires.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)        7 2023-02-22 13:22:05.000000 simfin-0.9.0/simfin.egg-info/top_level.txt
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-04-13 14:14:22.044146 simfin-0.9.1/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1259 2023-02-22 12:33:47.000000 simfin-0.9.1/LICENSE.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-04-13 14:14:22.043950 simfin-0.9.1/PKG-INFO
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7352 2023-02-22 12:33:47.000000 simfin-0.9.1/README.md
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)       38 2023-04-13 14:14:22.044205 simfin-0.9.1/setup.cfg
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1008 2023-04-13 14:10:04.000000 simfin-0.9.1/setup.py
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-04-13 14:14:22.042936 simfin-0.9.1/simfin/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1621 2023-04-13 14:11:07.000000 simfin-0.9.1/simfin/__init__.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11769 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/cache.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     4917 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/config.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    10036 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/datasets.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     6944 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/derived.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11021 2023-04-13 14:10:11.000000 simfin-0.9.1/simfin/download.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      743 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/exceptions.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    31133 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/hubs.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     8872 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/info.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11940 2023-04-13 14:10:11.000000 simfin-0.9.1/simfin/load.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     2925 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/load_info.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    19450 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/names.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7990 2023-02-22 13:21:56.000000 simfin-0.9.1/simfin/names_extra.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     3830 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/paths.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    17189 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/rel_change.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14284 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/resample.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    37350 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/signals.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14331 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/transform.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    15933 2023-04-13 14:10:11.000000 simfin-0.9.1/simfin/utils.py
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-04-13 14:14:22.043708 simfin-0.9.1/simfin.egg-info/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/PKG-INFO
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      521 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)        1 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)       22 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/requires.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)        7 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/top_level.txt
```

### Comparing `simfin-0.9.0/LICENSE.txt` & `simfin-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/PKG-INFO` & `simfin-0.9.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simple financial data for Python
 Home-page: https://github.com/simfin/simfin
 Author: SimFin
 Author-email: info@simfin.com
 License: MIT
 Keywords: financial data,finance
 Description-Content-Type: text/markdown
```

### Comparing `simfin-0.9.0/README.md` & `simfin-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/setup.py` & `simfin-0.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 # This is also defined in simfin/__init__.py and must be
 # updated in both places.
-MY_VERSION = '0.9.0'
+MY_VERSION = '0.9.1'
 
 setup(
     name='simfin',
     packages=['simfin'],
     version=MY_VERSION,
     description='Simple financial data for Python',
     long_description='SimFin makes it easy to obtain and use financial and '
```

### Comparing `simfin-0.9.0/simfin/__init__.py` & `simfin-0.9.1/simfin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This is also defined in setup.py and must be updated in both places.
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 # Expose the following as top-level imports.
 
 from simfin.cache import cache
 from simfin.config import set_api_key, load_api_key, get_api_key
 from simfin.config import set_data_dir, get_data_dir, get_download_dir
 from simfin.derived import ebitda, free_cash_flow, shares
```

### Comparing `simfin-0.9.0/simfin/cache.py` & `simfin-0.9.1/simfin/cache.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/config.py` & `simfin-0.9.1/simfin/config.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/datasets.py` & `simfin-0.9.1/simfin/datasets.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/derived.py` & `simfin-0.9.1/simfin/derived.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/download.py` & `simfin-0.9.1/simfin/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
     # Market.
     if market is not None:
         args += '&market=' + market
 
     # Base URL for the bulk-download API on the SimFin server.
     base_url = 'https://backend.simfin.com/api/bulk-download?'
-
     # Combine base URL and arguments.
     url = base_url + args
 
     return url
 
 
 def _url_info(name):
```

### Comparing `simfin-0.9.0/simfin/exceptions.py` & `simfin-0.9.1/simfin/exceptions.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/hubs.py` & `simfin-0.9.1/simfin/hubs.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/info.py` & `simfin-0.9.1/simfin/info.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/load.py` & `simfin-0.9.1/simfin/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 import pandas as pd
 from functools import partial
 
 from simfin.paths import _path_dataset
 from simfin.download import _maybe_download_dataset
 from simfin.names import TICKER, INDUSTRY_ID, MARKET_ID
 from simfin.names import DATE, REPORT_DATE, PUBLISH_DATE, RESTATED_DATE
+from simfin.utils import _filtered_file
+
 
 ##########################################################################
 # Load function.
 
-def load(dataset, variant=None, market=None,
+def load(dataset, variant=None, market=None, start_date=None, end_date=None,
          parse_dates=None, index=None, refresh_days=30):
     """
     Load the dataset from local disk and return it as a Pandas DataFrame.
     If the dataset does not exist on local disk, or if it is too old, then it
     is automatically downloaded from the SimFin server.
 
     This is the main function for downloading and loading datasets. It is
@@ -87,14 +89,20 @@
             - 'us': USA
             - 'de': Germany
             - 'sg': Singapore
 
         Some datasets such as 'industries' do not support the market-keyword
         and will generate a server-error if the market is set.
 
+    :param start_date:
+        datetime or string of format YYYY-MM-DD
+
+    :param end_date:
+        datetime or string of format YYYY-MM-DD
+
     :param parse_dates:
         String or list of strings with column-names that contain dates
         to be parsed. This depends on the dataset.
         For fundamental data it is [REPORT_DATE, PUBLISH_DATE, RESTATED_DATE].
         For shareprices it is [DATE].
         Format is always assumed to be YYYY-MM-DD.
 
@@ -135,15 +143,17 @@
     date_parser = lambda x: pd.to_datetime(x, yearfirst=True, dayfirst=False)
 
     # Print status message.
     print('- Loading from disk ... ', end='')
 
     # Full path for the CSV-file on local disk.
     path = _path_dataset(**dataset_args)
-
+    if start_date or end_date:
+        print('\n- Applying filter ... ', end='')
+        path = _filtered_file(path, start_date, end_date=end_date)
     # Load dataset into Pandas DataFrame.
     df = pd.read_csv(path, sep=';', header=0,
                      parse_dates=parse_dates, date_parser=date_parser)
 
     # Set the index and sort the data.
     if index is not None:
         # Set the index.
@@ -153,14 +163,15 @@
         df.sort_index(ascending=True, inplace=True)
 
     # Print status message.
     print('Done!')
 
     return df
 
+
 ##########################################################################
 # Specialized functions for loading datasets with fundamental data:
 # Income Statements, Balance Sheets and Cash-Flow Statements.
 
 # These are implemented very easily using functools.partial() which sets
 # some of the args in the load() function above. These args can still be
 # changed when the user calls the specialized functions.
@@ -240,20 +251,20 @@
 ##########################################################################
 
 ##########################################################################
 # Specialized functions for the 'derived' and 'derived-shareprices' datasets.
 
 load_derived = partial(load_fundamental, dataset='derived')
 load_derived.__doc__ = 'Load derived figures & ratios for all companies except banks ' \
-                      'and insurance companies.' + _DOC_LOAD
+                       'and insurance companies.' + _DOC_LOAD
 
 load_derived_banks = partial(load_fundamental, dataset='derived-banks')
 load_derived_banks.__doc__ = 'Load derived figures & ratios for banks.' + _DOC_LOAD
 
 load_derived_insurance = partial(load_fundamental, dataset='derived-insurance')
 load_derived_insurance.__doc__ = 'Load derived figures & ratios for insurance companies.' + _DOC_LOAD
 
 load_derived_shareprices = partial(load, dataset='derived-shareprices', variant='latest', market='us',
-                           index=[TICKER, DATE], parse_dates=[DATE])
+                                   index=[TICKER, DATE], parse_dates=[DATE])
 load_derived_shareprices.__doc__ = 'Load share-price ratios.' + _DOC_LOAD
 
 ##########################################################################
```

### Comparing `simfin-0.9.0/simfin/load_info.py` & `simfin-0.9.1/simfin/load_info.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/names.py` & `simfin-0.9.1/simfin/names.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/names_extra.py` & `simfin-0.9.1/simfin/names_extra.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/paths.py` & `simfin-0.9.1/simfin/paths.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/rel_change.py` & `simfin-0.9.1/simfin/rel_change.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/resample.py` & `simfin-0.9.1/simfin/resample.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/signals.py` & `simfin-0.9.1/simfin/signals.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/transform.py` & `simfin-0.9.1/simfin/transform.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.0/simfin/utils.py` & `simfin-0.9.1/simfin/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # www.simfin.com - www.github.com/simfin/simfin
 # See README.md for instructions and LICENSE.txt for license details.
 ##########################################################################
 
 import pandas as pd
 import os
 import time
-from datetime import timedelta
+import csv
+from datetime import timedelta, datetime
 
 from simfin.names import REPORT_DATE, TICKER
 
 ##########################################################################
 # Constants.
 
 #: Average number of business- or trading-days in a year.
@@ -30,14 +31,15 @@
 
 #: Number of months per year.
 MONTHS_PER_YEAR = 12
 
 #: Number of quarters per year.
 QUARTERS_PER_YEAR = 4
 
+
 ##########################################################################
 
 def add_date_offset(df, date_index=REPORT_DATE, offset=pd.DateOffset(days=90)):
     """
     Add an offset to the date-index of a Pandas DataFrame.
 
     This is useful if you want to add a lag of e.g. 3 months
@@ -79,14 +81,15 @@
     df2[date_index] += offset
 
     # Reinsert the dates into the index.
     df2 = df2.set_index(date_index, append=True)
 
     return df2
 
+
 ##########################################################################
 
 def apply(df, func, group_index=TICKER, **kwargs):
     """
     Apply a function to a Pandas DataFrame or Series with either a
     DatetimeIndex or MultiIndex. This is useful when you don't know
     whether a DataFrame contains data for a single or multiple stocks.
@@ -148,14 +151,15 @@
         # Split the DataFrame into sub-groups and perform
         # the operation on each sub-group and glue the
         # results back together into a single DataFrame.
         df_result = df.groupby(group_index).apply(_apply_group)
 
     return df_result
 
+
 ##########################################################################
 
 def convert_to_periods(freq, bdays=0, days=0, weeks=0,
                        months=0, quarters=0, years=0):
     """
     Convert the number of days, weeks, months, quarters and years
     into the equivalent number of periods that a DataFrame must be
@@ -244,14 +248,15 @@
         raise ValueError(msg)
 
     # Convert periods to int, it should already be rounded to nearest number.
     periods = int(periods)
 
     return periods, shifted_years
 
+
 ##########################################################################
 
 def rename_columns(df, new_names, inplace=False):
     """
     Rename the columns in a Pandas DataFrame or Series. This function
     is useful because the syntax is slightly different for DataFrame and
     Series (this is one of many annoying inconsistencies in Pandas).
@@ -287,14 +292,15 @@
         assert isinstance(new_names, str)
 
         # Rename the single "column" of a Series.
         df = df.rename(new_names, inplace=inplace)
 
     return df
 
+
 ##########################################################################
 # Functions for file-dates.
 
 def _file_age(path):
     """
     Return the age of the file with the given path, as the difference
     between the current time minus the file's last modification time.
@@ -373,25 +379,84 @@
     located in `other_paths`. This is a simple wrapper for `is_file_newer`.
 
     :param kwargs: Keyword args passed to `is_file_newer`.
     :return: Boolean.
     """
     return not _is_file_newer(**kwargs)
 
+
 ##########################################################################
 
 def _is_str_or_list_str(s):
     """
     Return boolean whether `s` is a string or list of strings.
     """
     return isinstance(s, str) or \
-          (isinstance(s, list) and all(isinstance(x, str) for x in s))
+        (isinstance(s, list) and all(isinstance(x, str) for x in s))
+
 
 ##########################################################################
 
 def _func_name(func):
     """
     Return the name of the function, or None if `func` is None.
     """
     return None if func is None else func.__name__
 
+
 ##########################################################################
+
+def _into_date(date):
+    if date is None:
+        return None
+    if isinstance(date, str):
+        return datetime.strptime(date, '%Y-%m-%d')
+    if isinstance(date, datetime):
+        return date
+    else:
+        raise Exception("filters date not in format")
+
+
+def _condition_function(start_date=None, end_date=None):
+    if start_date is not None:
+        if end_date is not None:
+            return lambda x: start_date < x < end_date
+        else:
+            return lambda x: start_date < x
+    else:
+        if end_date is not None:
+            return lambda x: x < end_date
+        else:
+            return None
+
+
+def _filtered_file(dataset_path, start_date=None, end_date=None):
+    start_date = _into_date(start_date)
+    end_date = _into_date(end_date)
+
+    con_fun = _condition_function(start_date, end_date)
+    # write new data file
+    new_file_name = os.path.basename(dataset_path)[0:-4] + "_filtered.csv"
+    new_file_path = os.path.join(os.path.dirname(dataset_path), new_file_name)
+
+    with open(new_file_path, 'w', newline='') as csvfile:
+        writer = csv.writer(csvfile, delimiter=';', quotechar='"')
+
+        with open(dataset_path) as csvfile:
+            datareader = csv.reader(csvfile, delimiter=';', quotechar='"')
+            index = 0
+            rd_col = "Report Date"
+            d_col = "Date"
+            for k, row in enumerate(datareader):
+                if k == 0:
+                    if rd_col in row:
+                        index = row.index(rd_col)
+                    elif d_col in row:
+                        index = row.index(d_col)
+                    else:
+                        raise ValueError("Date Column not found")
+                    writer.writerow(row)
+                if k > 0:
+                    date = datetime.strptime(str(row[index]), '%Y-%m-%d')
+                    if con_fun(date):
+                        writer.writerow(row)
+    return new_file_path
```

### Comparing `simfin-0.9.0/simfin.egg-info/PKG-INFO` & `simfin-0.9.1/simfin.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simple financial data for Python
 Home-page: https://github.com/simfin/simfin
 Author: SimFin
 Author-email: info@simfin.com
 License: MIT
 Keywords: financial data,finance
 Description-Content-Type: text/markdown
```

### Comparing `simfin-0.9.0/simfin.egg-info/SOURCES.txt` & `simfin-0.9.1/simfin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

