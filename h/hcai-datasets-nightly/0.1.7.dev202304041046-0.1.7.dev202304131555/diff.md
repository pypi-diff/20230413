# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202304041046.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202304131555.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304041046.tar", last modified: Tue Apr  4 10:46:42 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304131555.tar", last modified: Thu Apr 13 15:55:58 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202304041046.tar` & `hcai-datasets-nightly-0.1.7.dev202304131555.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.682800 hcai-datasets-nightly-0.1.7.dev202304041046/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-04 10:46:42.682800 hcai-datasets-nightly-0.1.7.dev202304041046/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.674800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.674800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.674800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.674800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    22278 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9858 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.678800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 10:46:42.682800 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-04 10:46:42.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-04 10:46:42.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 10:46:42.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-04 10:46:42.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-04 10:46:42.000000 hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 10:46:42.682800 hcai-datasets-nightly-0.1.7.dev202304041046/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-04 10:46:33.000000 hcai-datasets-nightly-0.1.7.dev202304041046/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19035 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22257 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304131555/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304041046
+Version: 0.1.7.dev202304131555
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/README.md` & `hcai-datasets-nightly-0.1.7.dev202304131555/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import numpy as np
 import os
 
 import nova_utils.db_utils.nova_types as nt
 import hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils as ndu
 import hcai_datasets.hcai_nova_dynamic.utils.nova_anno_utils as nau
 from nova_utils.interfaces.dataset_iterable import DatasetIterable
@@ -35,14 +37,15 @@
         right_context="0s",
         frame_size=None,
         stride=None,
         add_rest_class=True,
         flatten_samples=False,
         supervised_keys=None,
         lazy_loading=False,
+        fake_missing_data=True,
         **kwargs,
     ):
         """
         Initialize the HcaiNovaDynamic dataset builder
         Args:
           nova_data_dir: the directory to look for data. same as the directory specified in the nova gui.
           frame_size: the framesize to look at. the matching annotation will be calculated as majority vote from all annotations that are overlapping with the timeframe.
@@ -58,14 +61,15 @@
           sessions: list of sessions that should be loaded. must match the session names in nova.
           annotator: the name of the annotator that labeld the session. must match annotator names in nova.
           schemes: list of the annotation schemes to fetch
           roles: list of roles for which the annotation should be loaded.
           data_streams: list datastreams for which the annotation should be loaded. must match stream names in nova.
           start: optional start time_ms. use if only a specific chunk of a session should be retreived.
           end: optional end time_ms. use if only a specifc chunk of a session should be retreived.
+          fake_missing_data: If set to true missing datastreams will provide zero data and missing annotations will be empty. If set to false a session will be skipped if an expected data stream or annotation are not found.
           **kwargs: arguments that will be passed through to the dataset builder
         """
         super().__init__(*args, **kwargs)
         self.dataset = dataset
         self.nova_data_dir = nova_data_dir
         self.sessions = sessions
         self.roles = roles
@@ -87,14 +91,15 @@
         self.end_ms = ndu.parse_time_string_to_ms(end)
         if not self.end_ms:
             self.end_ms = float("inf")
 
         self.flatten_samples = flatten_samples
         self.add_rest_class = add_rest_class
         self.lazy_loading = lazy_loading
