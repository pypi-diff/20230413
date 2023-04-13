# Comparing `tmp/thetadata-0.9.1.tar.gz` & `tmp/thetadata-0.9.2.tar.gz`

## Comparing `thetadata-0.9.1.tar` & `thetadata-0.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.1/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.1/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/reference.md
--rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/quote_1min.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/trade_streaming.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.1/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.1/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.1/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/__init__.py
--rw-r--r--   0        0        0    56803 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/client.py
--rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/exceptions.py
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/py.typed
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 thetadata-0.9.1/thetadata/terminal.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.1/LICENSE
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.1/README.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 thetadata-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 thetadata-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.2/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.2/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/reference.md
+-rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/quote_1min.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.2/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.2/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.2/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/__init__.py
+-rw-r--r--   0        0        0    56832 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/client.py
+-rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/py.typed
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 thetadata-0.9.2/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.2/LICENSE
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.2/README.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 thetadata-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 thetadata-0.9.2/PKG-INFO
```

### Comparing `thetadata-0.9.1/mkdocs.yml` & `thetadata-0.9.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/.github/workflows/main.yml` & `thetadata-0.9.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/.github/workflows/python-publish.yml` & `thetadata-0.9.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/connection_msgs.py` & `thetadata-0.9.2/docs/connection_msgs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/explanation.md` & `thetadata-0.9.2/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/how-to-guides.md` & `thetadata-0.9.2/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/index.md` & `thetadata-0.9.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/logo.png` & `thetadata-0.9.2/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/manipulate_series.py` & `thetadata-0.9.2/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/tutorials.md` & `thetadata-0.9.2/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/cancel_streams.py` & `thetadata-0.9.2/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/eod.py` & `thetadata-0.9.2/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/get_last.py` & `thetadata-0.9.2/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/open_interest_streaming.py` & `thetadata-0.9.2/docs/options/open_interest_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/quote_1min.py` & `thetadata-0.9.2/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/quote_tick.py` & `thetadata-0.9.2/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/trade_streaming.py` & `thetadata-0.9.2/docs/options/trade_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/options/trade_streaming_full.py` & `thetadata-0.9.2/docs/options/trade_streaming_full.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/stocks/eod.py` & `thetadata-0.9.2/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/stocks/get_last.py` & `thetadata-0.9.2/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/stocks/quote_1min.py` & `thetadata-0.9.2/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/docs/stocks/quote_tick.py` & `thetadata-0.9.2/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/tests/test_client.py` & `thetadata-0.9.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/tests/test_docs.py` & `thetadata-0.9.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/thetadata/client.py` & `thetadata-0.9.2/thetadata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TickBody,
     ListBody,
     parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
-_VERSION = '0.9.0'
+_VERSION = '0.9.2'
 URL_BASE = "http://localhost:25510/"
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
 
 
@@ -243,15 +243,15 @@
 class ThetaClient:
     """A high-level, blocking client used to fetch market data. Instantiating this class
     runs a java background process, which is responsible for the heavy lifting of market
     data communication. Java 11 or higher is required to use this class."""
 
     def __init__(self, port: int = 11000, timeout: Optional[float] = 60, launch: bool = True, jvm_mem: int = 0,
                  username: str = "default", passwd: str = "default", auto_update: bool = True, use_bundle: bool = True,
-                 host: str = "localhost", streaming_port: int = 10000):
+                 host: str = "localhost", streaming_port: int = 10000, stable: bool = True):
         """Construct a client instance to interface with market data. If no username and passwd fields are provided,
             the terminal will connect to thetadata servers with free data permissions.
 
         :param port: The port number specified in the Theta Terminal config, which can usually be found under
                         %user.home%/ThetaData/ThetaTerminal.
         :param streaming_port: The port number of Theta Terminal Stream server
         :param host: The host name or IP address of Theta Terminal server
@@ -282,15 +282,15 @@
             terminal.kill_existing_terminal()
             if username == "default" or passwd == "default":
                 print('------------------------------------------------------------------------------------------------')
                 print("You are using the free version of Theta Data. You are currently limited to "
                       "20 requests / minute.\nA data subscription can be purchased at https://thetadata.net. "
                       "If you already have a ThetaData\nsubscription, specify the username and passwd parameters.")
                 print('------------------------------------------------------------------------------------------------')
-            if check_download(auto_update):
+            if check_download(auto_update, stable):
                 Thread(target=launch_terminal, args=[username, passwd, use_bundle, jvm_mem, auto_update]).start()
         else:
             print("You are not launching the terminal. This means you should have an external instance already running.")
 
     @contextmanager
     def connect(self):
         """Initiate a connection with the Theta Terminal. Requests can only be made inside this
```

### Comparing `thetadata-0.9.1/thetadata/enums.py` & `thetadata-0.9.2/thetadata/enums.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/thetadata/exceptions.py` & `thetadata-0.9.2/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/thetadata/parsing.py` & `thetadata-0.9.2/thetadata/parsing.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/thetadata/terminal.py` & `thetadata-0.9.2/thetadata/terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,26 +88,30 @@
         else:
             process = subprocess.Popen(["java", "-jar", "ThetaTerminal.jar", username, passwd],
                                        stdout=subprocess.PIPE, shell=True, cwd=cwd)
     for line in process.stdout:
         print(line.decode('utf-8').rstrip("\n"))
 
 
-def check_download(auto_update: bool) -> bool:
+def check_download(auto_update: bool, stable: bool) -> bool:
+    if stable:
+        link = 'https://download-latest.thetadata.us'
+    else:
+        link = 'https://download-unstable.thetadata.us'
     try:
         if not os.path.exists('ThetaTerminal.jar') or auto_update:
-            jar = urllib.request.urlopen("https://download-latest.thetadata.us")
+            jar = urllib.request.urlopen(link)
             with open('ThetaTerminal.jar', 'wb') as output:
                 output.write(jar.read())
                 output.close()
         return True
     except:
         try:
             if not os.path.exists('ThetaTerminal.jar') or auto_update:
-                jar = urllib.request.urlopen("http://download-latest.thetadata.us")
+                jar = urllib.request.urlopen(link)
                 with open('ThetaTerminal.jar', 'wb') as output:
                     output.write(jar.read())
                     output.close()
         except:
             print('Unable to fetch the latest terminal version. Please contact support.')
     return False
```

### Comparing `thetadata-0.9.1/LICENSE` & `thetadata-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/README.md` & `thetadata-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.1/pyproject.toml` & `thetadata-0.9.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `thetadata-0.9.1/PKG-INFO` & `thetadata-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
```

