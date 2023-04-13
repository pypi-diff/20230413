# Comparing `tmp/napari_svetlana-0.2.5.tar.gz` & `tmp/napari_svetlana-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_svetlana-0.2.5.tar", last modified: Thu Jan 26 15:15:01 2023, max compression
+gzip compressed data, was "napari_svetlana-0.2.6.tar", last modified: Thu Apr 13 09:59:28 2023, max compression
```

## Comparing `napari_svetlana-0.2.5.tar` & `napari_svetlana-0.2.6.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.882088 napari_svetlana-0.2.5/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    35148 2022-09-30 10:01:24.000000 napari_svetlana-0.2.5/LICENSE
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      161 2022-12-16 13:35:37.000000 napari_svetlana-0.2.5/MANIFEST.in
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     7042 2023-01-26 15:15:01.882088 napari_svetlana-0.2.5/PKG-INFO
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     5824 2023-01-26 15:13:55.000000 napari_svetlana-0.2.5/README.md
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      193 2022-11-18 17:02:26.000000 napari_svetlana-0.2.5/requirements.txt
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1568 2023-01-26 15:15:01.882088 napari_svetlana-0.2.5/setup.cfg
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)       84 2022-01-13 13:36:49.000000 napari_svetlana-0.2.5/setup.py
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.870088 napari_svetlana-0.2.5/src/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    12021 2022-12-16 09:19:44.000000 napari_svetlana-0.2.5/src/doc.png
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.874088 napari_svetlana-0.2.5/src/napari_svetlana/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1637 2022-10-28 13:39:12.000000 napari_svetlana-0.2.5/src/napari_svetlana/CNN2D.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1451 2022-10-28 14:54:23.000000 napari_svetlana-0.2.5/src/napari_svetlana/CNN3D.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      619 2022-08-18 08:46:58.000000 napari_svetlana-0.2.5/src/napari_svetlana/Config.json
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      879 2022-01-28 12:35:27.000000 napari_svetlana-0.2.5/src/napari_svetlana/CustomDataset.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1049 2022-02-23 16:55:08.000000 napari_svetlana-0.2.5/src/napari_svetlana/CustomDialog.py
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.878088 napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)        0 2022-11-18 15:27:56.000000 napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/__init__.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     8885 2022-10-28 15:39:37.000000 napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/base_cam.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      751 2022-10-28 15:45:49.000000 napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/grad_cam.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     7323 2022-10-28 15:40:31.000000 napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/image.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     2981 2022-11-18 15:27:56.000000 napari_svetlana-0.2.5/src/napari_svetlana/Prediction3DDataset.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     3742 2022-08-18 08:46:58.000000 napari_svetlana-0.2.5/src/napari_svetlana/PredictionDataset.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     3087 2022-10-28 14:43:55.000000 napari_svetlana-0.2.5/src/napari_svetlana/PredictionMulti3DDataset.py
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.878088 napari_svetlana-0.2.5/src/napari_svetlana/XP/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     3420 2022-07-28 07:51:59.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/Predict3Dbatch.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     2381 2022-07-28 09:35:39.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/Prediction3DDataset_dilation.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)        0 2022-07-28 07:51:59.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/__init__.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     2075 2022-07-29 09:19:22.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/compute_accuracy.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     3527 2022-08-18 08:46:58.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/extract_save_patches.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1558 2022-11-17 09:03:51.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/modulable_CNN3D.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1196 2022-10-27 12:17:14.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/redim.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     5315 2022-07-28 07:51:59.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/reseau.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    17178 2022-08-18 09:28:19.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training-stability_test.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    16325 2022-08-18 08:46:58.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_3D_1net.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    14958 2022-08-18 08:46:58.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    13280 2022-07-28 07:51:59.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    11531 2022-07-28 07:51:59.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_test.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    28297 2022-07-28 07:51:59.000000 napari_svetlana-0.2.5/src/napari_svetlana/XP/testeur.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      195 2022-04-29 13:42:41.000000 napari_svetlana-0.2.5/src/napari_svetlana/__init__.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)   152098 2023-01-06 16:49:32.000000 napari_svetlana-0.2.5/src/napari_svetlana/_batch_dock_widget.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    66687 2022-04-29 13:42:26.000000 napari_svetlana-0.2.5/src/napari_svetlana/_dock_widget.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1708 2022-01-13 13:36:49.000000 napari_svetlana-0.2.5/src/napari_svetlana/_function.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     2771 2022-01-13 13:36:49.000000 napari_svetlana-0.2.5/src/napari_svetlana/_reader.py
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.878088 napari_svetlana-0.2.5/src/napari_svetlana/_tests/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)        0 2022-01-13 13:36:49.000000 napari_svetlana-0.2.5/src/napari_svetlana/_tests/__init__.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1249 2022-02-24 14:10:43.000000 napari_svetlana-0.2.5/src/napari_svetlana/_tests/test_dock_widget.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      117 2022-02-24 14:10:43.000000 napari_svetlana-0.2.5/src/napari_svetlana/_tests/test_function.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      976 2022-02-24 14:10:43.000000 napari_svetlana-0.2.5/src/napari_svetlana/_tests/test_reader.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      127 2022-02-24 14:10:43.000000 napari_svetlana-0.2.5/src/napari_svetlana/_tests/test_writer.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      463 2022-01-13 13:36:49.000000 napari_svetlana-0.2.5/src/napari_svetlana/_writer.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)       77 2022-02-04 11:10:23.000000 napari_svetlana-0.2.5/src/napari_svetlana/debug.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     1205 2022-11-17 09:03:51.000000 napari_svetlana-0.2.5/src/napari_svetlana/mosa.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    62329 2022-02-22 09:26:37.000000 napari_svetlana-0.2.5/src/napari_svetlana/old_dock_widget.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     5073 2022-10-28 15:42:32.000000 napari_svetlana-0.2.5/src/napari_svetlana/test_gradcam.py
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     4837 2022-10-28 16:25:46.000000 napari_svetlana-0.2.5/src/napari_svetlana/test_gradcam3D.py
-drwxrwxr-x   0 cazorla   (1004) cazorla   (1005)        0 2023-01-26 15:15:01.874088 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     7042 2023-01-26 15:15:01.000000 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/PKG-INFO
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)     2036 2023-01-26 15:15:01.000000 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/SOURCES.txt
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)        1 2023-01-26 15:15:01.000000 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/dependency_links.txt
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)       50 2023-01-26 15:15:01.000000 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/entry_points.txt
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)      211 2023-01-26 15:15:01.000000 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/requires.txt
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)       16 2023-01-26 15:15:01.000000 napari_svetlana-0.2.5/src/napari_svetlana.egg-info/top_level.txt
--rw-rw-r--   0 cazorla   (1004) cazorla   (1005)    11935 2022-12-16 09:19:44.000000 napari_svetlana-0.2.5/src/webinar.png
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    35148 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/LICENSE
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      161 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/MANIFEST.in
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7412 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/PKG-INFO
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     6194 2023-04-13 09:15:00.000000 napari_svetlana-0.2.6/README.md
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      193 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/requirements.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1568 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/setup.cfg
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       84 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/setup.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/napari_svetlana/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1637 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CNN2D.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1451 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CNN3D.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      619 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Config.json
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      879 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CustomDataset.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1049 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/CustomDialog.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     8885 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/base_cam.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      751 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/grad_cam.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7323 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/image.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2981 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/Prediction3DDataset.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3742 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/PredictionDataset.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3087 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/PredictionMulti3DDataset.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/src/napari_svetlana/XP/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3420 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/Predict3Dbatch.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2381 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/Prediction3DDataset_dilation.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2075 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/compute_accuracy.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     3527 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/extract_save_patches.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1558 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/modulable_CNN3D.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1196 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/redim.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     5315 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/reseau.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    17178 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training-stability_test.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    16325 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_1net.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    14958 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    13280 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    11531 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_test.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    28297 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/XP/testeur.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      195 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)   152098 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_batch_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    66687 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1708 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_function.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2771 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_reader.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.790987 napari_svetlana-0.2.6/src/napari_svetlana/_tests/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        0 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/__init__.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1249 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      117 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_function.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      976 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_reader.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      127 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_writer.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      463 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/_writer.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       77 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/debug.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     1205 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/mosa.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)    62329 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/old_dock_widget.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     5073 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam.py
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     4837 2023-02-09 16:50:37.000000 napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam3D.py
+drwxrwxr-x   0 cazorla   (1001) cazorla   (1001)        0 2023-04-13 09:59:28.786987 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     7412 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/PKG-INFO
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)     2008 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/SOURCES.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)        1 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/dependency_links.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       50 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/entry_points.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)      211 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/requires.txt
+-rw-rw-r--   0 cazorla   (1001) cazorla   (1001)       16 2023-04-13 09:59:28.000000 napari_svetlana-0.2.6/src/napari_svetlana.egg-info/top_level.txt
```

### Comparing `napari_svetlana-0.2.5/LICENSE` & `napari_svetlana-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/PKG-INFO` & `napari_svetlana-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_svetlana
-Version: 0.2.5
+Version: 0.2.6
 Summary: A classification plugin for the ROIs of a segmentation mask.
 Author: Clément Cazorla
 Author-email: clement.cazorla31@gmail.com
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://bitbucket.org/koopa31/napari_svetlana/issues?status=new&status=open
 Project-URL: Documentation, https://svetlana-documentation.readthedocs.io/en/latest/
 Project-URL: Source Code, https://bitbucket.org/koopa31/napari_svetlana/src/main/
