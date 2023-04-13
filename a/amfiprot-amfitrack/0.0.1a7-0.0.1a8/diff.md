# Comparing `tmp/amfiprot_amfitrack-0.0.1a7.tar.gz` & `tmp/amfiprot_amfitrack-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amfiprot_amfitrack-0.0.1a7.tar", last modified: Wed Mar 22 09:35:37 2023, max compression
+gzip compressed data, was "amfiprot_amfitrack-0.0.1a8.tar", last modified: Thu Apr 13 12:27:24 2023, max compression
```

## Comparing `amfiprot_amfitrack-0.0.1a7.tar` & `amfiprot_amfitrack-0.0.1a8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 09:35:37.599011 amfiprot_amfitrack-0.0.1a7/
--rw-rw-rw-   0        0        0     1057 2023-02-24 10:11:22.000000 amfiprot_amfitrack-0.0.1a7/LICENSE
--rw-rw-rw-   0        0        0     1552 2023-03-22 09:35:37.599011 amfiprot_amfitrack-0.0.1a7/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-02-24 10:11:22.000000 amfiprot_amfitrack-0.0.1a7/README.md
--rw-rw-rw-   0        0        0      110 2023-02-24 10:11:22.000000 amfiprot_amfitrack-0.0.1a7/pyproject.toml
--rw-rw-rw-   0        0        0      671 2023-03-22 09:35:37.605013 amfiprot_amfitrack-0.0.1a7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-22 09:35:37.576006 amfiprot_amfitrack-0.0.1a7/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 09:35:37.583007 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack/
--rw-rw-rw-   0        0        0      124 2023-03-22 09:35:19.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack/__init__.py
--rw-rw-rw-   0        0        0      761 2023-02-24 10:11:22.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack/device.py
--rw-rw-rw-   0        0        0    18024 2023-03-22 09:34:50.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack/payload.py
-drwxrwxrwx   0        0        0        0 2023-03-22 09:35:37.598011 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/
--rw-rw-rw-   0        0        0     1552 2023-03-22 09:35:37.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-03-22 09:35:37.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 09:35:37.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-22 09:35:37.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-22 09:35:37.000000 amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 12:27:24.005969 amfiprot_amfitrack-0.0.1a8/
+-rw-rw-rw-   0        0        0     1057 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/LICENSE
+-rw-rw-rw-   0        0        0     1552 2023-04-13 12:27:24.005969 amfiprot_amfitrack-0.0.1a8/PKG-INFO
+-rw-rw-rw-   0        0        0     1119 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/README.md
+-rw-rw-rw-   0        0        0      110 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/pyproject.toml
+-rw-rw-rw-   0        0        0      671 2023-04-13 12:27:24.015981 amfiprot_amfitrack-0.0.1a8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 12:27:23.970065 amfiprot_amfitrack-0.0.1a8/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 12:27:23.980040 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/
+-rw-rw-rw-   0        0        0      124 2023-04-13 12:26:08.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/__init__.py
+-rw-rw-rw-   0        0        0      761 2023-04-05 08:30:15.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/device.py
+-rw-rw-rw-   0        0        0    19358 2023-04-05 09:16:31.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/payload.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:27:24.004012 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/
+-rw-rw-rw-   0        0        0     1552 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-13 12:27:23.000000 amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/top_level.txt
```

### Comparing `amfiprot_amfitrack-0.0.1a7/LICENSE` & `amfiprot_amfitrack-0.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a7/PKG-INFO` & `amfiprot_amfitrack-0.0.1a8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amfiprot_amfitrack
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: AmfiTrack extension for Amfiprot
 Author: Kristian Klein-Wengel
 Author-email: kkw@amfitech.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.6
```

### Comparing `amfiprot_amfitrack-0.0.1a7/README.md` & `amfiprot_amfitrack-0.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a7/setup.cfg` & `amfiprot_amfitrack-0.0.1a8/setup.cfg`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack/device.py` & `amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/device.py`

 * *Files identical despite different names*

### Comparing `amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack/payload.py` & `amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack/payload.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 import amfiprot.payload
 from amfiprot.payload import Payload
 
 
 class PayloadType(enum.IntEnum):
 
-    SOURCE_COIL_DATA = 0x10
-    REQUEST_CALIBRATION_SIGNAL = 0x11
+    SOURCE_COIL_DATA = 0x10  # DEPRECATED
+    REQUEST_CALIBRATION_SIGNAL = 0x11  
 
     CALIBRATE = 0x12
     CALIBRATE_IF_UNCALIBRATED = 0x13
 
-    EMF = 0x14
-    EMF_TIMESTAMP = 0x15
-    EMF_IMU = 0x16
-    EMF_IMU_TIMESTAMP = 0x17
-    IMU = 0x18
-    IMU_TIMESTAMP = 0x19
+    EMF = 0x14  # DEPRECATED
+    EMF_TIMESTAMP = 0x15  # DEPRECATED
+    EMF_IMU = 0x16  # DEPRECATED
+    EMF_IMU_TIMESTAMP = 0x17  # DEPRECATED
+    IMU = 0x18  # DEPRECATED
+    IMU_TIMESTAMP = 0x19  # DEPRECATED
     EMF_IMU_FRAME_ID = 0x1A
 
