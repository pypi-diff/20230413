# Comparing `tmp/napari-sam-0.3.4.tar.gz` & `tmp/napari-sam-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.4.tar", last modified: Thu Apr 13 07:47:00 2023, max compression
+gzip compressed data, was "napari-sam-0.3.5.tar", last modified: Thu Apr 13 19:07:07 2023, max compression
```

## Comparing `napari-sam-0.3.4.tar` & `napari-sam-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.200459 napari-sam-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 07:46:43.000000 napari-sam-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 07:46:43.000000 napari-sam-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 07:47:00.200459 napari-sam-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 07:46:43.000000 napari-sam-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 07:46:43.000000 napari-sam-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 07:47:00.204459 napari-sam-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.196459 napari-sam-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.200459 napari-sam-0.3.4/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36427 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-13 07:46:43.000000 napari-sam-0.3.4/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:47:00.200459 napari-sam-0.3.4/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 07:47:00.000000 napari-sam-0.3.4/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.187727 napari-sam-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 19:06:51.000000 napari-sam-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 19:06:51.000000 napari-sam-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:07:07.187727 napari-sam-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 19:06:51.000000 napari-sam-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 19:06:51.000000 napari-sam-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 19:07:07.187727 napari-sam-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.183727 napari-sam-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.187727 napari-sam-0.3.5/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.187727 napari-sam-0.3.5/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.4/LICENSE` & `napari-sam-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.4/PKG-INFO` & `napari-sam-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.4
+Version: 0.3.5
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.4 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.5 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.4/README.md` & `napari-sam-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.4/setup.cfg` & `napari-sam-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.4/src/napari_sam/_widget.py` & `napari-sam-0.3.5/src/napari_sam/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,19 @@
             self.image_layer = self.viewer.layers[self.cb_image_layers.currentText()]
             self.label_layer = self.viewer.layers[self.cb_label_layers.currentText()]
             self.label_layer_changes = None
 
             if self.image_layer.ndim != 2 and self.image_layer.ndim != 3:
                 raise RuntimeError("Only 2D and 3D images are supported.")
 
+            if self.image_layer.ndim == 2:
+                self.sam_logits = None
+            else:
+                self.sam_logits = [None] * self.image_layer.data.shape[0]
+
             if self.rb_click.isChecked():
                 self.annotator_mode = AnnotatorMode.CLICK
                 self.rb_bbox.setEnabled(False)
                 self.rb_auto.setEnabled(False)
                 self.rb_bbox.setStyleSheet("color: gray")
                 self.rb_auto.setStyleSheet("color: gray")
             elif self.rb_bbox.isChecked():
@@ -525,58 +530,77 @@
             labels_flattended = []
             for label, label_points in points.items():
                 points_flattened.extend(label_points)
                 label = int(label == point_label)
                 labels = [label] * len(label_points)
                 labels_flattended.extend(labels)
 
-            prediction, self.sam_logits = self.predict(points_flattened, labels_flattended)
+            prediction, predicted_slices = self.predict(points_flattened, labels_flattended)
         else:
             prediction = np.zeros_like(self.label_layer.data)
+            predicted_slices = slice(None, None)
 
         changed_indices = np.where(prediction == 1)
         index_labels_old = self.label_layer.data[changed_indices]
-        self.label_layer.data[self.label_layer.data == point_label] = 0
+        self.label_layer.data[predicted_slices][self.label_layer.data[predicted_slices] == point_label] = 0
         if self.segmentation_mode == SegmentationMode.SEMANTIC or point_label == 0:
             self.label_layer.data[prediction == 1] = point_label
         else:
             self.label_layer.data[(prediction == 1) & (self.label_layer.data == 0)] = point_label
         index_labels_new = self.label_layer.data[changed_indices]
         self.label_layer_changes = {"indices": changed_indices, "old_values": index_labels_old, "new_values": index_labels_new}
         self.label_layer.data = self.label_layer.data
+        self.old_points = copy.deepcopy(self.points_layer.data)
         # self.label_layer.refresh()
 
     def predict(self, points, labels):
         points = np.asarray(points)
+        old_point, new_point = self.find_changed_point(np.asarray(self.old_points), points)
         if self.image_layer.ndim == 2:
             self.sam_predictor.features = self.sam_features
