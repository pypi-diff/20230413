# Comparing `tmp/napari-sam-0.3.5.tar.gz` & `tmp/napari-sam-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.5.tar", last modified: Thu Apr 13 19:07:07 2023, max compression
+gzip compressed data, was "napari-sam-0.3.6.tar", last modified: Thu Apr 13 19:56:14 2023, max compression
```

## Comparing `napari-sam-0.3.5.tar` & `napari-sam-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.187727 napari-sam-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 19:06:51.000000 napari-sam-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 19:06:51.000000 napari-sam-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:07:07.187727 napari-sam-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 19:06:51.000000 napari-sam-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 19:06:51.000000 napari-sam-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 19:07:07.187727 napari-sam-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.183727 napari-sam-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.187727 napari-sam-0.3.5/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-13 19:06:51.000000 napari-sam-0.3.5/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:07:07.187727 napari-sam-0.3.5/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:07:07.000000 napari-sam-0.3.5/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 19:55:57.000000 napari-sam-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 19:55:57.000000 napari-sam-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:56:14.912959 napari-sam-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 19:55:57.000000 napari-sam-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 19:55:57.000000 napari-sam-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 19:56:14.916959 napari-sam-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39447 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.5/LICENSE` & `napari-sam-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.5/PKG-INFO` & `napari-sam-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.5
+Version: 0.3.6
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.5 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.6 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.5/README.md` & `napari-sam-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.5/setup.cfg` & `napari-sam-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.5/src/napari_sam/_widget.py` & `napari-sam-0.3.6/src/napari_sam/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,101 +70,126 @@
         self.comboboxes = [{"combobox": self.cb_image_layers, "layer_type": "image"}, {"combobox": self.cb_label_layers, "layer_type": "labels"}]
 
         self.g_annotation = QGroupBox("Annotation mode")
         self.l_annotation = QVBoxLayout()
 
         self.rb_click = QRadioButton("Click")
         self.rb_click.setChecked(True)
+        self.rb_click.setToolTip("Positive Click: Middle Mouse Button\n \n"
+                                 "Negative Click: Control + Middle Mouse Button \n \n"
+                                 "Undo: Control + Z \n \n"
+                                 "Select Point: Left Click \n \n"
+                                 "Delete Selected Point: Delete")
         self.l_annotation.addWidget(self.rb_click)
         self.rb_click.clicked.connect(self.on_everything_mode_checked)
 
         self.rb_bbox = QRadioButton("Bounding Box (WIP)")
         self.rb_bbox.setEnabled(False)
+        self.rb_bbox.setToolTip("This mode is still Work In Progress (WIP)")
         self.rb_bbox.setStyleSheet("color: gray")
         self.l_annotation.addWidget(self.rb_bbox)
 
         self.rb_auto = QRadioButton("Everything")
         # self.rb_auto.setEnabled(False)
         # self.rb_auto.setStyleSheet("color: gray")
+        self.rb_auto.setToolTip("Creates automatically an instance segmentation \n"
+                                            "of the entire image.\n"
+                                            "No user interaction possible.")
         self.l_annotation.addWidget(self.rb_auto)
         self.rb_auto.clicked.connect(self.on_everything_mode_checked)
 
         self.g_annotation.setLayout(self.l_annotation)
         self.layout().addWidget(self.g_annotation)
 
         self.g_segmentation = QGroupBox("Segmentation mode")
         self.l_segmentation = QVBoxLayout()
 
         self.rb_semantic = QRadioButton("Semantic")
         self.rb_semantic.setChecked(True)
+        self.rb_semantic.setToolTip("Enables the user to create a \n"
+                                 "multi-label (semantic) segmentation of different classes.\n \n"
+                                 "All objects from the same class \n"
+                                 "should be given the same label by the user.\n \n"
+                                 "The current label can be changed by the user \n"
+                                 "on the labels layer pane after selecting the labels layer.")
         # self.rb_semantic.setEnabled(False)
         # self.rb_semantic.setStyleSheet("color: gray")
         self.l_segmentation.addWidget(self.rb_semantic)
 
         self.rb_instance = QRadioButton("Instance")
