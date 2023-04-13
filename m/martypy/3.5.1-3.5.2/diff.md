# Comparing `tmp/martypy-3.5.1.tar.gz` & `tmp/martypy-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martypy-3.5.1.tar", last modified: Thu Apr 13 04:29:43 2023, max compression
+gzip compressed data, was "martypy-3.5.2.tar", last modified: Thu Apr 13 18:09:57 2023, max compression
```

## Comparing `martypy-3.5.1.tar` & `martypy-3.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:29:43.813494 martypy-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-13 04:29:31.000000 martypy-3.5.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-13 04:29:31.000000 martypy-3.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 04:29:31.000000 martypy-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-13 04:29:43.813494 martypy-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 04:29:31.000000 martypy-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:29:43.809494 martypy-3.5.1/martypy/
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/ClientGeneric.py
--rw-r--r--   0 runner    (1001) docker     (123)    34847 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/ClientMV1.py
--rw-r--r--   0 runner    (1001) docker     (123)    38446 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/ClientMV2.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/LikeHDLC.py
--rw-r--r--   0 runner    (1001) docker     (123)    55547 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/Marty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/ProtocolOverAscii.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICCommsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICCommsParams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICCommsSerial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICCommsTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICCommsWiFi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICHWElems.py
--rw-r--r--   0 runner    (1001) docker     (123)    34125 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICProtocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICROSSerial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RICStreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/RateAverager.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/ValueAverager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/WebSocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/WebSocketFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:29:43.813494 martypy-3.5.1/martypy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/tests/testBaudRateSelection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/tests/testColourSensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/tests/testStreamMP3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/tests/test_martypy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-13 04:29:31.000000 martypy-3.5.1/martypy/tests/testrob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:29:43.813494 martypy-3.5.1/martypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-13 04:29:43.000000 martypy-3.5.1/martypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-13 04:29:43.000000 martypy-3.5.1/martypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:29:43.000000 martypy-3.5.1/martypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 04:29:43.000000 martypy-3.5.1/martypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 04:29:43.000000 martypy-3.5.1/martypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 04:29:43.813494 martypy-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-13 04:29:31.000000 martypy-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:57.938136 martypy-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-13 18:09:47.000000 martypy-3.5.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-13 18:09:47.000000 martypy-3.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 18:09:47.000000 martypy-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-13 18:09:57.938136 martypy-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-13 18:09:47.000000 martypy-3.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:57.934136 martypy-3.5.2/martypy/
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/ClientGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34847 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/ClientMV1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38446 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/ClientMV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/LikeHDLC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55547 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/Marty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/ProtocolOverAscii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICCommsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICCommsParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICCommsSerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICCommsTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICCommsWiFi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICHWElems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34125 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICProtocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICROSSerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RICStreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/RateAverager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/ValueAverager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/WebSocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/WebSocketFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:57.934136 martypy-3.5.2/martypy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/tests/testBaudRateSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/tests/testColourSensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/tests/testStreamMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/tests/test_martypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-13 18:09:47.000000 martypy-3.5.2/martypy/tests/testrob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:09:57.934136 martypy-3.5.2/martypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-13 18:09:57.000000 martypy-3.5.2/martypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-13 18:09:57.000000 martypy-3.5.2/martypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:09:57.000000 martypy-3.5.2/martypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 18:09:57.000000 martypy-3.5.2/martypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:09:57.000000 martypy-3.5.2/martypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 18:09:57.938136 martypy-3.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-13 18:09:47.000000 martypy-3.5.2/setup.py
```

### Comparing `martypy-3.5.1/CHANGES.md` & `martypy-3.5.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/LICENSE.md` & `martypy-3.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/PKG-INFO` & `martypy-3.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martypy
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python library for Marty the Robot V1 and V2
 Home-page: http://github.com/robotical/martypy
 Author: Robotical
 Author-email: hello@robotical.io
 Maintainer: Robotical
 Maintainer-email: hello@robotical.io
 License: Apache 2.0
```

### Comparing `martypy-3.5.1/README.md` & `martypy-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/ClientGeneric.py` & `martypy-3.5.2/martypy/ClientGeneric.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/ClientMV1.py` & `martypy-3.5.2/martypy/ClientMV1.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/ClientMV2.py` & `martypy-3.5.2/martypy/ClientMV2.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/LikeHDLC.py` & `martypy-3.5.2/martypy/LikeHDLC.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/Marty.py` & `martypy-3.5.2/martypy/Marty.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/ProtocolOverAscii.py` & `martypy-3.5.2/martypy/ProtocolOverAscii.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICCommsBase.py` & `martypy-3.5.2/martypy/RICCommsBase.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICCommsParams.py` & `martypy-3.5.2/martypy/RICCommsParams.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICCommsSerial.py` & `martypy-3.5.2/martypy/RICCommsSerial.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICCommsTest.py` & `martypy-3.5.2/martypy/RICCommsTest.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICCommsWiFi.py` & `martypy-3.5.2/martypy/RICCommsWiFi.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICHWElems.py` & `martypy-3.5.2/martypy/RICHWElems.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICInterface.py` & `martypy-3.5.2/martypy/RICInterface.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICProtocols.py` & `martypy-3.5.2/martypy/RICProtocols.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICROSSerial.py` & `martypy-3.5.2/martypy/RICROSSerial.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RICStreamHandler.py` & `martypy-3.5.2/martypy/RICStreamHandler.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/RateAverager.py` & `martypy-3.5.2/martypy/RateAverager.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/WebSocket.py` & `martypy-3.5.2/martypy/WebSocket.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/WebSocketFrame.py` & `martypy-3.5.2/martypy/WebSocketFrame.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/tests/testBaudRateSelection.py` & `martypy-3.5.2/martypy/tests/testBaudRateSelection.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/tests/testColourSensor.py` & `martypy-3.5.2/martypy/tests/testColourSensor.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/tests/testStreamMP3.py` & `martypy-3.5.2/martypy/tests/testStreamMP3.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/tests/test_martypy.py` & `martypy-3.5.2/martypy/tests/test_martypy.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy/tests/testrob.py` & `martypy-3.5.2/martypy/tests/testrob.py`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/martypy.egg-info/PKG-INFO` & `martypy-3.5.2/martypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martypy
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python library for Marty the Robot V1 and V2
 Home-page: http://github.com/robotical/martypy
 Author: Robotical
 Author-email: hello@robotical.io
 Maintainer: Robotical
 Maintainer-email: hello@robotical.io
 License: Apache 2.0
```

### Comparing `martypy-3.5.1/martypy.egg-info/SOURCES.txt` & `martypy-3.5.2/martypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `martypy-3.5.1/setup.py` & `martypy-3.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="martypy",
-    version="3.5.1",
+    version="3.5.2",
     description="Python library for Marty the Robot V1 and V2",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Robotical",
     author_email="hello@robotical.io",
     copyright="Robotical",
     maintainer='Robotical',
     maintainer_email='hello@robotical.io',
     packages=find_packages(),
     url='http://github.com/robotical/martypy',
     license='Apache 2.0',
     install_requires=[
         'pyserial',
+        'packaging',
     ],
     extras_require={
         "tests": [
             "pytest",
         ],
     },
     keywords=[
```

