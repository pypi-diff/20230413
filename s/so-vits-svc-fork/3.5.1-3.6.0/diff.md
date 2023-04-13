# Comparing `tmp/so_vits_svc_fork-3.5.1.tar.gz` & `tmp/so_vits_svc_fork-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.5.1.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.6.0.tar", max compression
```

## Comparing `so_vits_svc_fork-3.5.1.tar` & `so_vits_svc_fork-3.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-13 13:47:14.979123 so_vits_svc_fork-3.5.1/LICENSE
--rw-r--r--   0        0        0    17996 2023-04-13 13:47:14.979123 so_vits_svc_fork-3.5.1/README.md
--rw-r--r--   0        0        0     3113 2023-04-13 13:47:16.067118 so_vits_svc_fork-3.5.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-13 13:47:16.019118 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2768 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25206 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1213 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-13 13:47:14.983123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1649 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1399 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1460 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    18359 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-13 13:47:14.987123 so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-13 15:50:55.964661 so_vits_svc_fork-3.6.0/LICENSE
+-rw-r--r--   0        0        0    17996 2023-04-13 15:50:55.964661 so_vits_svc_fork-3.6.0/README.md
+-rw-r--r--   0        0        0     3113 2023-04-13 15:50:57.088677 so_vits_svc_fork-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-13 15:50:57.040676 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22740 2023-04-13 15:50:55.968661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-13 15:50:55.968661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2768 2023-04-13 15:50:55.968661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-13 15:50:55.968661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-13 15:50:55.968661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25206 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24054 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1213 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1649 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1399 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1460 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    18359 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-13 15:50:55.972661 so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.6.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.5.1/LICENSE` & `so_vits_svc_fork-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/README.md` & `so_vits_svc_fork-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/pyproject.toml` & `so_vits_svc_fork-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.5.1"
+version = "3.6.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/inference/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -303,50 +303,72 @@
                 # empty cache
                 torch.cuda.empty_cache()
             result_audio = np.concatenate([result_audio, audio_chunk_infer])
         result_audio = result_audio[: audio.shape[0]]
         return result_audio
 
 
-def linear_crossfade(
+def sola_crossfade(
     first: ndarray[Any, dtype[float32]],
     second: ndarray[Any, dtype[float32]],
-    length: int,
+    crossfade_len: int,
+    sola_search_len: int,
 ) -> ndarray[Any, dtype[float32]]:
+    cor_nom = np.convolve(
+        second[: sola_search_len + crossfade_len],
+        np.flip(first[-crossfade_len:]),
+        "valid",
+    )
+    cor_den = np.sqrt(
+        np.convolve(
+            second[: sola_search_len + crossfade_len] ** 2,
+            np.ones(crossfade_len),
+            "valid",
+        )
+        + 1e-8
+    )
+    sola_shift = np.argmax(cor_nom / cor_den)
+    LOG.info(f"SOLA shift: {sola_shift}")
+    second = second[sola_shift : sola_shift + len(second) - sola_search_len]
     return np.concatenate(
         [
-            first[:-length],
-            first[-length:] * np.linspace(1, 0, length)
-            + second[:length] * np.linspace(0, 1, length),
-            second[length:],
+            first[:-crossfade_len],
+            first[-crossfade_len:] * np.linspace(1, 0, crossfade_len)
+            + second[:crossfade_len] * np.linspace(0, 1, crossfade_len),
+            second[crossfade_len:],
         ]
     )
 
 
 class Crossfader:
     def __init__(
         self,
         *,
         additional_infer_before_len: int,
         additional_infer_after_len: int,
         crossfade_len: int,
+        sola_search_len: int = 384,
     ) -> None:
         if additional_infer_before_len < 0:
             raise ValueError("additional_infer_len must be >= 0")
         if crossfade_len < 0:
             raise ValueError("crossfade_len must be >= 0")
         if additional_infer_after_len < 0:
             raise ValueError("additional_infer_len must be >= 0")
         if additional_infer_before_len < 0:
             raise ValueError("additional_infer_len must be >= 0")
         self.additional_infer_before_len = additional_infer_before_len
         self.additional_infer_after_len = additional_infer_after_len
         self.crossfade_len = crossfade_len
+        self.sola_search_len = sola_search_len
         self.last_input_left = np.zeros(
-            crossfade_len + additional_infer_before_len + additional_infer_after_len,
+            sola_search_len
+            + crossfade_len
+            + additional_infer_before_len
+            + additional_infer_after_len,
             dtype=np.float32,
         )
         self.last_infered_left = np.zeros(crossfade_len, dtype=np.float32)
 
     def process(
         self, input_audio: ndarray[Any, dtype[float32]], *args, **kwargs: Any
     ) -> ndarray[Any, dtype[float32]]:
@@ -380,47 +402,59 @@
             infer_audio_concat = self.infer(
                 np.pad(input_audio_concat, (pad_len, pad_len), mode="reflect"),
                 *args,
                 **kwargs,
             )[pad_len:-pad_len]
         else:
             infer_audio_concat = self.infer(input_audio_concat, *args, **kwargs)
+
+        # debug SOLA (using copy synthesis with a random shift)
+        """
+        rs = int(np.random.uniform(-200,200))
+        LOG.info(f"Debug random shift: {rs}")
+        infer_audio_concat = np.roll(input_audio_concat, rs)
+        """
+
         if len(infer_audio_concat) != len(input_audio_concat):
             raise ValueError(
                 f"Inferred audio length ({len(infer_audio_concat)}) should be equal to input audio length ({len(input_audio_concat)})."
             )
-
         infer_audio_to_use = infer_audio_concat[
             -(
-                self.crossfade_len + input_audio_len + self.additional_infer_after_len
-            ) : -(self.crossfade_len + self.additional_infer_after_len)
+                self.sola_search_len
+                + self.crossfade_len
+                + input_audio_len
+                + self.additional_infer_after_len
+            ) : -self.additional_infer_after_len
         ]
         assert (
-            len(infer_audio_to_use) == input_audio_len
-        ), f"{len(infer_audio_to_use)} != {input_audio_len}"
-        result_audio = linear_crossfade(
-            self.last_infered_left, infer_audio_to_use, self.crossfade_len
+            len(infer_audio_to_use)
+            == input_audio_len + self.sola_search_len + self.crossfade_len
+        ), f"{len(infer_audio_to_use)} != {input_audio_len + self.sola_search_len + self.cross_fade_len}"
+        _audio = sola_crossfade(
+            self.last_infered_left,
+            infer_audio_to_use,
+            self.crossfade_len,
+            self.sola_search_len,
         )
+        result_audio = _audio[: -self.crossfade_len]
         assert (
             len(result_audio) == input_audio_len
         ), f"{len(result_audio)} != {input_audio_len}"
 
         # update last input and inferred
         self.last_input_left = input_audio_concat[
             -(
-                self.crossfade_len
+                self.sola_search_len
+                + self.crossfade_len
                 + self.additional_infer_before_len
                 + self.additional_infer_after_len
             ) :
         ]
-        self.last_infered_left = infer_audio_concat[
-            -(
-                self.crossfade_len + self.additional_infer_after_len
-            ) : -self.additional_infer_after_len
-        ]
+        self.last_infered_left = _audio[-self.crossfade_len :]
         return result_audio
 
     def infer(
         self, input_audio: ndarray[Any, dtype[float32]]
     ) -> ndarray[Any, dtype[float32]]:
         return input_audio
```

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.6.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.5.1/PKG-INFO` & `so_vits_svc_fork-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.5.1
+Version: 3.6.0
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.5.1 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.6.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