+        self.rb_instance.setToolTip("Enables the user to create an \n"
+                                 "instance segmentation of different objects.\n \n"
+                                 "Objects can be from the same or different classes,\n"
+                                 "but each object should be given a unique label by the user. \n \n"
+                                 "The current label can be changed by the user \n"
+                                 "on the labels layer pane after selecting the labels layer.")
         # self.rb_instance.setEnabled(False)
         # self.rb_instance.setStyleSheet("color: gray")
         self.l_segmentation.addWidget(self.rb_instance)
 
         self.g_segmentation.setLayout(self.l_segmentation)
         self.layout().addWidget(self.g_segmentation)
 
         self.btn_activate = QPushButton("Activate")
         self.btn_activate.clicked.connect(self._activate)
         self.btn_activate.setEnabled(False)
         self.is_active = False
         self.layout().addWidget(self.btn_activate)
 
+        self.g_info_tooltip = QGroupBox("Tooltip Information")
+        self.l_info_tooltip = QVBoxLayout()
+        self.label_info_tooltip = QLabel("Every mode shows further information\n"
+                                         "when hovered over.")
+        self.l_info_tooltip.addWidget(self.label_info_tooltip)
+        self.g_info_tooltip.setLayout(self.l_info_tooltip)
+        self.layout().addWidget(self.g_info_tooltip)
+
         self.g_info_click = QGroupBox("Click Mode")
         self.l_info_click = QVBoxLayout()
-
         self.label_info_click = QLabel("Positive Click: Middle Mouse Button\n \n"
                                  "Negative Click: Control + Middle Mouse Button \n \n"
                                  "Undo: Control + Z \n \n"
                                  "Select Point: Left Click \n \n"
                                  "Delete Selected Point: Delete")
         self.l_info_click.addWidget(self.label_info_click)
         self.g_info_click.setLayout(self.l_info_click)
         self.layout().addWidget(self.g_info_click)
 
