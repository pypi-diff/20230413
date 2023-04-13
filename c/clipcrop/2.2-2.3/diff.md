# Comparing `tmp/clipcrop-2.2.tar.gz` & `tmp/clipcrop-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcrop-2.2.tar", last modified: Wed Apr 12 11:26:52 2023, max compression
+gzip compressed data, was "clipcrop-2.3.tar", last modified: Thu Apr 13 13:37:20 2023, max compression
```

## Comparing `clipcrop-2.2.tar` & `clipcrop-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:26:52.960560 clipcrop-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 11:26:44.000000 clipcrop-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-12 11:26:52.960560 clipcrop-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 11:26:44.000000 clipcrop-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:26:52.960560 clipcrop-2.2/clipcrop/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:26:44.000000 clipcrop-2.2/clipcrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-12 11:26:44.000000 clipcrop-2.2/clipcrop/clipcrop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:26:52.960560 clipcrop-2.2/clipcrop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 11:26:52.000000 clipcrop-2.2/clipcrop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 11:26:52.960560 clipcrop-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-12 11:26:44.000000 clipcrop-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:37:20.932810 clipcrop-2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 13:37:10.000000 clipcrop-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-13 13:37:20.932810 clipcrop-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-13 13:37:10.000000 clipcrop-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:37:20.932810 clipcrop-2.3/clipcrop/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:37:10.000000 clipcrop-2.3/clipcrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-13 13:37:10.000000 clipcrop-2.3/clipcrop/clipcrop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:37:20.932810 clipcrop-2.3/clipcrop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 13:37:20.000000 clipcrop-2.3/clipcrop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 13:37:20.936810 clipcrop-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 13:37:10.000000 clipcrop-2.3/setup.py
```

### Comparing `clipcrop-2.2/LICENSE` & `clipcrop-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clipcrop-2.2/PKG-INFO` & `clipcrop-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.2
+Version: 2.3
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.2/README.md` & `clipcrop-2.3/README.md`

 * *Files identical despite different names*

### Comparing `clipcrop-2.2/clipcrop/clipcrop.py` & `clipcrop-2.3/clipcrop/clipcrop.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,61 +17,54 @@
     DFE = DetrFeatureExtractor.from_pretrained('facebook/detr-resnet-50')
     DM = DetrForObjectDetection.from_pretrained('facebook/detr-resnet-50')
     CLIPM = CLIPModel.from_pretrained("openai/clip-vit-base-patch32")
     CLIPP = CLIPProcessor.from_pretrained("openai/clip-vit-base-patch32")
 
     return DFE, DM, CLIPM, CLIPP
 
-  def captcha(self, DFE, DM, CLIPM, CLIPP, th=0.95):
+  def captcha(self, CLIPM, CLIPP, th=3):
     
     self.th = th
-    self.DFE = DFE
-    self.DM = DM
     self.CLIPM = CLIPM
     self.CLIPP = CLIPP
 
     image = cv2.imread(self.image_path)
-    inputs = self.DFE(images=image, return_tensors="pt")
-    outputs = self.DM(**inputs)
-
-    # model predicts bounding boxes and corresponding COCO classes
-    logits = outputs.logits
-    bboxes = outputs.pred_boxes
-    probas = outputs.logits.softmax(-1)[0, :, :-1] #removing no class as detr maps 
-
-    keep = probas.max(-1).values > self.th
-    outs = self.DFE.post_process(outputs, torch.tensor(image.shape[:2]).unsqueeze(0))
-    bboxes_scaled = outs[0]['boxes'][keep].detach().numpy()
-    labels = outs[0]['labels'][keep].detach().numpy()
-    scores = outs[0]['scores'][keep].detach().numpy()
-    num = 5
-
-    images_list = []
-    for i,j in enumerate(bboxes_scaled):
-      
-      xmin = int(j[0])
-      ymin = int(j[1])
-      xmax = int(j[2])
-      ymax = int(j[3])
-      
-      roi = image[ymin:ymax, xmin:xmax]
-      roi_im = Image.fromarray(roi)
-      images_list.append(roi_im)
+    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+    blur = cv2.medianBlur(gray, 3)
+    sharpen_kernel = np.array([[-1,-1,-1], [-1,9,-1], [-1,-1,-1]])
+    sharpen = cv2.filter2D(blur, -1, sharpen_kernel)
+
+    # Threshold and morph close
+    thresh = cv2.threshold(sharpen, 160, 255, cv2.THRESH_BINARY_INV)[1]
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1,1))
+    close = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel, iterations=2)
+
+    # Find contours and filter using threshold area
+    cnts = cv2.findContours(close, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+    cnts = cnts[0] if len(cnts) == 2 else cnts[1]
+
+    image_number = 0
+    img_list = []
+    r_list = []
+    for c in cnts:    
+        x,y,w,h = cv2.boundingRect(c)
+        if w/h == 1 and (w, h) > (5, 5):
+            ROI = image[y:y+h, x:x+w]
+            img_list.append(Image.fromarray(ROI[:,:,::-1]))
+            r_list.append([(x, y), (x + w, y + h)])
+            image_number += 1
 
-    inps = self.CLIPP(text = [self.text], images=images_list , return_tensors="pt", padding=True)
+    inps = self.CLIPP(text = [self.text], images=img_list , return_tensors="pt", padding=True)
     outs = self.CLIPM(**inps)
     logits_per_image = outs.logits_per_text
     probs = logits_per_image.softmax(-1)
-    l_idx = np.argsort(probs[-1].detach().numpy())[::-1][0:num]
+    l_idx = list(np.argsort(probs[-1].detach().numpy())[::-1][0:self.th])
 
-    for i, j in enumerate(images_list):
-      if i in l_idx:
-        cv2.rectangle(image, (int(bboxes_scaled[i][0]), int(bboxes_scaled[i][1])), 
-        (int(bboxes_scaled[i][2]), int(bboxes_scaled[i][3])), 
-        (255,0,0), 4)
+    for x in l_idx:
+      cv2.rectangle(image, r_list[x][0], r_list[x][1], (36,255,12), 2)
 
     return Image.fromarray(image[:,:,::-1])
 
   def extract_image(self, DFE, DM, CLIPM, CLIPP, num=3):
 
     self.DFE = DFE
     self.DM = DM
```

### Comparing `clipcrop-2.2/clipcrop.egg-info/PKG-INFO` & `clipcrop-2.3/clipcrop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcrop
-Version: 2.2
+Version: 2.3
 Summary: Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers
 Home-page: https://github.com/Vishnunkumar/clipcrop/
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: clipcrop
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clipcrop-2.2/setup.py` & `clipcrop-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   'numpy',
   'opencv-python'
 ]
 
 
 setuptools.setup(
     name="clipcrop",
-    version="2.2",
+    version="2.3",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="Extract sections from your image by using OpenAI CLIP and Facebooks Detr implemented on HuggingFace Transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/clipcrop/',
     packages=[
```

