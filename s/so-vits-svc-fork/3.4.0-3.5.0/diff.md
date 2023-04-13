# Comparing `tmp/so_vits_svc_fork-3.4.0.tar.gz` & `tmp/so_vits_svc_fork-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.4.0.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.5.0.tar", max compression
```

## Comparing `so_vits_svc_fork-3.4.0.tar` & `so_vits_svc_fork-3.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-13 12:33:43.077324 so_vits_svc_fork-3.4.0/LICENSE
--rw-r--r--   0        0        0    17996 2023-04-13 12:33:43.077324 so_vits_svc_fork-3.4.0/README.md
--rw-r--r--   0        0        0     3113 2023-04-13 12:33:44.089337 so_vits_svc_fork-3.4.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-13 12:33:44.041337 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2768 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    24381 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0      809 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1649 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1399 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1460 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    18300 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-13 12:33:43.081323 so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-13 13:37:41.266299 so_vits_svc_fork-3.5.0/LICENSE
+-rw-r--r--   0        0        0    17996 2023-04-13 13:37:41.266299 so_vits_svc_fork-3.5.0/README.md
+-rw-r--r--   0        0        0     3113 2023-04-13 13:37:42.462306 so_vits_svc_fork-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-13 13:37:42.398305 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22740 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2768 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25206 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    22944 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0      809 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1649 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1399 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1460 2023-04-13 13:37:41.270299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    18300 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-13 13:37:41.274299 so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.5.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.4.0/LICENSE` & `so_vits_svc_fork-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/README.md` & `so_vits_svc_fork-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/pyproject.toml` & `so_vits_svc_fork-3.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.4.0"
+version = "3.5.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,25 @@
     input_devices_indices = [d["index"] for d in devices if d["max_input_channels"] > 0]
     output_devices_indices = [
         d["index"] for d in devices if d["max_output_channels"] > 0
     ]
     return input_devices, output_devices, input_devices_indices, output_devices_indices
 
 
+def after_inference(window: sg.Window, path: Path, auto_play: bool, output_path: Path):
+    try:
+        LOG.info(f"Finished inference for {path.stem}{path.suffix}")
+        window["infer"].update(disabled=False)
+
+        if auto_play:
+            play_audio(output_path)
+    except Exception as e:
+        LOG.exception(e)
+
+
 def main():
     try:
         ensure_pretrained_model(".", "contentvec", tqdm_cls=tqdm_tk)
     except Exception as e:
         LOG.exception(e)
         LOG.info("Trying tqdm.std...")
         try:
@@ -537,49 +548,60 @@
                 apply_preset(values["presets"])
                 update_speaker()
             elif event == "refresh_devices":
                 update_devices()
             elif event == "config_path":
                 update_speaker()
             elif event == "infer":
-                from so_vits_svc_fork.inference.main import infer
-
                 input_path = Path(values["input_path"])
                 output_path = (
                     input_path.parent / f"{input_path.stem}.out{input_path.suffix}"
                 )
                 if not input_path.exists() or not input_path.is_file():
                     LOG.warning(f"Input path {input_path} does not exist.")
                     continue
+
                 try:
-                    infer(
-                        # paths
-                        model_path=Path(values["model_path"]),
-                        output_path=output_path,
-                        input_path=input_path,
-                        config_path=Path(values["config_path"]),
-                        # svc config
-                        speaker=values["speaker"],
-                        cluster_model_path=Path(values["cluster_model_path"])
-                        if values["cluster_model_path"]
-                        else None,
-                        transpose=values["transpose"],
-                        auto_predict_f0=values["auto_predict_f0"],
-                        cluster_infer_ratio=values["cluster_infer_ratio"],
-                        noise_scale=values["noise_scale"],
-                        f0_method=values["f0_method"],
-                        # slice config
-                        db_thresh=values["silence_threshold"],
-                        pad_seconds=values["pad_seconds"],
-                        chunk_seconds=values["chunk_seconds"],
-                        absolute_thresh=values["absolute_thresh"],
-                        device="cpu" if not values["use_gpu"] else get_optimal_device(),
+                    from so_vits_svc_fork.inference.main import infer
+
+                    LOG.info("Starting inference...")
+                    window["infer"].update(disabled=True)
+                    infer_future = pool.schedule(
+                        infer,
+                        kwargs=dict(
+                            # paths
+                            model_path=Path(values["model_path"]),
+                            output_path=output_path,
+                            input_path=input_path,
+                            config_path=Path(values["config_path"]),
+                            # svc config
+                            speaker=values["speaker"],
+                            cluster_model_path=Path(values["cluster_model_path"])
+                            if values["cluster_model_path"]
+                            else None,
+                            transpose=values["transpose"],
+                            auto_predict_f0=values["auto_predict_f0"],
+                            cluster_infer_ratio=values["cluster_infer_ratio"],
+                            noise_scale=values["noise_scale"],
+                            f0_method=values["f0_method"],
+                            # slice config
+                            db_thresh=values["silence_threshold"],
+                            pad_seconds=values["pad_seconds"],
+                            chunk_seconds=values["chunk_seconds"],
+                            absolute_thresh=values["absolute_thresh"],
+                            device="cpu"
+                            if not values["use_gpu"]
+                            else get_optimal_device(),
+                        ),
+                    )
+                    infer_future.add_done_callback(
+                        lambda _future: after_inference(
+                            window, input_path, values["auto_play"], output_path
+                        )
                     )
-                    if values["auto_play"]:
-                        pool.schedule(play_audio, args=[output_path])
                 except Exception as e:
                     LOG.exception(e)
             elif event == "play_input":
                 if Path(values["input_path"]).exists():
                     pool.schedule(play_audio, args=[Path(values["input_path"])])
             elif event == "start_vc":
                 _, _, input_device_indices, output_device_indices = get_devices(
```

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.5.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.4.0/PKG-INFO` & `so_vits_svc_fork-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.4.0
+Version: 3.5.0
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
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.4.0 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.5.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

