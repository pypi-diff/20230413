# Comparing `tmp/ifd_python-7.1.tar.gz` & `tmp/ifd_python-7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.1.tar", max compression
+gzip compressed data, was "ifd_python-7.2.tar", max compression
```

## Comparing `ifd_python-7.1.tar` & `ifd_python-7.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.1/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.1/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      673 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      646 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Detection.py
--rw-r--r--   0        0        0     1948 2023-04-13 07:28:12.783707 ifd_python-7.1/ifd/entities/Image.py
--rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      416 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/Modele.py
--rw-r--r--   0        0        0      735 2023-04-13 07:28:12.783707 ifd_python-7.1/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/__init__.py
--rw-r--r--   0        0        0      656 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/repository/__init__.py
--rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.1/ifd/spec.py
--rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/tools.py
--rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.1/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 07:28:30.963551 ifd_python-7.1/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      327 2023-04-13 07:28:42.151455 ifd_python-7.1/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.2/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.2/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2019 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      796 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.2/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.2/ifd/spec.py
+-rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/tools.py
+-rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.2/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 09:26:41.129981 ifd_python-7.2/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      327 2023-04-13 09:26:50.061903 ifd_python-7.2/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.2/PKG-INFO
```

### Comparing `ifd_python-7.1/LICENSE` & `ifd_python-7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/README.md` & `ifd_python-7.2/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.2/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/ifd/entities/Classification.py` & `ifd_python-7.2/ifd/entities/OCR.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from .Modele import Modele
+from .Abstract import ADetection
 
-class Classification():
-    score: float = -1
-    label: str = ""
-    modele: Modele
+class OCR(ADetection):
+    score_ocr: float
+    label_ocr: str
+    score_match: float
 
     def serialize(self):
-        return {
-            "score": self.score,
-            "label": self.label,
-            "modele": self.modele.serialize() if isinstance(self.modele, Modele) else None
-        }
+        data = super().serialize()
+        data["score_ocr"] = self.score_ocr
+        data["label_ocr"] = self.label_ocr
+        data["score_match"] = self.score_match
+        return data
+        
     def deserialize(self, data):
+        super().deserialize(data)
+
         for field in data:
-            if field == "score":
-                self.score = data[field]
-            elif field == "label":
-                self.score = data[field]
-            elif field == "modele":
-                self.modele = Modele().deserialize(data[field])
+            if data[field] is None:
+                pass
+            elif field == "score_ocr":
+                self.score_ocr = data[field]
+            elif field == "label_ocr":
+                self.label_ocr = data[field]
+            elif field == "score_match":
+                self.score_match = data[field]
         return self
```

### Comparing `ifd_python-7.1/ifd/entities/Image.py` & `ifd_python-7.2/ifd/entities/Image.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,19 @@
             "classification": self.classification.serialize() if isinstance(self.classification, Classification) else None,
             "detections": [detection.serialize() if isinstance(detection, Detection) else None for detection in self.detections],
             "ocr": self.ocr.serialize() if isinstance(self.ocr,OCR) else None,
             "ref_infra_pto": self.ref_infra_pto,
             "is_blur": self.is_blur
         }
     def deserialize(self, data):
+        
         for field in data:
-            if field == "id":
+            if data[field] is None:
+                pass
+            elif field == "id":
                 self.id = data[field]
             elif field == "img_path":
                 self.img_path = data[field]
             elif field == "img_checksum":
                 self.img_checksum = data[field]
             elif field == "classification":
                 self.classification = Classification().deserialize(data[field])
```

### Comparing `ifd_python-7.1/ifd/entities/LogResult.py` & `ifd_python-7.2/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.2/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/ifd/entities/bbox.py` & `ifd_python-7.2/ifd/entities/bbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,17 @@
             "xmin": self.xmin,
             "xmax": self.xmax,
             "ymin": self.ymin,
             "ymax": self.ymax
         }
     def deserialize(self, data):
         for field in data:
-            if field == "xmin":
+            if data[field] is None:
+                pass
+            elif field == "xmin":
                 self.xmin = data[field]
             elif field == "xmax":
                 self.xmax = data[field]
             elif field == "ymin":
                 self.ymin = data[field]
             elif field == "ymax":
                 self.ymax = data[field]
```

### Comparing `ifd_python-7.1/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.2/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/ifd/tools.py` & `ifd_python-7.2/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.1/PKG-INFO` & `ifd_python-7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.1
+Version: 7.2
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