+        self.fake_missing_data = fake_missing_data
         self.nova_db_handler = NovaDBHandler(db_config_path, db_config_dict)
 
         # Retrieving meta information from the database
         mongo_schemes = self.nova_db_handler.get_schemes(
             dataset=dataset, schemes=schemes
         )
         mongo_data = self.nova_db_handler.get_data_streams(
@@ -159,15 +164,15 @@
                 scheme_valid = scheme["isValid"]
                 anno_schemes[label_id] = scheme_type
 
                 if scheme_type == nt.AnnoTypes.DISCRETE:
                     labels = scheme["labels"]
                     annos[label_id] = nau.DiscreteAnnotation(
                         role=role,
-                        add_rest_class=True,
+                        add_rest_class=self.add_rest_class,
                         scheme=scheme_name,
                         is_valid=scheme_valid,
                         labels=labels,
                     )
 
                 elif scheme_type == nt.AnnoTypes.CONTINUOUS:
                     min_val = scheme["min"]
@@ -223,82 +228,108 @@
                 sample_data_path = os.path.join(
                     self.nova_data_dir,
                     self.dataset,
                     self.sessions[0],
                     sample_stream_name,
                 )
                 dtype = nt.string_to_enum(nt.DataTypes, data_stream["type"])
+                try:
+                    if dtype == nt.DataTypes.VIDEO:
+                        data = VideoData(
+                            role=role,
+                            name=data_stream["name"],
+                            file_ext=data_stream["fileExt"],
+                            sr=data_stream["sr"],
+                            is_valid=data_stream["isValid"],
+                            sample_data_path=sample_data_path,
+                            lazy_loading=self.lazy_loading,
+                        )
+                    elif dtype == nt.DataTypes.AUDIO:
+                        data = AudioData(
+                            role=role,
+                            name=data_stream["name"],
+                            file_ext=data_stream["fileExt"],
+                            sr=data_stream["sr"],
+                            is_valid=data_stream["isValid"],
+                            sample_data_path=sample_data_path,
+                            lazy_loading=self.lazy_loading,
+                        )
+                    elif dtype == nt.DataTypes.FEATURE:
+                        data = StreamData(
+                            role=role,
+                            name=data_stream["name"],
+                            sr=data_stream["sr"],
+                            data_type=dtype,
+                            is_valid=data_stream["isValid"],
+                            sample_data_path=sample_data_path,
+                            lazy_loading=self.lazy_loading,
+                        )
+                    else:
+                        raise ValueError("Invalid data type".format(data_stream["type"]))
 
-                if dtype == nt.DataTypes.VIDEO:
-                    data = VideoData(
-                        role=role,
-                        name=data_stream["name"],
-                        file_ext=data_stream["fileExt"],
-                        sr=data_stream["sr"],
-                        is_valid=data_stream["isValid"],
-                        sample_data_path=sample_data_path,
-                        lazy_loading=self.lazy_loading,
-                    )
-                elif dtype == nt.DataTypes.AUDIO:
-                    data = AudioData(
-                        role=role,
-                        name=data_stream["name"],
-                        file_ext=data_stream["fileExt"],
-                        sr=data_stream["sr"],
-                        is_valid=data_stream["isValid"],
-                        sample_data_path=sample_data_path,
-                        lazy_loading=self.lazy_loading,
-                    )
-                elif dtype == nt.DataTypes.FEATURE:
-                    data = StreamData(
-                        role=role,
-                        name=data_stream["name"],
-                        sr=data_stream["sr"],
-                        data_type=dtype,
-                        is_valid=data_stream["isValid"],
-                        sample_data_path=sample_data_path,
-                        lazy_loading=self.lazy_loading,
-                    )
-                else:
-                    raise ValueError("Invalid data type {}".format(data_stream["type"]))
+                except FileNotFoundError as fnf:
+                    if self.fake_missing_data:
+                        raise FileNotFoundError
+                    else:
+                        print(f"WARNING: Ignoring exception - {fnf}")
+                        continue
 
                 data_id = merge_role_key(role=role, key=data_stream["name"])
                 data_info[data_id] = data
                 data_schemes[data_id] = dtype
 
         return data_info, data_schemes
 
     def _load_annotation_for_session(self, session, time_to_ms=False):
         for label_id, anno in self.annos.items():
-            mongo_anno = self.nova_db_handler.get_annos(
-                self.dataset, anno.scheme, session, self.annotator, anno.role
-            )
-            anno.set_annotation_from_mongo_doc(mongo_anno, time_to_ms=time_to_ms)
+            try:
+                mongo_anno = self.nova_db_handler.get_annos(
+                    self.dataset, anno.scheme, session, self.annotator, anno.role
+                )
+            except FileNotFoundError as fnf:
+                mongo_anno = []
+                if self.fake_missing_data:
+                    print(f"WARNING: {fnf} - Providing dummy data")
+                else:
+                    raise fnf
+            finally:
+                anno.set_annotation_from_mongo_doc(mongo_anno, time_to_ms=time_to_ms)
 
     def _open_data_reader_for_session(self, session):
         for data_id, data in self.data_info.items():
-            data_path = os.path.join(
-                self.nova_data_dir, self.dataset, session, data_id + "." + data.file_ext
-            )
-            data.open_file_reader(data_path)
+            try:
+                data_path = os.path.join(
+                    self.nova_data_dir, self.dataset, session, data_id + "." + data.file_ext
+                )
+                data.open_file_reader(data_path)
+            except FileNotFoundError as fnf:
+                if self.fake_missing_data:
+                    print(f"WARNING: {fnf} - Providing dummy data")
+                else:
+                    raise fnf
+
 
     def _yield_sample(self):
         """Yields examples."""
 
         # Needed to sort the samples later and assure that the order is the same as in nova. Necessary for CML till the tfds can be returned in order.
         sample_counter = 1
 
         for session in self.sessions:
 
             _frame_size_ms = self.frame_size_ms
             _stride_ms = self.stride_ms
 
             # Gather all data we need for this session
-            self._load_annotation_for_session(session, time_to_ms=True)
-            self._open_data_reader_for_session(session)
+            try:
+                self._load_annotation_for_session(session, time_to_ms=True)
+                self._open_data_reader_for_session(session)
+            except FileNotFoundError as fnf:
+                print(f"WARNING: {fnf} - Skipping session {session}")
+                continue
 
             session_info = self.nova_db_handler.get_session_info(self.dataset, session)[
                 0
             ]
             dur = session_info["duration"]
 
             # If we are loading any datastreams we check if any datastream is shorter than the duration stored in the database suggests
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import errno
 import copy
 import warnings
 import configparser
 
 from typing import Union
 from datetime import datetime
 from pymongo import MongoClient
@@ -290,18 +291,15 @@
             mongo_roles,
             dataset,
             self.ANNOTATION_COLLECTION,
         )
 
         # getting the annotation data and the session name
         if not mongo_annos:
