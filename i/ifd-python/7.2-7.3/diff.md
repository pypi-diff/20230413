# Comparing `tmp/ifd_python-7.2.tar.gz` & `tmp/ifd_python-7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.2.tar", max compression
+gzip compressed data, was "ifd_python-7.3.tar", max compression
```

## Comparing `ifd_python-7.2.tar` & `ifd_python-7.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.2/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.2/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2019 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Image.py
--rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Modele.py
--rw-r--r--   0        0        0      796 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/__init__.py
--rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.2/ifd/spec.py
--rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/tools.py
--rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 09:26:41.129981 ifd_python-7.2/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      327 2023-04-13 09:26:50.061903 ifd_python-7.2/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.3/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.3/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.3/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.3/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2019 2023-04-13 09:26:25.358120 ifd_python-7.3/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.3/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      796 2023-04-13 09:26:25.358120 ifd_python-7.3/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.3/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2187 2023-04-13 09:31:01.131698 ifd_python-7.3/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.3/ifd/spec.py
+-rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/tools.py
+-rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.3/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 09:31:17.203557 ifd_python-7.3/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      327 2023-04-13 09:31:26.443476 ifd_python-7.3/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.3/PKG-INFO
```

### Comparing `ifd_python-7.2/LICENSE` & `ifd_python-7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/README.md` & `ifd_python-7.3/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.3/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/Classification.py` & `ifd_python-7.3/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/Detection.py` & `ifd_python-7.3/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/Image.py` & `ifd_python-7.3/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/LogResult.py` & `ifd_python-7.3/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/OCR.py` & `ifd_python-7.3/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.3/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/entities/bbox.py` & `ifd_python-7.3/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.3/ifd/repository/AmqpImageRepository.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pika.spec
 from pika import PlainCredentials, ConnectionParameters, BasicProperties
 from pika.adapters.blocking_connection import BlockingChannel, BlockingConnection
 from .Interfaces import IImageRepository
+import json
 
 class AmqpImageRepository(IImageRepository):
     def __init__(self,
                  user: str,
                  password: str,
                  dns: str,
                  exchange: str,
@@ -53,12 +54,12 @@
     def sendMessageToChannel(self, message: str):
         if self._testIfConnectIsClose():
             self._connectToChannel()
 
         self._channel.basic_publish(
             exchange=self.exchange,
             routing_key='',
-            body=message,
+            body=json.dumps(message),
             properties=BasicProperties(
                 delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE
             )
         )
```

### Comparing `ifd_python-7.2/ifd/tools.py` & `ifd_python-7.3/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.2/PKG-INFO` & `ifd_python-7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.2
+Version: 7.3
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

