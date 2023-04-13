# Comparing `tmp/thetadata-0.9.0.tar.gz` & `tmp/thetadata-0.9.1.tar.gz`

## Comparing `thetadata-0.9.0.tar` & `thetadata-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.0/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.0/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/reference.md
--rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/quote_1min.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/trade_streaming.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.0/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.0/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.0/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/__init__.py
--rw-r--r--   0        0        0    42084 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/client.py
--rw-r--r--   0        0        0    19847 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/exceptions.py
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/py.typed
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 thetadata-0.9.0/thetadata/terminal.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 thetadata-0.9.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.0/LICENSE
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.0/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 thetadata-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 thetadata-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.1/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.1/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/reference.md
+-rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/quote_1min.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.1/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.1/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/__init__.py
+-rw-r--r--   0        0        0    56803 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/client.py
+-rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/py.typed
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.1/LICENSE
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.1/README.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 thetadata-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 thetadata-0.9.1/PKG-INFO
```

### Comparing `thetadata-0.9.0/mkdocs.yml` & `thetadata-0.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/.github/workflows/main.yml` & `thetadata-0.9.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/.github/workflows/python-publish.yml` & `thetadata-0.9.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/connection_msgs.py` & `thetadata-0.9.1/docs/connection_msgs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/explanation.md` & `thetadata-0.9.1/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/how-to-guides.md` & `thetadata-0.9.1/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/index.md` & `thetadata-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/logo.png` & `thetadata-0.9.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/manipulate_series.py` & `thetadata-0.9.1/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/tutorials.md` & `thetadata-0.9.1/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/cancel_streams.py` & `thetadata-0.9.1/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/eod.py` & `thetadata-0.9.1/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/get_last.py` & `thetadata-0.9.1/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/open_interest_streaming.py` & `thetadata-0.9.1/docs/options/open_interest_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/quote_1min.py` & `thetadata-0.9.1/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/quote_tick.py` & `thetadata-0.9.1/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/trade_streaming.py` & `thetadata-0.9.1/docs/options/trade_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/options/trade_streaming_full.py` & `thetadata-0.9.1/docs/options/trade_streaming_full.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/stocks/eod.py` & `thetadata-0.9.1/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/stocks/get_last.py` & `thetadata-0.9.1/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/stocks/quote_1min.py` & `thetadata-0.9.1/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/docs/stocks/quote_tick.py` & `thetadata-0.9.1/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/tests/test_client.py` & `thetadata-0.9.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/tests/test_docs.py` & `thetadata-0.9.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/thetadata/client.py` & `thetadata-0.9.1/thetadata/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Module that contains Theta Client class."""
 import datetime
 import threading
+import time
+import traceback
 from decimal import Decimal
 from threading import Thread
 from time import sleep
 from typing import Optional
 from contextlib import contextmanager
 
 import socket
+import requests
 
 from pandas import DataFrame
 from tqdm import tqdm
 import pandas as pd
 
 from . import terminal
 from .enums import *
 from .parsing import (
     Header,
     TickBody,
     ListBody,
+    parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
 _VERSION = '0.9.0'
-
+URL_BASE = "http://localhost:25510/"
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
 
 
 def _format_date(dt: date) -> str:
@@ -517,15 +521,16 @@
                     raise ValueError('undefined msg type: ' + str(msg.type))
             except ConnectionResetError:
                 msg.type = StreamMsgType.STREAM_DEAD
                 self._stream_impl(msg)
                 return
             except Exception as e:
                 msg.type = StreamMsgType.ERROR
-                print('Stream error: ' + str(e))
+                print('Stream error for contract: ' + msg.contract.to_string())
+                traceback.print_exc()
             self._stream_impl(msg)
 
     def _read_stream(self, n_bytes: int) -> bytearray:
         """from_bytes
           """
 
         buffer = bytearray(self._stream_server.recv(n_bytes))
@@ -639,14 +644,62 @@
         header: Header = Header.parse(hist_msg, header_data)
 
         # parse response body
         body_data = self._recv(header.size, progress_bar=progress_bar)
         body: DataFrame = TickBody.parse(hist_msg, header, body_data)
         return body
 
+    def get_hist_option_REST(
+        self,
+        req: OptionReqType,
+        root: str,
+        exp: date,
+        strike: float,
+        right: OptionRight,
+        date_range: DateRange,
+        interval_size: int = 0,
+        use_rth: bool = True,
+    ) -> pd.DataFrame:
+        """
+         Get historical options data.
+
+        :param req:            The request type.
+        :param root:           The root / underlying / ticker / symbol.
+        :param exp:            The expiration date. Must be after the start of `date_range`.
+        :param strike:         The strike price in USD, rounded to 1/10th of a cent.
+        :param right:          The right of an option. CALL = Bullish; PUT = Bearish
+        :param date_range:     The dates to fetch.
+        :param interval_size:  The interval size in milliseconds. Applicable to most requests except ReqType.TRADE.
+        :param use_rth:        If true, timestamps prior to 09:30 EST and after 16:00 EST will be ignored
+                                  (only applicable to intervals requests).
+
+        :return:               The requested data as a pandas DataFrame.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        req_fmt = req.name.lower()
+        strike_fmt = _format_strike(strike)
+        exp_fmt = _format_date(exp)
+        start_fmt = _format_date(date_range.start)
+        end_fmt = _format_date(date_range.end)
+        right_fmt = right.value
+        use_rth_fmt = str(use_rth).lower()
+        url = f"http://localhost:25510/hist/option/{req_fmt}"
+        querystring = {"root": root, "start_date": start_fmt, "end_date": end_fmt,
+                       "strike": strike_fmt, "exp": exp_fmt, "right": right_fmt,
+                       "ivl": interval_size, "rth": use_rth_fmt}
+        t1 = time.time()
+        response = requests.get(url, params=querystring)
+        t2 = time.time()
+        df = parse_flexible_REST(response)
+        t3 = time.time()
+        print(f'time for request.get: {t2-t1}')
+        print(f'time for parse_flexible_REST(): {t3-t2}')
+        return df
+
     def get_opt_at_time(
             self,
             req: OptionReqType,
             root: str,
             exp: date,
             strike: float,
             right: OptionRight,
@@ -684,14 +737,54 @@
         header: Header = Header.parse(hist_msg, header_data)
 
         # parse response body
         body_data = self._recv(header.size, progress_bar=False)
         body: DataFrame = TickBody.parse(hist_msg, header, body_data)
         return body
 
+    def get_opt_at_time_REST(
+            self,
+            req: OptionReqType,
+            root: str,
+            exp: date,
+            strike: float,
+            right: OptionRight,
+            date_range: DateRange,
+            ms_of_day: int = 0,
+    ) -> pd.DataFrame:
+        """
+         Returns the last tick at a provided millisecond of the day for a given request type.
+
+        :param req:            The request type.
+        :param root:           The root / underlying / ticker / symbol.
+        :param exp:            The expiration date. Must be after the start of `date_range`.
+        :param strike:         The strike price in USD, rounded to 1/10th of a cent.
+        :param right:          The right of an option. CALL = Bullish; PUT = Bearish
+        :param date_range:     The dates to fetch.
+        :param ms_of_day:      The time of day in milliseconds.
+
+        :return:               The requested data as a pandas DataFrame.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        # format data
+        req_fmt = req.name.lower()
+        strike_fmt = _format_strike(strike)
+        exp_fmt = _format_date(exp)
+        start_fmt = _format_date(date_range.start)
+        end_fmt = _format_date(date_range.end)
+        right_fmt = right.value
+
+        url = f"http://localhost:25510/at_time/option/{req_fmt}"
+        querystring = {"root": root, "start_date": start_fmt, "end_date": end_fmt, "strike": strike_fmt,
+                       "exp": exp_fmt, "right": right_fmt, "ivl": ms_of_day}
+        response = requests.get(url, params=querystring)
+        df = parse_flexible_REST(response)
+        return df
+
     def get_stk_at_time(
             self,
             req: StockReqType,
             root: str,
             date_range: DateRange,
             ms_of_day: int = 0,
     ) -> pd.DataFrame:
@@ -721,14 +814,45 @@
         header: Header = Header.parse(hist_msg, header_data)
 
         # parse response body
         body_data = self._recv(header.size, progress_bar=False)
         body: DataFrame = TickBody.parse(hist_msg, header, body_data)
         return body
 
+    def get_stk_at_time_REST(
+            self,
+            req: StockReqType,
+            root: str,
+            date_range: DateRange,
+            ms_of_day: int = 0,
+    ) -> pd.DataFrame:
+        """
+         Returns the last tick at a provided millisecond of the day for a given request type.
+
+        :param req:            The request type.
+        :param root:           The root / underlying / ticker / symbol.
+        :param date_range:     The dates to fetch.
+        :param ms_of_day:      The time of day in milliseconds.
+
+        :return:               The requested data as a pandas DataFrame.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        req_fmt = req.name.lower()
+        root_fmt = root.lower()
+        start_fmt = _format_date(date_range.start)
+        end_fmt = _format_date(date_range.end)
+
+        url = f"http://localhost:25510/at_time/stock/{req_fmt}"
+        querystring = {"root": root_fmt, "start_date": start_fmt,
+                       "end_date": end_fmt, "ivl": ms_of_day}
+        response = requests.get(url, params=querystring)
+        df = parse_flexible_REST(response)
+        return df
+
     def get_hist_stock(
             self,
             req: StockReqType,
             root: str,
             date_range: DateRange,
             interval_size: int = 0,
             use_rth: bool = True,
@@ -762,14 +886,47 @@
         header: Header = Header.parse(hist_msg, header_data)
 
         # parse response body
         body_data = self._recv(header.size, progress_bar=progress_bar)
         body: DataFrame = TickBody.parse(hist_msg, header, body_data)
         return body
 
+    def get_hist_stock_REST(
+            self,
+            req: StockReqType,
+            root: str,
+            date_range: DateRange,
+            interval_size: int = 0,
+            use_rth: bool = True,
+    ) -> pd.DataFrame:
+        """
+         Get historical stock data.
+
+        :param req:            The request type.
+        :param root:           The root symbol.
+        :param date_range:     The dates to fetch.
+        :param interval_size:  The interval size in milliseconds. Applicable only to OHLC & QUOTE requests.
+        :param use_rth:         If true, timestamps prior to 09:30 EST and after 16:00 EST will be ignored.
+
+        :return:               The requested data as a pandas DataFrame.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        # format data
+        req_fmt = req.name.lower()
+        start_fmt = _format_date(date_range.start)
+        end_fmt = _format_date(date_range.end)
+        use_rth_fmt = str(use_rth).lower()
+        url = f"http://localhost:25510/hist/stock/{req_fmt}"
+        params = {"root": root, "start_date": start_fmt, "end_date": end_fmt,
+                      "ivl": interval_size, "rth": use_rth_fmt}
+        response = requests.get(url, params=params)
+        df = parse_flexible_REST(response)
+        return df
+
     # LISTING DATA
 
     def get_dates_stk(self, root: str, req: StockReqType) -> pd.Series:
         """
         Get all dates of data available for a given stock contract and request type.
 
         :param req:            The request type.
@@ -782,14 +939,33 @@
         assert self._server is not None, _NOT_CONNECTED_MSG
         out = f"MSG_CODE={MessageType.ALL_DATES.value}&root={root}&sec={SecType.STOCK.value}&req={req.value}\n"
         self._server.send(out.encode("utf-8"))
         header = Header.parse(out, self._server.recv(20))
         body = ListBody.parse(out, header, self._recv(header.size), dates=True)
         return body.lst
 
+    def get_dates_stk_REST(self, root: str, req: StockReqType) -> pd.Series:
+        """
+        Get all dates of data available for a given stock contract and request type.
+
+        :param req:            The request type.
+        :param root:           The root / underlying / ticker / symbol.
+
+        :return:               dAll dates that Theta Data provides data for given a request.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        root_fmt = root.lower()
+        req_fmt = req.name.lower()
+        url = f"http://localhost:25510/list/dates/stock/{req_fmt}"
+        params = {'root': root_fmt}
+        response = requests.get(url, params=params)
+        series = parse_list_REST(response, dates=True)
+        return series
+
     def get_dates_opt(
             self,
             req: OptionReqType,
             root: str,
             exp: date,
             strike: float,
             right: OptionRight) -> pd.Series:
@@ -811,14 +987,45 @@
         exp_fmt = _format_date(exp)
         out = f"MSG_CODE={MessageType.ALL_DATES.value}&root={root}&exp={exp_fmt}&strike={strike}&right={right.value}&sec={SecType.OPTION.value}&req={req.value}\n"
         self._server.send(out.encode("utf-8"))
         header = Header.parse(out, self._server.recv(20))
         body = ListBody.parse(out, header, self._recv(header.size), dates=True)
         return body.lst
 
+    def get_dates_opt_REST(
+            self,
+            req: OptionReqType,
+            root: str,
+            exp: date,
+            strike: float,
+            right: OptionRight) -> pd.Series:
+        """
+        Get all dates of data available for a given options contract and request type.
+
+        :param req:            The request type.
+        :param root:           The root / underlying / ticker / symbol.
+        :param exp:            The expiration date. Must be after the start of `date_range`.
+        :param strike:         The strike price in USD.
+        :param right:          The right of an options.
+
+        :return:               All dates that Theta Data provides data for given a request.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        req = req.name.lower()
+        exp_fmt = _format_date(exp)
+        strike_fmt = _format_strike(strike)
+        right = right.value
+        sec = SecType.OPTION.value.lower()
+        url = f"http://localhost:25510/list/dates/{sec}/{req}"
+        params = {'root': root, 'exp': exp_fmt, 'strike': strike_fmt, 'right': right}
+        response = requests.get(url, params=params)
+        df = parse_list_REST(response, dates=True)
+        return df
+
     def get_dates_opt_bulk(
             self,
             req: OptionReqType,
             root: str,
             exp: date) -> pd.Series:
         """
         Get all dates of data available for a given options expiration and request type.
@@ -835,14 +1042,41 @@
         exp_fmt = _format_date(exp)
         out = f"MSG_CODE={MessageType.ALL_DATES_BULK.value}&root={root}&exp={exp_fmt}&sec={SecType.OPTION.value}&req={req.value}\n"
         self._server.send(out.encode("utf-8"))
         header = Header.parse(out, self._server.recv(20))
         body = ListBody.parse(out, header, self._recv(header.size), dates=True)
         return body.lst
 
+    def get_dates_opt_bulk_REST(
+            self,
+            req: OptionReqType,
+            root: str,
+            exp: date) -> pd.Series:
+        """
+        Get all dates of data available for a given options contract and request type.
+
+        :param req:            The request type.
+        :param root:           The root / underlying / ticker / symbol.
+        :param exp:            The expiration date. Must be after the start of `date_range`.
+        :param strike:         The strike price in USD.
+        :param right:          The right of an options.
+
+        :return:               All dates that Theta Data provides data for given a request.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        req = req.name.lower()
+        exp_fmt = _format_date(exp)
+        sec = SecType.OPTION.value.lower()
+        url = f"http://localhost:25510/list/dates/{sec}/{req}"
+        params = {'root': root, 'exp': exp_fmt}
+        response = requests.get(url, params=params)
+        df = parse_list_REST(response, dates=True)
+        return df
+
     def get_expirations(self, root: str) -> pd.Series:
         """
         Get all options expirations for a provided underlying root.
 
         :param root:           The root / underlying / ticker / symbol.
 
         :return:               All expirations that ThetaData provides data for.
@@ -852,14 +1086,30 @@
         assert self._server is not None, _NOT_CONNECTED_MSG
         out = f"MSG_CODE={MessageType.ALL_EXPIRATIONS.value}&root={root}\n"
         self._server.send(out.encode("utf-8"))
         header = Header.parse(out, self._server.recv(20))
         body = ListBody.parse(out, header, self._recv(header.size), dates=True)
         return body.lst
 
+    def get_expirations_REST(self, root: str) -> pd.Series:
+        """
+        Get all options expirations for a provided underlying root.
+
+        :param root:           The root / underlying / ticker / symbol.
+
+        :return:               All expirations that ThetaData provides data for.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        url = "http://localhost:25510/list/expirations"
+        params = {"root": root}
+        response = requests.get(url, params=params)
+        df = parse_list_REST(response)
+        return df
+
     def get_strikes(self, root: str, exp: date, date_range: DateRange = None,) -> pd.Series:
         """
         Get all options strike prices in US tenths of a cent.
 
         :param root:           The root / underlying / ticker / symbol.
         :param exp:            The expiration date.
         :param date_range:     If specified, this function will return strikes only if they have data for every
@@ -887,14 +1137,43 @@
         c = 0
         for i in body:
             s[c] = Decimal(i) / div
             c += 1
 
         return s
 
+
+    def get_strikes_REST(self, root: str, exp: date, date_range: DateRange = None,) -> pd.Series:
+        """
+        Get all options strike prices in US tenths of a cent.
+
+        :param root:           The root / underlying / ticker / symbol.
+        :param exp:            The expiration date.
+        :param date_range:     If specified, this function will return strikes only if they have data for every
+                                day in the date range.
+
+        :return:               The strike prices on the expiration.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        assert isinstance(exp, date)
+        exp_fmt = _format_date(exp)
+        root_fmt = root.lower()
+        if date_range is not None:
+            start_fmt = _format_date(date_range.start)
+            end_fmt = _format_date(date_range.end)
+            querystring = {"root": root_fmt, "exp": exp_fmt}
+        else:
+            querystring = {"root": root_fmt, "exp": exp_fmt}
+        url = "http://localhost:25510/list/strikes"
+        response = requests.get(url, params=querystring)
+        ser = parse_list_REST(response)
+        ser = ser.divide(1000)
+        return ser
+
     def get_roots(self, sec: SecType) -> pd.Series:
         """
         Get all roots for a certain security type.
 
         :param sec: The type of security.
 
         :return: All roots / underlyings / tickers / symbols for the security type.
@@ -904,14 +1183,30 @@
         assert self._server is not None, _NOT_CONNECTED_MSG
         out = f"MSG_CODE={MessageType.ALL_ROOTS.value}&sec={sec.value}\n"
         self._server.send(out.encode("utf-8"))
         header = Header.parse(out, self._server.recv(20))
         body = ListBody.parse(out, header, self._recv(header.size))
         return body.lst
 
+    def get_roots_REST(self, sec: SecType) -> pd.Series:
+        """
+        Get all roots for a certain security type.
+
+        :param sec: The type of security.
+
+        :return: All roots / underlyings / tickers / symbols for the security type.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        url = "http://localhost:25510/list/roots"
+        params = {'sec': sec.value}
+        response = requests.get(url, params=params)
+        df = parse_list_REST(response)
+        return df
+
     # LIVE DATA
 
     def get_last_option(
         self,
         req: OptionReqType,
         root: str,
         exp: date,
@@ -943,14 +1238,47 @@
         # parse response
         header: Header = Header.parse(hist_msg, self._server.recv(20))
         body: DataFrame = TickBody.parse(
             hist_msg, header, self._recv(header.size)
         )
         return body
 
+    def get_last_option_REST(
+        self,
+        req: OptionReqType,
+        root: str,
+        exp: date,
+        strike: float,
+        right: OptionRight,
+    ) -> pd.DataFrame:
+        """
+        Get the most recent options tick.
+
+        :param req:            The request type.
+        :param root:           The root symbol.
+        :param exp:            The expiration date.
+        :param strike:         The strike price in USD, rounded to 1/10th of a cent.
+        :param right:          The right of an options.
+
+        :return:               The requested data as a pandas DataFrame.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        root_fmt = root.lower()
+        req_fmt = req.name.lower()
+        right_fmt = right.value
+        strike_fmt = _format_strike(strike)
+        exp_fmt = _format_date(exp)
+
+        url = f"http://localhost:25510/snapshot/option/{req_fmt}"
+        querystring = {"root": root_fmt, "strike": strike_fmt, "exp": exp_fmt, "right": right_fmt}
+        response = requests.get(url, params=querystring)
+        df = parse_flexible_REST(response)
+        return df
+
     def get_last_stock(
         self,
         req: StockReqType,
         root: str,
     ) -> pd.DataFrame:
         """
         Get the most recent stock tick.
@@ -971,14 +1299,41 @@
         # parse response
         header: Header = Header.parse(hist_msg, self._server.recv(20))
         body: DataFrame = TickBody.parse(
             hist_msg, header, self._recv(header.size)
         )
         return body
 
+    def get_last_stock_REST(
+        self,
+        req: StockReqType,
+        root: str,
+    ) -> pd.DataFrame:
+        """
+        Get the most recent options tick.
+
+        :param req:            The request type.
+        :param root:           The root symbol.
+        :param exp:            The expiration date.
+        :param strike:         The strike price in USD, rounded to 1/10th of a cent.
+        :param right:          The right of an options.
+
+        :return:               The requested data as a pandas DataFrame.
+        :raises ResponseError: If the request failed.
+        :raises NoData:        If there is no data available for the request.
+        """
+        root_fmt = root.lower()
+        req_fmt = req.name.lower()
+
+        url = f"http://localhost:25510/snapshot/option/{req_fmt}"
+        querystring = {"root": root_fmt}
+        response = requests.get(url, params=querystring)
+        df = parse_flexible_REST(response)
+        return df
+
     def get_req(
         self,
         req: str,
     ) -> pd.DataFrame:
         """
         Make a historical data request given the raw text output of a data request. Typically used for debugging.
```

### Comparing `thetadata-0.9.0/thetadata/enums.py` & `thetadata-0.9.1/thetadata/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,25 @@
         :raises EnumParseError: If the code does not match a DataType
         """
         for member in cls:
             if code == member.value[0]:
                 return member
         raise exceptions._EnumParseError(code, cls)
 
+    @classmethod
+    def from_string(cls, name)-> DataType:
+        """Create a DataType by its associated name.
+
+        :raises EnumParseError: If the string does not match a DataType
+        """
+        for member in cls:
+            if name == member.name.lower():
+                return member
+        raise exceptions._EnumParseError(name, cls)
+
     def code(self) -> int:
         """:return: The datatype code associated w this type."""
         return self.value[0]
 
     def is_price(self) -> bool:
         """Check if this DataType indicates a price."""
         return self.value[1]
```

### Comparing `thetadata-0.9.0/thetadata/exceptions.py` & `thetadata-0.9.1/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/thetadata/terminal.py` & `thetadata-0.9.1/thetadata/terminal.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/LICENSE` & `thetadata-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/README.md` & `thetadata-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.0/pyproject.toml` & `thetadata-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -19,15 +19,15 @@
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "tqdm",
   "pandas",
   "wget",
   "psutil",
-
+  "ijson",
 ]
 
 [project.optional-dependencies]
 tests = [
   "coverage>=5.0.3",
   "pytest",
   "pytest-benchmark[histogram]>=3.2.1",
```

### Comparing `thetadata-0.9.0/PKG-INFO` & `thetadata-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
@@ -29,14 +29,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: ijson
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: wget
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
```