-            prediction, _, sam_logits = self.sam_predictor.predict(
+            prediction, _, self.sam_logits = self.sam_predictor.predict(
                 point_coords=np.flip(points, axis=-1),
                 point_labels=np.asarray(labels),
                 mask_input=self.sam_logits,
                 multimask_output=False,
             )
             prediction = prediction[0]
+            predicted_slices = None
         elif self.image_layer.ndim == 3:
             x_coords = np.unique(points[:, 0])
             groups = {x_coord: list(points[points[:, 0] == x_coord]) for x_coord in x_coords}  # Group points if they are on the same image slice
+            x_coord = new_point[0]
             prediction = np.zeros_like(self.label_layer.data)
 
-            for x_coord, group_points in groups.items():
-                group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
-                group_points = [point[1:] for point in group_points]
-                self.sam_predictor.features = self.sam_features[x_coord - 1]
-                prediction_yz, _, _ = self.sam_predictor.predict(
-                    point_coords=np.flip(group_points, axis=-1),
-                    point_labels=np.asarray(group_labels),
-                    mask_input=self.sam_logits,
-                    multimask_output=False,
-                )
-                prediction_yz = prediction_yz[0]
-                prediction[x_coord, :, :] = prediction_yz
+            group_points = groups[x_coord]
+            group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
+            group_points = [point[1:] for point in group_points]
+            self.sam_predictor.features = self.sam_features[x_coord]
+            prediction_yz, _, self.sam_logits[x_coord] = self.sam_predictor.predict(
+                point_coords=np.flip(group_points, axis=-1),
+                point_labels=np.asarray(group_labels),
+                mask_input=self.sam_logits[x_coord],
+                multimask_output=False,
+            )
+            prediction_yz = prediction_yz[0]
+            prediction[x_coord, :, :] = prediction_yz
+            predicted_slices = x_coord
+
+            # for x_coord, group_points in groups.items():
+            #     group_labels = [labels[np.argwhere(np.all(points == point, axis=1)).flatten()[0]] for point in group_points]
+            #     group_points = [point[1:] for point in group_points]
+            #     self.sam_predictor.features = self.sam_features[x_coord]
+            #     prediction_yz, _, _ = self.sam_predictor.predict(
+            #         point_coords=np.flip(group_points, axis=-1),
+            #         point_labels=np.asarray(group_labels),
+            #         mask_input=self.sam_logits,
+            #         multimask_output=False,
+            #     )
+            #     prediction_yz = prediction_yz[0]
+            #     prediction[x_coord, :, :] = prediction_yz
             sam_logits = None  # TODO: Use sam_logits
         # elif self.image_layer.ndim == 3:
         #     z_coords = np.unique(points[:, 2])
         #     groups = {x_coord: list(points[points[:, 2] == x_coord]) for x_coord in z_coords}  # Group points if they are on the same image slice
         #     image_point_proposals, image_label_proposals = [], []
         #
         #     for x_coord, group_points in groups.items():
@@ -617,15 +641,15 @@
         #         )
         #         prediction_yz = prediction_yz[0]
         #         prediction[x_coord, :, :] = prediction_yz  # prediction_yz is 2D
         #     print("")
         #     sam_logits = None  # TODO: Use sam_logits
         else:
             raise RuntimeError("Only 2D and 3D images are supported.")
-        return prediction, sam_logits
+        return prediction, predicted_slices
 
     def update_points_layer(self, points):
         selected_layer = None
         if self.viewer.layers.selection.active != self.points_layer:
             selected_layer = self.viewer.layers.selection.active
         if self.points_layer is not None:
             self.viewer.layers.remove(self.points_layer)
@@ -642,17 +666,14 @@
         self.point_size = int(np.min(self.image_layer.data.shape[:2]) / 100)
         if self.point_size == 0:
             self.point_size = 1
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             self.points_layer = self.viewer.add_points(name=self.points_layer_name, data=np.asarray(points_flattened), face_color=colors_flattended, edge_color="white", size=self.point_size)
         self.points_layer.editable = False
-        self.old_points = copy.deepcopy(self.points_layer.data)
-
-        # self.points_layer.events.data.connect(self.on_points_changed)
 
         if selected_layer is not None:
             self.viewer.layers.selection.active = selected_layer
         self.points_layer.refresh()
 
     def on_points_changed(self, event):
         self._save_history({"points": copy.deepcopy(self.points), "logits": self.sam_logits, "point_label": self.point_label})
@@ -668,33 +689,31 @@
         self.sam_logits = None
         self.run(self.points, self.point_label)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=FutureWarning)
             self.label_layer._save_history((self.label_layer_changes["indices"], self.label_layer_changes["old_values"], self.label_layer_changes["new_values"]))
 
     def find_changed_point(self, old_points, new_points):
-        # changed_point = None
-        # changed_label = None
-        # for label, label_points in self.points.items():
-        #     for point in label_points:
-        #         is_unchanged = False
-        #         for point_layer in self.points_layer.data:
-        #             if np.array_equal(point_layer, point):
-        #                 is_unchanged = True
-        #         if not is_unchanged:
-        #             return point, label
-        # if changed_point is None:
+        if len(new_points) == 0:
+            old_point = old_points
+        else:
+            old_point = np.array([x for x in old_points if not np.any((x == new_points).all(1))])
+        if len(old_points) == 0:
+            new_point = new_points
+        else:
+            new_point = np.array([x for x in new_points if not np.any((x == old_points).all(1))])
+
+        # if (len(old_point) != 0 and len(old_point) != 1) or (len(new_point) != 0 and len(new_point) != 1):
         #     raise RuntimeError("Could not identify a changed point.")
-        old_point = np.array([x for x in old_points if not np.any((x == new_points).all(1))])
-        new_point = np.array([x for x in new_points if not np.any((x == old_points).all(1))])
 
-        if len(old_point) != 1 or (len(new_point) != 0 and len(new_point) != 1):
-            raise RuntimeError("Could not identify a changed point.")
+        if len(old_point) == 0:
+            old_point = None
+        else:
+            old_point = old_point[0]
 
-        old_point = old_point[0]
         if len(new_point) == 0:
             new_point = None
         else:
             new_point = new_point[0]
 
         return old_point, new_point
```

### Comparing `napari-sam-0.3.4/src/napari_sam/utils.py` & `napari-sam-0.3.5/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.4/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.5/src/napari_sam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.4
+Version: 0.3.5
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.4 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.5 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

