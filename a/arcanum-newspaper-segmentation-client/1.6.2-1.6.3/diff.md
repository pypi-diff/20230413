# Comparing `tmp/arcanum-newspaper-segmentation-client-1.6.2.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.2.tar", last modified: Thu Apr 13 13:46:12 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.3.tar", last modified: Thu Apr 13 14:35:15 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.6.2.tar` & `arcanum-newspaper-segmentation-client-1.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:46:12.240389 arcanum-newspaper-segmentation-client-1.6.2/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.2/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-13 13:46:12.239434 arcanum-newspaper-segmentation-client-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.2/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 13:46:12.240389 arcanum-newspaper-segmentation-client-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-13 13:43:18.000000 arcanum-newspaper-segmentation-client-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:46:12.212465 arcanum-newspaper-segmentation-client-1.6.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:46:12.229419 arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-13 13:46:12.000000 arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-13 13:46:12.000000 arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:46:12.000000 arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-13 13:46:12.000000 arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 13:46:12.000000 arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 13:46:12.238395 arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    12514 2023-04-12 11:33:38.000000 arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     2669 2023-04-13 13:45:52.000000 arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.776889 arcanum-newspaper-segmentation-client-1.6.3/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-13 14:35:15.776889 arcanum-newspaper-segmentation-client-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.3/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:35:15.777886 arcanum-newspaper-segmentation-client-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-13 14:34:12.000000 arcanum-newspaper-segmentation-client-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.754164 arcanum-newspaper-segmentation-client-1.6.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.771930 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.775892 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    12514 2023-04-12 11:33:38.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     2682 2023-04-13 14:31:28.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/LICENSE` & `arcanum-newspaper-segmentation-client-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.2
+Version: 1.6.3
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/setup.py` & `arcanum-newspaper-segmentation-client-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.6.2",
+    version="1.6.3",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.2
+Version: 1.6.3
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/__init__.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from newspaper_segmentation_client import run_newspaper_segmentation_without_textract
 
 
 def render_pdf_page(page: fitz.Page, dpi: int = 150) -> Image:
     mat = fitz.Matrix(dpi / 72, dpi / 72)
     pix = page.get_pixmap(matrix=mat, annots=False, alpha=False)
-    return Image.frombytes("RGB", [pix.width, pix.height])
+    return Image.frombytes("RGB", (pix.width, pix.height), pix.samples)
 
 
 def bbox_to_textract_bounding_box(bbox: Tuple[float, float, float, float], image_box) -> Dict:
     left = min(max(0.0, (bbox[0] - image_box[0]) / (image_box[2] - image_box[0])), 1.0)
     top = min(max(0.0, (bbox[1] - image_box[1]) / (image_box[3] - image_box[1])), 1.0)
     right = min(max(0.0, (bbox[2] - image_box[0]) / (image_box[2] - image_box[0])), 1.0)
     bottom = min(max(0.0, (bbox[3] - image_box[1]) / (image_box[3] - image_box[1])), 1.0)
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.2/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

