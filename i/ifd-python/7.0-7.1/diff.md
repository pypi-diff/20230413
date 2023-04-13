# Comparing `tmp/ifd_python-7.0.tar.gz` & `tmp/ifd_python-7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.0.tar", max compression
+gzip compressed data, was "ifd_python-7.1.tar", max compression
```

## Comparing `ifd_python-7.0.tar` & `ifd_python-7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.0/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.0/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      673 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      646 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2089 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Image.py
--rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      416 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Modele.py
--rw-r--r--   0        0        0      741 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/__init__.py
--rw-r--r--   0        0        0      656 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/__init__.py
--rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.0/ifd/spec.py
--rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/tools.py
--rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 15:32:49.088205 ifd_python-7.0/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      327 2023-04-12 15:32:58.544122 ifd_python-7.0/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.1/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.1/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      646 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     1948 2023-04-13 07:28:12.783707 ifd_python-7.1/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      416 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      735 2023-04-13 07:28:12.783707 ifd_python-7.1/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.1/ifd/spec.py
+-rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/tools.py
+-rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:28:30.963551 ifd_python-7.1/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      327 2023-04-13 07:28:42.151455 ifd_python-7.1/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.1/PKG-INFO
```

### Comparing `ifd_python-7.0/LICENSE` & `ifd_python-7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/README.md` & `ifd_python-7.1/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.1/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/entities/Classification.py` & `ifd_python-7.1/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/entities/Detection.py` & `ifd_python-7.1/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/entities/Image.py` & `ifd_python-7.1/ifd/entities/Image.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,28 @@
     img_path : str = ""
     img_checksum: str = ""
     classification: Classification = None
     detections: list = []
     rotation: int = 0
     ocr : OCR = None
     is_blur : bool = False
-    RefPto : str = ""
     
     ref_infra_pto : str = ""
 
     def serialize(self):
         return {
             "id": self.id,
             "img_path": self.img_path,
             "img_checksum": self.img_checksum,
             "rotation": self.rotation,
             "classification": self.classification.serialize() if isinstance(self.classification, Classification) else None,
             "detections": [detection.serialize() if isinstance(detection, Detection) else None for detection in self.detections],
             "ocr": self.ocr.serialize() if isinstance(self.ocr,OCR) else None,
             "ref_infra_pto": self.ref_infra_pto,
-            "is_blur": self.is_blur,
-            "RefPto": self.RefPto
+            "is_blur": self.is_blur
         }
     def deserialize(self, data):
         for field in data:
             if field == "id":
                 self.id = data[field]
             elif field == "img_path":
                 self.img_path = data[field]
@@ -44,11 +42,8 @@
                 self.detections = [Detection().deserialize(element) for element in data[field]]
             elif field == "ocr":
                 self.ocr = OCR().deserialize(data[field])
             elif field == "ref_infra_pto":
                 self.ref_infra_pto = data[field]
             elif field == "is_blur":
                 self.is_blur = data[field]
-            elif field == "RefPto":
-                self.RefPto = data[field]
-
         return self
```

### Comparing `ifd_python-7.0/ifd/entities/LogResult.py` & `ifd_python-7.1/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/entities/OCR.py` & `ifd_python-7.1/ifd/entities/OCR.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .Abstract import ADetection
 
 class OCR(ADetection):
     score_ocr: float
     label_ocr: str
-    score_match: float = 0.0
+    score_match: float
 
     def serialize(self):
         data = super().serialize()
         data["score_ocr"] = self.score_ocr
         data["label_ocr"] = self.label_ocr
         data["score_match"] = self.score_match
         return data
```

### Comparing `ifd_python-7.0/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.1/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/entities/bbox.py` & `ifd_python-7.1/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.1/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/ifd/tools.py` & `ifd_python-7.1/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.0/PKG-INFO` & `ifd_python-7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.0
+Version: 7.1
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

