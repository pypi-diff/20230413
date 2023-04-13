# Comparing `tmp/sql-face-0.1.8.tar.gz` & `tmp/sql-face-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql-face-0.1.8.tar", last modified: Tue Mar 28 08:45:50 2023, max compression
+gzip compressed data, was "sql-face-0.1.9.tar", last modified: Tue Mar 28 09:09:32 2023, max compression
```

## Comparing `sql-face-0.1.8.tar` & `sql-face-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-03-28 08:45:50.094170 sql-face-0.1.8/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11337 2023-03-14 19:57:31.000000 sql-face-0.1.8/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      111 2023-03-14 19:57:31.000000 sql-face-0.1.8/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1146 2023-03-28 08:45:50.094170 sql-face-0.1.8/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      376 2023-03-14 20:41:08.000000 sql-face-0.1.8/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1341 2023-03-28 08:45:17.000000 sql-face-0.1.8/settings.ini
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-03-28 08:45:50.094170 sql-face-0.1.8/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2541 2023-03-14 19:57:31.000000 sql-face-0.1.8/setup.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-03-28 08:45:50.094170 sql-face-0.1.8/sql_face/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    33162 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/_modidx.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    38503 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/alchemy.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      225 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/core.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    29573 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/databases.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13319 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/faceangles.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    10779 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/qmagface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    36733 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/serfiq.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3526 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/sqldb.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15702 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7873 2023-03-28 08:45:27.000000 sql-face-0.1.8/sql_face/tface.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-03-28 08:45:50.094170 sql-face-0.1.8/sql_face.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1146 2023-03-28 08:45:49.000000 sql-face-0.1.8/sql_face.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-03-28 08:45:50.000000 sql-face-0.1.8/sql_face.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-03-28 08:45:49.000000 sql-face-0.1.8/sql_face.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-03-28 08:45:49.000000 sql-face-0.1.8/sql_face.egg-info/entry_points.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-03-27 22:51:45.000000 sql-face-0.1.8/sql_face.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-03-28 08:45:49.000000 sql-face-0.1.8/sql_face.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        9 2023-03-28 08:45:49.000000 sql-face-0.1.8/sql_face.egg-info/top_level.txt
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-03-28 09:09:32.806524 sql-face-0.1.9/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11337 2023-03-14 19:57:31.000000 sql-face-0.1.9/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      111 2023-03-14 19:57:31.000000 sql-face-0.1.9/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1146 2023-03-28 09:09:32.806524 sql-face-0.1.9/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      376 2023-03-14 20:41:08.000000 sql-face-0.1.9/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1341 2023-03-28 09:09:00.000000 sql-face-0.1.9/settings.ini
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-03-28 09:09:32.806524 sql-face-0.1.9/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2541 2023-03-14 19:57:31.000000 sql-face-0.1.9/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-03-28 09:09:32.802524 sql-face-0.1.9/sql_face/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    33162 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/_modidx.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    38406 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/alchemy.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      225 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/core.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    29573 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/databases.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13319 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/faceangles.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    10779 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/qmagface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    36733 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/serfiq.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3526 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/sqldb.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15910 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7873 2023-03-28 09:09:06.000000 sql-face-0.1.9/sql_face/tface.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-03-28 09:09:32.806524 sql-face-0.1.9/sql_face.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1146 2023-03-28 09:09:32.000000 sql-face-0.1.9/sql_face.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-03-28 09:09:32.000000 sql-face-0.1.9/sql_face.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-03-28 09:09:32.000000 sql-face-0.1.9/sql_face.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-03-28 09:09:32.000000 sql-face-0.1.9/sql_face.egg-info/entry_points.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-03-27 22:51:45.000000 sql-face-0.1.9/sql_face.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-03-28 09:09:32.000000 sql-face-0.1.9/sql_face.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        9 2023-03-28 09:09:32.000000 sql-face-0.1.9/sql_face.egg-info/top_level.txt
```

### Comparing `sql-face-0.1.8/LICENSE` & `sql-face-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/PKG-INFO` & `sql-face-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-face
-Version: 0.1.8
+Version: 0.1.9
 Summary: Saves face image attributes in SQL database.
 Home-page: https://github.com/AndreaMacarulla/sql-face
 Author: AndreaMacarulla
 Author-email: andrea.macarulla@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `sql-face-0.1.8/settings.ini` & `sql-face-0.1.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = sql-face
 lib_name = %(repo)s
-version = 0.1.08
+version = 0.1.09
 min_python = 3.8
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = sql_face
 nbs_path = nbs
```