-            print(
-                f"No annotations found for \n\t-annotator: {annotator}\n\t-scheme: {scheme}\n\t-session: {session}\n\t-role: {roles}"
-            )
-            return []
+            raise FileNotFoundError(errno.ENOENT, 'No such annotation', f"annotator: {annotator} - scheme: {scheme} - session: {session} - role: {roles}")
 
         else:
             # TODO: adapt for multiple roles, annotators etc.
             label = self.get_data_docs_by_prop(
                 mongo_annos[0]["data_id"], "_id", dataset
             )
             label = label["labels"]
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 from decord import VideoReader, AudioReader, cpu
 import numpy as np
 import os
-
+import sys
+import errno
 
 from nova_utils.db_utils import nova_types as nt
 from nova_utils.ssi_utils.ssi_stream_utils import Stream
 from hcai_datasets.hcai_nova_dynamic.utils.nova_string_utils import (
     merge_role_key,
 )
 from typing import Union
 from abc import ABC, abstractmethod
 
 
 class Data(ABC):
-
     def __init__(
-            self,
-            role: str = "",
-            name: str = "",
-            file_ext: str = "stream",
-            sr: int = 0,
-            data_type: nt.DataTypes = None,
-            is_valid: bool = True,
-            sample_data_path: str = "",
-            lazy_loading: bool = False,
+        self,
+        role: str = "",
+        name: str = "",
+        file_ext: str = "stream",
+        sr: int = 0,
+        data_type: nt.DataTypes = None,
+        is_valid: bool = True,
+        sample_data_path: str = "",
+        lazy_loading: bool = False,
     ):
+        """
+
+        Args:
+            role ():
+            name ():
+            file_ext ():
+            sr ():
+            data_type ():
+            is_valid ():
+            sample_data_path ():
+            lazy_loading ():
+        """
         self.role = role
         self.name = name
         self.is_valid = is_valid
         self.sr = sr
         self.file_ext = file_ext
         self.lazy_loading = lazy_loading
         self.data_type = data_type
@@ -37,18 +49,25 @@
         self.sample_data_shape = None
         self.np_data_type = None
         self.meta_loaded = False
 
         # Set when open_file_reader is called
         self.file_path = None
         self.file_reader = None
-        self.dur = None
+        self.dur = sys.maxsize
 
         if sample_data_path:
-            self.populate_meta_info(sample_data_path)
+            if not os.path.isfile(sample_data_path):
+                self.meta_loaded = False
+                print(
+                    f"WARNING: Sample file {sample_data_path} not found. Could not initialize meta data."
+                )
+                # raise FileNotFoundError( errno.ENOENT, os.strerror(errno.ENOENT), sample_data_path)
+            else:
+                self.populate_meta_info(sample_data_path)
 
     def data_stream_opend(self):
         if not self.file_reader:
             print(
                 "No datastream opened for {}".format(
                     merge_role_key(self.role, self.name)
                 )
@@ -57,39 +76,54 @@
 
     def get_info(self):
         if self.meta_loaded:
             if self.lazy_loading:
                 return {
                     "frame_start": {"dtype": np.float32, "shape": (1)},
                     "frame_end": {"dtype": np.float32, "shape": (1)},
-                    "file_path": {"dtype": np.str, "shape": (None,)}
+                    "file_path": {"dtype": np.str, "shape": (None,)},
                 }
             return self.get_info_hook()
         else:
             print(
                 "Meta data has not been loaded for file {}. Call get_meta_info() first.".format(
                     merge_role_key(self.role, self.name)
                 )
             )
 
-    def get_sample(self, frame_start: int, frame_end: int):
+    def get_sample(self, frame_start_ms: int, frame_end_ms: int):
         """
         Returns the sample for the respective frames. If lazy loading is true, only the filepath and frame_start, frame_end will be returned.
         """
-        if self.lazy_loading:
+
+        if not self.file_reader:
+            start_frame = milli_seconds_to_frame(self.sr, frame_start_ms)
+            end_frame = milli_seconds_to_frame(self.sr, frame_end_ms)
+            return np.zeros(self.sample_data_shape + (end_frame - start_frame, ))
+        elif self.lazy_loading:
             return {
-                "frame_start": frame_start,
-                "frame_end": frame_end,
+                "frame_start": frame_start_ms,
+                "frame_end": frame_end_ms,
                 "file_path": self.file_path,
             }
         else:
-            return self.get_sample_hook(frame_start, frame_end)
+            return self.get_sample_hook(frame_start_ms, frame_end_ms)
 
     def open_file_reader(self, path: str):
+        """
+        Args:
+            path ():
+        Raises:
+            FileNotFoundError: If path is not a file
+        """
         self.file_path = path
+        if not os.path.isfile(path):
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
+        if not self.meta_loaded:
+            self.populate_meta_info(path)
         self.open_file_reader_hook(path)
 
     @abstractmethod
     def get_info_hook(self):
         """
         Returns the features for this datastream to create the DatasetInfo for tensorflow
         """
@@ -124,95 +158,99 @@
         ...
 
 
 class AudioData(Data):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
+        # Overwrite default
+        self.sample_data_shape = (1, )
+
     def get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
-            "dtype": np.float32
+            "dtype": np.float32,
         }
 
     def get_sample_hook(self, frame_start_ms: int, frame_end_ms: int):
         start_frame = int(frame_start_ms * self.sr / 1000)
         end_frame = int(frame_end_ms * self.sr / 1000)
         chunk = self.file_reader.get_batch(
             list(range(start_frame, end_frame))
         ).asnumpy()
         return chunk
 
     def open_file_reader_hook(self, path: str):