-    SET_SEND_IMU = 0x20
-    SOURCE_COIL_CAL_DATA = 0x21
-    SOURCE_COIL_CAL_IMU_DATA = 0x22
+    SET_SEND_IMU = 0x20  # DEPRECATED
+    SOURCE_COIL_CAL_DATA = 0x21  # DEPRECATED
+    SOURCE_COIL_CAL_IMU_DATA = 0x22  # DEPRECATED
     SOURCE_CALIBRATION = 0x23
     SOURCE_MEASUREMENT = 0x24
 
-    METADATA = 0x80
-    EMF_META = 0x81
-    EMF_IMU_META = 0x82
+    METADATA = 0x80  # DEPRECATED
+    EMF_META = 0x81  # DEPRECATED
+    EMF_IMU_META = 0x82  # DEPRECATED
 
     RAW_B_FIELD_X = 0xA0  # DEPRECATED
     RAW_B_FIELD_Y = 0xA1  # DEPRECATED
     RAW_B_FIELD_Z = 0xA2  # DEPRECATED
     RAW_B_FIELD_REF = 0xA3  # DEPRECATED
     RAW_B_FIELD = 0xA4
     NORM_B_FIELD = 0xA5
@@ -179,15 +179,15 @@
     payload_type = 0x16
 
     def __init__(self, data):
         self.data = data
         self.emf = EmfData(data[0:21])
         self.sensor_status = data[21]
         self.source_coil_id = data[22]
-        self.imu = ImuData(data[23:47])
+        self.imu = ImuDataOld(data[23:47])
 
     def __len__(self) -> int:
         """ Length of the payload in bytes (without the CRC byte) """
         return len(self.data)
 
     def __str__(self) -> str:
         return "<EMF IMU> " + str(self.to_dict())
@@ -212,15 +212,15 @@
     payload_type = 0x16
 
     def __init__(self, data):
         self.data = data
         self.emf = EmfData(data[0:21])
         self.sensor_status = data[21]
         self.source_coil_id = data[22]
-        self.imu = ImuData(data[23:47])
+        self.imu = ImuDataOld(data[23:47])
         self.timestamp = int.from_bytes(data[47:49], byteorder='little', signed=False)
 
     def __len__(self) -> int:
         """ Length of the payload in bytes (without the CRC byte) """
         return len(self.data)
 
     def __str__(self) -> str:
@@ -247,16 +247,19 @@
 
     def __init__(self, data):
         self.data = data
         self.emf = EmfData(self.data[0:21])
         self.sensor_status = self.data[21]
         self.source_coil_id = self.data[22]
         self.calc_id = int.from_bytes(self.data[23:25], byteorder='little', signed=False)
-        self.imu = ImuData(self.data[25:39])
+        self.imu = ImuData(self.data[25:37])
+        self.sensor_state = self.data[37]
+        self.metal_distortion = self.data[38]
         self.gpio_state = int.from_bytes(self.data[39:41], byteorder='little', signed=False)
+        self.rssi = self.data[41]
         self.frame_id = int.from_bytes(self.data[42:45], byteorder='little', signed=False)
 
     def __len__(self) -> int:
         """ Length of the payload in bytes (without the CRC byte) """
         return len(self.data)
 
     def __str__(self) -> str:
@@ -268,17 +271,20 @@
 
     def to_bytes(self) -> array.array:
         return array.array('B', self.data)
 
     def to_dict(self) -> dict:
         return {
             'frame_id': self.frame_id,
-            'emf': self.emf,
-            'imu': self.imu,
+            'emf': str(self.emf),
+            'imu': str(self.imu),
             'sensor_status': self.sensor_status,
+            'sensor_state': self.sensor_state,
+            'metal_distortion': self.metal_distortion,
+            'rssi': self.rssi,
             'source_coil_id': self.source_coil_id,
             'calc_id': self.calc_id,
             'gpio_state': self.gpio_state
         }
 
 
 class RawBFieldPayload(amfiprot.payload.Payload):
@@ -384,19 +390,19 @@
 
 class SourceMeasurementPayload(amfiprot.payload.Payload):
     payload_type = PayloadType.SOURCE_MEASUREMENT
 
     def __init__(self, data):
         self.data = data
         self.current = struct.unpack("<3f", data[0:12])
-        # TODO:
-        #     lib_AmfiProt_Amfitrack_IMU_16b_t imu_data;
-        #     uint8_t source_status;      // Used to indicate battery status, sync to optitrack, hardware failures (broken wire)
-        #     uint8_t source_state;       // on/off state for: Phase modulation, offset coil, data over B-field, (maybe also cross talk calibration, frequency tuning, current tuning)
-        #     int8_t rssi;
+        self.imu = ImuData(self.data[12:24])
+        self.source_status = self.data[24]
+        self.source_state = self.data[25]
+        self.rssi = self.data[26]
+        self.frame_id = int.from_bytes(data[27:30], byteorder='little', signed=False)
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __str__(self) -> str:
         return "<Source Measurement Data> " + str(self.to_dict())
 