### Comparing `sql-face-0.1.8/setup.py` & `sql-face-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/_modidx.py` & `sql-face-0.1.9/sql_face/_modidx.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/alchemy.py` & `sql-face-0.1.9/sql_face/alchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,21 +703,21 @@
 
     model = load_model()
 
     updated_face_images = []
     count = 0
 
     for face_img in tqdm(all_face_img, desc='Computing embeddings QMagFace'):
-        
-        try:
-            img = face_img.CroppedImage.get_aligned_image(input_dir, ser_fiq = serfiq)
+        img = face_img.CroppedImage.get_aligned_image(input_dir, ser_fiq = serfiq)
+
+        if img:
             embedding = compute_qmagface_embeddings(img, model)
             face_img.FaceImage.embeddings = embedding
-        except:
-            img = face_img.CroppedImage.get_aligned_image(input_dir, ser_fiq = serfiq)
+
+        else:
             embedding = None
             face_img.FaceImage.embeddings = embedding
             print(f'Problem with embedding in Image id {face_img.CroppedImage.image_id}')
 
         updated_face_images.append({"faceImage_id": face_img.FaceImage.faceImage_id, "embeddings": face_img.FaceImage.embeddings})
         count += 1
         if count % 100 == 0:
```

### Comparing `sql-face-0.1.8/sql_face/databases.py` & `sql-face-0.1.9/sql_face/databases.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/faceangles.py` & `sql-face-0.1.9/sql_face/faceangles.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/qmagface.py` & `sql-face-0.1.9/sql_face/qmagface.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/serfiq.py` & `sql-face-0.1.9/sql_face/serfiq.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/sqldb.py` & `sql-face-0.1.9/sql_face/sqldb.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face/tables.py` & `sql-face-0.1.9/sql_face/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,16 +413,23 @@
             return image
 
     def get_aligned_image(self, input_dir, target_size:Tuple[int,int]=(112,112), ser_fiq = None):
         image = self.images.get_image(input_dir)        
         
         if self.detectors.name == 'mtcnn_serfiq':
              
-            aligned_image = ser_fiq.apply_mtcnn(image)                     
-            return np.transpose(aligned_image, (1,2,0)) 
+            aligned_image = ser_fiq.apply_mtcnn(image)
+            #TODO: FIX THIS
+            try:
+                align_img = np.transpose(aligned_image, (1,2,0))
+            except:
+                align_img = None
+                print(f'Problems with {self.image_id}, image detected {self.face_detected}')
+
+            return align_img
         
         else:
             
             aligned_image = DeepFace.detectFace(img_path = image, 
                                             target_size = target_size, 
                                             detector_backend = self.detectors.name, 
                                             align=True,
```

### Comparing `sql-face-0.1.8/sql_face/tface.py` & `sql-face-0.1.9/sql_face/tface.py`

 * *Files identical despite different names*

### Comparing `sql-face-0.1.8/sql_face.egg-info/PKG-INFO` & `sql-face-0.1.9/sql_face.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-face
-Version: 0.1.8
+Version: 0.1.9
 Summary: Saves face image attributes in SQL database.
 Home-page: https://github.com/AndreaMacarulla/sql-face
 Author: AndreaMacarulla
 Author-email: andrea.macarulla@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

