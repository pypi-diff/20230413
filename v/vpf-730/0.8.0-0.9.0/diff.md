# Comparing `tmp/vpf_730-0.8.0.tar.gz` & `tmp/vpf_730-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpf_730-0.8.0.tar", last modified: Mon Dec 26 19:01:08 2022, max compression
+gzip compressed data, was "vpf_730-0.9.0.tar", last modified: Thu Apr 13 16:04:43 2023, max compression
```

## Comparing `vpf_730-0.8.0.tar` & `vpf_730-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2022-12-26 19:01:08.703516 vpf_730-0.8.0/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1070 2022-07-25 11:02:16.000000 vpf_730-0.8.0/LICENCE
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     2490 2022-12-26 19:01:08.703516 vpf_730-0.8.0/PKG-INFO
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1694 2022-12-26 18:59:32.000000 vpf_730-0.8.0/README.md
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1426 2022-12-26 19:01:08.703516 vpf_730-0.8.0/setup.cfg
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       38 2022-07-31 18:35:19.000000 vpf_730-0.8.0/setup.py
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2022-12-26 19:01:08.703516 vpf_730-0.8.0/vpf_730/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      400 2022-12-22 22:19:35.000000 vpf_730-0.8.0/vpf_730/__init__.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       87 2022-08-01 20:18:01.000000 vpf_730-0.8.0/vpf_730/__main__.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     4118 2022-12-26 17:29:46.000000 vpf_730-0.8.0/vpf_730/logger.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     8551 2022-12-26 18:59:32.000000 vpf_730-0.8.0/vpf_730/main.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     9081 2022-12-22 23:57:01.000000 vpf_730-0.8.0/vpf_730/sender.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     3110 2022-12-22 22:19:35.000000 vpf_730-0.8.0/vpf_730/utils.py
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)    14698 2022-12-26 18:59:32.000000 vpf_730-0.8.0/vpf_730/vpf_730.py
-drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2022-12-26 19:01:08.703516 vpf_730-0.8.0/vpf_730.egg-info/
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     2490 2022-12-26 19:01:08.000000 vpf_730-0.8.0/vpf_730.egg-info/PKG-INFO
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      352 2022-12-26 19:01:08.000000 vpf_730-0.8.0/vpf_730.egg-info/SOURCES.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        1 2022-12-26 19:01:08.000000 vpf_730-0.8.0/vpf_730.egg-info/dependency_links.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       46 2022-12-26 19:01:08.000000 vpf_730-0.8.0/vpf_730.egg-info/entry_points.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       76 2022-12-26 19:01:08.000000 vpf_730-0.8.0/vpf_730.egg-info/requires.txt
--rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        8 2022-12-26 19:01:08.000000 vpf_730-0.8.0/vpf_730.egg-info/top_level.txt
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-13 16:04:43.768786 vpf_730-0.9.0/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1070 2022-07-25 11:02:16.000000 vpf_730-0.9.0/LICENCE
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     2490 2023-04-13 16:04:43.768786 vpf_730-0.9.0/PKG-INFO
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1694 2022-12-26 18:59:32.000000 vpf_730-0.9.0/README.md
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-13 16:04:43.768786 vpf_730-0.9.0/server/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        0 2022-11-05 15:21:49.000000 vpf_730-0.9.0/server/__init__.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      414 2022-12-22 21:04:55.000000 vpf_730-0.9.0/server/app.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     1426 2023-04-13 16:04:43.768786 vpf_730-0.9.0/setup.cfg
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       38 2022-07-31 18:35:19.000000 vpf_730-0.9.0/setup.py
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-13 16:04:43.768786 vpf_730-0.9.0/vpf_730/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      400 2022-12-22 22:19:35.000000 vpf_730-0.9.0/vpf_730/__init__.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       87 2022-08-01 20:18:01.000000 vpf_730-0.9.0/vpf_730/__main__.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     4118 2022-12-26 17:29:46.000000 vpf_730-0.9.0/vpf_730/logger.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     8551 2022-12-26 18:59:32.000000 vpf_730-0.9.0/vpf_730/main.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     9081 2022-12-22 23:57:01.000000 vpf_730-0.9.0/vpf_730/sender.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     3110 2022-12-22 22:19:35.000000 vpf_730-0.9.0/vpf_730/utils.py
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)    14842 2023-04-13 16:00:55.000000 vpf_730-0.9.0/vpf_730/vpf_730.py
+drwxrwxr-x   0 kittnjdr  (1000) kittnjdr  (1000)        0 2023-04-13 16:04:43.768786 vpf_730-0.9.0/vpf_730.egg-info/
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)     2490 2023-04-13 16:04:43.000000 vpf_730-0.9.0/vpf_730.egg-info/PKG-INFO
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)      385 2023-04-13 16:04:43.000000 vpf_730-0.9.0/vpf_730.egg-info/SOURCES.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)        1 2023-04-13 16:04:43.000000 vpf_730-0.9.0/vpf_730.egg-info/dependency_links.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       46 2023-04-13 16:04:43.000000 vpf_730-0.9.0/vpf_730.egg-info/entry_points.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       76 2023-04-13 16:04:43.000000 vpf_730-0.9.0/vpf_730.egg-info/requires.txt
+-rw-rw-r--   0 kittnjdr  (1000) kittnjdr  (1000)       15 2023-04-13 16:04:43.000000 vpf_730-0.9.0/vpf_730.egg-info/top_level.txt
```

### Comparing `vpf_730-0.8.0/LICENCE` & `vpf_730-0.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `vpf_730-0.8.0/PKG-INFO` & `vpf_730-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpf_730
-Version: 0.8.0
+Version: 0.9.0
 Summary: a library to read data from the Biral VPF-730 Present weather sensor
 Home-page: https://github.com/RUB_Clim/vpf-730
 Author: Jonas Kittner
 Author-email: jonas.kittner@ruhr-uni-bochum.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vpf_730-0.8.0/README.md` & `vpf_730-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vpf_730-0.8.0/setup.cfg` & `vpf_730-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vpf_730
-version = 0.8.0
+version = 0.9.0
 description = a library to read data from the Biral VPF-730 Present weather sensor
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RUB_Clim/vpf-730
 author = Jonas Kittner
 author_email = jonas.kittner@ruhr-uni-bochum.de
 license = MIT
```