-        self.g_info_everything = QGroupBox("Everything Mode")
-        self.l_info_everything = QVBoxLayout()
-
-        self.label_info_everything = QLabel("Creates automatically an instance segmentation \n"
-                                            "of the entire image.\n"
-                                            "No user interaction possible.")
-        self.l_info_everything.addWidget(self.label_info_everything)
-        self.g_info_everything.setLayout(self.l_info_everything)
-        self.layout().addWidget(self.g_info_everything)
-
-        self.g_info_semantic = QGroupBox("Semantic Mode")
-        self.l_info_semantic = QVBoxLayout()
-
-        self.label_info_semantic = QLabel("Enables the user to create a \n"
-                                 "multi-label (semantic) segmentation of different classes.\n \n"
-                                 "All objects from the same class \n"
-                                 "should be given the same label by the user.\n \n"
-                                 "The current label can be changed by the user \n"
-                                 "on the labels layer pane after selecting the labels layer.")
-        self.l_info_semantic.addWidget(self.label_info_semantic)
-        self.g_info_semantic.setLayout(self.l_info_semantic)
-        self.layout().addWidget(self.g_info_semantic)
-
-        self.g_info_instance = QGroupBox("Instance Mode")
-        self.l_info_instance = QVBoxLayout()
-
-        self.label_info_instance = QLabel("Enables the user to create an \n"
-                                 "instance segmentation of different objects.\n \n"
-                                 "Objects can be from the same or different classes,\n"
-                                 "but each object should be given a unique label by the user. \n \n"
-                                 "The current label can be changed by the user \n"
-                                 "on the labels layer pane after selecting the labels layer.")
-        self.l_info_instance.addWidget(self.label_info_instance)
-        self.g_info_instance.setLayout(self.l_info_instance)
-        self.layout().addWidget(self.g_info_instance)
+        # self.g_info_everything = QGroupBox("Everything Mode")
+        # self.l_info_everything = QVBoxLayout()
+        # self.label_info_everything = QLabel("Creates automatically an instance segmentation \n"
+        #                                     "of the entire image.\n"
+        #                                     "No user interaction possible.")
+        # self.l_info_everything.addWidget(self.label_info_everything)
+        # self.g_info_everything.setLayout(self.l_info_everything)
+        # self.layout().addWidget(self.g_info_everything)
+
+        # self.g_info_semantic = QGroupBox("Semantic Mode")
+        # self.l_info_semantic = QVBoxLayout()
+        # self.label_info_semantic = QLabel("Enables the user to create a \n"
+        #                          "multi-label (semantic) segmentation of different classes.\n \n"
+        #                          "All objects from the same class \n"
+        #                          "should be given the same label by the user.\n \n"
+        #                          "The current label can be changed by the user \n"
+        #                          "on the labels layer pane after selecting the labels layer.")
+        # self.l_info_semantic.addWidget(self.label_info_semantic)
+        # self.g_info_semantic.setLayout(self.l_info_semantic)
+        # self.layout().addWidget(self.g_info_semantic)
+
+        # self.g_info_instance = QGroupBox("Instance Mode")
+        # self.l_info_instance = QVBoxLayout()
+        # self.label_info_instance = QLabel("Enables the user to create an \n"
+        #                          "instance segmentation of different objects.\n \n"
+        #                          "Objects can be from the same or different classes,\n"
+        #                          "but each object should be given a unique label by the user. \n \n"
+        #                          "The current label can be changed by the user \n"
+        #                          "on the labels layer pane after selecting the labels layer.")
+        # self.l_info_instance.addWidget(self.label_info_instance)
+        # self.g_info_instance.setLayout(self.l_info_instance)
+        # self.layout().addWidget(self.g_info_instance)
 
         self.image_name = None
         self.image_layer = None
         self.label_layer = None
         self.label_layer_changes = None
         self.label_color_mapping = None
         self.points_layer = None
@@ -368,24 +393,25 @@
                 self.create_label_color_mapping()
 
                 with warnings.catch_warnings():
                     warnings.filterwarnings("ignore", category=FutureWarning)
                     self._history_limit = self.label_layer._history_limit
                 self._reset_history()
 
-                self.viewer.mouse_drag_callbacks.append(self.callback_click)
-                self.viewer.keymap['Delete'] = self.on_delete
-                self.label_layer.keymap['Control-Z'] = self.on_undo
-                self.label_layer.keymap['Control-Shift-Z'] = self.on_redo
                 if self.image_layer.ndim == 3:
                     self.image_layer.events.contrast_limits.connect(self.on_contrast_limits_change)
 
                 self.set_image()
                 self.update_points_layer(None)
 
+                self.viewer.mouse_drag_callbacks.append(self.callback_click)
+                self.viewer.keymap['Delete'] = self.on_delete
+                self.label_layer.keymap['Control-Z'] = self.on_undo
+                self.label_layer.keymap['Control-Shift-Z'] = self.on_redo
+
             elif self.annotator_mode == AnnotatorMode.AUTO:
                 image = self.image_layer.data
                 if not self.image_layer.rgb:
                     image = np.stack((image,)*3, axis=-1)  # Expand to 3-channel image
                 image = image[..., :3]  # Remove a potential alpha channel
                 records = self.sam_anything_predictor.generate(image)
                 masks = np.asarray([record["segmentation"] for record in records])
```

### Comparing `napari-sam-0.3.5/src/napari_sam/utils.py` & `napari-sam-0.3.6/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.5/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.6/src/napari_sam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.5
+Version: 0.3.6
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
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.5 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.6 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

