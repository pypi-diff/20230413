# Comparing `tmp/so_vits_svc_fork-3.1.9.tar.gz` & `tmp/so_vits_svc_fork-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.1.9.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.2.0.tar", max compression
```

## Comparing `so_vits_svc_fork-3.1.9.tar` & `so_vits_svc_fork-3.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-10 15:12:13.832778 so_vits_svc_fork-3.1.9/LICENSE
--rw-r--r--   0        0        0    17996 2023-04-10 15:12:13.832778 so_vits_svc_fork-3.1.9/README.md
--rw-r--r--   0        0        0     3113 2023-04-10 15:12:15.144885 so_vits_svc_fork-3.1.9/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-10 15:12:15.088879 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22637 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1275 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2712 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2826 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    24381 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    22944 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0      731 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1627 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1377 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1438 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2997 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4614 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4693 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    17588 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13081 2023-04-10 15:12:13.840779 so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.1.9/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-13 07:57:26.485295 so_vits_svc_fork-3.2.0/LICENSE
+-rw-r--r--   0        0        0    17996 2023-04-13 07:57:26.485295 so_vits_svc_fork-3.2.0/README.md
+-rw-r--r--   0        0        0     3113 2023-04-13 07:57:27.489318 so_vits_svc_fork-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-13 07:57:27.441317 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22645 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1275 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2768 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2826 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    24381 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    22944 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0      809 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-13 07:57:26.489296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1627 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1377 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1438 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2997 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4614 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4693 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    18134 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13081 2023-04-13 07:57:26.493296 so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    19965 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.2.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.1.9/LICENSE` & `so_vits_svc_fork-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/README.md` & `so_vits_svc_fork-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/pyproject.toml` & `so_vits_svc_fork-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.1.9"
+version = "3.2.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,7 +813,10 @@
     main(
         input_dir=input_dir,
         output_path=output_path,
         n_clusters=n_clusters,
         verbose=True,
         use_minibatch=minibatch,
     )
+
+
+cli()
```

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,27 @@
     n_clusters: int,
     use_minibatch: bool = True,
     verbose: bool = False,
 ) -> dict:
     input_dir = Path(input_dir)
     LOG.info(f"Loading features from {input_dir}")
     features = []
-    nums = 0
     for path in input_dir.rglob("*.data.pt"):
         features.append(
             torch.load(path, weights_only=True)["content"].squeeze(0).numpy().T
         )
+    if not features:
+        raise ValueError(f"No features found in {input_dir}")
     features = np.concatenate(features, axis=0).astype(np.float32)
     if features.shape[0] < n_clusters:
         raise ValueError(
             "Too few HuBERT features to cluster. Consider using a smaller number of clusters."
         )
     LOG.info(
-        f"Nums: {nums}, shape: {features.shape}, size: {features.nbytes/1024**2:.2f} MB, dtype: {features.dtype}"
+        f"shape: {features.shape}, size: {features.nbytes/1024**2:.2f} MB, dtype: {features.dtype}"
     )
     with timer() as t:
         if use_minibatch:
             kmeans = MiniBatchKMeans(
                 n_clusters=n_clusters,
                 verbose=verbose,
                 batch_size=4096,
```

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import os
+import sys
 from logging import (
     DEBUG,
     INFO,
     FileHandler,
     StreamHandler,
     basicConfig,
     captureWarnings,
+    getLogger,
 )
 from pathlib import Path
 
 from rich.logging import RichHandler
 
 LOGGER_INIT = False
 
 
 def init_logger() -> None:
     global LOGGER_INIT
     if LOGGER_INIT:
         return
 
     IN_COLAB = os.getenv("COLAB_RELEASE_TAG")
-    IS_TEST = "test" in Path(__file__).parent.stem
+    IS_TEST = "test" in Path.cwd().stem
 
     basicConfig(
-        level=DEBUG if IS_TEST else INFO,
+        level=INFO,
         format="%(asctime)s %(message)s",
         datefmt="[%X]",
         handlers=[
             RichHandler() if not IN_COLAB else StreamHandler(),
             FileHandler(f"{__name__.split('.')[0]}.log"),
         ],
     )
