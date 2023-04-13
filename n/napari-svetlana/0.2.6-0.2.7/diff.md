# Comparing `tmp/napari_svetlana-0.2.6.tar.gz` & `tmp/napari_svetlana-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_svetlana-0.2.6.tar", last modified: Thu Apr 13 09:59:28 2023, max compression
+gzip compressed data, was "napari_svetlana-0.2.7.tar", last modified: Thu Apr 13 10:17:52 2023, max compression
```

## Comparing `napari_svetlana-0.2.6.tar` & `napari_svetlana-0.2.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    35148 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/LICENSE
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      161 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/MANIFEST.in
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7412 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/PKG-INFO
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     6194 2023-04-13 09:15:00.000000 napari_svetlana-0.2.6/README.md
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      193 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/requirements.txt
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1568 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/setup.cfg
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       84 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/setup.py
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/napari_svetlana/
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1637 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CNN2D.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1451 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CNN3D.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      619 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Config.json
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      879 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CustomDataset.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1049 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CustomDialog.py
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/__init__.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     8885 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/base_cam.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      751 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/grad_cam.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7323 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/image.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2981 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Prediction3DDataset.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3742 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/PredictionDataset.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3087 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/PredictionMulti3DDataset.py
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/src/napari_svetlana/XP/
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3420 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/Predict3Dbatch.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2381 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/Prediction3DDataset_dilation.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/__init__.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2075 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/compute_accuracy.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3527 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/extract_save_patches.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1558 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/modulable_CNN3D.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1196 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/redim.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     5315 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/reseau.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    17178 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training-stability_test.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    16325 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_1net.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    14958 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    13280 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    11531 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_test.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    28297 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/testeur.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      195 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/__init__.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)   152098 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_batch_dock_widget.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    66687 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_dock_widget.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1708 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_function.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2771 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_reader.py
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/src/napari_svetlana/_tests/
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/__init__.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1249 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_dock_widget.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      117 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_function.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      976 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_reader.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      127 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_writer.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      463 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_writer.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       77 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/debug.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1205 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/mosa.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    62329 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/old_dock_widget.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     5073 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam.py
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     4837 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam3D.py
-drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7412 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/PKG-INFO
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2008 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/SOURCES.txt
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        1 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/dependency_links.txt
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       50 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/entry_points.txt
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      211 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/requires.txt
--rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       16 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/top_level.txt
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    35148 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/LICENSE
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      161 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/MANIFEST.in
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7412 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/PKG-INFO
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     6194 2023-04-13 09:15:00.000000 napari_svetlana-0.2.7/README.md
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      193 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/requirements.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1568 2023-04-13 10:17:52.407575 napari_svetlana-0.2.7/setup.cfg
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       84 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/setup.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.399574 napari_svetlana-0.2.7/src/
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/src/napari_svetlana/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1637 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/CNN2D.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1451 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/CNN3D.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      619 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/Config.json
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      879 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/CustomDataset.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1049 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/CustomDialog.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     8885 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/base_cam.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      751 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/grad_cam.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7323 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/image.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2981 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/Prediction3DDataset.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3742 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/PredictionDataset.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3087 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/PredictionMulti3DDataset.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/src/napari_svetlana/XP/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3420 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/Predict3Dbatch.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2381 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/Prediction3DDataset_dilation.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2075 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/compute_accuracy.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3527 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/extract_save_patches.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1558 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/modulable_CNN3D.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1196 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/redim.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     5315 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/reseau.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    17178 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training-stability_test.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    16325 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_3D_1net.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    14958 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    13280 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    11531 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_test.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    28297 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/XP/testeur.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      195 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)   152098 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_batch_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    66687 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1708 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_function.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2771 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_reader.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/src/napari_svetlana/_tests/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_tests/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1249 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_tests/test_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      117 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_tests/test_function.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      976 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_tests/test_reader.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      127 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_tests/test_writer.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      463 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/_writer.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       77 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/debug.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1205 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/mosa.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    62329 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/old_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     5073 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/test_gradcam.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     4837 2023-02-09 16:50:37.000000 napari_svetlana-0.2.7/src/napari_svetlana/test_gradcam3D.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 10:17:52.403575 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7412 2023-04-13 10:17:52.000000 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/PKG-INFO
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2008 2023-04-13 10:17:52.000000 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/SOURCES.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        1 2023-04-13 10:17:52.000000 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/dependency_links.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       50 2023-04-13 10:17:52.000000 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/entry_points.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      211 2023-04-13 10:17:52.000000 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/requires.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       16 2023-04-13 10:17:52.000000 napari_svetlana-0.2.7/src/napari_svetlana.egg-info/top_level.txt
```

### Comparing `napari_svetlana-0.2.6/LICENSE` & `napari_svetlana-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/PKG-INFO` & `napari_svetlana-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_svetlana
-Version: 0.2.6
+Version: 0.2.7
 Summary: A classification plugin for the ROIs of a segmentation mask.
 Author: Clément Cazorla
 Author-email: clement.cazorla31@gmail.com
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://bitbucket.org/koopa31/napari_svetlana/issues?status=new&status=open
 Project-URL: Documentation, https://svetlana-documentation.readthedocs.io/en/latest/
 Project-URL: Source Code, https://bitbucket.org/koopa31/napari_svetlana/src/main/
