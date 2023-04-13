# Comparing `tmp/elkpy-1.0.1.tar.gz` & `tmp/elkpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkpy-1.0.1.tar", last modified: Thu Mar  9 09:05:31 2023, max compression
+gzip compressed data, was "elkpy-1.1.0.tar", last modified: Thu Apr 13 12:09:51 2023, max compression
```

## Comparing `elkpy-1.0.1.tar` & `elkpy-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-03-09 09:05:31.855950 elkpy-1.0.1/
--rw-r--r--   0 max        (501) staff       (20)    35128 2022-11-22 16:17:54.000000 elkpy-1.0.1/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     5120 2023-03-09 09:05:31.856009 elkpy-1.0.1/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     4447 2022-11-22 16:17:47.000000 elkpy-1.0.1/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-03-09 09:05:31.855210 elkpy-1.0.1/elkpy/
--rw-r--r--   0 max        (501) staff       (20)       22 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/__init__.py
--rw-r--r--   0 max        (501) staff       (20)    19388 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/audiographcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     9934 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/audioroutingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16365 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/cvgatecontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1989 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/grpc_gen.py
--rw-r--r--   0 max        (501) staff       (20)     8021 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/keyboardcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    19656 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/midicontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15159 2023-03-03 12:50:44.000000 elkpy-1.0.1/elkpy/notificationcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     5032 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/osccontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15841 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/parametercontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6506 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/programcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     3056 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/sessioncontroller.py
--rw-r--r--   0 max        (501) staff       (20)    22973 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/sushi_info_types.py
--rw-r--r--   0 max        (501) staff       (20)     6191 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/sushicontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1994 2022-11-22 16:17:47.000000 elkpy-1.0.1/elkpy/sushierrors.py
--rw-r--r--   0 max        (501) staff       (20)     9701 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/sushiprocessor.py
--rw-r--r--   0 max        (501) staff       (20)     3024 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/systemcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6641 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/timingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     7011 2022-10-07 06:43:16.000000 elkpy-1.0.1/elkpy/transportcontroller.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-03-09 09:05:31.855860 elkpy-1.0.1/elkpy.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     5120 2023-03-09 09:05:31.000000 elkpy-1.0.1/elkpy.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      686 2023-03-09 09:05:31.000000 elkpy-1.0.1/elkpy.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-03-09 09:05:31.000000 elkpy-1.0.1/elkpy.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)        9 2023-03-09 09:05:31.000000 elkpy-1.0.1/elkpy.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        6 2023-03-09 09:05:31.000000 elkpy-1.0.1/elkpy.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)      701 2023-03-09 09:03:33.000000 elkpy-1.0.1/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)      330 2023-03-09 09:05:31.856246 elkpy-1.0.1/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)       69 2022-11-22 16:53:01.000000 elkpy-1.0.1/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.102546 elkpy-1.1.0/
+-rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.0/COPYING
+-rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.0/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-13 12:09:51.102616 elkpy-1.1.0/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.0/README.md
+-rw-r--r--   0 max        (501) staff       (20)      694 2023-03-30 14:23:24.000000 elkpy-1.1.0/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)      330 2023-04-13 12:09:51.102852 elkpy-1.1.0/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.0/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.096992 elkpy-1.1.0/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.101844 elkpy-1.1.0/src/elkpy/
+-rw-r--r--   0 max        (501) staff       (20)        0 2023-03-30 13:21:26.000000 elkpy-1.1.0/src/elkpy/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    19388 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/audiographcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     9934 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/audioroutingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16365 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/cvgatecontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     1989 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/grpc_gen.py
+-rw-r--r--   0 max        (501) staff       (20)     8021 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/keyboardcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    19656 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/midicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    15224 2023-04-06 14:39:28.000000 elkpy-1.1.0/src/elkpy/notificationcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     5032 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/osccontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    15841 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/parametercontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6506 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/programcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     3056 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sessioncontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    22973 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushi_info_types.py
+-rw-r--r--   0 max        (501) staff       (20)     6191 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     1994 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushierrors.py
+-rw-r--r--   0 max        (501) staff       (20)     9701 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushiprocessor.py
+-rw-r--r--   0 max        (501) staff       (20)     3024 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/systemcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6641 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/timingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     7011 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/transportcontroller.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.102451 elkpy-1.1.0/src/elkpy.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      790 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)        9 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        6 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/top_level.txt
```

### Comparing `elkpy-1.0.1/LICENSE` & `elkpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/PKG-INFO` & `elkpy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: COPYING
 
 # Sushi - gRPC controller wrapper #
 
 A simple wrapper for controlling sushi over gRPC via a python script.
 
 ### Prerequisites ###
```

### Comparing `elkpy-1.0.1/README.md` & `elkpy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/audiographcontroller.py` & `elkpy-1.1.0/src/elkpy/audiographcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/audioroutingcontroller.py` & `elkpy-1.1.0/src/elkpy/audioroutingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/cvgatecontroller.py` & `elkpy-1.1.0/src/elkpy/cvgatecontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/grpc_gen.py` & `elkpy-1.1.0/src/elkpy/grpc_gen.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/keyboardcontroller.py` & `elkpy-1.1.0/src/elkpy/keyboardcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/midicontroller.py` & `elkpy-1.1.0/src/elkpy/midicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/notificationcontroller.py` & `elkpy-1.1.0/src/elkpy/notificationcontroller.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,19 @@
         """ Attaches the asyncio event loop to the thread and start looping over it.
             Should not be called by the User.
             """
         asyncio.set_event_loop(loop)
         loop.run_forever()
 
     def close(self):
-        self.loop.call_soon_threadsafe(self.loop.stop)
-        self.notification_thread.join()
+        if self._async:
+            return
+        else:
+            self.loop.call_soon_threadsafe(self.loop.stop)
+            self.notification_thread.join()
 
     def __del__(self):
         self.close()
 
     #################################################
     # Notification stream processing                #
     # Should not be called directly by the user.    #
```

### Comparing `elkpy-1.0.1/elkpy/osccontroller.py` & `elkpy-1.1.0/src/elkpy/osccontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/parametercontroller.py` & `elkpy-1.1.0/src/elkpy/parametercontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/programcontroller.py` & `elkpy-1.1.0/src/elkpy/programcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/sessioncontroller.py` & `elkpy-1.1.0/src/elkpy/sessioncontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/sushi_info_types.py` & `elkpy-1.1.0/src/elkpy/sushi_info_types.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/sushicontroller.py` & `elkpy-1.1.0/src/elkpy/sushicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/sushierrors.py` & `elkpy-1.1.0/src/elkpy/sushierrors.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/sushiprocessor.py` & `elkpy-1.1.0/src/elkpy/sushiprocessor.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/systemcontroller.py` & `elkpy-1.1.0/src/elkpy/systemcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/timingcontroller.py` & `elkpy-1.1.0/src/elkpy/timingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy/transportcontroller.py` & `elkpy-1.1.0/src/elkpy/transportcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.0.1/elkpy.egg-info/PKG-INFO` & `elkpy-1.1.0/src/elkpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: COPYING
 
 # Sushi - gRPC controller wrapper #
 
 A simple wrapper for controlling sushi over gRPC via a python script.
 
 ### Prerequisites ###
```

### Comparing `elkpy-1.0.1/pyproject.toml` & `elkpy-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools>=59.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elkpy"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Maxime Gendebien", email="max@elk.audio" },
   { name="Ruben Svensson", email="ruben@elk.audio" },
 ]
 description = "A basic controller for sushi using gRPC"
 readme = "README.md"
 requires-python = ">=3.7"
```