+    if IS_TEST:
+        getLogger(sys.modules[__name__].__package__).setLevel(DEBUG)
     captureWarnings(True)
     LOGGER_INIT = True
```

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,25 +62,30 @@
     config_path = Path(config_path)
     model_path = Path(model_path)
 
     hparams = utils.get_backup_hparams(config_path, model_path)
     utils.ensure_pretrained_model(model_path, hparams.model.get("type_", "hifi-gan"))
 
     datamodule = VCDataModule(hparams)
+    strategy = (
+        "ddp_find_unused_parameters_true" if torch.cuda.device_count() > 1 else "auto"
+    )
+    LOG.info(f"Using strategy: {strategy}")
     trainer = pl.Trainer(
         logger=TensorBoardLogger(model_path),
         # profiler="simple",
         val_check_interval=hparams.train.eval_interval,
         max_epochs=hparams.train.epochs,
         check_val_every_n_epoch=None,
         precision="16-mixed"
         if hparams.train.fp16_run
         else "bf16-mixed"
         if hparams.train.get("bf16_run", False)
         else 32,
+        strategy=strategy,
     )
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
     trainer.fit(model, datamodule=datamodule)
 
 
 class VitsLightning(pl.LightningModule):
     def __init__(self, reset_optimizer: bool = False, **hparams: Any):
@@ -322,15 +327,14 @@
         y = commons.slice_segments(
             y,
             ids_slice * self.hparams.data.hop_length,
             self.hparams.train.segment_size,
         )
 
         # generator loss
-        LOG.debug("Calculating generator loss")
         y_d_hat_r, y_d_hat_g, fmap_r, fmap_g = self.net_d(y, y_hat)
 
         with autocast(enabled=False):
             loss_mel = F.l1_loss(y_mel, y_hat_mel) * self.hparams.train.c_mel
             loss_kl = (
                 kl_loss(z_p, logs_q, m_p, logs_p, z_mask) * self.hparams.train.c_kl
             )
@@ -384,18 +388,21 @@
                     "all/norm_lf0": so_vits_svc_fork.utils.plot_data_to_numpy(
                         lf0[0, 0, :].cpu().float().numpy(),
                         norm_lf0[0, 0, :].detach().cpu().float().numpy(),
                     ),
                 }
             )
 
+        accumulate_grad_batches = self.hparams.train.get("accumulate_grad_batches", 1)
+        should_update = (batch_idx + 1) % accumulate_grad_batches == 0
         # optimizer
-        optim_g.zero_grad()
-        self.manual_backward(loss_gen_all)
-        optim_g.step()
+        self.manual_backward(loss_gen_all / accumulate_grad_batches)
+        if should_update:
+            optim_g.step()
+            optim_g.zero_grad()
         self.untoggle_optimizer(optim_g)
 
         # Discriminator
         # train
         self.toggle_optimizer(optim_d)
         y_d_hat_r, y_d_hat_g, _, _ = self.net_d(y, y_hat.detach())
 
@@ -409,19 +416,25 @@
         # log loss
         self.log_("loss/d/total", loss_disc_all, prog_bar=True)
         self.log_(
             "grad_norm_d", commons.clip_grad_value_(self.net_d.parameters(), None)
         )
 
         # optimizer
-        optim_d.zero_grad()
-        self.manual_backward(loss_disc_all)
-        optim_d.step()
+        self.manual_backward(loss_disc_all / accumulate_grad_batches)
+        if should_update:
+            optim_d.step()
+            optim_d.zero_grad()
         self.untoggle_optimizer(optim_d)
 
+        # end of epoch
+        if self.trainer.is_last_batch:
+            self.scheduler_g.step()
+            self.scheduler_d.step()
+
     def validation_step(self, batch, batch_idx):
         with torch.no_grad():
             self.net_g.eval()
             c, f0, _, mel, y, g, _, uv = batch
             y_hat = self.net_g.infer(c, f0, uv, g=g)
             y_hat_mel = mel_spectrogram_torch(y_hat.squeeze(1).float(), self.hparams)
             self.log_audio_dict(
```

### Comparing `so_vits_svc_fork-3.1.9/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.2.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.1.9/PKG-INFO` & `so_vits_svc_fork-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.1.9
+Version: 3.2.0
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
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.1.9 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.2.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