-        if not os.path.isfile(path):
-            print("Session file not found at {}.".format(path))
-            raise FileNotFoundError()
         self.file_reader = AudioReader(path, ctx=cpu(0), mono=False)
         self.dur = self.file_reader.duration()
 
     def populate_meta_info(self, path: str):
-        if not os.path.isfile(path):
-            print("Sample file not found at {}. Can't load metadata.".format(path))
-            raise FileNotFoundError()
+        """
+
+        Args:
+            path ():
+        """
+
         file_reader = AudioReader(path, ctx=cpu(0), mono=False)
         n_channels = file_reader.shape[0]
         self.sample_data_shape = (None, n_channels)
         self.meta_loaded = True
 
     def close_file_reader(self):
         return True
 
 
 class VideoData(Data):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
+        # Overwrite default
+        self.sample_data_shape = (480, 640, 3)
+
+
     def get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
-            "dtype": np.float32
+            "dtype": np.float32,
         }
 
     def get_sample_hook(self, frame_start_ms: int, frame_end_ms: int):
         start_frame = int(frame_start_ms * self.sr / 1000)
         end_frame = int(frame_end_ms * self.sr / 1000)
         chunk = self.file_reader.get_batch(
             list(range(start_frame, end_frame))
         ).asnumpy()
         return chunk
 
     def open_file_reader_hook(self, path: str):
-        if not os.path.isfile(path):
-            print("Session file not found at {}.".format(path))
-            raise FileNotFoundError()
         self.file_reader = VideoReader(path, ctx=cpu(0))
         fps = self.file_reader.get_avg_fps()
         frame_count = len(self.file_reader)
         self.dur = frame_count / fps
 
     def populate_meta_info(self, path: str):
-        if not os.path.isfile(path):
-            print("Sample file not found at {}. Can't load metadata.".format(path))
-            raise FileNotFoundError()
         file_reader = VideoReader(path)
         self.sample_data_shape = file_reader[0].shape
         self.meta_loaded = True
 
     def close_file_reader(self):
         return True
 
 
 class StreamData(Data):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        # Overwrite default
+        self.sample_data_shape = (1, )
+
 
     def get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
-            "dtype": self.np_data_type
+            "dtype": self.np_data_type,
         }
 
     def get_sample_hook(self, frame_start_ms: int, frame_end_ms: int):
         try:
             self.data_stream_opend()
             start_frame = milli_seconds_to_frame(self.sr, frame_start_ms)
             end_frame = milli_seconds_to_frame(self.sr, frame_end_ms)
@@ -299,8 +337,10 @@
                     frame
                 )
             )
             return float(frame)
         except ValueError:
             raise ValueError("Invalid input format for frame: {}".format(frame))
 
-    print(f'WARNING: Could  not automatically parse time "{frame}" to seconds. Returning None ')
+    print(
+        f'WARNING: Could  not automatically parse time "{frame}" to seconds. Returning None '
+    )
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304041046
+Version: 0.1.7.dev202304131555
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304041046/setup.py` & `hcai-datasets-nightly-0.1.7.dev202304131555/setup.py`

 * *Files identical despite different names*