@@ -405,16 +411,20 @@
         return self.payload_type
 
     def to_bytes(self) -> array.array:
         return array.array('B', self.data)
 
     def to_dict(self) -> dict:
         return {
-            'current': self.current
-            # TODO: add missing fields
+            'frame_id': self.frame_id,
+            'current': self.current,
+            'imu': str(self.imu),
+            'source_status': self.source_status,
+            'source_state': self.source_state,
+            'rssi': self.rssi
         }
 
 class SignDataPayload(amfiprot.Payload):
     payload_type = PayloadType.SIGN_DATA
 
     def __init__(self, data):
         self.data = data
@@ -523,28 +533,42 @@
         self.quat_x = float(int.from_bytes(data[9:12], byteorder='little', signed=True)) / 1000000.0
         self.quat_y = float(int.from_bytes(data[12:15], byteorder='little', signed=True)) / 1000000.0
         self.quat_z = float(int.from_bytes(data[15:18], byteorder='little', signed=True)) / 1000000.0
         self.quat_w = float(int.from_bytes(data[18:21], byteorder='little', signed=True)) / 1000000.0
 
     def __str__(self):
         return f"Position: ({self.pos_x:.2f}, {self.pos_y:.2f}, {self.pos_z:.2f}) " \
-               f"Quaternions: ({self.quat_x:.2f}, {self.quat_y:.2f}, {self.quat_z:.2f}, {self.quat_w:.2f})"
+               f"Orientation: ({self.quat_x:.2f}, {self.quat_y:.2f}, {self.quat_z:.2f}, {self.quat_w:.2f})"
 
-class ImuData:
+class ImuDataOld:
     def __init__(self, data):
         self.acc_x = float(int.from_bytes(data[0:2], byteorder='little', signed=True)) * 0.000122  # In g
         self.acc_y = float(int.from_bytes(data[2:4], byteorder='little', signed=True)) * 0.000122
         self.acc_z = float(int.from_bytes(data[4:6], byteorder='little', signed=True)) * 0.000122
 
         self.gyro_x = float(int.from_bytes(data[6:8], byteorder='little', signed=True)) * 0.07  # In deg per sec
         self.gyro_y = float(int.from_bytes(data[8:10], byteorder='little', signed=True)) * 0.07
         self.gyro_z = float(int.from_bytes(data[10:12], byteorder='little', signed=True)) * 0.07
 
         self.quat_x = float(int.from_bytes(data[12:15], byteorder='little', signed=True)) / 1000000.0
         self.quat_y = float(int.from_bytes(data[15:18], byteorder='little', signed=True)) / 1000000.0
         self.quat_z = float(int.from_bytes(data[18:21], byteorder='little', signed=True)) / 1000000.0
         self.quat_w = float(int.from_bytes(data[21:24], byteorder='little', signed=True)) / 1000000.0
-
+        
     def __str__(self):
         return f"Acc: ({self.acc_x:.2f}, {self.acc_y:.2f}, {self.acc_z:.2f}) " \
                f"Gyro: ({self.gyro_x:.2f}, {self.gyro_y:.2f}, {self.gyro_z:.2f}) " \
                f"Quaternions: ({self.quat_x:.2f},{self.quat_y:.2f}, {self.quat_z:.2f}, {self.quat_w:.2f})"
+
+class ImuData:
+    def __init__(self, data):
+        self.acc_x = float(int.from_bytes(data[0:2], byteorder='little', signed=True)) * 0.000122  # In g
+        self.acc_y = float(int.from_bytes(data[2:4], byteorder='little', signed=True)) * 0.000122
+        self.acc_z = float(int.from_bytes(data[4:6], byteorder='little', signed=True)) * 0.000122
+
+        self.gyro_x = float(int.from_bytes(data[6:8], byteorder='little', signed=True)) * 0.07  # In deg per sec
+        self.gyro_y = float(int.from_bytes(data[8:10], byteorder='little', signed=True)) * 0.07
+        self.gyro_z = float(int.from_bytes(data[10:12], byteorder='little', signed=True)) * 0.07
+
+    def __str__(self):
+        return f"Acc: ({self.acc_x:.2f}, {self.acc_y:.2f}, {self.acc_z:.2f}) " \
+               f"Gyro: ({self.gyro_x:.2f}, {self.gyro_y:.2f}, {self.gyro_z:.2f}) " \
```

### Comparing `amfiprot_amfitrack-0.0.1a7/src/amfiprot_amfitrack.egg-info/PKG-INFO` & `amfiprot_amfitrack-0.0.1a8/src/amfiprot_amfitrack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amfiprot-amfitrack
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: AmfiTrack extension for Amfiprot
 Author: Kristian Klein-Wengel
 Author-email: kkw@amfitech.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.6
```