### Comparing `vpf_730-0.8.0/vpf_730/logger.py` & `vpf_730-0.9.0/vpf_730/logger.py`

 * *Files identical despite different names*

### Comparing `vpf_730-0.8.0/vpf_730/main.py` & `vpf_730-0.9.0/vpf_730/main.py`

 * *Files identical despite different names*

### Comparing `vpf_730-0.8.0/vpf_730/sender.py` & `vpf_730-0.9.0/vpf_730/sender.py`

 * *Files identical despite different names*

### Comparing `vpf_730-0.8.0/vpf_730/utils.py` & `vpf_730-0.9.0/vpf_730/utils.py`

 * *Files identical despite different names*

### Comparing `vpf_730-0.8.0/vpf_730/vpf_730.py` & `vpf_730-0.9.0/vpf_730/vpf_730.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,20 +126,21 @@
         convenience and is using :const:`OBSTRUCTION_TO_VISION` internally.
 
         :return: text message containing the obstruction to vision type
         """
         return OBSTRUCTION_TO_VISION[self.obstruction_to_vision]
 
     @classmethod
-    def from_msg(cls, msg: bytes) -> Measurement:
+    def from_msg(cls, msg: bytes, timestamp: int) -> Measurement:
         """Constructs a new :func:`Measurement` from the bytes read.
 
         :param msg: bytes representing a message read from the sensor using
             :func:`VPF730.measure` e.g.
             ``b'PW01,0060,0000,001.19 KM,NP ,HZ,00.06,00.0000,+020.5 C,0000,002.51,002.51,+011.10,  0000,000,OOO,002.51'``
+        :param timestamp: unix timestamp in UTC when the sensor was read
 
         :return: a new instance of :func:`Measurement`.
         """  # noqa: E501
         # checksum is off by default
         msg_str = msg.decode()
         msg_list = msg_str.strip().split(',')
         # checks
@@ -154,15 +155,15 @@
         if obstruction_to_vision not in OBSTRUCTION_TO_VISION:
             raise ValueError(
                 f'unknown obstruction to vision type {obstruction_to_vision!r}'
                 f'. Must be one of: {", ".join(obstruction_to_vision)}',
             )
 
         return cls(
-            timestamp=int(datetime.now(timezone.utc).timestamp()),
+            timestamp=timestamp,
             # strip the message header
             sensor_id=int(msg_list[0].lstrip('PW')),
             last_measurement_period=int(msg_list[1]),
             time_since_report=int(msg_list[2]),
             optical_range=float(msg_list[3].rstrip('KM')),
             precipitation_type_msg=precipitation_type_msg,
             obstruction_to_vision=obstruction_to_vision,
@@ -369,16 +370,17 @@
             in the sensor using the ``OSAMx`` command, where ``x`` is ``0`` for
             automatic message transmission disabled and ``1`` for automatic
             message transmission enabled (default: ``True``).
 
         :return: a new :func:`Measurement` containing the data read from the
             sensor
         """
+        timestamp = int(datetime.now(timezone.utc).timestamp())
         with self.open_ser():
             if polled_mode is True:
                 self._ser.write(b'D?\r\n')
 
             msg = self._ser.read_until(b'\r\n')
             if msg:
-                return Measurement.from_msg(msg)
+                return Measurement.from_msg(msg=msg, timestamp=timestamp)
             else:
                 return None
```

### Comparing `vpf_730-0.8.0/vpf_730.egg-info/PKG-INFO` & `vpf_730-0.9.0/vpf_730.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpf-730
-Version: 0.8.0
+Version: 0.9.0
 Summary: a library to read data from the Biral VPF-730 Present weather sensor
 Home-page: https://github.com/RUB_Clim/vpf-730
 Author: Jonas Kittner
 Author-email: jonas.kittner@ruhr-uni-bochum.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