@@ -109,15 +109,20 @@
 ## Tutorial
 
 Many advanced features are available in Svetlana, such as data augmentation or contextual information reduction, to optimize the performance of your classifier. Thus, we strongly encourage you to
 check our [Youtube tutorial](https://www.youtube.com/watch?v=u_FKuHta-RE) and
 our [documentation](https://svetlana-documentation.readthedocs.io/en/latest/).
 A folder in the repository called "[Demo images](https://bitbucket.org/koopa31/napari_svetlana/src/main/Demo%20images/)",
 contains two demo images, identical to the ones of the Youtube tutorial. Feel free to use them to test all the features
-that Sevtlana offers.
+that Svetlana offers.
+
+## Similar Napari plugins
+
+Joel Luethi developed a similar method for objects classification called [napari feature classifier](https://www.napari-hub.org/plugins/napari-feature-classifier).
+Also, [apoc](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification) by Robert Haase is available in Napari for pixels and objects classification.
 
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
```

### Comparing `napari_svetlana-0.2.5/README.md` & `napari_svetlana-0.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,20 @@
 ## Tutorial
 
 Many advanced features are available in Svetlana, such as data augmentation or contextual information reduction, to optimize the performance of your classifier. Thus, we strongly encourage you to
 check our [Youtube tutorial](https://www.youtube.com/watch?v=u_FKuHta-RE) and
 our [documentation](https://svetlana-documentation.readthedocs.io/en/latest/).
 A folder in the repository called "[Demo images](https://bitbucket.org/koopa31/napari_svetlana/src/main/Demo%20images/)",
 contains two demo images, identical to the ones of the Youtube tutorial. Feel free to use them to test all the features
-that Sevtlana offers.
+that Svetlana offers.
+
+## Similar Napari plugins
+
+Joel Luethi developed a similar method for objects classification called [napari feature classifier](https://www.napari-hub.org/plugins/napari-feature-classifier).
+Also, [apoc](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification) by Robert Haase is available in Napari for pixels and objects classification.
 
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
```

### Comparing `napari_svetlana-0.2.5/setup.cfg` & `napari_svetlana-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_svetlana
-version = 0.2.5
+version = 0.2.6
 author = Clément Cazorla
 author_email = clement.cazorla31@gmail.com
 license = GPL-3.0-only
 description = A classification plugin for the ROIs of a segmentation mask.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/CNN2D.py` & `napari_svetlana-0.2.6/src/napari_svetlana/CNN2D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/CNN3D.py` & `napari_svetlana-0.2.6/src/napari_svetlana/CNN3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/Config.json` & `napari_svetlana-0.2.6/src/napari_svetlana/Config.json`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/CustomDataset.py` & `napari_svetlana-0.2.6/src/napari_svetlana/CustomDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/CustomDialog.py` & `napari_svetlana-0.2.6/src/napari_svetlana/CustomDialog.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/base_cam.py` & `napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/base_cam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/grad_cam.py` & `napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/grad_cam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/Grad_Cam/image.py` & `napari_svetlana-0.2.6/src/napari_svetlana/Grad_Cam/image.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/Prediction3DDataset.py` & `napari_svetlana-0.2.6/src/napari_svetlana/Prediction3DDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/PredictionDataset.py` & `napari_svetlana-0.2.6/src/napari_svetlana/PredictionDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/PredictionMulti3DDataset.py` & `napari_svetlana-0.2.6/src/napari_svetlana/PredictionMulti3DDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/Predict3Dbatch.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/Predict3Dbatch.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/Prediction3DDataset_dilation.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/Prediction3DDataset_dilation.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/compute_accuracy.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/compute_accuracy.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/extract_save_patches.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/extract_save_patches.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/modulable_CNN3D.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/modulable_CNN3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/redim.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/redim.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/reseau.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/reseau.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training-stability_test.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training-stability_test.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_3D_1net.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_1net.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/script_training_test.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/script_training_test.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/XP/testeur.py` & `napari_svetlana-0.2.6/src/napari_svetlana/XP/testeur.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/_batch_dock_widget.py` & `napari_svetlana-0.2.6/src/napari_svetlana/_batch_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/_dock_widget.py` & `napari_svetlana-0.2.6/src/napari_svetlana/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/_function.py` & `napari_svetlana-0.2.6/src/napari_svetlana/_function.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/_reader.py` & `napari_svetlana-0.2.6/src/napari_svetlana/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/_tests/test_dock_widget.py` & `napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/_tests/test_reader.py` & `napari_svetlana-0.2.6/src/napari_svetlana/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/mosa.py` & `napari_svetlana-0.2.6/src/napari_svetlana/mosa.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/old_dock_widget.py` & `napari_svetlana-0.2.6/src/napari_svetlana/old_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/test_gradcam.py` & `napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana/test_gradcam3D.py` & `napari_svetlana-0.2.6/src/napari_svetlana/test_gradcam3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana.egg-info/PKG-INFO` & `napari_svetlana-0.2.6/src/napari_svetlana.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svetlana
-Version: 0.2.5
+Version: 0.2.6
 Summary: A classification plugin for the ROIs of a segmentation mask.
 Author: Clément Cazorla
 Author-email: clement.cazorla31@gmail.com
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://bitbucket.org/koopa31/napari_svetlana/issues?status=new&status=open
 Project-URL: Documentation, https://svetlana-documentation.readthedocs.io/en/latest/
 Project-URL: Source Code, https://bitbucket.org/koopa31/napari_svetlana/src/main/
@@ -109,15 +109,20 @@
 ## Tutorial
 
 Many advanced features are available in Svetlana, such as data augmentation or contextual information reduction, to optimize the performance of your classifier. Thus, we strongly encourage you to
 check our [Youtube tutorial](https://www.youtube.com/watch?v=u_FKuHta-RE) and
 our [documentation](https://svetlana-documentation.readthedocs.io/en/latest/).
 A folder in the repository called "[Demo images](https://bitbucket.org/koopa31/napari_svetlana/src/main/Demo%20images/)",
 contains two demo images, identical to the ones of the Youtube tutorial. Feel free to use them to test all the features
-that Sevtlana offers.
+that Svetlana offers.
+
+## Similar Napari plugins
+
+Joel Luethi developed a similar method for objects classification called [napari feature classifier](https://www.napari-hub.org/plugins/napari-feature-classifier).
+Also, [apoc](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification) by Robert Haase is available in Napari for pixels and objects classification.
 
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
```

### Comparing `napari_svetlana-0.2.5/src/napari_svetlana.egg-info/SOURCES.txt` & `napari_svetlana-0.2.6/src/napari_svetlana.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
-src/doc.png
-src/webinar.png
 src/napari_svetlana/CNN2D.py
 src/napari_svetlana/CNN3D.py
 src/napari_svetlana/Config.json
 src/napari_svetlana/CustomDataset.py
 src/napari_svetlana/CustomDialog.py
 src/napari_svetlana/Prediction3DDataset.py
 src/napari_svetlana/PredictionDataset.py
```