```

### Comparing `napari_svetlana-0.2.6/README.md` & `napari_svetlana-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/setup.cfg` & `napari_svetlana-0.2.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_svetlana
-version = 0.2.6
+version = 0.2.7
 author = Clément Cazorla
 author_email = clement.cazorla31@gmail.com
 license = GPL-3.0-only
 description = A classification plugin for the ROIs of a segmentation mask.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/CNN2D.py` & `napari_svetlana-0.2.7/src/napari_svetlana/CNN2D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/CNN3D.py` & `napari_svetlana-0.2.7/src/napari_svetlana/CNN3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/Config.json` & `napari_svetlana-0.2.7/src/napari_svetlana/Config.json`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/CustomDataset.py` & `napari_svetlana-0.2.7/src/napari_svetlana/CustomDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/CustomDialog.py` & `napari_svetlana-0.2.7/src/napari_svetlana/CustomDialog.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/base_cam.py` & `napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/base_cam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/grad_cam.py` & `napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/grad_cam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/image.py` & `napari_svetlana-0.2.7/src/napari_svetlana/Grad_Cam/image.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/Prediction3DDataset.py` & `napari_svetlana-0.2.7/src/napari_svetlana/Prediction3DDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/PredictionDataset.py` & `napari_svetlana-0.2.7/src/napari_svetlana/PredictionDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/PredictionMulti3DDataset.py` & `napari_svetlana-0.2.7/src/napari_svetlana/PredictionMulti3DDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/Predict3Dbatch.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/Predict3Dbatch.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/Prediction3DDataset_dilation.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/Prediction3DDataset_dilation.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/compute_accuracy.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/compute_accuracy.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/extract_save_patches.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/extract_save_patches.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/modulable_CNN3D.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/modulable_CNN3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/redim.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/redim.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/reseau.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/reseau.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training-stability_test.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training-stability_test.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_1net.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_3D_1net.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_test.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/script_training_test.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/XP/testeur.py` & `napari_svetlana-0.2.7/src/napari_svetlana/XP/testeur.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/_batch_dock_widget.py` & `napari_svetlana-0.2.7/src/napari_svetlana/_batch_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/_dock_widget.py` & `napari_svetlana-0.2.7/src/napari_svetlana/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/_function.py` & `napari_svetlana-0.2.7/src/napari_svetlana/_function.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/_reader.py` & `napari_svetlana-0.2.7/src/napari_svetlana/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_dock_widget.py` & `napari_svetlana-0.2.7/src/napari_svetlana/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_reader.py` & `napari_svetlana-0.2.7/src/napari_svetlana/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/mosa.py` & `napari_svetlana-0.2.7/src/napari_svetlana/mosa.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/old_dock_widget.py` & `napari_svetlana-0.2.7/src/napari_svetlana/old_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam.py` & `napari_svetlana-0.2.7/src/napari_svetlana/test_gradcam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam3D.py` & `napari_svetlana-0.2.7/src/napari_svetlana/test_gradcam3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana.egg-info/PKG-INFO` & `napari_svetlana-0.2.7/src/napari_svetlana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svetlana
-Version: 0.2.6
+Version: 0.2.7
 Summary: A classification plugin for the ROIs of a segmentation mask.
 Author: Clément Cazorla
 Author-email: clement.cazorla31@gmail.com
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://bitbucket.org/koopa31/napari_svetlana/issues?status=new&status=open
 Project-URL: Documentation, https://svetlana-documentation.readthedocs.io/en/latest/
 Project-URL: Source Code, https://bitbucket.org/koopa31/napari_svetlana/src/main/
```

### Comparing `napari_svetlana-0.2.6/src/napari_svetlana.egg-info/SOURCES.txt` & `napari_svetlana-0.2.7/src/napari_svetlana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

