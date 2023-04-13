# Comparing `tmp/clinicadl-1.2.0.tar.gz` & `tmp/clinicadl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinicadl-1.2.0.tar", max compression
+gzip compressed data, was "clinicadl-1.3.0.tar", max compression
```

## Comparing `clinicadl-1.2.0.tar` & `clinicadl-1.3.0.tar`

### file list

```diff
@@ -1,131 +1,141 @@
--rw-r--r--   0        0        0     1093 2023-02-15 15:39:57.831000 clinicadl-1.2.0/LICENSE.txt
--rwxr-xr-x   0        0        0     3737 2023-02-15 15:39:57.831000 clinicadl-1.2.0/README.md
--rw-r--r--   0        0        0      162 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/__init__.py
--rw-r--r--   0        0        0     1608 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/cmdline.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/__init__.py
--rw-r--r--   0        0        0    14819 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/generate.py
--rw-r--r--   0        0        0      697 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/generate_cli.py
--rw-r--r--   0        0        0     1581 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/generate_random_cli.py
--rw-r--r--   0        0        0     1637 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/generate_shepplogan_cli.py
--rw-r--r--   0        0        0     1709 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/generate_trivial_cli.py
--rwxr-xr-x   0        0        0     9736 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/generate/generate_utils.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/interpret/__init__.py
--rw-r--r--   0        0        0     4210 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/interpret/gradients.py
--rw-r--r--   0        0        0     2745 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/interpret/interpret.py
--rw-r--r--   0        0        0     3434 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/interpret/interpret_cli.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/predict/__init__.py
--rw-r--r--   0        0        0     3061 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/predict/predict.py
--rw-r--r--   0        0        0     3364 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/predict/predict_cli.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/prepare_data/__init__.py
--rw-r--r--   0        0        0     7474 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/prepare_data/prepare_data.py
--rw-r--r--   0        0        0     8627 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/prepare_data/prepare_data_cli.py
--rw-r--r--   0        0        0    17336 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/prepare_data/prepare_data_utils.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/__init__.py
--rw-r--r--   0        0        0      665 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/qc_cli.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_linear/__init__.py
--rwxr-xr-x   0        0        0     1738 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_linear/cli.py
--rw-r--r--   0        0        0    22989 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_linear/models.py
--rwxr-xr-x   0        0        0     5520 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_linear/quality_check.py
--rwxr-xr-x   0        0        0     8350 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_linear/utils.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_volume/__init__.py
--rw-r--r--   0        0        0      793 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_volume/cli.py
--rw-r--r--   0        0        0     1898 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_volume/quality_check.py
--rw-r--r--   0        0        0     4670 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/quality_check/t1_volume/utils.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/random_search/__init__.py
--rwxr-xr-x   0        0        0      747 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/random_search/random_search.py
--rw-r--r--   0        0        0      566 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/random_search/random_search_cli.py
--rw-r--r--   0        0        0     6443 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/random_search/random_search_utils.py
--rw-r--r--   0        0        0     1307 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/resources/config/train_config.toml
--rw-r--r--   0        0        0      101 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/resources/masks/README.md
--rwxr-xr-x   0        0        0        0 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/resources/masks/__init__.py
--rw-r--r--   0        0        0      117 2023-02-15 15:39:57.831000 clinicadl-1.2.0/clinicadl/resources/models/README.md
--rwxr-xr-x   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/resources/models/__init__.py
--rwxr-xr-x   0        0        0       25 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/__init__.py
--rw-r--r--   0        0        0     1210 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/from_json_cli.py
--rw-r--r--   0        0        0      773 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/list_models_cli.py
--rw-r--r--   0        0        0     2004 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/resume.py
--rw-r--r--   0        0        0      526 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/resume_cli.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/tasks/__init__.py
--rw-r--r--   0        0        0     2331 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/tasks/classification_cli.py
--rw-r--r--   0        0        0     2167 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/tasks/reconstruction_cli.py
--rw-r--r--   0        0        0     2180 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/tasks/regression_cli.py
--rw-r--r--   0        0        0     3693 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/tasks/task_utils.py
--rw-r--r--   0        0        0      352 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/train.py
--rw-r--r--   0        0        0      707 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/train_cli.py
--rw-r--r--   0        0        0     8213 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/train_option.py
--rw-r--r--   0        0        0     6008 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/train/train_utils.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/adapt/__init__.py
--rw-r--r--   0        0        0     3872 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/adapt/adapt.py
--rw-r--r--   0        0        0     1158 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/adapt/adapt_cli.py
--rw-r--r--   0        0        0       44 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/analysis/__init__.py
--rw-r--r--   0        0        0     7726 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/analysis/analysis.py
--rw-r--r--   0        0        0      670 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/analysis/analysis_cli.py
--rw-r--r--   0        0        0     1268 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/cli.py
--rw-r--r--   0        0        0       60 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_labels/__init__.py
--rw-r--r--   0        0        0    15916 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_labels/get_labels.py
--rw-r--r--   0        0        0     2197 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_labels/get_labels_cli.py
--rw-r--r--   0        0        0     2416 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_metadata/__init__.py
--rw-r--r--   0        0        0     2188 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_metadata/get_metadata.py
--rw-r--r--   0        0        0     1014 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py
--rw-r--r--   0        0        0       45 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_progression/__init__.py
--rw-r--r--   0        0        0     7417 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_progression/get_progression.py
--rw-r--r--   0        0        0      811 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/get_progression/get_progression_cli.py
--rw-r--r--   0        0        0    23294 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/getlabels/getlabels.py
--rw-r--r--   0        0        0       35 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/kfold/__init__.py
--rw-r--r--   0        0        0     6482 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/kfold/kfold.py
--rw-r--r--   0        0        0     1170 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/kfold/kfold_cli.py
--rw-r--r--   0        0        0     4060 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py
--rw-r--r--   0        0        0       35 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/split/__init__.py
--rw-r--r--   0        0        0    12078 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/split/split.py
--rw-r--r--   0        0        0     2470 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/tsvtools/split/split_cli.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/caps_dataset/__init__.py
--rw-r--r--   0        0        0    39699 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/caps_dataset/data.py
--rw-r--r--   0        0        0       45 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/cli_param/__init__.py
--rw-r--r--   0        0        0     1164 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/cli_param/argument.py
--rw-r--r--   0        0        0     4997 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/cli_param/option.py
--rw-r--r--   0        0        0      897 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/cli_param/option_group.py
--rw-r--r--   0        0        0      264 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/cmdline_utils.py
--rw-r--r--   0        0        0      803 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/descriptors.py
--rw-r--r--   0        0        0     1264 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/early_stopping.py
--rw-r--r--   0        0        0      755 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/exceptions.py
--rw-r--r--   0        0        0     2369 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/logger.py
--rw-r--r--   0        0        0      192 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/maps_manager/__init__.py
--rw-r--r--   0        0        0    11309 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/maps_manager/iotools.py
--rw-r--r--   0        0        0     4565 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/maps_manager/logwriter.py
--rw-r--r--   0        0        0    83960 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/maps_manager/maps_manager.py
--rw-r--r--   0        0        0     5702 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/maps_manager/maps_manager_utils.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/meta_maps/__init__.py
--rw-r--r--   0        0        0     2409 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/meta_maps/getter.py
--rw-r--r--   0        0        0    10173 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/metric_module.py
--rw-r--r--   0        0        0      293 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/autoencoder/__init__.py
--rw-r--r--   0        0        0     4751 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/autoencoder/cnn_transformer.py
--rw-r--r--   0        0        0     1496 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/autoencoder/models.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/cnn/__init__.py
--rw-r--r--   0        0        0     7652 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/cnn/models.py
--rw-r--r--   0        0        0     8632 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/cnn/random.py
--rw-r--r--   0        0        0     2394 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/cnn/resnet.py
--rw-r--r--   0        0        0     2822 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/network.py
--rw-r--r--   0        0        0     4044 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/network_utils.py
--rw-r--r--   0        0        0     4389 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/sub_network.py
--rw-r--r--   0        0        0        0 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/vae/__init__.py
--rw-r--r--   0        0        0     2225 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/vae/base_vae.py
--rw-r--r--   0        0        0    10052 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/vae/vae_utils.py
--rw-r--r--   0        0        0    12099 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/network/vae/vanilla_vae.py
--rw-r--r--   0        0        0     1160 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/preprocessing.py
--rw-r--r--   0        0        0     3661 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/seed.py
--rw-r--r--   0        0        0       68 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/split_manager/__init__.py
--rw-r--r--   0        0        0     1142 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/split_manager/kfold.py
--rw-r--r--   0        0        0      816 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/split_manager/single_split.py
--rw-r--r--   0        0        0     9815 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/split_manager/split_manager.py
--rw-r--r--   0        0        0      142 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/task_manager/__init__.py
--rw-r--r--   0        0        0     7163 2023-02-15 15:39:57.835000 clinicadl-1.2.0/clinicadl/utils/task_manager/classification.py
--rw-r--r--   0        0        0     3540 2023-02-15 15:39:57.839000 clinicadl-1.2.0/clinicadl/utils/task_manager/reconstruction.py
--rw-r--r--   0        0        0     5464 2023-02-15 15:39:57.839000 clinicadl-1.2.0/clinicadl/utils/task_manager/regression.py
--rw-r--r--   0        0        0     6976 2023-02-15 15:39:57.839000 clinicadl-1.2.0/clinicadl/utils/task_manager/task_manager.py
--rw-r--r--   0        0        0     9383 2023-02-15 15:39:57.839000 clinicadl-1.2.0/clinicadl/utils/tsvtools_utils.py
--rw-r--r--   0        0        0     2068 2023-02-15 15:39:57.843000 clinicadl-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 clinicadl-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-13 12:16:19.852665 clinicadl-1.3.0/LICENSE.txt
+-rwxr-xr-x   0        0        0     3737 2023-04-13 12:16:19.852665 clinicadl-1.3.0/README.md
+-rw-r--r--   0        0        0      162 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/__init__.py
+-rw-r--r--   0        0        0     1608 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/cmdline.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/generate/__init__.py
+-rw-r--r--   0        0        0    21940 2023-04-13 12:16:19.852665 clinicadl-1.3.0/clinicadl/generate/generate.py
+-rw-r--r--   0        0        0      797 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_cli.py
+-rw-r--r--   0        0        0     1760 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_hypometabolic_cli.py
+-rw-r--r--   0        0        0     1569 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_random_cli.py
+-rw-r--r--   0        0        0     1637 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_shepplogan_cli.py
+-rw-r--r--   0        0        0     1759 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_trivial_cli.py
+-rwxr-xr-x   0        0        0     9883 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/generate/generate_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/__init__.py
+-rw-r--r--   0        0        0     4210 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/gradients.py
+-rw-r--r--   0        0        0     3524 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/interpret.py
+-rw-r--r--   0        0        0     3568 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/interpret/interpret_cli.py
+-rw-r--r--   0        0        0     2816 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/mlflow_test.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/predict/__init__.py
+-rw-r--r--   0        0        0     3089 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/predict/predict.py
+-rw-r--r--   0        0        0     3301 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/predict/predict_cli.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/__init__.py
+-rw-r--r--   0        0        0     7512 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/prepare_data.py
+-rw-r--r--   0        0        0     8624 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_cli.py
+-rw-r--r--   0        0        0    17717 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/pet_linear/cli.py
+-rw-r--r--   0        0        0     4484 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/pet_linear/quality_check.py
+-rw-r--r--   0        0        0     1044 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/pet_linear/utils.py
+-rw-r--r--   0        0        0      747 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/qc_cli.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/__init__.py
+-rwxr-xr-x   0        0        0     1787 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/cli.py
+-rw-r--r--   0        0        0    22989 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/models.py
+-rwxr-xr-x   0        0        0     5435 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/quality_check.py
+-rwxr-xr-x   0        0        0     8355 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_linear/utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/cli.py
+-rw-r--r--   0        0        0     1823 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/quality_check.py
+-rw-r--r--   0        0        0     4622 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/quality_check/t1_volume/utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/__init__.py
+-rwxr-xr-x   0        0        0      723 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/random_search.py
+-rw-r--r--   0        0        0      628 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/random_search_cli.py
+-rw-r--r--   0        0        0     6558 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/random_search/random_search_utils.py
+-rw-r--r--   0        0        0     1324 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/config/train_config.toml
+-rw-r--r--   0        0        0      101 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/masks/README.md
+-rwxr-xr-x   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/masks/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/models/README.md
+-rwxr-xr-x   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/resources/models/__init__.py
+-rwxr-xr-x   0        0        0       25 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/__init__.py
+-rw-r--r--   0        0        0     1251 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/from_json_cli.py
+-rw-r--r--   0        0        0      773 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/list_models_cli.py
+-rw-r--r--   0        0        0     2057 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/resume.py
+-rw-r--r--   0        0        0      526 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/resume_cli.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/__init__.py
+-rw-r--r--   0        0        0     2354 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/classification_cli.py
+-rw-r--r--   0        0        0     2190 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/reconstruction_cli.py
+-rw-r--r--   0        0        0     2203 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/regression_cli.py
+-rw-r--r--   0        0        0     3589 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/tasks/task_utils.py
+-rw-r--r--   0        0        0      377 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train.py
+-rw-r--r--   0        0        0      707 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train_cli.py
+-rw-r--r--   0        0        0     8541 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train_option.py
+-rw-r--r--   0        0        0     6102 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/train/train_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/adapt/__init__.py
+-rw-r--r--   0        0        0     3692 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt.py
+-rw-r--r--   0        0        0     1136 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt_cli.py
+-rw-r--r--   0        0        0       44 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/analysis/__init__.py
+-rw-r--r--   0        0        0     7885 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis.py
+-rw-r--r--   0        0        0      670 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis_cli.py
+-rw-r--r--   0        0        0     1268 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/cli.py
+-rw-r--r--   0        0        0       60 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/__init__.py
+-rw-r--r--   0        0        0    16143 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels.py
+-rw-r--r--   0        0        0     2479 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels_cli.py
+-rw-r--r--   0        0        0     2509 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/__init__.py
+-rw-r--r--   0        0        0     2465 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata.py
+-rw-r--r--   0        0        0      964 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py
+-rw-r--r--   0        0        0       45 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_progression/__init__.py
+-rw-r--r--   0        0        0     7525 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression.py
+-rw-r--r--   0        0        0      811 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression_cli.py
+-rw-r--r--   0        0        0    23294 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/getlabels/getlabels.py
+-rw-r--r--   0        0        0       35 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/kfold/__init__.py
+-rw-r--r--   0        0        0     6369 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold.py
+-rw-r--r--   0        0        0     1170 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold_cli.py
+-rw-r--r--   0        0        0     3997 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py
+-rw-r--r--   0        0        0       35 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/split/__init__.py
+-rw-r--r--   0        0        0    12006 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/split/split.py
+-rw-r--r--   0        0        0     2470 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/tsvtools/split/split_cli.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/caps_dataset/__init__.py
+-rw-r--r--   0        0        0    39601 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/caps_dataset/data.py
+-rw-r--r--   0        0        0       45 2023-04-13 12:16:19.856665 clinicadl-1.3.0/clinicadl/utils/cli_param/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cli_param/argument.py
+-rw-r--r--   0        0        0     5309 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cli_param/option.py
+-rw-r--r--   0        0        0      897 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cli_param/option_group.py
+-rw-r--r--   0        0        0      264 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/cmdline_utils.py
+-rw-r--r--   0        0        0      803 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/descriptors.py
+-rw-r--r--   0        0        0     1264 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/early_stopping.py
+-rw-r--r--   0        0        0      755 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/exceptions.py
+-rw-r--r--   0        0        0     2362 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/logger.py
+-rw-r--r--   0        0        0      192 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/__init__.py
+-rw-r--r--   0        0        0    11591 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/iotools.py
+-rw-r--r--   0        0        0     4480 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/logwriter.py
+-rw-r--r--   0        0        0    86481 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager.py
+-rw-r--r--   0        0        0     8725 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/meta_maps/__init__.py
+-rw-r--r--   0        0        0     2412 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/meta_maps/getter.py
+-rw-r--r--   0        0        0    10173 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/metric_module.py
+-rw-r--r--   0        0        0      354 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/autoencoder/__init__.py
+-rw-r--r--   0        0        0     4751 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/autoencoder/cnn_transformer.py
+-rw-r--r--   0        0        0     1496 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/autoencoder/models.py
+-rw-r--r--   0        0        0     4491 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/SECNN.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/__init__.py
+-rw-r--r--   0        0        0    10360 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/models.py
+-rw-r--r--   0        0        0     8632 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/random.py
+-rw-r--r--   0        0        0     2394 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet.py
+-rw-r--r--   0        0        0     3033 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet3D.py
+-rw-r--r--   0        0        0     2822 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/network.py
+-rw-r--r--   0        0        0     4065 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/network_utils.py
+-rw-r--r--   0        0        0     4377 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/sub_network.py
+-rw-r--r--   0        0        0        0 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/__init__.py
+-rw-r--r--   0        0        0     2238 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/base_vae.py
+-rw-r--r--   0        0        0    10052 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/vae_utils.py
+-rw-r--r--   0        0        0    12099 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/network/vae/vanilla_vae.py
+-rw-r--r--   0        0        0     1280 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/preprocessing.py
+-rw-r--r--   0        0        0     3661 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/seed.py
+-rw-r--r--   0        0        0       68 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/__init__.py
+-rw-r--r--   0        0        0     1133 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/kfold.py
+-rw-r--r--   0        0        0     7204 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/out.txt
+-rw-r--r--   0        0        0     7801 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/ref.txt
+-rw-r--r--   0        0        0      798 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/single_split.py
+-rw-r--r--   0        0        0     9703 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/split_manager.py
+-rw-r--r--   0        0        0     5059 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/split_manager/test.txt
+-rw-r--r--   0        0        0      142 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/__init__.py
+-rw-r--r--   0        0        0     7162 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/classification.py
+-rw-r--r--   0        0        0     3540 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/reconstruction.py
+-rw-r--r--   0        0        0     5471 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/regression.py
+-rw-r--r--   0        0        0     6976 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/task_manager/task_manager.py
+-rw-r--r--   0        0        0     9402 2023-04-13 12:16:19.860665 clinicadl-1.3.0/clinicadl/utils/tsvtools_utils.py
+-rw-r--r--   0        0        0     2068 2023-04-13 12:16:19.868665 clinicadl-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5356 1970-01-01 00:00:00.000000 clinicadl-1.3.0/PKG-INFO
```

### Comparing `clinicadl-1.2.0/LICENSE.txt` & `clinicadl-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/README.md` & `clinicadl-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/cmdline.py` & `clinicadl-1.3.0/clinicadl/cmdline.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/generate/generate.py` & `clinicadl-1.3.0/clinicadl/generate/generate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,93 @@
 # coding: utf8
 
 """
 This file generates data for trivial or intractable (random) data for binary classification.
 """
 import tarfile
-from os import makedirs
-from os.path import basename, dirname, exists, join
+from logging import getLogger
+from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import nibabel as nib
 import numpy as np
 import pandas as pd
 import torch
 from clinica.utils.inputs import RemoteFileStructure, clinica_file_reader, fetch_file
+from joblib import Parallel, delayed
+from nilearn.image import resample_to_img
 
 from clinicadl.prepare_data.prepare_data_utils import compute_extract_json
 from clinicadl.utils.caps_dataset.data import CapsDataset
+from clinicadl.utils.exceptions import DownloadError
 from clinicadl.utils.maps_manager.iotools import check_and_clean, commandline_to_json
 from clinicadl.utils.preprocessing import write_preprocessing
 from clinicadl.utils.tsvtools_utils import extract_baseline
 
 from .generate_utils import (
     find_file_type,
     generate_shepplogan_phantom,
     im_loss_roi_gaussian_distribution,
     load_and_check_tsv,
+    mask_processing,
     write_missing_mods,
 )
 
+logger = getLogger("clinicadl.generate")
+
 
 def generate_random_dataset(
-    caps_directory: str,
-    output_dir: str,
+    caps_directory: Path,
+    output_dir: Path,
     n_subjects: int,
-    tsv_path: Optional[str] = None,
+    tsv_path: Optional[Path] = None,
     mean: float = 0,
     sigma: float = 0.5,
     preprocessing: str = "t1-linear",
     multi_cohort: bool = False,
     uncropped_image: bool = False,
-    acq_label: Optional[str] = None,
+    tracer: Optional[str] = None,
     suvr_reference_region: Optional[str] = None,
 ):
     """
     Generates a random dataset.
 
     Creates a random dataset for intractable classification task from the first
     subject of the tsv file (other subjects/sessions different from the first
     one are ignored. Degree of noise can be parameterized.
 
-    Args:
-        caps_directory: Path to the (input) CAPS directory.
-        output_dir: folder containing the synthetic dataset in (output)
-            CAPS format.
-        n_subjects: number of subjects in each class of the
-            synthetic dataset
-        tsv_path: path to tsv file of list of subjects/sessions.
-        mean: mean of the gaussian noise
-        sigma: standard deviation of the gaussian noise
-        preprocessing: preprocessing performed. Must be in ['t1-linear', 't1-extensive'].
-        multi_cohort: If True caps_directory is the path to a TSV file linking cohort names and paths.
-        uncropped_image: If True the uncropped image of `t1-linear` or `pet-linear` will be used.
-        acq_label: name of the tracer when using `pet-linear` preprocessing.
-        suvr_reference_region: name of the reference region when using `pet-linear` preprocessing.
-
-    Returns:
-        A folder written on the output_dir location (in CAPS format), also a
-        tsv file describing this output
+    Parameters
+    ----------
+    caps_directory: Path
+        Path to the (input) CAPS directory.
+    output_dir: Path
+        Folder containing the synthetic dataset in CAPS format.
+    n_subjects: int
+        Number of subjects in each class of the synthetic dataset
+    tsv_path: Path
+        Path to tsv file of list of subjects/sessions.
+    mean: float
+        Mean of the gaussian noise
+    sigma: float
+        Standard deviation of the gaussian noise
+    preprocessing: str
+        Preprocessing performed. Must be in ['t1-linear', 't1-extensive'].
+    multi_cohort: bool
+        If True caps_directory is the path to a TSV file linking cohort names and paths.
+    uncropped_image: bool
+        If True the uncropped image of `t1-linear` or `pet-linear` will be used.
+    tracer: str
+        name of the tracer when using `pet-linear` preprocessing.
+    suvr_reference_region: str
+        name of the reference region when using `pet-linear` preprocessing.
+
+    Returns
+    -------
+    A folder written on the output_dir location (in CAPS format), also a
+    tsv file describing this output
 
     """
     commandline_to_json(
         {
             "output_dir": output_dir,
             "caps_dir": caps_directory,
             "preprocessing": preprocessing,
@@ -82,105 +99,123 @@
     # Transform caps_directory in dict
     caps_dict = CapsDataset.create_caps_dict(caps_directory, multi_cohort=multi_cohort)
 
     # Read DataFrame
     data_df = load_and_check_tsv(tsv_path, caps_dict, output_dir)
 
     # Create subjects dir
-    makedirs(join(output_dir, "subjects"), exist_ok=True)
+    (output_dir / "subjects").mkdir(parents=True, exist_ok=True)
 
     # Retrieve image of first subject
     participant_id = data_df.loc[0, "participant_id"]
     session_id = data_df.loc[0, "session_id"]
     cohort = data_df.loc[0, "cohort"]
 
     # Find appropriate preprocessing file type
     file_type = find_file_type(
-        preprocessing, uncropped_image, acq_label, suvr_reference_region
+        preprocessing, uncropped_image, tracer, suvr_reference_region
     )
 
-    image_paths = clinica_file_reader(
-        [participant_id], [session_id], caps_dict[cohort], file_type
-    )[0]
-    image_nii = nib.load(image_paths[0])
+    image_path = Path(
+        clinica_file_reader(
+            [participant_id], [session_id], caps_dict[cohort], file_type
+        )[0][0]
+    )
+    image_nii = nib.load(image_path)
     image = image_nii.get_data()
 
     # Create output tsv file
     participant_id_list = [f"sub-RAND{i}" for i in range(2 * n_subjects)]
     session_id_list = ["ses-M00"] * 2 * n_subjects
     diagnosis_list = ["AD"] * n_subjects + ["CN"] * n_subjects
     data = np.array([participant_id_list, session_id_list, diagnosis_list])
     data = data.T
     output_df = pd.DataFrame(
         data, columns=["participant_id", "session_id", "diagnosis"]
     )
     output_df["age_bl"] = 60
     output_df["sex"] = "F"
-    output_df.to_csv(join(output_dir, "data.tsv"), sep="\t", index=False)
+    output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
 
-    input_filename = basename(image_paths[0])
+    input_filename = image_path.name
     filename_pattern = "_".join(input_filename.split("_")[2::])
     for i in range(2 * n_subjects):
         gauss = np.random.normal(mean, sigma, image.shape)
         participant_id = f"sub-RAND{i}"
         noisy_image = image + gauss
         noisy_image_nii = nib.Nifti1Image(
             noisy_image, header=image_nii.header, affine=image_nii.affine
         )
-        noisy_image_nii_path = join(
-            output_dir, "subjects", participant_id, "ses-M00", "t1_linear"
+        noisy_image_nii_path = (
+            output_dir / "subjects" / participant_id / "ses-M00" / "t1_linear"
         )
+
         noisy_image_nii_filename = f"{participant_id}_ses-M00_{filename_pattern}"
-        makedirs(noisy_image_nii_path, exist_ok=True)
-        nib.save(noisy_image_nii, join(noisy_image_nii_path, noisy_image_nii_filename))
+        noisy_image_nii_path.mkdir(parents=True, exist_ok=True)
+        nib.save(noisy_image_nii, noisy_image_nii_path / noisy_image_nii_filename)
 
     write_missing_mods(output_dir, output_df)
 
+    logger.info(f"Random dataset was generated at {output_dir}")
+
 
 def generate_trivial_dataset(
-    caps_directory: str,
-    output_dir: str,
+    caps_directory: Path,
+    output_dir: Path,
     n_subjects: int,
-    tsv_path: Optional[str] = None,
+    tsv_path: Optional[Path] = None,
     preprocessing: str = "t1-linear",
-    mask_path: Optional[str] = None,
+    mask_path: Optional[Path] = None,
     atrophy_percent: float = 60,
     multi_cohort: bool = False,
     uncropped_image: bool = False,
-    acq_label: str = "fdg",
+    tracer: str = "fdg",
     suvr_reference_region: str = "pons",
 ):
     """
     Generates a fully separable dataset.
 
     Generates a dataset, based on the images of the CAPS directory, where a
     half of the image is processed using a mask to occlude a specific region.
     This procedure creates a dataset fully separable (images with half-right
     processed and image with half-left processed)
 
-    Args:
-        caps_directory: path to the CAPS directory.
-        output_dir: folder containing the synthetic dataset in CAPS format.
-        n_subjects: number of subjects in each class of the synthetic dataset.
-        tsv_path: path to tsv file of list of subjects/sessions.
-        preprocessing: preprocessing performed. Must be in ['linear', 'extensive'].
-        mask_path: path to the extracted masks to generate the two labels.
-        atrophy_percent: percentage of atrophy applied.
-        multi_cohort: If True caps_directory is the path to a TSV file linking cohort names and paths.
-        uncropped_image: If True the uncropped image of `t1-linear` or `pet-linear` will be used.
-        acq_label: name of the tracer when using `pet-linear` preprocessing.
-        suvr_reference_region: name of the reference region when using `pet-linear` preprocessing.
+    Parameters
+    ----------
+    caps_directory: Path
+        Path to the CAPS directory.
+    output_dir: Path
+        Folder containing the synthetic dataset in CAPS format.
+    n_subjects: int
+        Number of subjects in each class of the synthetic dataset.
+    tsv_path: Path
+        Path to tsv file of list of subjects/sessions.
+    preprocessing: str
+        Preprocessing performed. Must be in ['linear', 'extensive'].
+    mask_path: Path
+        Path to the extracted masks to generate the two labels.
+    atrophy_percent: float
+        Percentage of atrophy applied.
+    multi_cohort: bool
+        If True caps_directory is the path to a TSV file linking cohort names and paths.
+    uncropped_image: bool
+        If True the uncropped image of `t1-linear` or `pet-linear` will be used.
+    tracer: str
+        Name of the tracer when using `pet-linear` preprocessing.
+    suvr_reference_region: str
+        Name of the reference region when using `pet-linear` preprocessing.
 
-    Returns:
+    Returns
+    -------
         Folder structure where images are stored in CAPS format.
 
-    Raises:
+    Raises
+    ------
         IndexError: if `n_subjects` is higher than the length of the TSV file at `tsv_path`.
     """
-    from pathlib import Path
 
     from clinicadl.utils.exceptions import DownloadError
 
     commandline_to_json(
         {
             "output_dir": output_dir,
             "caps_dir": caps_directory,
@@ -192,112 +227,117 @@
 
     # Transform caps_directory in dict
     caps_dict = CapsDataset.create_caps_dict(caps_directory, multi_cohort=multi_cohort)
     # Read DataFrame
     data_df = load_and_check_tsv(tsv_path, caps_dict, output_dir)
     data_df = extract_baseline(data_df)
 
-    home = str(Path.home())
-    cache_clinicadl = join(home, ".cache", "clinicadl", "ressources", "masks")
+    home = Path.home()
+    cache_clinicadl = home / ".cache" / "clinicadl" / "ressources" / "masks"
     url_aramis = "https://aramislab.paris.inria.fr/files/data/masks/"
     FILE1 = RemoteFileStructure(
         filename="AAL2.tar.gz",
         url=url_aramis,
         checksum="89427970921674792481bffd2de095c8fbf49509d615e7e09e4bc6f0e0564471",
     )
-    makedirs(cache_clinicadl, exist_ok=True)
+    cache_clinicadl.mkdir(parents=True, exist_ok=True)
 
     if n_subjects > len(data_df):
         raise IndexError(
             f"The number of subjects {n_subjects} cannot be higher "
             f"than the number of subjects in the baseline dataset of size {len(data_df)}"
         )
 
     if mask_path is None:
-        if not exists(join(cache_clinicadl, "AAL2")):
+        if not (cache_clinicadl / "AAL2").is_dir():
             print("Downloading AAL2 masks...")
             try:
                 mask_path_tar = fetch_file(FILE1, cache_clinicadl)
                 tar_file = tarfile.open(mask_path_tar)
                 print("File: " + mask_path_tar)
                 try:
                     tar_file.extractall(cache_clinicadl)
                     tar_file.close()
-                    mask_path = join(cache_clinicadl, "AAL2")
+                    mask_path = cache_clinicadl / "AAL2"
                 except RuntimeError:
                     print("Unable to extract downloaded files.")
             except IOError as err:
                 print("Unable to download required templates:", err)
                 raise DownloadError(
                     """Unable to download masks, please download them
                     manually at https://aramislab.paris.inria.fr/files/data/masks/
                     and provide a valid path."""
                 )
         else:
-            mask_path = join(cache_clinicadl, "AAL2")
+            mask_path = cache_clinicadl / "AAL2"
 
     # Create subjects dir
-    makedirs(join(output_dir, "subjects"), exist_ok=True)
+    (output_dir / "subjects").mkdir(parents=True, exist_ok=True)
 
     # Output tsv file
     columns = ["participant_id", "session_id", "diagnosis", "age_bl", "sex"]
     output_df = pd.DataFrame(columns=columns)
     diagnosis_list = ["AD", "CN"]
 
     # Find appropriate preprocessing file type
     file_type = find_file_type(
-        preprocessing, uncropped_image, acq_label, suvr_reference_region
+        preprocessing, uncropped_image, tracer, suvr_reference_region
     )
 
     for i in range(2 * n_subjects):
         data_idx = i // 2
         label = i % 2
 
         participant_id = data_df.loc[data_idx, "participant_id"]
         session_id = data_df.loc[data_idx, "session_id"]
         cohort = data_df.loc[data_idx, "cohort"]
-        image_paths = clinica_file_reader(
-            [participant_id], [session_id], caps_dict[cohort], file_type
-        )[0]
-        image_nii = nib.load(image_paths[0])
+        image_path = Path(
+            clinica_file_reader(
+                [participant_id], [session_id], caps_dict[cohort], file_type
+            )[0][0]
+        )
+        image_nii = nib.load(image_path)
         image = image_nii.get_data()
 
-        input_filename = basename(image_paths[0])
+        input_filename = image_path.name
         filename_pattern = "_".join(input_filename.split("_")[2::])
 
-        trivial_image_nii_dir = join(
-            output_dir, "subjects", f"sub-TRIV{i}", session_id, preprocessing
+        trivial_image_nii_dir = (
+            output_dir / "subjects" / f"sub-TRIV{i}" / session_id / preprocessing
         )
+
         trivial_image_nii_filename = f"sub-TRIV{i}_{session_id}_{filename_pattern}"
 
-        makedirs(trivial_image_nii_dir, exist_ok=True)
+        trivial_image_nii_dir.mkdir(parents=True, exist_ok=True)
 
-        atlas_to_mask = nib.load(join(mask_path, f"mask-{label + 1}.nii")).get_data()
+        atlas_to_mask = nib.load(mask_path / f"mask-{label + 1}.nii").get_data()
 
         # Create atrophied image
         trivial_image = im_loss_roi_gaussian_distribution(
             image, atlas_to_mask, atrophy_percent
         )
         trivial_image_nii = nib.Nifti1Image(trivial_image, affine=image_nii.affine)
         trivial_image_nii.to_filename(
-            join(trivial_image_nii_dir, trivial_image_nii_filename)
+            trivial_image_nii_dir / trivial_image_nii_filename
         )
 
         # Append row to output tsv
         row = [f"sub-TRIV{i}", session_id, diagnosis_list[label], 60, "F"]
         row_df = pd.DataFrame([row], columns=columns)
         output_df = pd.concat([output_df, row_df])
 
-    output_df.to_csv(join(output_dir, "data.tsv"), sep="\t", index=False)
+    output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
 
     write_missing_mods(output_dir, output_df)
 
+    logger.info(f"Trivial dataset was generated at {output_dir}")
+
 
 def generate_shepplogan_dataset(
-    output_dir: str,
+    output_dir: Path,
     img_size: int,
     labels_distribution: Dict[str, Tuple[float, float, float]],
     extract_json: str = None,
     samples: int = 100,
     smoothing: bool = True,
 ):
     """
@@ -309,15 +349,15 @@
         img_size: size of the square image.
         labels_distribution: gives the proportions of the three subtypes (ordered in a tuple) for each label.
         extract_json: name of the JSON file in which generation details are stored.
         samples: number of samples generated per class.
         smoothing: if True, an additional random smoothing is performed on top of all operations on each image.
     """
 
-    check_and_clean(join(output_dir, "subjects"))
+    check_and_clean(output_dir / "subjects")
     commandline_to_json(
         {
             "output_dir": output_dir,
             "img_size": img_size,
             "labels_distribution": labels_distribution,
             "samples": samples,
             "smoothing": smoothing,
@@ -332,51 +372,52 @@
             session_id = "ses-M00"
             subtype = np.random.choice(
                 np.arange(len(labels_distribution[label])), p=labels_distribution[label]
             )
             row_df = pd.DataFrame(
                 [[participant_id, session_id, label, subtype]], columns=columns
             )
-            data_df = data_df.append(row_df)
+            data_df = pd.concat([data_df, row_df])
 
             # Image generation
-            slice_path = join(
-                output_dir,
-                "subjects",
-                participant_id,
-                session_id,
-                "deeplearning_prepare_data",
-                "slice_based",
-                "custom",
-                f"{participant_id}_{session_id}_space-SheppLogan_axis-axi_channel-single_slice-0_phantom.pt",
+            slice_path = (
+                output_dir
+                / "subjects"
+                / participant_id
+                / session_id
+                / "deeplearning_prepare_data"
+                / "slice_based"
+                / "custom"
+                / f"{participant_id}_{session_id}_space-SheppLogan_axis-axi_channel-single_slice-0_phantom.pt"
             )
-            slice_dir = dirname(slice_path)
-            makedirs(slice_dir, exist_ok=True)
+
+            slice_dir = slice_path.parent
+            slice_dir.mkdir(parents=True, exist_ok=True)
 
             slice_np = generate_shepplogan_phantom(
                 img_size, label=subtype, smoothing=smoothing
             )
             slice_tensor = torch.from_numpy(slice_np).float().unsqueeze(0)
             torch.save(slice_tensor, slice_path)
 
-            image_path = join(
-                output_dir,
-                "subjects",
-                participant_id,
-                session_id,
-                "shepplogan",
-                f"{participant_id}_{session_id}_space-SheppLogan_phantom.nii.gz",
+            image_path = (
+                output_dir
+                / "subjects"
+                / participant_id
+                / session_id
+                / "shepplogan"
+                / f"{participant_id}_{session_id}_space-SheppLogan_phantom.nii.gz"
             )
-            image_dir = dirname(image_path)
-            makedirs(image_dir, exist_ok=True)
-            with open(image_path, "w") as f:
+            image_dir = image_path.parent
+            image_dir.mkdir(parents=True, exist_ok=True)
+            with image_path.open("w") as f:
                 f.write("0")
 
     # Save data
-    data_df.to_csv(join(output_dir, "data.tsv"), sep="\t", index=False)
+    data_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
 
     # Save preprocessing JSON file
     preprocessing_dict = {
         "preprocessing": "custom",
         "mode": "slice",
         "use_uncropped_image": False,
         "prepare_dl": True,
@@ -389,7 +430,187 @@
             "pattern": f"*_space-SheppLogan_phantom.nii.gz",
             "description": "Custom suffix",
             "needed_pipeline": "shepplogan",
         },
     }
     write_preprocessing(preprocessing_dict, output_dir)
     write_missing_mods(output_dir, data_df)
+
+    logger.info(f"Shepplogan dataset was generated at {output_dir}")
+
+
+def generate_hypometabolic_dataset(
+    caps_directory: Path,
+    output_dir: Path,
+    n_subjects: int,
+    n_proc: int,
+    tsv_path: Optional[Path] = None,
+    preprocessing: str = "pet-linear",
+    pathology: str = "ad",
+    anomaly_degree: float = 30,
+    sigma: int = 5,
+    uncropped_image: bool = False,
+):
+    """
+    Generates a dataset, based on the images of the CAPS directory, where all
+    the images are processed using a mask to generate a specific pathology.
+
+    Parameters
+    ----------
+    caps_directory: Path
+        Path to the CAPS directory.
+    output_dir: Path
+        Folder containing the synthetic dataset in CAPS format.
+    n_subjects: int
+        Number of subjects in each class of the synthetic dataset.
+    n_proc: int
+        Number of cores used during the task.
+    tsv_path: Path
+        Path to tsv file of list of subjects/sessions.
+    preprocessing: str
+        Preprocessing performed. For now it must be 'pet-linear'.
+    pathology: str
+        Name of the pathology to generate.
+    anomaly_degree: float
+        Percentage of pathology applied.
+    sigma: int
+        It is the parameter of the gaussian filter used for smoothing.
+    uncropped_image: bool
+        If True the uncropped image of `t1-linear` or `pet-linear` will be used.
+
+    Returns
+    -------
+    Folder structure where images are stored in CAPS format.
+
+
+    Raises
+    ------
+    IndexError: if `n_subjects` is higher than the length of the TSV file at `tsv_path`.
+    """
+
+    commandline_to_json(
+        {
+            "output_dir": output_dir,
+            "caps_dir": caps_directory,
+            "preprocessing": preprocessing,
+            "n_subjects": n_subjects,
+            "n_proc": n_proc,
+            "pathology": pathology,
+            "anomaly_degree": anomaly_degree,
+        }
+    )
+
+    # Transform caps_directory in dict
+    caps_dict = CapsDataset.create_caps_dict(caps_directory, multi_cohort=False)
+    # Read DataFrame
+    data_df = load_and_check_tsv(tsv_path, caps_dict, output_dir)
+    data_df = extract_baseline(data_df)
+
+    if n_subjects > len(data_df):
+        raise IndexError(
+            f"The number of subjects {n_subjects} cannot be higher "
+            f"than the number of subjects in the baseline dataset of size {len(data_df)}"
+            f"Please add the '--n_subjects' option and re-run the command."
+        )
+    checksum_dir = {
+        "ad": "2100d514a3fabab49fe30702700085a09cdad449bdf1aa04b8f804e238e4dfc2",
+        "bvftd": "5a0ad28dff649c84761aa64f6e99da882141a56caa46675b8bf538a09fce4f81",
+        "lvppa": "1099f5051c79d5b4fdae25226d97b0e92f958006f6545f498d4b600f3f8a422e",
+        "nfvppa": "9512a4d4dc0003003c4c7526bf2d0ddbee65f1c79357f5819898453ef7271033",
+        "pca": "ace36356b57f4db73e17c421a7cfd7ae056a1b258b8126534cf65d8d0be9527a",
+        "svppa": "44f2e00bf2d2d09b532cb53e3ba61d6087b4114768cc8ae3330ea84c4b7e0e6a",
+    }
+    home = Path.home()
+    cache_clinicadl = home / ".cache" / "clinicadl" / "ressources" / "masks_hypo"
+    url_aramis = "https://aramislab.paris.inria.fr/files/data/masks/hypo/"
+    FILE1 = RemoteFileStructure(
+        filename=f"mask_hypo_{pathology}.nii",
+        url=url_aramis,
+        checksum=checksum_dir[pathology],
+    )
+    cache_clinicadl.mkdir(parents=True, exist_ok=True)
+    if not (cache_clinicadl / f"mask_hypo_{pathology}.nii").is_file():
+        logger.info(f"Downloading {pathology} masks...")
+        # mask_path = fetch_file(FILE1, cache_clinicadl)
+        try:
+            mask_path = fetch_file(FILE1, cache_clinicadl)
+        except:
+            DownloadError(
+                """Unable to download masks, please download them
+                manually at https://aramislab.paris.inria.fr/files/data/masks/
+                and provide a valid path."""
+            )
+
+    else:
+        mask_path = cache_clinicadl / f"mask_hypo_{pathology}.nii"
+
+    mask_nii = nib.load(mask_path)
+
+    # Find appropriate preprocessing file type
+    file_type = find_file_type(
+        preprocessing, uncropped_image, "18FFDG", "cerebellumPons2"
+    )
+
+    # Output tsv file
+    columns = ["participant_id", "session_id", "pathology", "percentage"]
+    output_df = pd.DataFrame(columns=columns)
+    participants = [data_df.loc[i, "participant_id"] for i in range(n_subjects)]
+    sessions = [data_df.loc[i, "session_id"] for i in range(n_subjects)]
+    cohort = caps_directory
+
+    images_paths = clinica_file_reader(participants, sessions, cohort, file_type)[0]
+    image_nii = nib.load(images_paths[0])
+
+    mask_resample_nii = resample_to_img(mask_nii, image_nii, interpolation="nearest")
+    mask = mask_resample_nii.get_fdata()
+
+    mask = mask_processing(mask, anomaly_degree, sigma)
+
+    # Create subjects dir
+    (output_dir / "subjects").mkdir(parents=True, exist_ok=True)
+
+    def generate_hypometabolic_image(i, output_df):
+        image_path = Path(images_paths[i])
+        image_nii = nib.load(image_path)
+        image = image_nii.get_fdata()
+        if image_path.suffix == ".gz":
+            input_filename = Path(image_path.stem).stem
+        else:
+            input_filename = image_path.stem
+        input_filename = input_filename.strip("pet")
+        hypo_image_nii_dir = (
+            output_dir / "subjects" / participants[i] / sessions[i] / preprocessing
+        )
+        hypo_image_nii_filename = (
+            f"{input_filename}pat-{pathology}_deg-{int(anomaly_degree)}_pet.nii.gz"
+        )
+        hypo_image_nii_dir.mkdir(parents=True, exist_ok=True)
+
+        # Create atrophied image
+        hypo_image = image * mask
+        hypo_image_nii = nib.Nifti1Image(hypo_image, affine=image_nii.affine)
+        hypo_image_nii.to_filename(hypo_image_nii_dir / hypo_image_nii_filename)
+
+        # Append row to output tsv
+        row = [
+            participants[i],
+            sessions[i],
+            pathology,
+            anomaly_degree,
+        ]
+        row_df = pd.DataFrame([row], columns=columns)
+        output_df = pd.concat([output_df, row_df])
+        return output_df
+
+    results_list = Parallel(n_jobs=n_proc)(
+        delayed(generate_hypometabolic_image)(i, output_df) for i in range(n_subjects)
+    )
+    for result_df in results_list:
+        output_df = pd.concat([result_df, output_df])
+
+    output_df.to_csv(output_dir / "data.tsv", sep="\t", index=False)
+
+    write_missing_mods(output_dir, output_df)
+
+    logger.info(
+        f"Hypometabolic dataset was generated, with {anomaly_degree} % of dementia {pathology} at {output_dir}."
+    )
```

### Comparing `clinicadl-1.2.0/clinicadl/generate/generate_random_cli.py` & `clinicadl-1.3.0/clinicadl/generate/generate_random_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 @click.option(
     "--sigma",
     type=float,
     default=0.5,
     help="Standard deviation of the gaussian noise added to synthetic images.",
 )
 @cli_param.option.use_uncropped_image
-@cli_param.option.acq_label
+@cli_param.option.tracer
 @cli_param.option.suvr_reference_region
 def cli(
     caps_directory,
     generated_caps_directory,
     preprocessing,
     participants_tsv,
     n_subjects,
     mean,
     sigma,
     use_uncropped_image,
-    acq_label,
+    tracer,
     suvr_reference_region,
 ):
     """Addition of random gaussian noise to brain images.
 
     CAPS_DIRECTORY is the CAPS folder from where input brain images will be loaded.
 
     GENERATED_CAPS_DIRECTORY is a CAPS folder where the random dataset will be saved.
@@ -49,14 +49,14 @@
         preprocessing=preprocessing,
         tsv_path=participants_tsv,
         output_dir=generated_caps_directory,
         n_subjects=n_subjects,
         mean=mean,
         sigma=sigma,
         uncropped_image=use_uncropped_image,
-        acq_label=acq_label,
+        tracer=tracer,
         suvr_reference_region=suvr_reference_region,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinicadl-1.2.0/clinicadl/generate/generate_shepplogan_cli.py` & `clinicadl-1.3.0/clinicadl/generate/generate_shepplogan_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/generate/generate_trivial_cli.py` & `clinicadl-1.3.0/clinicadl/generate/generate_trivial_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,46 @@
+from pathlib import Path
+
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="trivial", no_args_is_help=True)
 @cli_param.argument.caps_directory
 @cli_param.argument.generated_caps
 @cli_param.option.preprocessing
 @cli_param.option.participant_list
 @cli_param.option.n_subjects
 @click.option(
     "--mask_path",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
     help="Path to the extracted masks to generate the two labels. "
     "Default will try to download masks and store them at '~/.cache/clinicadl'.",
 )
 @click.option(
     "--atrophy_percent",
     type=float,
     default=60.0,
     help="Percentage of atrophy applied.",
 )
 @cli_param.option.use_uncropped_image
-@cli_param.option.acq_label
+@cli_param.option.tracer
 @cli_param.option.suvr_reference_region
 def cli(
     caps_directory,
     generated_caps_directory,
     preprocessing,
     participants_tsv,
     n_subjects,
     mask_path,
     atrophy_percent,
     use_uncropped_image,
-    acq_label,
+    tracer,
     suvr_reference_region,
 ):
     """Generation of trivial dataset with addition of synthetic brain atrophy.
 
     CAPS_DIRECTORY is the CAPS folder from where input brain images will be loaded.
 
     GENERATED_CAPS_DIRECTORY is a CAPS folder where the trivial dataset will be saved.
@@ -50,14 +52,14 @@
         tsv_path=participants_tsv,
         preprocessing=preprocessing,
         output_dir=generated_caps_directory,
         n_subjects=n_subjects,
         mask_path=mask_path,
         atrophy_percent=atrophy_percent,
         uncropped_image=use_uncropped_image,
-        acq_label=acq_label,
+        tracer=tracer,
         suvr_reference_region=suvr_reference_region,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinicadl-1.2.0/clinicadl/generate/generate_utils.py` & `clinicadl-1.3.0/clinicadl/generate/generate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 # coding: utf8
 
 import random
+from copy import copy
+from pathlib import Path
 from typing import Dict
 
 import numpy as np
 import pandas as pd
 from clinica.utils.input_files import T1W_LINEAR, T1W_LINEAR_CROPPED, pet_linear_nii
 from scipy.ndimage import gaussian_filter
 from skimage.draw import ellipse
 
 from clinicadl.utils.exceptions import ClinicaDLArgumentError
 
 
 def find_file_type(
     preprocessing: str,
     uncropped_image: bool,
-    acq_label: str,
+    tracer: str,
     suvr_reference_region: str,
 ) -> Dict[str, str]:
     if preprocessing == "t1-linear":
         if uncropped_image:
             file_type = T1W_LINEAR
         else:
             file_type = T1W_LINEAR_CROPPED
     elif preprocessing == "pet-linear":
-        if acq_label is None or suvr_reference_region is None:
+        if tracer is None or suvr_reference_region is None:
             raise ClinicaDLArgumentError(
-                "acq_label and suvr_reference_region must be defined "
+                "`tracer` and `suvr_reference_region` must be defined "
                 "when using `pet-linear` preprocessing."
             )
-        file_type = pet_linear_nii(acq_label, suvr_reference_region, uncropped_image)
+        file_type = pet_linear_nii(tracer, suvr_reference_region, uncropped_image)
     else:
         raise NotImplementedError(
             f"Generation of synthetic data is not implemented for preprocessing {preprocessing}"
         )
 
     return file_type
 
 
-def write_missing_mods(output_dir: str, output_df: pd.DataFrame):
-    from copy import copy
-    from os import makedirs
-    from os.path import join
-
-    missing_path = join(output_dir, "missing_mods")
-    makedirs(missing_path, exist_ok=True)
+def write_missing_mods(output_dir: Path, output_df: pd.DataFrame):
+    missing_path = output_dir / "missing_mods"
+    missing_path.mkdir(parents=True, exist_ok=True)
 
     sessions = output_df.session_id.unique()
     for session in sessions:
         session_df = output_df[output_df.session_id == session]
         out_df = copy(session_df[["participant_id"]])
         out_df["synthetic"] = [1] * len(out_df)
         out_df.to_csv(
-            join(missing_path, f"missing_mods_{session}.tsv"), sep="\t", index=False
+            missing_path / f"missing_mods_{session}.tsv", sep="\t", index=False
         )
 
 
 def load_and_check_tsv(
-    tsv_path: str, caps_dict: Dict[str, str], output_path: str
+    tsv_path: Path, caps_dict: Dict[str, Path], output_path: Path
 ) -> pd.DataFrame:
-    from os.path import join
-
     from clinica.iotools.utils.data_handling import create_subs_sess_list
 
     from clinicadl.utils.caps_dataset.data import check_multi_cohort_tsv
 
     if tsv_path is not None:
         if len(caps_dict) == 1:
             df = pd.read_csv(tsv_path, sep="\t")
@@ -88,15 +84,15 @@
     else:
         df = pd.DataFrame()
         for cohort, caps_path in caps_dict.items():
             create_subs_sess_list(
                 caps_path, output_path, is_bids_dir=False, use_session_tsv=False
             )
             cohort_df = pd.read_csv(
-                join(output_path, "subjects_sessions_list.tsv"), sep="\t"
+                output_path / "subjects_sessions_list.tsv", sep="\t"
             )
             cohort_df["cohort"] = cohort
             df = pd.concat([df, cohort_df])
 
     return df
 
 
@@ -315,7 +311,14 @@
     if smoothing:
         sigma = random.uniform(0, 1)
         img = gaussian_filter(img, sigma * img_size / 100.0)  # smoothing of data
 
     img.clip(0, 1)
 
     return img
+
+
+def mask_processing(mask, percentage, sigma):
+    inverse_mask = 1 - mask
+    inverse_mask[inverse_mask == 0] = 1 - percentage / 100
+    gaussian_mask = gaussian_filter(inverse_mask, sigma=sigma)
+    return gaussian_mask
```

### Comparing `clinicadl-1.2.0/clinicadl/interpret/gradients.py` & `clinicadl-1.3.0/clinicadl/interpret/gradients.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/interpret/interpret.py` & `clinicadl-1.3.0/clinicadl/interpret/interpret.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,84 @@
+from pathlib import Path
 from typing import List
 
 from clinicadl import MapsManager
 
 
 def interpret(
-    maps_dir: str,
+    maps_dir: Path,
     data_group: str,
     name: str,
     method: str,
-    caps_directory: str,
-    tsv_path: str,
+    caps_directory: Path,
+    tsv_path: Path,
     selection_metrics: List[str],
     diagnoses: List[str],
     multi_cohort: bool,
     target_node: int,
     save_individual: bool,
     batch_size: int,
     n_proc: int,
     gpu: bool,
     verbose=0,
     overwrite: bool = False,
     overwrite_name: bool = False,
     level: int = None,
+    save_nifti: bool = False,
 ):
     """
     This function loads a MAPS and interprets all the models selected using a metric in selection_metrics.
 
-    Args:
-        maps_dir: path to the MAPS.
-        data_group: name of the data group interpreted.
-        name: name of the attribution map extracted.
-        method: method used for extraction (ex: gradients, grad-cam...).
-        caps_directory: path to the CAPS folder. For more information please refer to
-            [clinica documentation](https://aramislab.paris.inria.fr/clinica/docs/public/latest/CAPS/Introduction/).
-        tsv_path: path to a TSV file containing the list of participants and sessions to interpret.
-        target_node: Node from which the interpretation is computed.
-        save_individual: If True saves the individual map of each participant / session couple.
-        gpu: if true, it uses gpu.
-        n_proc: num_workers used in DataLoader
-        batch_size: batch size of the DataLoader
-        selection_metrics: list of metrics to find best models to be evaluated.
-        diagnoses: list of diagnoses to be tested if tsv_path is a folder.
-        multi_cohort: If True caps_directory is the path to a TSV file linking cohort names and paths.
-        verbose: level of verbosity (0: warning, 1: info, 2: debug).
-        overwrite: If True former definition of data group is erased.
-        overwrite_name: If True former interpretability map with the same name is erased.
-        level: layer number in the convolutional part after which the feature map is chosen.
+    Parameters
+    ----------
+    maps_dir: str (Path)
+        Path to the MAPS
+    data_group: str
+        Name of the data group interpreted.
+    name: str
+        Name of the interpretation procedure.
+    method: str
+        Method used for extraction (ex: gradients, grad-cam...).
+    caps_directory: str (Path)
+        Path to the CAPS folder. For more information please refer to
+        [clinica documentation](https://aramislab.paris.inria.fr/clinica/docs/public/latest/CAPS/Introduction/).
+        Default will load the value of an existing data group.
+    tsv_path: str (Path)
+        Path to a TSV file containing the list of participants and sessions to test.
+        Default will load the DataFrame of an existing data group.
+    selection_metrics: list of str
+        List of metrics to find best models to be evaluated..
+        Default performs the interpretation on all selection metrics available.
+    multi_cohort: bool
+        If True caps_directory is the path to a TSV file linking cohort names and paths.
+    diagnoses: list of str
+        List of diagnoses to load if tsv_path is a split_directory.
+        Default uses the same as in training step.
+    target_node: int
+        Node from which the interpretation is computed.
+    save_individual: bool
+        If True saves the individual map of each participant / session couple.
+    batch_size: int
+        If given, sets the value of batch_size, else use the same as in training step.
+    n_proc: int
+        If given, sets the value of num_workers, else use the same as in training step.
+    gpu: bool
+        If given, a new value for the device of the model will be computed.
+    overwrite: bool
+        If True former definition of data group is erased.
+    overwrite_name: bool
+        If True former interpretability map with the same name is erased.
+    level: int
+        Layer number in the convolutional part after which the feature map is chosen.
+    save_nifi : bool
+        If True, save the interpretation map in nifti format.
+    verbose: int
+        Level of verbosity (0: warning, 1: info, 2: debug).
     """
+
     verbose_list = ["warning", "info", "debug"]
     if verbose > 2:
         verbose_str = "debug"
     else:
         verbose_str = verbose_list[verbose]
 
     maps_manager = MapsManager(maps_dir, verbose=verbose_str)
@@ -68,8 +96,9 @@
         save_individual=save_individual,
         batch_size=batch_size,
         n_proc=n_proc,
         gpu=gpu,
         overwrite=overwrite,
         overwrite_name=overwrite_name,
         level=level,
+        save_nifti=save_nifti,
     )
```

### Comparing `clinicadl-1.2.0/clinicadl/interpret/interpret_cli.py` & `clinicadl-1.3.0/clinicadl/interpret/interpret_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command("interpret", no_args_is_help=True)
 @cli_param.argument.input_maps
@@ -27,22 +29,22 @@
     type=str,
     multiple=True,
     help="Load the model selected on the metrics given.",
 )
 # Data
 @click.option(
     "--participants_tsv",
-    type=click.Path(exists=True),
+    type=click.Path(exists=True, path_type=Path),
     default=None,
     help="Path to a TSV file with participants/sessions to process, "
     "if different from the one used during network training.",
 )
 @click.option(
     "--caps_directory",
-    type=click.Path(exists=True),
+    type=click.Path(exists=True, path_type=Path),
     default=None,
     help="Input CAPS directory, if different from the one used during network training.",
 )
 @click.option(
     "--multi_cohort",
     type=bool,
     default=False,
@@ -76,14 +78,15 @@
 @click.option(
     "--overwrite_name",
     "-on",
     is_flag=True,
     default=False,
     help="Overwrite the name if it already exists.",
 )
+@cli_param.option.save_nifti
 def cli(
     input_maps_directory,
     data_group,
     name,
     method,
     caps_directory,
     participants_tsv,
@@ -94,14 +97,15 @@
     target_node,
     save_individual,
     batch_size,
     n_proc,
     gpu,
     overwrite,
     overwrite_name,
+    save_nifti,
 ):
     """Interpretation of trained models using saliency map method.
 
     INPUT_MAPS_DIRECTORY is the MAPS folder from where the model to interpret will be loaded.
 
     DATA_GROUP is the name of the subjects and sessions list used for the interpretation.
 
@@ -130,9 +134,10 @@
         save_individual=save_individual,
         batch_size=batch_size,
         n_proc=n_proc,
         gpu=gpu,
         overwrite=overwrite,
         overwrite_name=overwrite_name,
         level=level_grad_cam,
+        save_nifti=save_nifti,
         # verbose=verbose,
     )
```

### Comparing `clinicadl-1.2.0/clinicadl/predict/predict.py` & `clinicadl-1.3.0/clinicadl/predict/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # coding: utf8
+from pathlib import Path
 from typing import List
 
 from clinicadl import MapsManager
 from clinicadl.utils.exceptions import ClinicaDLArgumentError
 
 
 def predict(
-    maps_dir: str,
+    maps_dir: Path,
     data_group: str,
-    caps_directory: str,
-    tsv_path: str,
+    caps_directory: Path,
+    tsv_path: Path,
     use_labels: bool = True,
     label: str = None,
     gpu: bool = True,
     n_proc: int = 0,
     batch_size: int = 1,
     selection_metrics: List[str] = None,
     diagnoses: List[str] = None,
```

### Comparing `clinicadl-1.2.0/clinicadl/predict/predict_cli.py` & `clinicadl-1.3.0/clinicadl/predict/predict_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+from pathlib import Path
+
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="predict", no_args_is_help=True)
 @cli_param.argument.input_maps
 @cli_param.argument.data_group
 @click.option(
     "--caps_directory",
-    type=click.Path(exists=True),
+    type=click.Path(exists=True, path_type=Path),
     default=None,
     help="Data using CAPS structure, if different from the one used during network training.",
 )
 @click.option(
     "--participants_tsv",
     default=None,
-    type=click.Path(),
+    type=click.Path(exists=True, path_type=Path),
     help="""Path to the file with subjects/sessions to process, if different from the one used during network training.
     If it includes the filename will load the TSV file directly.
     Else will load the baseline TSV files of wanted diagnoses produced by `tsvtool split`.""",
 )
 @click.option(
     "--use_labels/--no_labels",
     default=True,
@@ -58,21 +60,15 @@
 @click.option(
     "--save_tensor",
     type=bool,
     default=False,
     is_flag=True,
     help="Save the reconstruction output in the MAPS in Pytorch tensor format.",
 )
-@click.option(
-    "--save_nifti",
-    type=bool,
-    default=False,
-    is_flag=True,
-    help="Save the reconstruction output in the MAPS in NIfTI format.",
-)
+@cli_param.option.save_nifti
 @cli_param.option.use_gpu
 @cli_param.option.n_proc
 @cli_param.option.batch_size
 @cli_param.option.overwrite
 def cli(
     input_maps_directory,
     data_group,
```

### Comparing `clinicadl-1.2.0/clinicadl/prepare_data/prepare_data.py` & `clinicadl-1.3.0/clinicadl/prepare_data/prepare_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from logging import getLogger
+from pathlib import Path
 
 
-def DeepLearningPrepareData(caps_directory, tsv_file, n_proc, parameters):
-    import os
-    from os import path
-
+def DeepLearningPrepareData(caps_directory: Path, tsv_file: Path, n_proc, parameters):
     from clinica.utils.inputs import check_caps_folder, clinica_file_reader
     from clinica.utils.nipype import container_from_filename
     from clinica.utils.participant import get_subject_session_list
     from joblib import Parallel, delayed
     from torch import save as save_tensor
 
     from clinicadl.utils.exceptions import ClinicaDLArgumentError
     from clinicadl.utils.preprocessing import write_preprocessing
 
     from .prepare_data_utils import check_mask_list, compute_folder_and_file_type
 
-    logger = getLogger("clinicadl.extract")
+    logger = getLogger("clinicadl.prepare_data")
 
     # Get subject and session list
     check_caps_folder(caps_directory)
-    logger.debug(f"CAPS directory : {caps_directory}.")
+    logger.debug(f"CAPS directory: {caps_directory}.")
     is_bids_dir = False
     sessions, subjects = get_subject_session_list(
         caps_directory, tsv_file, is_bids_dir, False, None
     )
     if parameters["prepare_dl"]:
         logger.info(
             f"{parameters['mode']}s will be extracted in Pytorch tensor from {len(sessions)} images."
@@ -45,56 +43,58 @@
     logger.debug(
         f"Selected images are preprocessed with {parameters['preprocessing']} pipeline`."
     )
     mod_subfolder, file_type = compute_folder_and_file_type(parameters)
     parameters["file_type"] = file_type
 
     # Input file:
-    input_files = clinica_file_reader(subjects, sessions, caps_directory, file_type)[0]
+    input_files = clinica_file_reader(
+        subjects, sessions, caps_directory.as_posix(), file_type
+    )[0]
 
     def write_output_imgs(output_mode, container, subfolder):
         # Write the extracted tensor on a .pt file
         for filename, tensor in output_mode:
-            output_file_dir = path.join(
-                caps_directory,
-                container,
-                "deeplearning_prepare_data",
-                subfolder,
-                mod_subfolder,
+            output_file_dir = (
+                caps_directory
+                / container
+                / "deeplearning_prepare_data"
+                / subfolder
+                / mod_subfolder
             )
-            if not path.exists(output_file_dir):
-                os.makedirs(output_file_dir)
-            output_file = path.join(output_file_dir, filename)
+            if not output_file_dir.is_dir():
+                output_file_dir.mkdir(parents=True, exist_ok=True)
+            output_file = output_file_dir / filename
             save_tensor(tensor, output_file)
-            logger.debug(f"    Output tensor saved at {output_file}")
+            logger.debug(f"Output tensor saved at {output_file}")
 
     if parameters["mode"] == "image" or not parameters["prepare_dl"]:
 
         def prepare_image(file):
             from .prepare_data_utils import extract_images
 
-            logger.debug(f"  Processing of {file}.")
+            logger.debug(f"Processing of {file}.")
             container = container_from_filename(file)
             subfolder = "image_based"
-            output_mode = extract_images(file)
-            logger.debug(f"    Image extracted.")
+            output_mode = extract_images(Path(file))
+            logger.debug(f"Image extracted.")
             write_output_imgs(output_mode, container, subfolder)
 
         Parallel(n_jobs=n_proc)(delayed(prepare_image)(file) for file in input_files)
 
     elif parameters["prepare_dl"] and parameters["mode"] == "slice":
 
         def prepare_slice(file):
             from .prepare_data_utils import extract_slices
 
             logger.debug(f"  Processing of {file}.")
             container = container_from_filename(file)
             subfolder = "slice_based"
             output_mode = extract_slices(
-                file,
+                Path(file),
                 slice_direction=parameters["slice_direction"],
                 slice_mode=parameters["slice_mode"],
                 discarded_slices=parameters["discarded_slices"],
             )
             logger.debug(f"    {len(output_mode)} slices extracted.")
             write_output_imgs(output_mode, container, subfolder)
 
@@ -105,15 +105,15 @@
         def prepare_patch(file):
             from .prepare_data_utils import extract_patches
 
             logger.debug(f"  Processing of {file}.")
             container = container_from_filename(file)
             subfolder = "patch_based"
             output_mode = extract_patches(
-                file,
+                Path(file),
                 patch_size=parameters["patch_size"],
                 stride_size=parameters["stride_size"],
             )
             logger.debug(f"    {len(output_mode)} patches extracted.")
             write_output_imgs(output_mode, container, subfolder)
 
         Parallel(n_jobs=n_proc)(delayed(prepare_patch)(file) for file in input_files)
@@ -137,32 +137,34 @@
                 from .prepare_data_utils import PATTERN_DICT, TEMPLATE_DICT
 
                 parameters["roi_template"] = TEMPLATE_DICT[parameters["preprocessing"]]
                 parameters["roi_mask_pattern"] = PATTERN_DICT[
                     parameters["preprocessing"]
                 ]
 
-            parameters["masks_location"] = path.join(
-                caps_directory, "masks", f"tpl-{parameters['roi_template']}"
+            parameters["masks_location"] = (
+                caps_directory / "masks" / f"tpl-{parameters['roi_template']}"
             )
+
             if len(parameters["roi_list"]) == 0:
                 raise ClinicaDLArgumentError(
                     "A list of regions of interest must be given."
                 )
             else:
                 check_mask_list(
                     parameters["masks_location"],
                     parameters["roi_list"],
                     parameters["roi_mask_pattern"],
                     None
                     if parameters["use_uncropped_image"] is None
                     else not parameters["use_uncropped_image"],
                 )
+
             output_mode = extract_roi(
-                file,
+                Path(file),
                 masks_location=parameters["masks_location"],
                 mask_pattern=parameters["roi_mask_pattern"],
                 cropped_input=None
                 if parameters["use_uncropped_image"] is None
                 else not parameters["use_uncropped_image"],
                 roi_names=parameters["roi_list"],
                 uncrop_output=parameters["uncropped_roi"],
```

### Comparing `clinicadl-1.2.0/clinicadl/prepare_data/prepare_data_cli.py` & `clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Optional
 
 import click
 
 from clinicadl.utils import cli_param
 
 from .prepare_data import DeepLearningPrepareData
@@ -11,25 +12,25 @@
 @click.command(name="image", no_args_is_help=True)
 @cli_param.argument.caps_directory
 @cli_param.argument.modality
 @cli_param.option.n_proc
 @cli_param.option.subjects_sessions_tsv
 @cli_param.option.extract_json
 @cli_param.option.use_uncropped_image
-@cli_param.option.acq_label
+@cli_param.option.tracer
 @cli_param.option.suvr_reference_region
 @cli_param.option.custom_suffix
 def image_cli(
-    caps_directory: str,
+    caps_directory: Path,
     modality: str,
     n_proc: int,
-    subjects_sessions_tsv: Optional[str] = None,
+    subjects_sessions_tsv: Optional[Path] = None,
     extract_json: str = None,
     use_uncropped_image: bool = False,
-    acq_label: Optional[str] = None,
+    tracer: Optional[str] = None,
     suvr_reference_region: Optional[str] = None,
     custom_suffix: str = "",
 ):
     """Extract image from nifti images.
 
     CAPS_DIRECTORY is the CAPS folder where nifti images are stored and tensor will be saved.
 
@@ -38,15 +39,15 @@
     parameters = get_parameters_dict(
         modality,
         "image",
         False,
         extract_json,
         use_uncropped_image,
         custom_suffix,
-        acq_label,
+        tracer,
         suvr_reference_region,
     )
     DeepLearningPrepareData(
         caps_directory=caps_directory,
         tsv_file=subjects_sessions_tsv,
         n_proc=n_proc,
         parameters=parameters,
@@ -71,28 +72,28 @@
 @click.option(
     "-ss",
     "--stride_size",
     default=50,
     show_default=True,
     help="Stride size.",
 )
-@cli_param.option.acq_label
+@cli_param.option.tracer
 @cli_param.option.suvr_reference_region
 @cli_param.option.custom_suffix
 def patch_cli(
-    caps_directory: str,
+    caps_directory: Path,
     modality: str,
     n_proc: int,
     save_features: bool = False,
-    subjects_sessions_tsv: Optional[str] = None,
+    subjects_sessions_tsv: Optional[Path] = None,
     extract_json: str = None,
     use_uncropped_image: bool = False,
     patch_size: int = 50,
     stride_size: int = 50,
-    acq_label: Optional[str] = None,
+    tracer: Optional[str] = None,
     suvr_reference_region: Optional[str] = None,
     custom_suffix: str = "",
 ):
     """Extract patch from nifti images.
 
     CAPS_DIRECTORY is the CAPS folder where nifti images are stored and tensor will be saved.
 
@@ -101,15 +102,15 @@
     parameters = get_parameters_dict(
         modality,
         "patch",
         save_features,
         extract_json,
         use_uncropped_image,
         custom_suffix,
-        acq_label,
+        tracer,
         suvr_reference_region,
     )
     parameters["patch_size"] = patch_size
     parameters["stride_size"] = stride_size
 
     DeepLearningPrepareData(
         caps_directory=caps_directory,
@@ -152,29 +153,29 @@
     type=int,
     default=(0, 0),
     multiple=2,
     help="""Number of slices discarded from respectively the beginning and
         the end of the MRI volume.  If only one argument is given, it will be
         used for both sides.""",
 )
-@cli_param.option.acq_label
+@cli_param.option.tracer
 @cli_param.option.suvr_reference_region
 @cli_param.option.custom_suffix
 def slice_cli(
-    caps_directory: str,
+    caps_directory: Path,
     modality: str,
     n_proc: int,
     save_features: bool = False,
-    subjects_sessions_tsv: Optional[str] = None,
+    subjects_sessions_tsv: Optional[Path] = None,
     extract_json: str = None,
     use_uncropped_image: bool = False,
     slice_direction: int = 0,
     slice_mode: str = "rgb",
     discarded_slices: int = 0,
-    acq_label: Optional[str] = None,
+    tracer: Optional[str] = None,
     suvr_reference_region: Optional[str] = None,
     custom_suffix: str = "",
 ):
     """Extract slice from nifti images.
 
     CAPS_DIRECTORY is the CAPS folder where nifti images are stored and tensor will be saved.
 
@@ -183,15 +184,15 @@
     parameters = get_parameters_dict(
         modality,
         "slice",
         save_features,
         extract_json,
         use_uncropped_image,
         custom_suffix,
-        acq_label,
+        tracer,
         suvr_reference_region,
     )
     parameters["slice_direction"] = slice_direction
     parameters["slice_mode"] = slice_mode
     parameters["discarded_slices"] = discarded_slices
 
     DeepLearningPrepareData(
@@ -238,30 +239,30 @@
     "-cmp",
     type=str,
     default="",
     help="""Mask pattern if MODALITY is `custom`.
             If given will select only the masks containing the string given.
             The mask with the shortest name is taken.""",
 )
-@cli_param.option.acq_label
+@cli_param.option.tracer
 @cli_param.option.suvr_reference_region
 @cli_param.option.custom_suffix
 def roi_cli(
-    caps_directory: str,
+    caps_directory: Path,
     modality: str,
     n_proc: int,
     save_features: bool = False,
-    subjects_sessions_tsv: Optional[str] = None,
+    subjects_sessions_tsv: Optional[Path] = None,
     extract_json: str = None,
     use_uncropped_image: bool = False,
     roi_list: list = [],
     roi_uncrop_output: bool = False,
     roi_custom_template: str = "",
     roi_custom_mask_pattern: str = "",
-    acq_label: Optional[str] = None,
+    tracer: Optional[str] = None,
     suvr_reference_region: Optional[str] = None,
     custom_suffix: str = "",
 ):
     """Extract roi from nifti images.
 
     CAPS_DIRECTORY is the CAPS folder where nifti images are stored and tensor will be saved.
 
@@ -270,15 +271,15 @@
     parameters = get_parameters_dict(
         modality,
         "roi",
         save_features,
         extract_json,
         use_uncropped_image,
         custom_suffix,
-        acq_label,
+        tracer,
         suvr_reference_region,
     )
     parameters["roi_list"] = roi_list
     parameters["uncropped_roi"] = roi_uncrop_output
     parameters["roi_custom_template"] = roi_custom_template
     parameters["roi_custom_mask_pattern"] = roi_custom_mask_pattern
```

### Comparing `clinicadl-1.2.0/clinicadl/prepare_data/prepare_data_utils.py` & `clinicadl-1.3.0/clinicadl/prepare_data/prepare_data_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,84 +1,105 @@
 # coding: utf8
-from os import path
+from pathlib import Path
 from time import time
 from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 import torch
 
 
 def get_parameters_dict(
     modality: str,
     extract_method: str,
     save_features: bool,
     extract_json: str,
     use_uncropped_image: bool,
     custom_suffix: str,
-    acq_label: str,
+    tracer: str,
     suvr_reference_region: str,
 ) -> Dict[str, Any]:
     """
-    Args:
-        modality: preprocessing procedure performed with Clinica.
-        extract_method: mode of extraction (image, slice, patch, roi).
-        save_features: If True modes are extracted, else images are extracted
-            and the extraction of modes is done on-the-fly during training.
-        extract_json: Name of the JSON file created to sum up the arguments of tensor extraction.
-        use_uncropped_image: If True the cropped version of the image is used
-            (specific to t1-linear and pet-linear).
-        custom_suffix: string used to identify images when modality is custom.
-        acq_label: name of the tracer (specific to PET pipelines).
-        suvr_reference_region: name of the reference region for normalization
-            specific to PET pipelines)
+    Parameters
+    ----------
+    modality: str
+        Preprocessing procedure performed with Clinica.
+    extract_method: str
+        Mode of extraction (image, slice, patch, roi).
+    save_features: bool
+        If True modes are extracted, else images are extracted
+        and the extraction of modes is done on-the-fly during training.
+    extract_json: str
+        Name of the JSON file created to sum up the arguments of tensor extraction.
+    use_uncropped_image: bool
+        If True the cropped version of the image is used
+        (specific to t1-linear and pet-linear).
+    custom_suffix: str
+        String used to identify images when modality is custom.
+    tracer: str
+        Name of the tracer (specific to PET pipelines).
+    suvr_reference_region: str
+        Name of the reference region for normalization specific to PET pipelines)
     Returns:
         The dictionary of parameters specific to the preprocessing
     """
     parameters = {
         "preprocessing": modality,
         "mode": extract_method,
         "use_uncropped_image": use_uncropped_image,
         "prepare_dl": save_features,
     }
 
     if modality == "custom":
         parameters["custom_suffix"] = custom_suffix
     if modality == "pet-linear":
-        parameters["acq_label"] = acq_label
+        parameters["tracer"] = tracer
         parameters["suvr_reference_region"] = suvr_reference_region
 
     parameters["extract_json"] = compute_extract_json(extract_json)
 
     return parameters
 
 
 def compute_extract_json(extract_json: str) -> str:
     if extract_json is None:
         return f"extract_{int(time())}.json"
-    elif not extract_json.endswith(".json"):
+    elif not extract_json.suffix == ".json":
         return f"{extract_json}.json"
     else:
         return extract_json
 
 
 def compute_folder_and_file_type(
     parameters: Dict[str, Any]
 ) -> Tuple[str, Dict[str, str]]:
-    from clinica.utils.input_files import T1W_LINEAR, T1W_LINEAR_CROPPED, pet_linear_nii
+    from clinica.utils.input_files import (
+        FLAIR_T2W_LINEAR,
+        FLAIR_T2W_LINEAR_CROPPED,
+        T1W_LINEAR,
+        T1W_LINEAR_CROPPED,
+        pet_linear_nii,
+    )
 
     if parameters["preprocessing"] == "t1-linear":
         mod_subfolder = "t1_linear"
         if parameters["use_uncropped_image"]:
             file_type = T1W_LINEAR
         else:
             file_type = T1W_LINEAR_CROPPED
+
+    elif parameters["preprocessing"] == "flair-linear":
+        mod_subfolder = "flair_linear"
+        if parameters["use_uncropped_image"]:
+            file_type = FLAIR_T2W_LINEAR
+        else:
+            file_type = FLAIR_T2W_LINEAR_CROPPED
     elif parameters["preprocessing"] == "pet-linear":
         mod_subfolder = "pet_linear"
         file_type = pet_linear_nii(
-            parameters["acq_label"],
+            parameters["tracer"],
             parameters["suvr_reference_region"],
             parameters["use_uncropped_image"],
         )
     elif parameters["preprocessing"] == "custom":
         mod_subfolder = "custom"
         file_type = {
             "pattern": f"*{parameters['custom_suffix']}",
@@ -108,15 +129,15 @@
             f"Maximum two number of discarded slices can be defined. "
             f"You gave discarded slices = {discarded_slices}."
         )
     return begin_discard, end_discard
 
 
 def extract_slices(
-    nii_path: str,
+    nii_path: Path,
     slice_direction: int = 0,
     slice_mode: str = "single",
     discarded_slices: Union[int, tuple] = 0,
 ) -> List[Tuple[str, torch.Tensor]]:
     """Extracts the slices from three directions
     This function extracts slices form the preprocessed nifti image.
 
@@ -180,39 +201,38 @@
             (slice_tensor, slice_tensor, slice_tensor)
         )  # shape is 3 * W * L
 
     return slice_tensor.clone()
 
 
 def extract_slice_path(
-    img_path: str, slice_direction: int, slice_mode: str, slice_index: int
+    img_path: Path, slice_direction: int, slice_mode: str, slice_index: int
 ) -> str:
-
     direction_dict = {0: "sag", 1: "cor", 2: "axi"}
     if slice_direction not in direction_dict:
         raise KeyError(
             f"Slice direction {slice_direction} should be in {direction_dict.keys()} corresponding to {direction_dict}."
         )
 
-    input_img_filename = path.basename(img_path)
+    input_img_filename = img_path.name
     txt_idx = input_img_filename.rfind("_")
     it_filename_prefix = input_img_filename[0:txt_idx]
     it_filename_suffix = input_img_filename[txt_idx:]
     it_filename_suffix = it_filename_suffix.replace(".nii.gz", ".pt")
     return (
         f"{it_filename_prefix}_axis-{direction_dict[slice_direction]}"
         f"_channel-{slice_mode}_slice-{slice_index}{it_filename_suffix}"
     )
 
 
 ############
 # PATCH    #
 ############
 def extract_patches(
-    nii_path: str,
+    nii_path: Path,
     patch_size: int,
     stride_size: int,
 ) -> List[Tuple[str, torch.Tensor]]:
     """Extracts the patches
     This function extracts patches form the preprocessed nifti image. Patch size
     if provided as input and also the stride size. If stride size is smaller
     than the patch size an overlap exist between consecutive patches. If stride
@@ -271,58 +291,55 @@
         # the dimension of patches_tensor is [1, patch_num1, patch_num2, patch_num3, patch_size1, patch_size2, patch_size3]
         patches_tensor = patches_tensor.view(-1, patch_size, patch_size, patch_size)
 
     return patches_tensor[patch_index, ...].unsqueeze_(0).clone()
 
 
 def extract_patch_path(
-    img_path: str, patch_size: int, stride_size: int, patch_index: int
+    img_path: Path, patch_size: int, stride_size: int, patch_index: int
 ) -> str:
-    input_img_filename = path.basename(img_path)
+    input_img_filename = img_path.name
     txt_idx = input_img_filename.rfind("_")
     it_filename_prefix = input_img_filename[0:txt_idx]
     it_filename_suffix = input_img_filename[txt_idx:]
     it_filename_suffix = it_filename_suffix.replace(".nii.gz", ".pt")
 
     return f"{it_filename_prefix}_patchsize-{patch_size}_stride-{stride_size}_patch-{patch_index}{it_filename_suffix}"
 
 
 ############
 # IMAGE    #
 ############
-def extract_images(input_img: str) -> List[Tuple[str, torch.Tensor]]:
+def extract_images(input_img: Path) -> List[Tuple[str, torch.Tensor]]:
     """Extract the images
     This function convert nifti image to tensor (.pt) version of the image.
     Tensor version is saved at the same location than input_img.
     Args:
         input_img: path to the NifTi input image.
     Returns:
         filename (str): single tensor file  saved on the disk. Same location than input file.
     """
-
-    import os
-
     import nibabel as nib
     import torch
 
     image_array = nib.load(input_img).get_fdata(dtype="float32")
     image_tensor = torch.from_numpy(image_array).unsqueeze(0).float()
     # make sure the tensor type is torch.float32
     output_file = (
-        os.path.basename(input_img).replace(".nii.gz", ".pt"),
+        Path(input_img.name.replace(".nii.gz", ".pt")),
         image_tensor.clone(),
     )
 
     return [output_file]
 
 
 ############
 # ROI    #
 ############
-def check_mask_list(masks_location, roi_list, mask_pattern, cropping):
+def check_mask_list(masks_location: Path, roi_list, mask_pattern, cropping):
     import nibabel as nib
     import numpy as np
 
     for roi in roi_list:
         roi_path, desc = find_mask_path(masks_location, roi, mask_pattern, cropping)
         if roi_path is None:
             raise FileNotFoundError(
@@ -333,68 +350,65 @@
         if mask_values != {0, 1}:
             raise ValueError(
                 "The ROI masks used should be binary (composed of 0 and 1 only)."
             )
 
 
 def find_mask_path(
-    masks_location: str, roi: str, mask_pattern: str, cropping: bool
+    masks_location: Path, roi: str, mask_pattern: str, cropping: bool
 ) -> Tuple[str, str]:
     """
     Finds masks corresponding to the pattern asked and containing the adequate cropping description
 
     Args:
         masks_location: directory containing the masks.
         roi: name of the region.
         mask_pattern: pattern which should be found in the filename of the mask.
         cropping: if True the original image should contain the substring 'desc-Crop'.
 
     Returns:
         path of the mask or None if nothing was found.
         a human-friendly description of the pattern looked for.
     """
-    from glob import glob
-    from os import path
 
     # Check that pattern begins and ends with _ to avoid mixing keys
     if mask_pattern is None:
         mask_pattern = ""
 
-    candidates_pattern = path.join(
-        masks_location, f"*{mask_pattern}*_roi-{roi}_mask.nii*"
-    )
+    candidates_pattern = f"*{mask_pattern}*_roi-{roi}_mask.nii*"
+
     desc = f"The mask should follow the pattern {candidates_pattern}. "
-    candidates = glob(candidates_pattern)
+    candidates = [e for e in masks_location.glob(candidates_pattern)]
     if cropping is None:
-        pass
+        # pass
+        candidates2 = candidates
     elif cropping:
-        candidates = [mask for mask in candidates if "_desc-Crop_" in mask]
+        candidates2 = [mask for mask in candidates if "_desc-Crop_" in mask.name]
         desc += f"and contain '_desc-Crop_' string."
     else:
-        candidates = [mask for mask in candidates if "_desc-Crop_" not in mask]
+        candidates2 = [mask for mask in candidates if "_desc-Crop_" not in mask.name]
         desc += f"and not contain '_desc-Crop_' string."
 
-    if len(candidates) == 0:
+    if len(candidates2) == 0:
         return None, desc
     else:
-        return min(candidates, key=len), desc
+        return min(candidates2), desc
 
 
-def compute_output_pattern(mask_path, crop_output):
+def compute_output_pattern(mask_path: Path, crop_output):
     """
     Computes the output pattern of the region cropped (without the source file prefix)
     Args:
         mask_path: path to the masks
         crop_output: If True the output is cropped, and the descriptor CropRoi must exist
     Returns:
         the output pattern
     """
-    from os import path
 
-    mask_filename = path.basename(mask_path)
+    mask_filename = mask_path.name
     template_id = mask_filename.split("_")[0].split("-")[1]
     mask_descriptors = mask_filename.split("_")[1:-2:]
     roi_id = mask_filename.split("_")[-2].split("-")[1]
     if "desc-Crop" not in mask_descriptors and crop_output:
         mask_descriptors = ["desc-CropRoi"] + mask_descriptors
     elif "desc-Crop" in mask_descriptors:
         mask_descriptors = [
@@ -412,16 +426,16 @@
     else:
         output_pattern = f"space-{template_id}_{mask_pattern}_roi-{roi_id}"
 
     return output_pattern
 
 
 def extract_roi(
-    nii_path: str,
-    masks_location: str,
+    nii_path: Path,
+    masks_location: Path,
     mask_pattern: str,
     cropped_input: bool,
     roi_names: List[str],
     uncrop_output: bool,
 ) -> List[Tuple[str, torch.Tensor]]:
     """Extracts regions of interest defined by masks
     This function extracts regions of interest from preprocessed nifti images.
@@ -460,15 +474,14 @@
 
 
 def extract_roi_tensor(
     image_tensor: torch.Tensor,
     mask_np,
     uncrop_output: bool,
 ) -> torch.Tensor:
-
     if len(mask_np.shape) == 3:
         mask_np = np.expand_dims(mask_np, axis=0)
     elif len(mask_np.shape) == 4:
         assert mask_np.shape[0] == 1
     else:
         raise ValueError(
             "ROI masks must be 3D or 4D tensors. "
@@ -484,29 +497,31 @@
                 mask_np.any((0, 1, 3)),
                 mask_np.any((0, 1, 2)),
             )
         ]
     return roi_tensor.float().clone()
 
 
-def extract_roi_path(img_path: str, mask_path: str, uncrop_output: bool) -> str:
-    input_img_filename = path.basename(img_path)
+def extract_roi_path(img_path: Path, mask_path: Path, uncrop_output: bool) -> str:
+    input_img_filename = img_path.name
 
     sub_ses_prefix = "_".join(input_img_filename.split("_")[0:3:])
     if not sub_ses_prefix.endswith("_T1w"):
         sub_ses_prefix = "_".join(input_img_filename.split("_")[0:2:])
     input_suffix = input_img_filename.split("_")[-1].split(".")[0]
 
     output_pattern = compute_output_pattern(mask_path, not uncrop_output)
 
     return f"{sub_ses_prefix}_{output_pattern}_{input_suffix}.pt"
 
 
 TEMPLATE_DICT = {
     "t1-linear": "MNI152NLin2009cSym",
     "pet-linear": "MNI152NLin2009cSym",
+    "flair-linear": "MNI152NLin2009cSym",
 }
 
 PATTERN_DICT = {
     "t1-linear": "res-1x1x1",
     "pet-linear": "res-1x1x1",
+    "flair-linear": "res-1x1x1",
 }
```

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_linear/cli.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from pathlib import Path
+
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="t1-linear", no_args_is_help=True)
 @cli_param.argument.caps_directory
 @click.argument(
     "output_tsv",
-    type=str,
+    type=click.Path(path_type=Path),
 )
 @cli_param.option.participant_list
 @click.option(
     "--threshold",
     type=float,
     default=0.5,
     show_default=True,
```

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_linear/models.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_linear/quality_check.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/quality_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """
 This file contains all methods needed to perform the quality check procedure after t1-linear preprocessing.
 """
 from logging import getLogger
-from os import makedirs
-from os.path import abspath, dirname, exists, join
 from pathlib import Path
 
 import pandas as pd
 import torch
 from clinica.utils.inputs import RemoteFileStructure, fetch_file
 from torch.utils.data import DataLoader
-from torchvision.models import ResNet18_Weights, resnet18
 
 from clinicadl.generate.generate_utils import load_and_check_tsv
 from clinicadl.utils.caps_dataset.data import CapsDataset
 from clinicadl.utils.exceptions import ClinicaDLArgumentError
 
 from .models import resnet_darq_qc_18 as darq_r18
 from .models import resnet_deep_qc_18 as deep_r18
 from .models import squeezenet_qc as darq_sq101
 from .utils import QCDataset
 
+logger = getLogger("clinicadl.quality-check")
+
 
 def quality_check(
-    caps_dir: str,
-    output_path: str,
-    tsv_path: str = None,
+    caps_dir: Path,
+    output_path: Path,
+    tsv_path: Path = None,
     threshold: float = 0.5,
     batch_size: int = 1,
     n_proc: int = 0,
     gpu: bool = True,
     network: str = "darq",
     use_tensor: bool = False,
     use_uncropped_image: bool = True,
@@ -58,24 +57,24 @@
     use_uncropped_image: bool
         To use uncropped images instead of the cropped ones.
 
     """
 
     logger = getLogger("clinicadl.quality_check")
 
-    if not output_path.endswith(".tsv"):
+    if not output_path.suffix == ".tsv":
         raise ClinicaDLArgumentError(f"Output path {output_path} must be a TSV file.")
 
     # Fetch QC model
-    home = str(Path.home())
+    home = Path.home()
 
-    cache_clinicadl = join(home, ".cache", "clinicadl", "models")
+    cache_clinicadl = home / ".cache" / "clinicadl" / "models"
     url_aramis = "https://aramislab.paris.inria.fr/files/data/models/dl/qc/"
 
-    makedirs(cache_clinicadl, exist_ok=True)
+    cache_clinicadl.mkdir(parents=True, exist_ok=True)
 
     if network == "deep_qc":
         FILE1 = RemoteFileStructure(
             filename="resnet18.pth.tar",
             url=url_aramis,
             checksum="a97a781be3820b06424fe891ec405c78b87ad51a27b6b81614dbdb996ce60104",
         )
@@ -95,19 +94,19 @@
         FILE1 = RemoteFileStructure(
             filename="sq101_darq.pth",
             url=url_aramis,
             checksum="1f4f3ebd20aaa726d634165a89df12461d9b7c6f2f45931bd29d16cf2616d00f",
         )
         model = darq_sq101()
 
-    model_file = join(cache_clinicadl, FILE1.filename)
+    model_file = cache_clinicadl / FILE1.filename
 
     logger.info("Downloading quality check model.")
 
-    if not (exists(model_file)):
+    if not (model_file.is_file()):
         try:
             model_file = fetch_file(FILE1, cache_clinicadl)
         except IOError as err:
             print("Unable to download required model for QC process:", err)
 
     # Load QC model
     logger.debug("Loading quality check model.")
@@ -119,15 +118,15 @@
 
     with torch.no_grad():
         # Transform caps_dir in dict
         caps_dict = CapsDataset.create_caps_dict(caps_dir, multi_cohort=False)
 
         # Load DataFrame
         logger.debug("Loading data to check.")
-        df = load_and_check_tsv(tsv_path, caps_dict, dirname(abspath(output_path)))
+        df = load_and_check_tsv(tsv_path, caps_dict, output_path.resolve().parent)
 
         dataset = QCDataset(caps_dir, df, use_tensor, use_uncropped_image)
         dataloader = DataLoader(
             dataset, num_workers=n_proc, batch_size=batch_size, pin_memory=True
         )
 
         columns = ["participant_id", "session_id", "pass_probability", "pass"]
```

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_linear/utils.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_linear/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """
 Copied from https://github.com/vfonov/darq
 """
 
-from os import path
+from pathlib import Path
 
 import nibabel as nib
 import torch
 from clinica.utils.input_files import T1W_LINEAR, T1W_LINEAR_CROPPED
 from clinica.utils.inputs import clinica_file_reader
 from torch.utils.data import Dataset
 
 from clinicadl.prepare_data.prepare_data_utils import compute_folder_and_file_type
 
 
 class QCDataset(Dataset):
     """Dataset of MRI organized in a CAPS folder."""
 
     def __init__(
-        self, img_dir, data_df, use_extracted_tensors=False, use_uncropped_image=True
+        self,
+        img_dir: Path,
+        data_df,
+        use_extracted_tensors=False,
+        use_uncropped_image=True,
     ):
         """
         Args:
             img_dir (string): Directory of all the images.
             data_df (DataFrame): Subject and session list.
 
         """
@@ -32,15 +36,15 @@
         self.use_extracted_tensors = use_extracted_tensors
         self.use_uncropped_image = use_uncropped_image
 
         if ("session_id" not in list(self.df.columns.values)) or (
             "participant_id" not in list(self.df.columns.values)
         ):
             raise Exception(
-                "the data file is not in the correct format."
+                "The data file is not in the correct format."
                 "Columns should include ['participant_id', 'session_id']"
             )
 
         self.normalization = MinMaxNormalization()
 
         self.preprocessing_dict = {
             "preprocessing": "t1-linear",
@@ -56,37 +60,34 @@
     def __getitem__(self, idx):
         subject = self.df.loc[idx, "participant_id"]
         session = self.df.loc[idx, "session_id"]
 
         if self.use_extracted_tensors:
             file_type = self.preprocessing_dict["file_type"]
             file_type["pattern"] = file_type["pattern"].replace(".nii.gz", ".pt")
-            image_path_list = clinica_file_reader(
-                [subject],
-                [session],
-                self.img_dir,
-                file_type,
-            )
-            image_filename = path.basename(image_path_list[0][0])
+            image_output = clinica_file_reader(
+                [subject], [session], self.img_dir, file_type
+            )[0]
+            image_path = Path(image_output[0])
+            image_filename = image_path.name
             folder, _ = compute_folder_and_file_type(self.preprocessing_dict)
-            image_dir = path.join(
-                self.img_dir,
-                "subjects",
-                subject,
-                session,
-                "deeplearning_prepare_data",
-                "image_based",
-                folder,
+            image_dir = (
+                self.img_dir
+                / "subjects"
+                / subject
+                / session
+                / "deeplearning_prepare_data"
+                / "image_based"
+                / folder
             )
 
-            image_path = path.join(image_dir, image_filename)
+            image_path = image_dir / image_filename
             image = torch.load(image_path)
             image = self.pt_transform(image)
         else:
-
             image_path = clinica_file_reader(
                 [subject],
                 [session],
                 self.img_dir,
                 T1W_LINEAR if self.use_uncropped_image else T1W_LINEAR_CROPPED,
             )[0]
             image = nib.load(image_path[0])
@@ -190,15 +191,14 @@
         for i in range(3):
             # try the dimension of input_image[i]
             # rotate the slice with 90 degree, I don't know why, but read from
             # nifti file, the img has been rotated, thus we do not have the same
             # direction with the pretrained model
 
             if len(input_images[i].shape) == 3:
-
                 slice = np.reshape(
                     input_images[i],
                     (input_images[i].shape[0], input_images[i].shape[1]),
                 )
             else:
                 slice = input_images[i]
```

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_volume/cli.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_volume/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from pathlib import Path
+
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="t1-volume", no_args_is_help=True)
 @cli_param.argument.caps_directory
 @click.argument(
     "output_directory",
-    type=str,
+    type=click.Path(path_type=Path),
 )
 @click.argument(
     "group_label",
     type=str,
 )
 def cli(
     caps_directory,
```

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_volume/quality_check.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_volume/quality_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 """
 Automatically reject images incorrectly preprocessed by t1-volume (Unified Segmentation) with 3 criterion
 1) max < 0.95
 2) percentage of non zero values < 15 % or > 50 %
 3) frontal similarity of T1 volume with the template < 0.40
 """
 from logging import getLogger
-from os import path
+from pathlib import Path
 
 import pandas as pd
 
 from .utils import extract_metrics
 
 
-def quality_check(caps_dir, output_directory, group_label):
-
+def quality_check(caps_dir: Path, output_directory: Path, group_label):
     logger = getLogger("clinicadl.quality_check")
 
     extract_metrics(
         caps_dir=caps_dir, output_dir=output_directory, group_label=group_label
     )
     logger.info(
-        f"Quality check metrics extracted at {path.join(output_directory, 'QC_metrics.tsv')}."
+        f"Quality check metrics extracted at {output_directory / 'QC_metrics.tsv'}."
     )
-    qc_df = pd.read_csv(path.join(output_directory, "QC_metrics.tsv"), sep="\t")
+    qc_df = pd.read_csv(output_directory / "QC_metrics.tsv", sep="\t")
 
     rejection1_df = qc_df[qc_df.max_intensity > 0.95]
-    rejection1_df.to_csv(
-        path.join(output_directory, "pass_step-1.tsv"), sep="\t", index=False
-    )
+    rejection1_df.to_csv(output_directory / "pass_step-1.tsv", sep="\t", index=False)
     logger.info(
-        f"Number of sessions removed based on max intensity: {len(qc_df) - len(rejection1_df)}."
+        f"Number of sessions removed, based on max intensity: {len(qc_df) - len(rejection1_df)}."
     )
     logger.debug(f"{rejection1_df}")
 
     rejection2_df = rejection1_df[
         (rejection1_df.non_zero_percentage < 0.5)
         & (rejection1_df.non_zero_percentage > 0.15)
     ]
-    rejection2_df.to_csv(
-        path.join(output_directory, "pass_step-2.tsv"), sep="\t", index=False
-    )
+    rejection2_df.to_csv(output_directory / "pass_step-2.tsv", sep="\t", index=False)
     logger.info(
         f"Number of sessions removed based on non-zero voxels: {len(rejection1_df) - len(rejection2_df)}."
     )
     logger.debug(f"{rejection2_df}")
 
     rejection3_df = rejection2_df[rejection2_df.frontal_similarity > 0.10]
-    rejection3_df.to_csv(
-        path.join(output_directory, "pass_step-3.tsv"), sep="\t", index=False
-    )
+    rejection3_df.to_csv(output_directory / "pass_step-3.tsv", sep="\t", index=False)
     logger.info(
         f"Number of sessions removed based on frontal similarity with DARTEL "
         f"template: {len(rejection2_df) - len(rejection3_df)}."
     )
     logger.debug(f"{rejection3_df}")
```

### Comparing `clinicadl-1.2.0/clinicadl/quality_check/t1_volume/utils.py` & `clinicadl-1.3.0/clinicadl/quality_check/t1_volume/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 """
 Produces a tsv file to study all the nii files and perform the quality check.
 """
-import os
-from os import path
+
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
 import pandas as pd
 from clinica.utils.inputs import RemoteFileStructure, fetch_file
 
 
-def extract_metrics(caps_dir, output_dir, group_label):
-    if not path.exists(output_dir):
-        os.makedirs(output_dir)
+def extract_metrics(caps_dir: Path, output_dir: Path, group_label):
+    if not output_dir.is_dir():
+        output_dir.mkdir(parents=True)
 
     # Load eyes segmentation
-    home = str(Path.home())
-    cache_clinicadl = path.join(home, ".cache", "clinicadl", "segmentation")
+    home = Path.home()
+    cache_clinicadl = home / ".cache" / "clinicadl" / "segmentation"
     url_aramis = "https://aramislab.paris.inria.fr/files/data/template/"
     FILE1 = RemoteFileStructure(
         filename="eyes_segmentation.nii.gz",
         url=url_aramis,
         checksum="56f699c06cafc62ad8bb5b41b188c7c412d684d810a11d6f4cbb441c0ce944ee",
     )
 
-    if not (path.exists(cache_clinicadl)):
-        os.makedirs(cache_clinicadl)
+    if not cache_clinicadl.is_dir():
+        cache_clinicadl.mkdir(parents=True)
 
-    segmentation_file = path.join(cache_clinicadl, FILE1.filename)
+    segmentation_file = cache_clinicadl / FILE1.filename
 
-    if not (path.exists(segmentation_file)):
+    if not segmentation_file.is_file():
         try:
             segmentation_file = fetch_file(FILE1, cache_clinicadl)
         except IOError as err:
             raise IOError("Unable to download required eyes segmentation for QC:", err)
 
     segmentation_nii = nib.load(segmentation_file)
     segmentation_np = segmentation_nii.get_fdata()
 
     # Get the GM template
-    template_path = path.join(
-        caps_dir,
-        "groups",
-        f"group-{group_label}",
-        "t1",
-        f"group-{group_label}_template.nii.gz",
+    template_path = (
+        caps_dir
+        / "groups"
+        / f"group-{group_label}"
+        / "t1"
+        / f"group-{group_label}_template.nii.gz"
     )
     template_nii = nib.load(template_path)
     template_np = template_nii.get_fdata()
     template_np = np.sum(template_np, axis=3)
     template_segmentation_np = template_np * segmentation_np
 
     # Get the data
-    filename = path.join(output_dir, "QC_metrics.tsv")
+    filename = output_dir / "QC_metrics.tsv"
     columns = [
         "participant_id",
         "session_id",
         "max_intensity",
         "non_zero_percentage",
         "frontal_similarity",
     ]
-    results_df = pd.DataFrame()
+    results_df = pd.DataFrame(columns=columns)
 
-    subjects = os.listdir(path.join(caps_dir, "subjects"))
-    subjects = [subject for subject in subjects if subject[:4:] == "sub-"]
+    subjects = list((caps_dir / "subjects").iterdir())
+    subjects = [subject for subject in subjects if str(subject)[:4:] == "sub-"]
     for subject in subjects:
-        subject_path = path.join(caps_dir, "subjects", subject)
-        sessions = os.listdir(subject_path)
-        sessions = [session for session in sessions if session[:4:] == "ses-"]
+        subject_path = caps_dir / "subjects" / subject
+        sessions = list(subject_path.iterdir())
+        sessions = [session for session in sessions if str(session)[:4:] == "ses-"]
         for session in sessions:
-            image_path = path.join(
-                subject_path,
-                session,
-                "t1",
-                "spm",
-                "segmentation",
-                "normalized_space",
-                subject
+            image_path = (
+                subject_path
+                / session
+                / "t1"
+                / "spm"
+                / "segmentation"
+                / "normalized_space"
+                / subject
                 + "_"
                 + session
-                + "_T1w_segm-graymatter_space-Ixi549Space_modulated-off_probability.nii.gz",
+                + "_T1w_segm-graymatter_space-Ixi549Space_modulated-off_probability.nii.gz"
             )
 
-            if path.exists(image_path):
+            if image_path.is_file():
                 # GM analysis
                 image_nii = nib.load(image_path)
                 image_np = image_nii.get_fdata()
                 image_segmentation_np = image_np * segmentation_np
                 eyes_nmi_value = nmi(
                     occlusion1=template_segmentation_np,
                     occlusion2=image_segmentation_np,
```

### Comparing `clinicadl-1.2.0/clinicadl/random_search/random_search.py` & `clinicadl-1.3.0/clinicadl/random_search/random_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 Launch a random network training.
 """
-
-from os import path
-
-import toml
+from pathlib import Path
 
 from clinicadl.random_search.random_search_utils import get_space_dict, random_sampling
 from clinicadl.train import train
 
 
-def launch_search(launch_directory, job_name):
-
-    if not path.exists(path.join(launch_directory, "random_search.toml")):
+def launch_search(launch_directory: Path, job_name):
+    if not (launch_directory / "random_search.toml").is_file():
         raise FileNotFoundError(
-            f"TOML file 'random_search.toml' must be written in directory {launch_directory}."
+            f"TOML file 'random_search.toml' must be written in directory: {launch_directory}."
         )
     space_options = get_space_dict(launch_directory)
     options = random_sampling(space_options)
 
-    maps_directory = path.join(launch_directory, job_name)
+    maps_directory = launch_directory / job_name
     split = options.pop("split")
     options["architecture"] = "RandomArchitecture"
 
     train(maps_directory, options, split)
```

### Comparing `clinicadl-1.2.0/clinicadl/random_search/random_search_cli.py` & `clinicadl-1.3.0/clinicadl/random_search/random_search_cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from pathlib import Path
+
 import click
 
 
 @click.command("random-search", no_args_is_help=True)
 @click.argument(
     "launch_directory",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
 )
 @click.argument("name", type=str)
 def cli(
     launch_directory,
     name,
 ):
     """Hyperparameter exploration using random search.
```

### Comparing `clinicadl-1.2.0/clinicadl/random_search/random_search_utils.py` & `clinicadl-1.3.0/clinicadl/random_search/random_search_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import random
-from os import path
+from pathlib import Path
 from typing import Any, Dict, Tuple
 
 import toml
 
 from clinicadl.train.train_utils import build_train_dict
 from clinicadl.utils.exceptions import ClinicaDLConfigurationError
+from clinicadl.utils.maps_manager.maps_manager_utils import change_str_to_path
 from clinicadl.utils.preprocessing import read_preprocessing
 
 
-def get_space_dict(launch_directory: str) -> Dict[str, Any]:
+def get_space_dict(launch_directory: Path) -> Dict[str, Any]:
     """Transforms the TOML dictionary in one dimension dictionary."""
-    toml_path = path.join(launch_directory, "random_search.toml")
+    toml_path = launch_directory / "random_search.toml"
     toml_options = toml.load(toml_path)
 
     if "Random_Search" not in toml_options:
         raise ClinicaDLConfigurationError(
             "Category 'Random_Search' must be defined in the random_search.toml file. "
             "All random search arguments AND options must be defined in this category."
         )
 
     space_dict = dict()
     for key in toml_options["Random_Search"]:
         space_dict[key] = toml_options["Random_Search"][key]
 
+    space_dict = change_str_to_path(space_dict)
     # Check presence of mandatory arguments
     mandatory_arguments = [
         "network_task",
         "tsv_path",
         "caps_directory",
         "preprocessing_json",
         "n_convblocks",
@@ -53,48 +55,48 @@
     for option, value in random_search_specific_options.items():
         if option not in space_dict:
             space_dict[option] = value
 
     train_default = build_train_dict(toml_path, space_dict["network_task"])
 
     # Mode and preprocessing
-    preprocessing_json = path.join(
-        space_dict["caps_directory"],
-        "tensor_extraction",
-        space_dict.pop("preprocessing_json"),
+    preprocessing_json = (
+        space_dict["caps_directory"]
+        / "tensor_extraction"
+        / space_dict.pop("preprocessing_json")
     )
 
     preprocessing_dict = read_preprocessing(preprocessing_json)
     train_default["preprocessing_dict"] = preprocessing_dict
     train_default["mode"] = preprocessing_dict["mode"]
 
     space_dict.update(train_default)
 
     return space_dict
 
 
 def sampling_fn(value, sampling_type: str):
     if isinstance(value, (tuple, list)):
-        if sampling_type is "fixed":
+        if sampling_type == "fixed":
             return value
-        elif sampling_type is "choice":
+        elif sampling_type == "choice":
             return random.choice(value)
-        elif sampling_type is "exponent":
+        elif sampling_type == "exponent":
             exponent = random.uniform(*value)
             return 10**-exponent
-        elif sampling_type is "randint":
+        elif sampling_type == "randint":
             return random.randint(*value)
-        elif sampling_type is "uniform":
+        elif sampling_type == "uniform":
             return random.uniform(*value)
         else:
             raise NotImplementedError(
                 f"Sampling type {sampling_type} is not implemented"
             )
     else:
-        if sampling_type is "exponent":
+        if sampling_type == "exponent":
             return 10**-value
         else:
             return value
 
 
 def random_sampling(rs_options: Dict[str, Any]) -> Dict[str, Any]:
     """
```

### Comparing `clinicadl-1.2.0/clinicadl/resources/config/train_config.toml` & `clinicadl-1.3.0/clinicadl/resources/config/train_config.toml`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,8 @@
 optimizer = "Adam"
 epochs = 20
 learning_rate = 1e-4
 weight_decay = 1e-4
 patience = 0
 tolerance = 0.0
 accumulation_steps = 1
+profiler = false
```

### Comparing `clinicadl-1.2.0/clinicadl/train/from_json_cli.py` & `clinicadl-1.3.0/clinicadl/train/from_json_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from logging import getLogger
+from pathlib import Path
 
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="from_json", no_args_is_help=True)
 @click.argument(
     "config_json",
-    type=click.Path(exists=True),
+    type=click.Path(exists=True, path_type=Path),
 )
 @cli_param.argument.output_maps
 @click.option(
     "--split",
     "-s",
     type=int,
     # default=(),
```

### Comparing `clinicadl-1.2.0/clinicadl/train/list_models_cli.py` & `clinicadl-1.3.0/clinicadl/train/list_models_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/train/resume.py` & `clinicadl-1.3.0/clinicadl/train/resume.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 """
 Automatic relaunch of jobs that were stopped before the end of training.
 Unfinished splits are detected as they do not contain a "performances" sub-folder
 """
-import os
+
 from logging import getLogger
-from os import path
+from pathlib import Path
 
 from clinicadl import MapsManager
 
 
 def replace_arg(options, key_name, value):
     if value is not None:
         setattr(options, key_name, value)
 
 
-def automatic_resume(model_path, user_split_list=None, verbose=0):
+def automatic_resume(model_path: Path, user_split_list=None, verbose=0):
     logger = getLogger("clinicadl")
 
     verbose_list = ["warning", "info", "debug"]
     maps_manager = MapsManager(model_path, verbose=verbose_list[verbose])
 
     existing_split_list = maps_manager._find_splits()
     stopped_splits = [
         split
         for split in existing_split_list
-        if "tmp"
-        in os.listdir(path.join(model_path, f"{maps_manager.split_name}-{split}"))
+        if (model_path / f"{maps_manager.split_name}-{split}" / "tmp")
+        in list((model_path / f"{maps_manager.split_name}-{split}").iterdir())
     ]
 
     # Find finished split
     finished_splits = list()
     for split in existing_split_list:
         if split not in stopped_splits:
             performance_dir_list = [
                 performance_dir
-                for performance_dir in os.listdir(
-                    path.join(model_path, f"{maps_manager.split_name}-{split}")
+                for performance_dir in list(
+                    (model_path / f"{maps_manager.split_name}-{split}").iterdir()
                 )
-                if "best-" in performance_dir
+                if "best-" in performance_dir.name
             ]
             if len(performance_dir_list) > 0:
                 finished_splits.append(split)
 
     split_manager = maps_manager._init_split_manager(split_list=user_split_list)
     split_iterator = split_manager.split_iterator()
```

### Comparing `clinicadl-1.2.0/clinicadl/train/resume_cli.py` & `clinicadl-1.3.0/clinicadl/train/resume_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/train/tasks/classification_cli.py` & `clinicadl-1.3.0/clinicadl/train/tasks/classification_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 @train_option.epochs
 @train_option.learning_rate
 @train_option.weight_decay
 @train_option.dropout
 @train_option.patience
 @train_option.tolerance
 @train_option.accumulation_steps
+@train_option.profiler
 # transfer learning
 @train_option.transfer_path
 @train_option.transfer_selection_metric
 # Task-related
 @train_option.label
 @train_option.selection_metrics
 @train_option.selection_threshold
```

### Comparing `clinicadl-1.2.0/clinicadl/train/tasks/reconstruction_cli.py` & `clinicadl-1.3.0/clinicadl/train/tasks/reconstruction_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 @train_option.epochs
 @train_option.learning_rate
 @train_option.weight_decay
 @train_option.dropout
 @train_option.patience
 @train_option.tolerance
 @train_option.accumulation_steps
+@train_option.profiler
 # transfer learning
 @train_option.transfer_path
 @train_option.transfer_selection_metric
 # Task-related
 @train_option.selection_metrics
 @train_option.reconstruction_loss
 def cli(**kwargs):
```

### Comparing `clinicadl-1.2.0/clinicadl/train/tasks/regression_cli.py` & `clinicadl-1.3.0/clinicadl/train/tasks/regression_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 @train_option.epochs
 @train_option.learning_rate
 @train_option.weight_decay
 @train_option.dropout
 @train_option.patience
 @train_option.tolerance
 @train_option.accumulation_steps
+@train_option.profiler
 # transfer learning
 @train_option.transfer_path
 @train_option.transfer_selection_metric
 # Task-related
 @train_option.label
 @train_option.selection_metrics
 @train_option.regression_loss
```

### Comparing `clinicadl-1.2.0/clinicadl/train/tasks/task_utils.py` & `clinicadl-1.3.0/clinicadl/train/tasks/task_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from logging import getLogger
 from typing import List
 
 from clinicadl.utils.caps_dataset.data import CapsDataset
 from clinicadl.utils.preprocessing import read_preprocessing
 
 
@@ -11,28 +10,30 @@
     Common training framework for all tasks
 
     Args:
         network_task: task learnt by the network.
         task_options_list: list of options specific to the task.
         kwargs: other arguments and options for network training.
     """
+    from pathlib import Path
+
     from clinicadl.train.train import train
     from clinicadl.train.train_utils import build_train_dict
 
     logger = getLogger("clinicadl.task_manager")
 
     config_file_name = None
     if kwargs["config_file"]:
-        config_file_name = kwargs["config_file"].name
+        config_file_name = Path(kwargs["config_file"])
     train_dict = build_train_dict(config_file_name, network_task)
 
     # Add arguments
     train_dict["network_task"] = network_task
-    train_dict["caps_directory"] = kwargs["caps_directory"]
-    train_dict["tsv_path"] = kwargs["tsv_directory"]
+    train_dict["caps_directory"] = Path(kwargs["caps_directory"])
+    train_dict["tsv_path"] = Path(kwargs["tsv_directory"])
 
     # Change value in train dict depending on user provided options
     standard_options_list = [
         "accumulation_steps",
         "architecture",
         "baseline",
         "batch_size",
@@ -47,14 +48,15 @@
         "multi_cohort",
         "multi_network",
         "n_proc",
         "n_splits",
         "normalize",
         "optimizer",
         "patience",
+        "profiler",
         "tolerance",
         "transfer_selection_metric",
         "weight_decay",
         "sampler",
         "seed",
         "split",
         "compensation",
@@ -64,33 +66,29 @@
 
     for option in all_options_list:
         if (kwargs[option] is not None and not isinstance(kwargs[option], tuple)) or (
             isinstance(kwargs[option], tuple) and len(kwargs[option]) != 0
         ):
             train_dict[option] = kwargs[option]
     if not train_dict["multi_cohort"]:
-        preprocessing_json = os.path.join(
-            train_dict["caps_directory"],
-            "tensor_extraction",
-            kwargs["preprocessing_json"],
+        preprocessing_json = (
+            train_dict["caps_directory"]
+            / "tensor_extraction"
+            / kwargs["preprocessing_json"]
         )
     else:
         caps_dict = CapsDataset.create_caps_dict(
             train_dict["caps_directory"], train_dict["multi_cohort"]
         )
         json_found = False
         for caps_name, caps_path in caps_dict.items():
-            if os.path.exists(
-                os.path.join(
-                    caps_path, "tensor_extraction", kwargs["preprocessing_json"]
-                )
-            ):
-                preprocessing_json = os.path.join(
-                    caps_path, "tensor_extraction", kwargs["preprocessing_json"]
-                )
+            preprocessing_json = (
+                caps_path / "tensor_extraction" / kwargs["preprocessing_json"]
+            )
+            if preprocessing_json.is_file():
                 logger.info(
                     f"Preprocessing JSON {preprocessing_json} found in CAPS {caps_name}."
                 )
                 json_found = True
         if not json_found:
             raise ValueError(
                 f"Preprocessing JSON {kwargs['preprocessing_json']} was not found for any CAPS "
@@ -105,8 +103,8 @@
     # Add default values if missing
     if (
         preprocessing_dict["mode"] == "roi"
         and "roi_background_value" not in preprocessing_dict
     ):
         preprocessing_dict["roi_background_value"] = 0
 
-    train(kwargs["output_maps_directory"], train_dict, train_dict.pop("split"))
+    train(Path(kwargs["output_maps_directory"]), train_dict, train_dict.pop("split"))
```

### Comparing `clinicadl-1.2.0/clinicadl/train/train_cli.py` & `clinicadl-1.3.0/clinicadl/train/train_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/train/train_option.py` & `clinicadl-1.3.0/clinicadl/train/train_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     type=click.Path(exists=True),
 )
 output_maps = cli_param.argument.output_maps
 # train option
 config_file = click.option(
     "--config_file",
     "-c",
-    type=click.File(),
+    type=click.Path(exists=True),
     help="Path to the TOML or JSON file containing the values of the options needed for training.",
 )
 # Computational
 gpu = cli_param.option_group.computational_group.option(
     "--gpu/--no-gpu",
     type=bool,
     default=None,
@@ -253,14 +253,21 @@
     "--accumulation_steps",
     "-asteps",
     type=int,
     # default=1,
     help="Accumulates gradients during the given number of iterations before performing the weight update "
     "in order to virtually increase the size of the batch.",
 )
+profiler = cli_param.option_group.optimization_group.option(
+    "--profiler/--no-profiler",
+    type=bool,
+    default=None,
+    help="Use `--profiler` to enable Pytorch profiler for the first 30 steps after a short warmup. "
+    "It will make an execution trace and some statistics about the CPU and GPU usage.",
+)
 # transfer learning
 transfer_path = cli_param.option_group.transfer_learning_group.option(
     "-tp",
     "--transfer_path",
     type=click.Path(),
     # default=0.0,
     help="Path of to a MAPS used for transfer learning.",
```

### Comparing `clinicadl-1.2.0/clinicadl/train/train_utils.py` & `clinicadl-1.3.0/clinicadl/train/train_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-import os
+from pathlib import Path
 from typing import Any, Dict
 
 import toml
 
 from clinicadl.utils.exceptions import ClinicaDLConfigurationError
 from clinicadl.utils.maps_manager.maps_manager_utils import (
+    change_str_to_path,
     read_json,
     remove_unused_tasks,
 )
 
 
-def build_train_dict(config_file: str, task: str) -> Dict[str, Any]:
+def build_train_dict(config_file: Path, task: str) -> Dict[str, Any]:
     """
     Read the configuration file given by the user.
     If it is a TOML file, ensures that the format corresponds to the one in resources.
     Args:
         config_file: path to a configuration file (JSON of TOML).
         task: task learnt by the network (example: classification, regression, reconstruction...).
     Returns:
         dictionary of values ready to use for the MapsManager
     """
     if config_file is None:
         # read default values
-        clinicadl_root_dir = os.path.abspath(os.path.join(__file__, "../.."))
-        config_path = os.path.join(
-            clinicadl_root_dir,
-            "resources",
-            "config",
-            "train_config.toml",
+        clinicadl_root_dir = (Path(__file__) / "../..").resolve()
+        config_path = (
+            Path(clinicadl_root_dir) / "resources" / "config" / "train_config.toml"
         )
         config_dict = toml.load(config_path)
         config_dict = remove_unused_tasks(config_dict, task)
-
+        config_dict = change_str_to_path(config_dict)
         train_dict = dict()
         # Fill train_dict from TOML files arguments
         for config_section in config_dict:
             for key in config_dict[config_section]:
                 train_dict[key] = config_dict[config_section][key]
 
-    elif config_file.endswith(".toml"):
+    elif config_file.suffix == ".toml":
         user_dict = toml.load(config_file)
         if "Random_Search" in user_dict:
             del user_dict["Random_Search"]
 
         # read default values
-        clinicadl_root_dir = os.path.abspath(os.path.join(__file__, "../.."))
-        config_path = os.path.join(
-            clinicadl_root_dir,
-            "resources",
-            "config",
-            "train_config.toml",
+        clinicadl_root_dir = (Path(__file__) / "../..").resolve()
+        config_path = (
+            Path(clinicadl_root_dir) / "resources" / "config" / "train_config.toml"
         )
         config_dict = toml.load(config_path)
         # Check that TOML file has the same format as the one in clinicadl/resources/config/train_config.toml
         if user_dict is not None:
+            user_dict = change_str_to_path(user_dict)
             for section_name in user_dict:
                 if section_name not in config_dict:
                     raise ClinicaDLConfigurationError(
                         f"{section_name} section is not valid in TOML configuration file. "
                         f"Please see the documentation to see the list of option in TOML configuration file."
                     )
                 for key in user_dict[section_name]:
@@ -74,22 +70,22 @@
         config_dict = remove_unused_tasks(config_dict, task)
 
         # Fill train_dict from TOML files arguments
         for config_section in config_dict:
             for key in config_dict[config_section]:
                 train_dict[key] = config_dict[config_section][key]
 
-    elif config_file.endswith(".json"):
+    elif config_file.suffix == ".json":
         train_dict = read_json(config_file)
+        train_dict = change_str_to_path(train_dict)
 
     else:
         raise ClinicaDLConfigurationError(
             f"config_file {config_file} should be a TOML or a JSON file."
         )
-
     return train_dict
 
 
 def get_model_list(architecture=None, input_size=None, model_layers=False):
     """
     Print the list of models available in ClinicaDL.
     If --architecture is given, information about how to use this model will be displayed.
@@ -129,15 +125,15 @@
         if dimension == "2D":
             shape_str = "C@HxW,"
         elif dimension == "3D":
             shape_str = "C@DxHxW,"
         elif dimension == "2D or 3D":
             shape_str = "C@HxW or C@DxHxW,"
 
-        shape_str = "\n\tThe input must be in the shape ".expandtabs(4) + shape_str
+        shape_str = f"\n\tThe input must be in the shape {shape_str}".expandtabs(4)
         input_size_str = f" for example input_size can be {input_size}."
 
         task_str = f"\n\tThis model can be used for {' or '.join(model_class.get_task())}.\n".expandtabs(
             4
         )
 
         print(
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/adapt/adapt.py` & `clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import json
-import os
 from logging import getLogger
+from pathlib import Path
 
 import pandas as pd
 
 from clinicadl.utils.exceptions import ClinicaDLArgumentError
 
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.adapt")
 
 
-def concat_files(file_path, df_baseline, df_all):
+def concat_files(file_path: Path, df_baseline, df_all):
     """
     Read a file and concatenates it to the right dataframe (baseline or not).
 
     Parameters
     ----------
     file_path: str (path)
         Path to the TSV file (with "participant_id" and "session_id" in the columns).
     df_baseline: DataFrame
         Dataframe with only baseline sessions.
     df_all: DataFrame
         Dataframe with all sessions.
     """
 
     label_df = pd.read_csv(file_path, sep="\t")
-    if file_path.endswith("baseline.tsv"):
+    if file_path.name.endswith("baseline.tsv"):
         df_baseline = pd.concat([df_baseline, label_df])
-    elif file_path.endswith(".tsv"):
+    elif file_path.name.endswith(".tsv"):
         df_all = pd.concat([df_all, label_df])
     return df_all, df_baseline
 
 
-def adapt(old_tsv_dir: str, new_tsv_dir: str, subset_name="labels", labels_list="AD"):
+def adapt(old_tsv_dir: Path, new_tsv_dir: Path, subset_name="labels", labels_list="AD"):
     """
     Produces a new split/kfold directories that fit with clinicaDL 1.2.0.
 
     Parameters
     ----------
     old_tsv_dir: str (path)
         Path to the old directory.
@@ -44,79 +44,74 @@
     subset_name: str
         Name of the output file of `clinicadl get-labels`.
     labels_list: list of str
         list of labels (in the old way, each labels had its own TSV file).
 
     """
 
-    if not os.path.exists(old_tsv_dir):
+    if not old_tsv_dir.is_dir():
         raise ClinicaDLArgumentError(
             f"the directory: {old_tsv_dir} doesn't exists"
             "Please give an existing path"
         )
-    if not os.path.exists(new_tsv_dir):
-        os.makedirs(new_tsv_dir, exist_ok=True)
+    if not new_tsv_dir.is_dir():
+        new_tsv_dir.mkdir(parents=True, exist_ok=True)
 
-    files_list = os.listdir(old_tsv_dir)
+    files_list = list(old_tsv_dir.iterdir())
 
     df_baseline = pd.DataFrame()
     df_all = pd.DataFrame()
 
     for file in files_list:
-        path = os.path.join(old_tsv_dir, file)
-        if os.path.isfile(path) and path.endswith(".tsv"):
+        path = old_tsv_dir / file
+        if path.is_file() and path.name.endswith(".tsv"):
             df_all, df_baseline = concat_files(path, df_baseline, df_all)
 
     if not df_all.empty:
-        df_all.to_csv(os.path.join(new_tsv_dir, subset_name + ".tsv"), sep="\t")
+        df_all.to_csv(new_tsv_dir / subset_name + ".tsv", sep="\t")
     if not df_baseline.empty:
-        df_baseline.to_csv(
-            os.path.join(new_tsv_dir, subset_name + "_baseline.tsv"), sep="\t"
-        )
+        df_baseline.to_csv(new_tsv_dir / subset_name + "_baseline.tsv", sep="\t")
 
     if "split.json" in files_list:
-        new_split_dir = os.path.join(new_tsv_dir, "split")
-        with open(os.path.join(old_tsv_dir, "split.json"), "r") as f:
+        new_split_dir = new_tsv_dir / "split"
+        with (old_tsv_dir / "split.json").open(mode="r") as f:
             parameters_split = json.load(f)
         subset_name = parameters_split["subset_name"]
         adapt(
-            os.path.join(old_tsv_dir, subset_name),
+            old_tsv_dir / subset_name,
             new_split_dir,
             subset_name,
             labels_list,
         )
-        adapt(os.path.join(old_tsv_dir, "train"), new_split_dir, "train", labels_list)
+        adapt(old_tsv_dir / "train", new_split_dir, "train", labels_list)
 
     if "kfold.json" in files_list:
-        with open(os.path.join(old_tsv_dir, "kfold.json"), "r") as f:
+        with (old_tsv_dir / "kfold.json").open(mode="r") as f:
             parameters_kfold = json.load(f)
 
         subset_name = parameters_kfold["subset_name"]
         n_splits = parameters_kfold["n_splits"]
 
-        new_fold_dir = os.path.join(new_tsv_dir, str(n_splits) + "_fold")
-        os.makedirs(new_fold_dir)
+        new_fold_dir = new_tsv_dir / (str(n_splits) + "_fold")
+        new_fold_dir.mkdir(parents=True)
 
         for i in range(n_splits):
-            new_kfold_dir = os.path.join(
-                new_tsv_dir, str(n_splits) + "_fold", "split-" + str(i)
+            new_kfold_dir = (
+                new_tsv_dir / (str(n_splits) + "_fold") / ("split-" + str(i))
             )
+
             adapt(
-                os.path.join(
-                    old_tsv_dir, "train_splits-" + str(n_splits), "split-" + str(i)
-                ),
+                old_tsv_dir / ("train_splits-" + str(n_splits)) / ("split-" + str(i)),
                 new_kfold_dir,
                 "train",
                 labels_list,
             )
             adapt(
-                os.path.join(
-                    old_tsv_dir,
-                    subset_name + "_splits-" + str(n_splits),
-                    "split-" + str(i),
-                ),
+                old_tsv_dir
+                / (subset_name + "_splits-" + str(n_splits))
+                / ("split-" + str(i)),
                 new_kfold_dir,
                 subset_name,
                 labels_list,
             )
 
     logger.info(f"New directory was created at {new_tsv_dir}")
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/adapt/adapt_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/adapt/adapt_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,19 @@
     to the last version.
 
     OLD_TSV_DIR is the output directory of the split/kfold pipeline that contains all the TSV files with clinicaDL 1.1.1 and earlier versions.
 
     Results are stored in NEW_TSV_DIR.
     """
 
-    import os
-
     from clinicadl.utils.exceptions import ClinicaDLArgumentError
 
     from .adapt import adapt
 
-    if os.path.exists(new_tsv_dir):
+    if new_tsv_dir.is_dir():
         raise ClinicaDLArgumentError(
             f"\nThe directory: {new_tsv_dir} already exists.\n"
             "Please give another path for the new tsv directory."
         )
 
     adapt(old_tsv_dir=old_tsv_dir, new_tsv_dir=new_tsv_dir, labels_list=labels_list)
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/analysis/analysis.py` & `clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 # coding: utf-8
 
-import os
 from copy import copy
 from logging import getLogger
-from os import path
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from clinicadl.utils.exceptions import ClinicaDLArgumentError, ClinicaDLTSVError
 from clinicadl.utils.tsvtools_utils import (
     add_demographics,
     cleaning_nan_diagnoses,
     find_label,
     first_session,
     merged_tsv_reader,
     next_session,
 )
 
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.analysis")
 
 
-def demographics_analysis(merged_tsv, data_tsv, results_tsv, diagnoses):
+def demographics_analysis(
+    merged_tsv: Path, data_tsv: Path, results_tsv: Path, diagnoses
+):
     """
     Produces a tsv file with rows corresponding to the labels defined by the diagnoses list,
     and the columns being demographic statistics.
 
-    Writes one tsv file at results_tsv containing the demographic analysis of the tsv files in data_tsv.
+    Writes one tsv file at results_tsv, containing the demographic analysis of the tsv files in data_tsv.
 
     Parameters
     ----------
     merged_tsv: str (path)
         Path to the file obtained by the command clinica iotools merge-tsv.
     data_tsv: str (path)
         Path to the folder containing data extracted by clinicadl tsvtool get-labels.
     results_tsv: str (path)
         Path to the output tsv file (filename included).
     diagnoses: list of str
         Labels selected for the demographic analysis.
 
     """
 
-    if not path.exists(data_tsv):
+    if not data_tsv.is_file():
         raise ClinicaDLTSVError(f"{data_tsv} file was not found. ")
 
-    if not path.exists(merged_tsv):
+    if not merged_tsv.is_file():
         raise ClinicaDLTSVError(f"{merged_tsv} file was not found. ")
     merged_df = pd.read_csv(merged_tsv, sep="\t")
     merged_df.set_index(["participant_id", "session_id"], inplace=True)
     merged_df = cleaning_nan_diagnoses(merged_df)
 
-    parent_directory = path.abspath(path.join(results_tsv, os.pardir))
-    os.makedirs(parent_directory, exist_ok=True)
+    parent_directory = results_tsv.resolve().parent
+    parent_directory.mkdir(parents=True, exist_ok=True)
 
     fields_dict = {
         "age": find_label(merged_df.columns.values, "age"),
         "sex": find_label(merged_df.columns.values, "sex"),
         "MMSE": find_label(merged_df.columns.values, "mms"),
         "CDR": "cdr_global",
     }
@@ -114,14 +115,16 @@
 
                     feature_absence = isinstance(
                         merged_df.loc[(subject, first_session_id), "diagnosis"], float
                     )
                 demographics_subject_df = merged_df.loc[subject]
 
                 # Extract features
+                logger.debug(f"extract features for subject {subject}")
+
                 results_df.loc[diagnosis, "n_subjects"] += 1
                 results_df.loc[diagnosis, "n_scans"] += len(subject_df)
                 diagnosis_dict[diagnosis]["age"].append(
                     merged_df.loc[(subject, first_session_id), fields_dict["age"]]
                 )
                 diagnosis_dict[diagnosis]["MMSE"].append(
                     merged_df.loc[(subject, first_session_id), fields_dict["MMSE"]]
@@ -166,14 +169,16 @@
                 else:
                     tt = 3  # warn(f"Patient {subject} has CDR {cdr}")
         else:
             raise ClinicaDLArgumentError(
                 f"There is no subject with diagnosis {diagnosis}"
             )
     for diagnosis in diagnoses:
+        logger.debug(f"compute stats for diagnosis {diagnosis}")
+
         results_df.loc[diagnosis, "mean_age"] = np.nanmean(
             diagnosis_dict[diagnosis]["age"]
         )
         results_df.loc[diagnosis, "std_age"] = np.nanstd(
             diagnosis_dict[diagnosis]["age"]
         )
         results_df.loc[diagnosis, "min_age"] = np.nanmin(
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/analysis/analysis_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/analysis/analysis_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_labels/get_labels.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,48 +8,47 @@
 
 NB: Other preprocessing may be needed on the merged file obtained: for example the selection of subjects older than 62
 in the OASIS dataset is not done in this script. Moreover a quality check may be needed at the end of preprocessing
 pipelines, leading to the removal of some subjects.
 """
 from copy import copy
 from logging import getLogger
-from os import path
+from pathlib import Path
 from typing import Dict, List
 
 import numpy as np
 import pandas as pd
 
 from clinicadl.utils.exceptions import ClinicaDLArgumentError, ClinicaDLTSVError
 from clinicadl.utils.maps_manager.iotools import commandline_to_json
 from clinicadl.utils.tsvtools_utils import (
     cleaning_nan_diagnoses,
     find_label,
     first_session,
     last_session,
-    merged_tsv_reader,
     neighbour_session,
 )
 
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.get_labels")
 
 
 def infer_or_drop_diagnosis(bids_df: pd.DataFrame) -> pd.DataFrame:
     """
     Deduce the diagnosis when missing from previous and following sessions of the subject. If not identical, the session
     is dropped. Sessions with no diagnosis are also dropped when there are the last sessions of the follow-up.
 
     Parameters
     ----------
     bids_df: DataFrame
-        Columns including ['participant_id', 'session_id', 'diagnosis']
+        Columns including ['participant_id', 'session_id', 'diagnosis'].
 
     Returns
     -------
     bids_copy_df: DataFrame
-        Cleaned copy of the input bids_df
+        Cleaned copy of the input bids_df.
     """
     bids_copy_df = copy(bids_df)
     found_diag_interpol = 0
     nb_drop = 0
 
     for subject, subject_df in bids_df.groupby(level=0):
         session_list = []
@@ -158,15 +157,14 @@
     bids_copy_df: DataFrame
         Cleaned copy of the input bids_df
     """
     bids_copy_df = copy(bids_df)
     nb_unique = 0
 
     for subject, subject_df in bids_df.groupby(level=0):
-
         session_list = [session for _, session in subject_df.index.values]
         session_list.sort()
         nb_session = len(session_list)
         if nb_session == 1:
             bids_copy_df.drop((subject, session_list[0]), inplace=True)
             subject_df.drop((subject, session_list[0]), inplace=True)
             nb_unique += 1
@@ -192,25 +190,25 @@
         Cleaned copy of the input bids_df
 
     """
 
     output_df = copy(bids_df)
     nb_subjects = 0
     for subject, subject_df in bids_df.groupby(level=0):
-        for (_, session) in subject_df.index.values:
+        for _, session in subject_df.index.values:
             group = subject_df.loc[(subject, session), "diagnosis"]
             if group not in diagnosis_list:
                 output_df.drop((subject, session), inplace=True)
                 nb_subjects += 1
 
     logger.info(f"Dropped subjects (diagnoses): {nb_subjects}")
     return output_df
 
 
-def apply_restriction(bids_df: pd.DataFrame, restriction_path: str) -> pd.DataFrame:
+def apply_restriction(bids_df: pd.DataFrame, restriction_path: Path) -> pd.DataFrame:
     """
     Application of a restriction (for example after the removal of some subjects after a preprocessing pipeline)
 
     Parameters
     ----------
     bids_df: DataFrame
         Columns must include ['participant_id', 'session_id', 'diagnosis']
@@ -237,23 +235,24 @@
                 bids_copy_df.drop((subject, session), inplace=True)
                 nb_subjects += 1
     logger.info(f"Dropped subjects (apply restriction): {nb_subjects}")
     return bids_copy_df
 
 
 def get_labels(
-    bids_directory: str,
+    bids_directory: Path,
     diagnoses: List[str],
     modality: str = "t1w",
-    restriction_path: str = None,
+    restriction_path: Path = None,
     variables_of_interest: List[str] = None,
     remove_smc: bool = True,
-    merged_tsv: str = None,
-    missing_mods: str = None,
+    merged_tsv: Path = None,
+    missing_mods: Path = None,
     remove_unique_session: bool = False,
+    output_dir: Path = None,
 ):
     """
     Writes one TSV file based on merged_tsv and missing_mods.
 
 
     Parameters
     ----------
@@ -273,19 +272,26 @@
         Path to a folder of a older of a CAPS compliant dataset
     merged_tsv: str (path)
         Path to the output of clinica iotools merge-tsv if already exists
     missing_mods: str (path)
         Path to the output directory of clinica iotools check-missing-modalities if already exists
     remove_unique_session: bool
         If True, subjects with only one session are removed.
+    output_dir: str (path)
+        Path to the directory where the output labels.tsv will be stored.
     """
 
-    from pathlib import Path
+    from clinica.utils.inputs import check_bids_folder
+
+    if not output_dir.suffix == "tsv":
+        results_directory = bids_directory.parents[0]
+        output_tsv = results_directory / "labels.tsv"
+    else:
+        results_directory = output_dir
 
-    results_directory = Path(bids_directory).parents[0]
     output_tsv = results_directory / "labels.tsv"
 
     commandline_to_json(
         {
             "bids_directory": bids_directory,
             "output_dir": results_directory,
             "diagnoses": diagnoses,
@@ -296,48 +302,44 @@
             "missing_mods": missing_mods,
             "merged_tsv": merged_tsv,
             "remove_unique_session": remove_unique_session,
         },
         filename="labels.json",
     )
 
-    import os
-
-    from clinica.iotools.utils.data_handling import (
-        compute_missing_mods,
-        create_merge_file,
-    )
-    from clinica.utils.inputs import check_bids_folder
-
     # Create the results directory
-    os.makedirs(results_directory, exist_ok=True)
+    results_directory.mkdir(parents=True, exist_ok=True)
 
     # Generating the output of `clinica iotools check-missing-modalities``
-    missing_mods_directory = os.path.join(results_directory, "missing_mods")
+    missing_mods_directory = results_directory / "missing_mods"
     if missing_mods is not None:
         missing_mods_directory = missing_mods
 
-    if not os.path.exists(missing_mods_directory):
+    if not missing_mods_directory.is_dir():
+        from clinica.iotools.utils.data_handling import compute_missing_mods
+
         check_bids_folder(bids_directory)
         compute_missing_mods(bids_directory, missing_mods_directory, "missing_mods")
 
     logger.info(
         f"output of clinica iotools check-missing-modalities: {missing_mods_directory}"
     )
 
     # Generating the output of `clinica iotools merge-tsv `
-    merged_tsv_path = os.path.join(results_directory, "merged.tsv")
+    merged_tsv_path = results_directory / "merged.tsv"
     if merged_tsv is not None:
         merged_tsv_path = merged_tsv
-    elif not os.path.exists(merged_tsv_path):
+    elif not merged_tsv_path.is_file():
+        from clinica.iotools.utils.data_handling import create_merge_file
+
         logger.info("create merge tsv")
         check_bids_folder(bids_directory)
         create_merge_file(
             bids_directory,
-            os.path.join(results_directory, "merged.tsv"),
+            results_directory / "merged.tsv",
             caps_dir=None,
             pipelines=None,
             ignore_scan_files=None,
             ignore_sessions_files=None,
             volume_atlas_selection=None,
             freesurfer_atlas_selection=None,
             pvc_restriction=None,
@@ -345,15 +347,15 @@
             group_selection=False,
             tracers_selection=False,
         )
 
     logger.info(f"output of clinica iotools merge-tsv: {merged_tsv_path}")
 
     # Reading files
-    if not path.exists(merged_tsv_path):
+    if not merged_tsv_path.is_file():
         raise ClinicaDLTSVError(f"{merged_tsv_path} file was not found. ")
     bids_df = pd.read_csv(merged_tsv_path, sep="\t")
     bids_df.set_index(["participant_id", "session_id"], inplace=True)
     variables_list = []
 
     if "dx1" in bids_df.columns:
         bids_df.rename(columns={"dx1": "diagnosis"}, inplace=True)
@@ -364,40 +366,40 @@
         variables_list.append(find_label(bids_df.columns.values, "diagnosis"))
     except ValueError:
         logger.warning(
             "The age, sex or diagnosis values were not found in the dataset."
         )
 
     # Cleaning NaN diagnosis
+    logger.debug("Cleaning NaN diagnosis")
     bids_df = cleaning_nan_diagnoses(bids_df)
 
     # Checking the variables of interest
     if variables_of_interest is not None:
         variables_set = set(variables_of_interest) | set(variables_list)
         variables_list = list(variables_set)
         if not set(variables_list).issubset(set(bids_df.columns.values)):
             raise ClinicaDLArgumentError(
                 f"The variables asked by the user {variables_of_interest} do not "
                 f"exist in the data set."
             )
 
     # Loading missing modalities files
-    list_files = os.listdir(missing_mods_directory)
+    list_files = list(missing_mods_directory.iterdir())
     missing_mods_dict = {}
 
     for file in list_files:
-        filename, fileext = path.splitext(file)
+        fileext = file.suffix
+        filename = file.stem
         if fileext == ".tsv":
             session = filename.split("_")[-1]
-            missing_mods_df = pd.read_csv(
-                path.join(missing_mods_directory, file), sep="\t"
-            )
+            missing_mods_df = pd.read_csv(missing_mods_directory / file, sep="\t")
             if len(missing_mods_df) == 0:
                 raise ClinicaDLTSVError(
-                    f"Given TSV file at {path.join(missing_mods_directory, file)} loads an empty DataFrame."
+                    f"Given TSV file at {missing_mods_directory /file} loads an empty DataFrame."
                 )
 
             missing_mods_df.set_index("participant_id", drop=True, inplace=True)
             missing_mods_dict[session] = missing_mods_df
 
     # Remove SMC patients
     if remove_smc:
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_labels/get_labels_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_labels/get_labels_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-from typing import List
+from pathlib import Path
 
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="get-labels", no_args_is_help=True)
 @cli_param.argument.bids_directory
+@cli_param.argument.results_tsv
 @cli_param.option.diagnoses
 @cli_param.option.modality
 @cli_param.option.variables_of_interest
 @click.option(
     "--restriction_tsv",
     help="Path to a TSV file containing the sessions that can be included.",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 @click.option(
     "--keep_smc",
     help="This flag allows to keep SMC participants, else they are removed.",
     type=bool,
     default=False,
     is_flag=True,
 )
 @click.option(
     "--merged_tsv",
     help="Path to a TSV file containing the results of clinica iotools merge-tsv command if different of results_directory/merged.tsv",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 @click.option(
     "--missing_mods",
     help="Path to a directory containing the results of clinica iotools missing-modalities command if different of results_directory/missing_mods/",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 @click.option(
     "--remove_unique_session",
     help="This flag allows to remove subjects with a unique session, else they are kept.",
     type=bool,
     default=False,
     is_flag=True,
 )
 def cli(
     bids_directory,
+    results_tsv,
     diagnoses,
     modality,
     restriction_tsv,
     variables_of_interest,
     keep_smc,
     missing_mods,
     merged_tsv,
@@ -56,14 +58,15 @@
     """Get labels in a tsv file.
 
     This command executes the two following commands:
         - `clinica iotools merge-tsv`
         - `clinica iotools check-missing-modalities`
 
     BIDS_DIRECTORY is the path to the BIDS directory.
+    RESULTS_TSV is the path (including the name of the file) where the results will be save
 
     Defaults diagnoses are CN and AD.
 
     Outputs are stored in OUTPUT_TSV.
     """
     from .get_labels import get_labels
 
@@ -76,12 +79,13 @@
         modality=modality,
         restriction_path=restriction_tsv,
         variables_of_interest=variables_of_interest,
         remove_smc=not keep_smc,
         missing_mods=missing_mods,
         merged_tsv=merged_tsv,
         remove_unique_session=remove_unique_session,
+        output_dir=results_tsv,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_labels/old_get_labels_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import List
+from pathlib import Path
 
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="getlabels", no_args_is_help=True)
 @cli_param.argument.bids_directory
 @cli_param.option.diagnoses
 @cli_param.option.modality
 @cli_param.option.variables_of_interest
 @click.option(
     "--restriction_tsv",
     help="Path to a TSV file containing the sessions that can be included.",
-    type=str,
+    type=click.Path(exists=True),
     default=None,
 )
 @click.option(
     "--keep_smc",
     help="This flag allows to keep SMC participants, else they are removed.",
     type=bool,
     default=False,
     is_flag=True,
 )
 @click.option(
     "--merged_tsv",
     help="Path to a TSV file containing the results of clinica iotools merge-tsv command if different of results_directory/merged.tsv",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 @click.option(
     "--missing_mods",
     help="Path to a directory containing the results of clinica iotools missing-modalities command if different of results_directory/missing_mods/",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 @click.option(
     "--remove_unique_session",
     help="This flag allows to remove subjects with a unique session, else they are kept.",
     type=bool,
     default=False,
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_metadata/get_metadata.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from logging import getLogger
-from os import path
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from clinicadl.utils.exceptions import ClinicaDLArgumentError, ClinicaDLTSVError
 from clinicadl.utils.tsvtools_utils import merged_tsv_reader
 
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.get_metadata")
 
 
 def get_metadata(
-    data_tsv: str, merged_tsv: str, variables_of_interest=None
+    data_tsv: Path, merged_tsv: Path, variables_of_interest=None
 ) -> pd.DataFrame:
     """
     Get the meta data in metadata_df to write them in output_df.
     If variables_of_interest is None, the function writes all the data that are in metadata_df for the list of subjects in output_df.
 
     Parameters
     ----------
     data_tsv: str (Path)
         Columns must include ['participant_id', 'session_id']
     merged_tsv: str (Path)
-        output of `clinica merge-tsv`
+        Output of `clinica merge-tsv`
     variables_of_interest: list of str
         List of columns that will be added in the output DataFrame.
 
     Returns
     -------
     """
 
@@ -37,29 +37,33 @@
     variables_metadata = metadata_df.columns.tolist()
 
     variables_intersection = list(
         set(variables_metadata).intersection(set(variables_in))
     )
 
     if variables_of_interest is None:
-
-        variables_list = np.unique(variables_in)
+        variables_list = np.unique(variables_metadata)
+        logger.debug(
+            f"Adding the following columns to the input tsv file: {variables_list}"
+        )
         result_df = pd.merge(metadata_df, in_out_df, on=variables_intersection)
         result_df.set_index(["participant_id", "session_id"], inplace=True)
 
     else:
-
         if not set(variables_of_interest).issubset(set(metadata_df.columns.values)):
             raise ClinicaDLArgumentError(
                 f"The variables asked by the user {variables_of_interest} do not "
                 f"exist in the data set."
             )
         else:
             variables_of_interest = list(variables_of_interest)
             variables_list = np.unique(variables_of_interest + variables_in)
+            logger.debug(
+                f"Adding the following columns to the input tsv file: {variables_list}"
+            )
             result_df = pd.merge(metadata_df, in_out_df, on=variables_intersection)
             result_df = result_df[variables_list]
             result_df.set_index(["participant_id", "session_id"], inplace=True)
 
     result_df.to_csv(data_tsv, sep="\t")
 
     logger.info(f"metadata were added in: {data_tsv}")
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_metadata/get_metadata_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from pathlib import Path
-from typing import List
-
 import click
 
 from clinicadl.utils import cli_param
 
 
 @click.command(name="get-metadata", no_args_is_help=True)
 @cli_param.argument.data_tsv
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_progression/get_progression.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-import os
 from copy import copy
 from logging import getLogger
-from os import path
 from pathlib import Path
 
 import pandas as pd
 
 from clinicadl.tsvtools.get_labels import infer_or_drop_diagnosis
 from clinicadl.utils.tsvtools_utils import (
     after_end_screening,
     last_session,
     merged_tsv_reader,
     neighbour_session,
 )
 
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.get_progression")
 
 
 def get_progression(
-    data_tsv: str,
+    data_tsv: Path,
     horizon_time: int = 36,
     stability_dict: dict = None,
 ):
-
     """
-    A method to get the progression for each sessions depending on their stability on the time horizon
+    A method to get the progression for each sessions, depending on their stability on the time horizon
     Outputs are written in data_tsv
 
     Parameters
     ----------
     data_tsv: str (path)
         Path to a tsv file with columns including ["participants_id", "session_id", "dignosis"]
     horizon_time: int
@@ -38,19 +35,19 @@
 
     """
 
     # Reading files
     bids_df = merged_tsv_reader(data_tsv)
 
     if "diagnosis" not in bids_df.columns:
-
-        parents_path = path.abspath(data_tsv)
-        while not os.path.exists(path.join(parents_path, "labels.tsv")):
-            parents_path = Path(parents_path).parents[0]
-            labels_df = pd.read_csv(path.join(parents_path, "labels.tsv"), sep="\t")
+        logger.debug("Looking for the 'diagnosis' column in others files")
+        parents_path = (data_tsv.resolve()).parent
+        while not (parents_path / "labels.tsv").is_file():
+            parents_path = parents_path.parent
+            labels_df = pd.read_csv(parents_path / "labels.tsv", sep="\t")
             bids_df = pd.merge(
                 bids_df,
                 labels_df,
                 how="inner",
                 on=["participant_id", "session_id"],
             )
         if "dx1" in bids_df.columns:
@@ -76,14 +73,15 @@
     bids_copy_df = copy(bids_df)
 
     # Do not take into account the case of missing diag = nan
 
     for subject, subject_df in bids_df.groupby(level=0):
         session_list = [session for _, session in subject_df.index.values]
         session_list.sort()
+        logger.debug(f"Getting progression for subject {subject}")
         for _, session in subject_df.index.values:
             diagnosis = subject_df.loc[(subject, session), "diagnosis"]
             diagnosis_dict = stability_dict[diagnosis]
             session_nb = int(session[5::])
             horizon_session_nb = session_nb + horizon_time
             if horizon_session_nb < 10:
                 horizon_session = "ses-M00" + str(horizon_session_nb)
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/get_progression/get_progression_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/get_progression/get_progression_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/getlabels/getlabels.py` & `clinicadl-1.3.0/clinicadl/tsvtools/getlabels/getlabels.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/kfold/kfold.py` & `clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # coding: utf8
 
-import os
 from logging import getLogger
-from os import makedirs, path
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import StratifiedKFold
 
 from clinicadl.utils.exceptions import ClinicaDLTSVError
 from clinicadl.utils.maps_manager.iotools import commandline_to_json
 from clinicadl.utils.tsvtools_utils import extract_baseline, retrieve_longitudinal
 
 sex_dict = {"M": 0, "F": 1}
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.kfold")
 
 
 def write_splits(
     diagnosis_df: pd.DataFrame,
     split_label: str,
     n_splits: int,
     subset_name: str,
-    results_directory: str,
+    results_directory: Path,
 ):
     """
     Split data at the subject-level in training and test to have equivalent distributions in split_label.
     Writes test and train Dataframes.
 
     Parameters
     ----------
@@ -66,40 +64,40 @@
         train_df.reset_index(inplace=True, drop=True)
         test_df.reset_index(inplace=True, drop=True)
 
         # train_df = train_df[["participant_id", "session_id"]]
         # test_df = test_df[["participant_id", "session_id"]]
         # long_train_df = long_train_df[["participant_id", "session_id"]]
 
-        os.makedirs(path.join(results_directory, f"split-{i}"))
+        (results_directory / f"split-{i}").mkdir(parents=True)
 
         train_df.to_csv(
-            path.join(results_directory, f"split-{i}", "train_baseline.tsv"),
+            results_directory / f"split-{i}" / "train_baseline.tsv",
             sep="\t",
             index=False,
         )
         test_df.to_csv(
-            path.join(results_directory, f"split-{i}", f"{subset_name}_baseline.tsv"),
+            results_directory / f"split-{i}" / f"{subset_name}_baseline.tsv",
             sep="\t",
             index=False,
         )
 
         long_train_df.to_csv(
-            path.join(results_directory, f"split-{i}", "train.tsv"),
+            results_directory / f"split-{i}" / "train.tsv",
             sep="\t",
             index=False,
         )
 
 
 def split_diagnoses(
-    data_tsv: str,
+    data_tsv: Path,
     n_splits: int = 5,
     subset_name: str = None,
     stratification: str = None,
-    merged_tsv: str = None,
+    merged_tsv: Path = None,
 ):
     """
     Performs a k-fold split for each label independently on the subject level.
     The output (the tsv file) will have two new columns :
         - split, with the number of the split the subject is in.
         - datagroup, with the name of the group (train or subset_name) the subject is in.
 
@@ -116,53 +114,50 @@
         Name of the subset that is complementary to train.
     stratification: str
         Name of variable used to stratify k-fold.
     merged_tsv: str
         Path to the merged.tsv file, output of clinica iotools merge-tsv.
     """
 
-    parents_path = Path(data_tsv).parents[0]
+    parents_path = data_tsv.parent
     split_numero = 1
     folder_name = f"{n_splits}_fold"
 
-    while os.path.exists(parents_path / folder_name):
+    while (parents_path / folder_name).is_dir():
         split_numero += 1
         folder_name = f"{n_splits}_fold_{split_numero}"
     results_directory = parents_path / folder_name
-    makedirs(results_directory)
+    results_directory.mkdir(parents=True)
 
     commandline_to_json(
         {
             "output_dir": results_directory,
             "n_splits": n_splits,
             "subset_name": subset_name,
             "stratification": stratification,
         },
         filename="kfold.json",
     )
 
-    # Read files
-    from os.path import join
-
-    # diagnosis_df_path = Path(data_tsv).name
     diagnosis_df = pd.read_csv(data_tsv, sep="\t")
     list_columns = diagnosis_df.columns.values
     if (
         "diagnosis" not in list_columns
         or ("age" not in list_columns and "age_bl" not in list_columns)
         or "sex" not in list_columns
     ):
+        logger.debug("Looking for the missing columns in others files.")
         if merged_tsv is None:
-            parents_path = path.abspath(parents_path)
+            parents_path = parents_path.resolve()
             n = 0
-            while not os.path.exists(path.join(parents_path, "labels.tsv")) and n <= 4:
-                parents_path = Path(parents_path).parents[0]
+            while not (parents_path / "labels.tsv").is_file() and n <= 4:
+                parents_path = parents_path.parent
                 n += 1
             try:
-                labels_df = pd.read_csv(path.join(parents_path, "labels.tsv"), sep="\t")
+                labels_df = pd.read_csv(parents_path / "labels.tsv", sep="\t")
                 diagnosis_df = pd.merge(
                     diagnosis_df,
                     labels_df,
                     how="inner",
                     on=["participant_id", "session_id"],
                 )
             except:
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/kfold/kfold_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/kfold/kfold_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/prepare_experiment/prepare_experiment_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,20 @@
         subset_name="test",
         p_age_threshold=p_age_threshold,
         p_sex_threshold=p_sex_threshold,
         ignore_demographics=ignore_demographics,
         categorical_split_variable=None,
         not_only_baseline=flag_not_baseline,
     )
-    from os.path import exists
-    from pathlib import Path
 
-    parents_path = Path(data_tsv).parents[0]
+    parents_path = data_tsv.parents[0]
     split_numero = 1
     folder_name = "split"
 
-    while exists(parents_path / folder_name):
+    while (parents_path / folder_name).is_dir():
         split_numero += 1
         folder_name = f"split_{split_numero}"
     if split_numero > 2:
         folder_name = f"split_{split_numero-1}"
     else:
         folder_name = "split"
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/split/split.py` & `clinicadl-1.3.0/clinicadl/tsvtools/split/split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # coding: utf8
 
-import os
 from logging import getLogger
-from os import makedirs, path
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from scipy.stats import ks_2samp, ttest_ind
 from sklearn.model_selection import StratifiedShuffleSplit
 
@@ -20,15 +18,15 @@
     extract_baseline,
     find_label,
     remove_unicity,
     retrieve_longitudinal,
 )
 
 sex_dict = {"M": 0, "F": 1}
-logger = getLogger("clinicadl")
+logger = getLogger("clinicadl.tsvtools.split")
 
 
 def KStests(train_df, test_df, threshold=0.5):
     pmin = 1
     column = ""
     for col in train_df.columns:
         if col == "session_id":
@@ -61,17 +59,16 @@
     split_label,
     n_test,
     p_age_threshold=0.80,
     p_sex_threshold=0.80,
     supplementary_train_df=None,
     ignore_demographics=False,
 ):
-
     """
-    Split data at the subject-level in training and test set with equivalent age, sex and split_label distributions
+    Split data at the subject-level in training and test set with equivalent age, sex and split_label distributions.
 
     Parameters
     ----------
     diagnosis_df: DataFrame
         Columns including ['participant_id', 'session_id', 'group']
     split_label: str
         Label on which the split is done (categorical variables)
@@ -131,18 +128,16 @@
         category = category_conversion(category)
         category = remove_unicity(category)
 
         flag_selection = True
         n_try = 0
 
         while flag_selection:
-
             splits = StratifiedShuffleSplit(n_splits=1, test_size=n_test)
             for train_index, test_index in splits.split(category, category):
-
                 # Find the value for different demographics (age & sex)
                 if len(set(age)) != 1:
                     age_test = [float(age[idx]) for idx in test_index]
                     age_train = [float(age[idx]) for idx in train_index] + sup_train_age
                     _, p_age = ttest_ind(age_test, age_train, nan_policy="omit")
                 else:
                     p_age = 1
@@ -177,15 +172,15 @@
         test_df = baseline_df.loc[idx_test]
         train_df = baseline_df.loc[idx_train]
 
     return train_df, test_df
 
 
 def split_diagnoses(
-    data_tsv,
+    data_tsv: Path,
     n_test=100,
     subset_name="test",
     p_age_threshold=0.80,
     p_sex_threshold=0.80,
     categorical_split_variable=None,
     ignore_demographics=False,
     verbose=0,
@@ -225,23 +220,23 @@
     ------------
     writes three files per <label>.tsv file present in data_tsv:
         - data_tsv/train/<label>.tsv
         - data_tsv/train/<label>_baseline.tsv
         - data_tsv/<subset_name>/<label>_baseline.tsv
     """
 
-    parents_path = Path(data_tsv).parents[0]
+    parents_path = data_tsv.parents[0]
     split_numero = 1
     folder_name = f"split"
 
-    while os.path.exists(parents_path / folder_name):
+    while (parents_path / folder_name).is_dir():
         split_numero += 1
         folder_name = f"split_{split_numero}"
     results_path = parents_path / folder_name
-    makedirs(results_path)
+    results_path.mkdir(parents=True)
 
     commandline_to_json(
         {
             "output_dir": results_path,
             "n_test": n_test,
             "subset_name": subset_name,
             "p_age_threshold": p_age_threshold,
@@ -257,15 +252,15 @@
 
     if categorical_split_variable is None:
         categorical_split_variable = "diagnosis"
     else:
         categorical_split_variable.append("diagnosis")
 
     # Read files
-    diagnosis_df_path = Path(data_tsv).name
+    diagnosis_df_path = data_tsv.name
     diagnosis_df = pd.read_csv(data_tsv, sep="\t")
     list_columns = diagnosis_df.columns.values
     if multi_diagnoses:
         train, test, p_min = shuffle_choice(diagnosis_df, n_shuffle=5000)
 
         train_df = extract_baseline(train)
         test_df = extract_baseline(test)
@@ -281,21 +276,21 @@
 
     elif n_test > 0:
         if (
             "diagnosis" not in list_columns
             or ("age" not in list_columns and "age_bl" not in list_columns)
             or "sex" not in list_columns
         ):
-            parents_path = path.abspath(parents_path)
+            parents_path = parents_path.resolve()
             n = 0
-            while not os.path.exists(path.join(parents_path, "labels.tsv")) and n <= 4:
-                parents_path = Path(parents_path).parents[0]
+            while not (parents_path / "labels.tsv").is_file() and n <= 4:
+                parents_path = parents_path.parents[0]
                 n += 1
             try:
-                labels_df = pd.read_csv(path.join(parents_path, "labels.tsv"), sep="\t")
+                labels_df = pd.read_csv(parents_path / "labels.tsv", sep="\t")
                 diagnosis_df = pd.merge(
                     diagnosis_df,
                     labels_df,
                     how="inner",
                     on=["participant_id", "session_id"],
                 )
             except:
@@ -330,13 +325,13 @@
     else:
         train_df = extract_baseline(diagnosis_df)
         # train_df = train_df[["participant_id", "session_id"]]
         if not_only_baseline:
             long_train_df = diagnosis_df
 
     name = "train_baseline.tsv"
-    df_to_tsv(name, str(results_path), train_df, baseline=True)
+    df_to_tsv(name, results_path, train_df, baseline=True)
 
     long_train_df = retrieve_longitudinal(train_df, diagnosis_df)
     # long_train_df = long_train_df[["participant_id", "session_id"]]
     name = "train.tsv"
-    df_to_tsv(name, str(results_path), long_train_df)
+    df_to_tsv(name, results_path, long_train_df)
```

### Comparing `clinicadl-1.2.0/clinicadl/tsvtools/split/split_cli.py` & `clinicadl-1.3.0/clinicadl/tsvtools/split/split_cli.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/caps_dataset/data.py` & `clinicadl-1.3.0/clinicadl/utils/caps_dataset/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # coding: utf8
 
 import abc
 from logging import getLogger
-from os import path
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import torch
 import torchvision.transforms as transforms
@@ -39,15 +38,15 @@
 # Datasets loaders
 #################################
 class CapsDataset(Dataset):
     """Abstract class for all derived CapsDatasets."""
 
     def __init__(
         self,
-        caps_directory: str,
+        caps_directory: Path,
         data_df: pd.DataFrame,
         preprocessing_dict: Dict[str, Any],
         transformations: Optional[Callable],
         label_presence: bool,
         label: str = None,
         label_code: Dict[Any, int] = None,
         augmentation_transformations: Optional[Callable] = None,
@@ -64,24 +63,23 @@
         self.preprocessing_dict = preprocessing_dict
 
         if not hasattr(self, "elem_index"):
             raise AttributeError(
                 "Child class of CapsDataset must set elem_index attribute."
             )
         if not hasattr(self, "mode"):
-            raise AttributeError("Child class of CapsDataset must set mode attribute.")
+            raise AttributeError("Child class of CapsDataset, must set mode attribute.")
 
         self.df = data_df
 
         mandatory_col = {"participant_id", "session_id", "cohort"}
         if self.label_presence and self.label is not None:
             mandatory_col.add(self.label)
 
         if not mandatory_col.issubset(set(self.df.columns.values)):
-
             raise Exception(
                 f"the data file is not in the correct format."
                 f"Columns should include {mandatory_col}"
             )
         self.elem_per_image = self.num_elem_per_image()
         self.size = self[0]["image"].size()
 
@@ -109,20 +107,19 @@
         else:
             return self.label_code[str(target)]
 
     def __len__(self) -> int:
         return len(self.df) * self.elem_per_image
 
     @staticmethod
-    def create_caps_dict(caps_directory: str, multi_cohort: bool) -> Dict[str, str]:
-
+    def create_caps_dict(caps_directory: Path, multi_cohort: bool) -> Dict[str, Path]:
         from clinica.utils.inputs import check_caps_folder
 
         if multi_cohort:
-            if not caps_directory.endswith(".tsv"):
+            if not caps_directory.suffix == ".tsv":
                 raise ClinicaDLArgumentError(
                     "If multi_cohort is True, the CAPS_DIRECTORY argument should be a path to a TSV file."
                 )
             else:
                 caps_df = pd.read_csv(caps_directory, sep="\t")
                 check_multi_cohort_tsv(caps_df, "CAPS")
                 caps_dict = dict()
@@ -152,27 +149,27 @@
 
         # Try to find .nii.gz file
         try:
             file_type = self.preprocessing_dict["file_type"]
             results = clinica_file_reader(
                 [participant], [session], self.caps_dict[cohort], file_type
             )
-            filepath = results[0]
-            image_filename = path.basename(filepath[0]).replace(".nii.gz", ".pt")
+            filepath = Path(results[0][0])
+            image_filename = filepath.name.replace(".nii.gz", ".pt")
             folder, _ = compute_folder_and_file_type(self.preprocessing_dict)
-            image_dir = path.join(
-                self.caps_dict[cohort],
-                "subjects",
-                participant,
-                session,
-                "deeplearning_prepare_data",
-                "image_based",
-                folder,
+            image_dir = (
+                self.caps_dict[cohort]
+                / "subjects"
+                / participant
+                / session
+                / "deeplearning_prepare_data"
+                / "image_based"
+                / folder
             )
-            image_path = path.join(image_dir, image_filename)
+            image_path = image_dir / image_filename
         # Try to find .pt file
         except ClinicaCAPSError:
             file_type = self.preprocessing_dict["file_type"]
             file_type["pattern"] = file_type["pattern"].replace(".nii.gz", ".pt")
             results = clinica_file_reader(
                 [participant], [session], self.caps_dict[cohort], file_type
             )
@@ -199,15 +196,14 @@
         session = self.df.loc[image_idx, "session_id"]
         cohort = self.df.loc[image_idx, "cohort"]
 
         if self.elem_index is None:
             elem_idx = idx % self.elem_per_image
         else:
             elem_idx = self.elem_index
-
         if self.label_presence and self.label is not None:
             target = self.df.loc[image_idx, self.label]
             label = self.label_fn(target)
         else:
             label = -1
 
         return participant, session, cohort, elem_idx, label
@@ -277,15 +273,15 @@
 
 
 class CapsDatasetImage(CapsDataset):
     """Dataset of MRI organized in a CAPS folder."""
 
     def __init__(
         self,
-        caps_directory: str,
+        caps_directory: Path,
         data_file: pd.DataFrame,
         preprocessing_dict: Dict[str, Any],
         train_transformations: Optional[Callable] = None,
         label_presence: bool = True,
         label: str = None,
         label_code: Dict[str, int] = None,
         all_transformations: Optional[Callable] = None,
@@ -302,14 +298,15 @@
             label_code: label code that links the output node number to label value.
             all_transformations: Optional transform to be applied during training and evaluation.
             multi_cohort: If True caps_directory is the path to a TSV file linking cohort names and paths.
 
         """
 
         self.mode = "image"
+        self.prepare_dl = preprocessing_dict["prepare_dl"]
         super().__init__(
             caps_directory,
             data_file,
             preprocessing_dict,
             augmentation_transformations=train_transformations,
             label_presence=label_presence,
             label=label,
@@ -336,27 +333,27 @@
 
         sample = {
             "image": image,
             "label": label,
             "participant_id": participant,
             "session_id": session,
             "image_id": 0,
-            "image_path": image_path,
+            "image_path": image_path.as_posix(),
         }
 
         return sample
 
     def num_elem_per_image(self):
         return 1
 
 
 class CapsDatasetPatch(CapsDataset):
     def __init__(
         self,
-        caps_directory: str,
+        caps_directory: Path,
         data_file: pd.DataFrame,
         preprocessing_dict: Dict[str, Any],
         train_transformations: Optional[Callable] = None,
         patch_index: Optional[int] = None,
         label_presence: bool = True,
         label: str = None,
         label_code: Dict[str, int] = None,
@@ -400,21 +397,21 @@
         return self.patch_index
 
     def __getitem__(self, idx):
         participant, session, cohort, patch_idx, label = self._get_meta_data(idx)
         image_path = self._get_image_path(participant, session, cohort)
 
         if self.prepare_dl:
-            patch_dir = path.dirname(image_path).replace(
+            patch_dir = image_path.parent.as_posix().replace(
                 "image_based", f"{self.mode}_based"
             )
             patch_filename = extract_patch_path(
                 image_path, self.patch_size, self.stride_size, patch_idx
             )
-            patch_tensor = torch.load(path.join(patch_dir, patch_filename))
+            patch_tensor = torch.load(Path(patch_dir).resolve() / patch_filename)
 
         else:
             image = torch.load(image_path)
             patch_tensor = extract_patch_tensor(
                 image, self.patch_size, self.stride_size, patch_idx
             )
 
@@ -452,15 +449,15 @@
         num_patches = patches_tensor.shape[0]
         return num_patches
 
 
 class CapsDatasetRoi(CapsDataset):
     def __init__(
         self,
-        caps_directory: str,
+        caps_directory: Path,
         data_file: pd.DataFrame,
         preprocessing_dict: Dict[str, Any],
         roi_index: Optional[int] = None,
         train_transformations: Optional[Callable] = None,
         label_presence: bool = True,
         label: str = None,
         label_code: Dict[str, int] = None,
@@ -514,19 +511,19 @@
             raise NotImplementedError(
                 "Default regions are not available anymore in ClinicaDL. "
                 "Please define appropriate masks and give a roi_list."
             )
 
         if self.prepare_dl:
             mask_path = self.mask_paths[roi_idx]
-            roi_dir = path.dirname(image_path).replace(
+            roi_dir = image_path.parent.as_posix().replace(
                 "image_based", f"{self.mode}_based"
             )
             roi_filename = extract_roi_path(image_path, mask_path, self.uncropped_roi)
-            roi_tensor = torch.load(path.join(roi_dir, roi_filename))
+            roi_tensor = torch.load(Path(roi_dir) / roi_filename)
 
         else:
             image = torch.load(image_path)
             mask_array = self.mask_arrays[roi_idx]
             roi_tensor = extract_roi_tensor(image, mask_array, self.uncropped_roi)
 
         if self.transformations:
@@ -551,15 +548,15 @@
         if self.roi_list is None:
             return 2
         else:
             return len(self.roi_list)
 
     def _get_mask_paths_and_tensors(
         self,
-        caps_directory: str,
+        caps_directory: Path,
         multi_cohort: bool,
         preprocessing_dict: Dict[str, Any],
     ) -> Tuple[List[str], List]:
         """Loads the masks necessary to regions extraction"""
         import nibabel as nib
 
         caps_dict = self.create_caps_dict(caps_directory, multi_cohort)
@@ -596,33 +593,33 @@
             pattern = PATTERN_DICT[preprocessing_dict["preprocessing"]]
         else:
             raise NotImplementedError(
                 f"Pattern of mask for preprocessing {preprocessing_dict['preprocessing']} "
                 f"is not defined."
             )
 
-        mask_location = path.join(caps_directory, "masks", f"tpl-{template_name}")
+        mask_location = caps_directory / "masks" / f"tpl-{template_name}"
 
         mask_paths, mask_arrays = list(), list()
         for roi in self.roi_list:
             logger.info(f"Find mask for roi {roi}.")
             mask_path, desc = find_mask_path(mask_location, roi, pattern, True)
             if mask_path is None:
                 raise FileNotFoundError(desc)
             mask_nii = nib.load(mask_path)
-            mask_paths.append(mask_path)
+            mask_paths.append(Path(mask_path))
             mask_arrays.append(mask_nii.get_fdata())
 
         return mask_paths, mask_arrays
 
 
 class CapsDatasetSlice(CapsDataset):
     def __init__(
         self,
-        caps_directory: str,
+        caps_directory: Path,
         data_file: pd.DataFrame,
         preprocessing_dict: Dict[str, Any],
         slice_index: Optional[int] = None,
         train_transformations: Optional[Callable] = None,
         label_presence: bool = True,
         label: str = None,
         label_code: Dict[str, int] = None,
@@ -673,21 +670,21 @@
 
     def __getitem__(self, idx):
         participant, session, cohort, slice_idx, label = self._get_meta_data(idx)
         slice_idx = slice_idx + self.discarded_slices[0]
         image_path = self._get_image_path(participant, session, cohort)
 
         if self.prepare_dl:
-            slice_dir = path.dirname(image_path).replace(
+            slice_dir = image_path.parent.as_posix().replace(
                 "image_based", f"{self.mode}_based"
             )
             slice_filename = extract_slice_path(
                 image_path, self.slice_direction, self.slice_mode, slice_idx
             )
-            slice_tensor = torch.load(path.join(slice_dir, slice_filename))
+            slice_tensor = torch.load(Path(slice_dir) / slice_filename)
 
         else:
             image_path = self._get_image_path(participant, session, cohort)
             image = torch.load(image_path)
             slice_tensor = extract_slice_tensor(
                 image, self.slice_direction, self.slice_mode, slice_idx
             )
@@ -720,15 +717,15 @@
             image.size(self.slice_direction + 1)
             - self.discarded_slices[0]
             - self.discarded_slices[1]
         )
 
 
 def return_dataset(
-    input_dir: str,
+    input_dir: Path,
     data_df: pd.DataFrame,
     preprocessing_dict: Dict[str, Any],
     all_transformations: Optional[Callable],
     label: str = None,
     label_code: Dict[str, int] = None,
     train_transformations: Optional[Callable] = None,
     cnn_index: int = None,
@@ -748,15 +745,14 @@
         cnn_index: Index of the CNN in a multi-CNN paradigm (optional).
         label_presence: If True the diagnosis will be extracted from the given DataFrame.
         multi_cohort: If True caps_directory is the path to a TSV file linking cohort names and paths.
 
     Returns:
          the corresponding dataset.
     """
-
     if cnn_index is not None and preprocessing_dict["mode"] == "image":
         raise NotImplementedError(
             f"Multi-CNN is not implemented for {preprocessing_dict['mode']} mode."
         )
 
     if preprocessing_dict["mode"] == "image":
         return CapsDatasetImage(
@@ -958,28 +954,28 @@
 
     return train_transformations, all_transformations
 
 
 ################################
 # TSV files loaders
 ################################
-def load_data_test(test_path, diagnoses_list, baseline=True, multi_cohort=False):
+def load_data_test(test_path: Path, diagnoses_list, baseline=True, multi_cohort=False):
     """
     Load data not managed by split_manager.
 
     Args:
         test_path (str): path to the test TSV files / split directory / TSV file for multi-cohort
         diagnoses_list (List[str]): list of the diagnoses wanted in case of split_dir or multi-cohort
         baseline (bool): If True baseline sessions only used (split_dir handling only).
         multi_cohort (bool): If True considers multi-cohort setting.
     """
     # TODO: computes baseline sessions on-the-fly to manager TSV file case
 
     if multi_cohort:
-        if not test_path.endswith(".tsv"):
+        if not test_path.suffix == ".tsv":
             raise ClinicaDLArgumentError(
                 "If multi_cohort is given, the TSV_DIRECTORY argument should be a path to a TSV file."
             )
         else:
             tsv_df = pd.read_csv(test_path, sep="\t")
             check_multi_cohort_tsv(tsv_df, "labels")
             test_df = pd.DataFrame()
@@ -1004,30 +1000,29 @@
             if found_diagnoses != set(diagnoses_list):
                 raise ValueError(
                     f"The diagnoses found in the multi cohort dataset {found_diagnoses} "
                     f"do not correspond to the diagnoses wanted {set(diagnoses_list)}."
                 )
             test_df.reset_index(inplace=True, drop=True)
     else:
-        if test_path.endswith(".tsv"):
+        if test_path.suffix == ".tsv":
             tsv_df = pd.read_csv(test_path, sep="\t")
             multi_col = {"cohort", "path"}
             if multi_col.issubset(tsv_df.columns.values):
                 raise ClinicaDLConfigurationError(
                     "To use multi-cohort framework, please add 'multi_cohort=true' in your configuration file or '--multi_cohort' flag to the command line."
                 )
         test_df = load_data_test_single(test_path, diagnoses_list, baseline=baseline)
         test_df["cohort"] = "single"
 
     return test_df
 
 
-def load_data_test_single(test_path, diagnoses_list, baseline=True):
-
-    if test_path.endswith(".tsv"):
+def load_data_test_single(test_path: Path, diagnoses_list, baseline=True):
+    if test_path.suffix == ".tsv":
         test_df = pd.read_csv(test_path, sep="\t")
         if "diagnosis" not in test_df.columns.values:
             raise ClinicaDLTSVError(
                 f"'diagnosis' column must be present in TSV file {test_path}."
             )
         test_df = test_df[test_df.diagnosis.isin(diagnoses_list)]
         if len(test_df) == 0:
@@ -1035,33 +1030,33 @@
                 f"Diagnoses wanted {diagnoses_list} were not found in TSV file {test_path}."
             )
         return test_df
 
     test_df = pd.DataFrame()
 
     if baseline:
-        if not path.exists(path.join(Path(test_path).parents[0], "train_baseline.tsv")):
-            if not path.join(Path(test_path).parents[0], "labels_baseline.tsv"):
+        if not (test_path.parent / "train_baseline.tsv").is_file():
+            if not (test_path.parent / "labels_baseline.tsv").is_file():
                 raise ClinicaDLTSVError(
-                    f"There is no train_baseline.tsv nor labels_baseline.tsv in your folder {Path(test_path).parents[0]} "
+                    f"There is no train_baseline.tsv nor labels_baseline.tsv in your folder {test_path.parents[0]} "
                 )
             else:
-                test_path = path.join(Path(test_path).parents[0], "labels_baseline.tsv")
+                test_path = test_path.parent / "labels_baseline.tsv"
         else:
-            test_path = path.join(Path(test_path).parents[0], "train_baseline.tsv")
+            test_path = test_path.parent / "train_baseline.tsv"
     else:
-        if not path.exists(path.join(Path(test_path).parents[0], "train.tsv")):
-            if not path.join(Path(test_path).parents[0], "labels.tsv"):
+        if not (test_path.parent / "train.tsv").is_file():
+            if not (test_path.parent / "labels.tsv").is_file():
                 raise ClinicaDLTSVError(
-                    f"There is no train.tsv or labels.tsv in your folder {Path(test_path).parents[0]} "
+                    f"There is no train.tsv or labels.tsv in your folder {test_path.parent} "
                 )
             else:
-                test_path = path.join(Path(test_path).parents[0], "labels.tsv")
+                test_path = test_path.parent / "labels.tsv"
         else:
-            test_path = path.join(Path(test_path).parents[0], "train.tsv")
+            test_path = test_path.parent / "train.tsv"
 
     test_df = pd.read_csv(test_path, sep="\t")
 
     test_df.reset_index(inplace=True, drop=True)
 
     return test_df
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/cli_param/argument.py` & `clinicadl-1.3.0/clinicadl/utils/cli_param/argument.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 """Common CLI arguments used by ClinicaDL pipelines."""
+from pathlib import Path
+
 import click
 
-bids_directory = click.argument("bids_directory", type=click.Path(exists=True))
-caps_directory = click.argument("caps_directory", type=click.Path(exists=True))
-input_maps = click.argument("input_maps_directory", type=click.Path(exists=True))
-output_maps = click.argument("output_maps_directory", type=click.Path())
-results_tsv = click.argument("results_tsv", type=str)
+bids_directory = click.argument(
+    "bids_directory", type=click.Path(exists=True, path_type=Path)
+)
+caps_directory = click.argument("caps_directory", type=click.Path(path_type=Path))
+input_maps = click.argument(
+    "input_maps_directory", type=click.Path(exists=True, path_type=Path)
+)
+output_maps = click.argument("output_maps_directory", type=click.Path(path_type=Path))
+results_tsv = click.argument("results_tsv", type=click.Path(path_type=Path))
 
 # ANALYSIS
-merged_tsv = click.argument("merged_tsv", type=click.Path(exists=True))
+merged_tsv = click.argument("merged_tsv", type=click.Path(exists=True, path_type=Path))
 
 # TSV TOOLS
-data_tsv = click.argument("data_tsv", type=click.Path(exists=True))
-old_tsv_dir = click.argument("old_tsv_dir", type=click.Path(exists=True))
-new_tsv_dir = click.argument("new_tsv_dir", type=click.Path())
+data_tsv = click.argument("data_tsv", type=click.Path(exists=True, path_type=Path))
+old_tsv_dir = click.argument(
+    "old_tsv_dir", type=click.Path(exists=True, path_type=Path)
+)
+new_tsv_dir = click.argument("new_tsv_dir", type=click.Path(path_type=Path))
 dataset = click.argument("dataset", type=click.Choice(["AIBL", "OASIS"]))
 
 # GENERATE
-generated_caps = click.argument("generated_caps_directory", type=click.Path())
+generated_caps = click.argument(
+    "generated_caps_directory", type=click.Path(path_type=Path)
+)
 
 # PREDICT
 data_group = click.argument("data_group", type=str)
 
 # TRAIN
 preprocessing_json = click.argument("preprocessing_json", type=str)
 
 # EXTRACT
 modality = click.argument(
     "modality",
-    type=click.Choice(["t1-linear", "pet-linear", "custom"]),
+    type=click.Choice(["t1-linear", "pet-linear", "flair-linear", "custom"]),
 )
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/cli_param/option.py` & `clinicadl-1.3.0/clinicadl/utils/cli_param/option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Common CLI options used by Clinica pipelines."""
 
+from pathlib import Path
+
 import click
 from clinica.utils.pet import LIST_SUVR_REFERENCE_REGIONS
 
 # TSV TOOLS
 diagnoses = click.option(
     "--diagnoses",
     "-d",
@@ -32,37 +34,37 @@
     default="validation",
     help="Name of the subset that is complementary to train.",
 )
 test_tsv = click.option(
     "--test_tsv",
     "-tt",
     help="Name of the test file in tsv format",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 caps_directory = click.option(
     "--caps_directory",
     "-c",
     help="input folder of a CAPS compliant dataset",
-    type=str,
+    type=click.Path(exists=True, path_type=Path),
     default=None,
 )
 variables_of_interest = click.option(
     "--variables_of_interest",
     "-voi",
     help="Variables of interest that will be kept in the final lists. "
     "Will always keep the group (that correspond to the diagnosis in most case), subgroup (that correspond to the progression of the disease in the case of a progressive disease), age and sex needed for the split procedure.",
     type=str,
     multiple=True,
     default=None,
 )
 # GENERATE
 participant_list = click.option(
     "--participants_tsv",
-    type=click.Path(exists=True),
+    type=click.Path(exists=True, path_type=Path),
     help="Path to a TSV file including a list of participants/sessions.",
 )
 n_subjects = click.option(
     "--n_subjects",
     type=int,
     default=300,
     help="Number of subjects in each class of the synthetic dataset.",
@@ -104,15 +106,15 @@
     is_flag=True,
     help="""Extract the selected mode to save the tensor. By default, the pipeline only save images and the mode extraction
             is done when images are loaded in the train.""",
 )
 subjects_sessions_tsv = click.option(
     "-tsv",
     "--subjects_sessions_tsv",
-    type=click.Path(exists=True, resolve_path=True),
+    type=click.Path(exists=True, resolve_path=True, path_type=Path),
     help="TSV file containing a list of subjects with their sessions.",
 )
 extract_json = click.option(
     "-ej",
     "--extract_json",
     type=str,
     default=None,
@@ -124,20 +126,20 @@
     "-uui",
     "--use_uncropped_image",
     is_flag=True,
     default=False,
     help="Use the uncropped image instead of the cropped image generated by t1-linear or pet-linear.",
 )
 
-acq_label = click.option(
-    "--acq_label",
+tracer = click.option(
+    "--tracer",
     type=str,
     help=(
         "Acquisition label if MODALITY is `pet-linear`. "
-        "Name of the tracer used for the PET acquisition (trc-<acq_label>). "
+        "Name of the tracer used for the PET acquisition (trc-<tracer>). "
         "For instance it can be '18FFDG' for fluorodeoxyglucose or '18FAV45' for florbetapir."
     ),
 )
 suvr_reference_region = click.option(
     "-suvr",
     "--suvr_reference_region",
     type=click.Choice(LIST_SUVR_REFERENCE_REGIONS),
@@ -164,7 +166,17 @@
     "--overwrite",
     "-o",
     default=False,
     is_flag=True,
     help="Will overwrite data group if existing. Please give caps_directory and partcipants_tsv to"
     " define new data group.",
 )
+
+# Predict and interpret
+
+save_nifti = click.option(
+    "--save_nifti",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Save the output map(s) in the MAPS in NIfTI format.",
+)
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/cli_param/option_group.py` & `clinicadl-1.3.0/clinicadl/utils/cli_param/option_group.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/descriptors.py` & `clinicadl-1.3.0/clinicadl/utils/descriptors.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/early_stopping.py` & `clinicadl-1.3.0/clinicadl/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/exceptions.py` & `clinicadl-1.3.0/clinicadl/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/logger.py` & `clinicadl-1.3.0/clinicadl/utils/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import sys
-from os import getcwd, path
+from pathlib import Path
 
 
 class StdLevelFilter(logging.Filter):
     def __init__(self, err=False):
         super().__init__()
         self.err = err
 
@@ -12,32 +12,33 @@
         if record.levelno <= logging.WARNING:
             return not self.err
         return self.err
 
 
 # Create formatter for console
 class ConsoleFormatter(logging.Formatter):
-
     FORMATS = {
         logging.INFO: "%(asctime)s - %(message)s",
         logging.WARNING: "%(asctime)s - %(levelname)s: %(message)s",
     }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt, "%H:%M:%S")
         return formatter.format(record)
 
 
 def setup_logging(verbose: bool = False) -> None:
     """
     Setup ClinicaDL's logging facilities.
-    Args:
-        verbose: The desired level of verbosity for logging.
-            (False (default): INFO, True: DEBUG)
+    Parameters
+    ----------
+    verbose: bool
+        The desired level of verbosity for logging.
+        (False (default): INFO, True: DEBUG)
     """
     logging_level = "DEBUG" if verbose else "INFO"
 
     # Define the module level logger.
     logger = logging.getLogger("clinicadl")
     logger.setLevel(logging_level)
 
@@ -63,11 +64,9 @@
             "%(asctime)s - %(name)s - %(levelname)s: %(message)s", "%Y-%m-%d %H:%M:%S"
         )
         debug_file_name = "clinicadl_debug.log"
         file_handler = logging.FileHandler(debug_file_name)
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(debug_file_formatter)
         logger.addHandler(file_handler)
-        print(getcwd())
-        logger.warning(
-            f"Debug log will be saved at {path.join(getcwd(), debug_file_name)}"
-        )
+        print(Path.cwd())
+        logger.warning(f"Debug log will be saved at {Path.cwd() / debug_file_name}")
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/maps_manager/iotools.py` & `clinicadl-1.3.0/clinicadl/utils/maps_manager/iotools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # coding: utf8
 import logging
+from pathlib import Path, PosixPath
 
 from clinicadl.utils.exceptions import ClinicaDLArgumentError
 
 LOG_LEVELS = [logging.WARNING, logging.INFO, logging.DEBUG]
 
 
 computational_list = ["gpu", "batch_size", "n_proc", "evaluation_steps"]
 
 
-def write_requirements_version(output_path):
+def write_requirements_version(output_path: Path):
     import subprocess
-    from os import path
     from warnings import warn
 
     try:
         env_variables = subprocess.check_output("pip freeze", shell=True).decode(
             "utf-8"
         )
-        with open(path.join(output_path, "environment.txt"), "w") as file:
+        with (output_path / "environment.txt").open(mode="w") as file:
             file.write(env_variables)
     except subprocess.CalledProcessError:
         warn(
             "You do not have the right to execute pip freeze. Your environment will not be written"
         )
 
 
-def check_and_clean(d):
-    import os
+def check_and_clean(directory_path: Path):
     import shutil
 
-    if os.path.exists(d):
-        shutil.rmtree(d)
-    os.makedirs(d)
+    if directory_path.is_dir():
+        shutil.rmtree(directory_path)
+    directory_path.mkdir(parents=True)
 
 
 def commandline_to_json(commandline, logger=None, filename="commandline.json"):
     """
     This is a function to write the python argparse object into a json file.
     This helps for DL when searching for hyperparameters
     Args:
@@ -46,63 +45,68 @@
 
     :return:
     """
     if logger is None:
         logger = logging
 
     import json
-    import os
     from copy import copy
 
     if isinstance(commandline, dict):
         commandline_arg_dict = copy(commandline)
     else:
         commandline_arg_dict = copy(vars(commandline))
     output_dir = commandline_arg_dict["output_dir"]
-    os.makedirs(output_dir, exist_ok=True)
+    output_dir.mkdir(parents=True, exist_ok=True)
 
     # remove these entries from the commandline log file
     remove_list = ["func", "output_dir", "launch_dir", "name", "verbose", "logname"]
     for variable in remove_list:
         if variable in commandline_arg_dict:
             del commandline_arg_dict[variable]
 
+    # change path to str for json.dumps
+    for key, value in commandline_arg_dict.items():
+        if isinstance(value, PosixPath):
+            commandline_arg_dict[key] = value.as_posix()
+
     # save to json file
-    json = json.dumps(commandline_arg_dict, skipkeys=True, indent=4)
-    logger.info(f"Path of json file: {os.path.join(output_dir, 'commandline.json')}")
-    f = open(os.path.join(output_dir, filename), "w")
+    json = json.dumps(commandline_arg_dict, skipkeys=True, ensure_ascii=False, indent=4)
+    logger.info(f"Path of json file: {output_dir / 'commandline.json'}")
+    f = open(output_dir / filename, "w")
     f.write(json)
     f.close()
 
 
-def read_json(options=None, json_path=None, test=False, read_computational=False):
+def read_json(
+    options=None, json_path: Path = None, test=False, read_computational=False
+):
     """
     Read a json file to update options dictionary.
     Ensures retro-compatibility with previous namings in clinicadl.
 
     Args:
         options: (dict) options of the model.
         json_path: (str) If given path to the json file, else found with options.model_path.
         test: (bool) If given the reader will ignore some options specific to data.
         read_computational: (bool) if set to True, the computational arguments are also read.
     Returns:
         options (dict) options of the model updated
     """
     import json
-    from os import path
 
     if options is None:
         options = {}
 
     evaluation_parameters = ["diagnosis_path", "input_dir", "diagnoses"]
     prep_compatibility_dict = {"mni": "t1-extensive", "linear": "t1-linear"}
     if json_path is None:
-        json_path = path.join(options["model_path"], "commandline.json")
+        json_path = options["model_path"] / "commandline.json"
 
-    with open(json_path, "r") as f:
+    with json_path.open(mode="r") as f:
         json_data = json.load(f)
 
     for key, item in json_data.items():
         # We do not change computational options
         if key in computational_list and not read_computational:
             pass
         # If used for evaluation, some parameters were already given
@@ -340,19 +344,21 @@
         ):
             print(type(obj), obj.size(), obj.is_cuda)
             cnt_tensor += 1
     print("Count: ", cnt_tensor)
 
 
 def cpuStats():
-    import os
+    import multiprocessing
     import sys
 
     import psutil
 
     print(sys.version)
     print(psutil.cpu_percent())
     print(psutil.virtual_memory())  # physical memory usage
-    pid = os.getpid()
+    process = multiprocessing.current_process()
+    pid = process.pid
+
     py = psutil.Process(pid)
     memoryUse = py.memory_info()[0] / 2.0**30  # memory use in GB...I think
     print("memory GB:", memoryUse)
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/maps_manager/logwriter.py` & `clinicadl-1.3.0/clinicadl/utils/maps_manager/logwriter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from os import makedirs, path
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 
 class LogWriter:
     """
     Write training logs in the MAPS
     """
 
     def __init__(
         self,
-        maps_path,
+        maps_path: Path,
         evaluation_metrics,
         split,
         resume=False,
         beginning_epoch=0,
         network=None,
     ):
         from time import time
@@ -30,47 +30,43 @@
             selection.split("-")[0] + "_valid" for selection in evaluation_metrics
         ]
         self.columns = ["epoch", "iteration", "time"] + columns_train + columns_valid
 
         self.evaluation_metrics = evaluation_metrics
         self.maps_path = maps_path
 
-        self.file_dir = path.join(self.maps_path, f"split-{split}", "training_logs")
+        self.file_dir = self.maps_path / f"split-{split}" / "training_logs"
         if network is not None:
-            self.file_dir = path.join(self.file_dir, f"network-{network}")
-        makedirs(self.file_dir, exist_ok=True)
-        tsv_path = path.join(self.file_dir, "training.tsv")
+            self.file_dir = self.file_dir / f"network-{network}"
+        self.file_dir.mkdir(parents=True, exist_ok=True)
+        tsv_path = self.file_dir / "training.tsv"
 
         self.beginning_epoch = beginning_epoch
         if not resume:
             results_df = pd.DataFrame(columns=self.columns)
-            with open(tsv_path, "w") as f:
+            with tsv_path.open(mode="w") as f:
                 results_df.to_csv(f, index=False, sep="\t")
             self.beginning_time = time()
         else:
-            if not path.exists(tsv_path):
+            if not tsv_path.is_file():
                 raise FileNotFoundError(
                     f"The training.tsv file of the split {split} in the MAPS "
                     f"{self.maps_path} does not exist."
                 )
             truncated_tsv = pd.read_csv(tsv_path, sep="\t")
             truncated_tsv.set_index(["epoch", "iteration"], inplace=True)
             truncated_tsv.drop(self.beginning_epoch, level=0, inplace=True)
             if len(truncated_tsv) == 0:
                 self.beginning_time = 0
             else:
                 self.beginning_time = time() + truncated_tsv.iloc[-1, 0]
             truncated_tsv.to_csv(tsv_path, index=True, sep="\t")
 
-        self.writer_train = SummaryWriter(
-            path.join(self.file_dir, "tensorboard", "train")
-        )
-        self.writer_valid = SummaryWriter(
-            path.join(self.file_dir, "tensorboard", "validation")
-        )
+        self.writer_train = SummaryWriter(self.file_dir / "tensorboard" / "train")
+        self.writer_valid = SummaryWriter(self.file_dir / "tensorboard" / "validation")
 
     def step(self, epoch, i, metrics_train, metrics_valid, len_epoch):
         """
         Write a new row on the output file training.tsv.
 
         Args:
             epoch (int): current epoch number
@@ -78,15 +74,15 @@
             metrics_train (Dict[str:float]): metrics on the training set
             metrics_valid (Dict[str:float]): metrics on the validation set
             len_epoch (int): number of iterations in an epoch
         """
         from time import time
 
         # Write TSV file
-        tsv_path = path.join(self.file_dir, "training.tsv")
+        tsv_path = self.file_dir / "training.tsv"
 
         t_current = time() - self.beginning_time
         general_row = [epoch, i, t_current]
         train_row = list()
         valid_row = list()
         for selection in self.evaluation_metrics:
             if selection in metrics_train:
@@ -105,15 +101,15 @@
                     if selection in key
                 ]
                 train_row.append(np.mean(train_values))
                 valid_row.append(np.mean(valid_values))
 
         row = [general_row + train_row + valid_row]
         row_df = pd.DataFrame(row, columns=self.columns)
-        with open(tsv_path, "a") as f:
+        with tsv_path.open(mode="a") as f:
             row_df.to_csv(f, header=False, index=False, sep="\t")
 
         # Write tensorboard logs
         global_step = i + epoch * len_epoch
         for metric_idx, metric in enumerate(self.evaluation_metrics):
             self.writer_train.add_scalar(
                 metric,
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/maps_manager/maps_manager.py` & `clinicadl-1.3.0/clinicadl/utils/maps_manager/maps_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
-import os
 import shutil
 import subprocess
 from datetime import datetime
 from glob import glob
 from logging import getLogger
-from os import listdir, makedirs, path
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import torch
 from torch.utils.data import DataLoader
 
 from clinicadl.utils.caps_dataset.data import (
@@ -25,14 +24,16 @@
     ClinicaDLDataLeakageError,
     MAPSError,
 )
 from clinicadl.utils.logger import setup_logging
 from clinicadl.utils.maps_manager.logwriter import LogWriter
 from clinicadl.utils.maps_manager.maps_manager_utils import (
     add_default_values,
+    change_path_to_str,
+    change_str_to_path,
     read_json,
 )
 from clinicadl.utils.metric_module import RetainBest
 from clinicadl.utils.network.network import Network
 from clinicadl.utils.seed import get_seed, pl_worker_init_function, seed_everything
 
 logger = getLogger("clinicadl.maps_manager")
@@ -41,65 +42,69 @@
 level_list: List[str] = ["warning", "info", "debug"]
 # TODO save weights on CPU for better compatibility
 
 
 class MapsManager:
     def __init__(
         self,
-        maps_path: str,
+        maps_path: Path,
         parameters: Dict[str, Any] = None,
         verbose: str = "info",
     ):
         """
 
         Parameters
         ----------
         maps_path: str (path)
-            path of the MAPS
+            Path of the MAPS
         parameters: Dict[str, Any]
-            parameters of the training step. If given a new MAPS is created.
+            Parameters of the training step. If given a new MAPS is created.
         verbose: str
             Logging level ("debug", "info", "warning")
         """
-        self.maps_path = path.abspath(maps_path)
+        self.maps_path = maps_path.resolve()
         if verbose is not None:
             if verbose not in level_list:
                 raise ValueError(f"verbose value {verbose} must be in {level_list}.")
             setup_logging(level_list.index(verbose))
 
         # Existing MAPS
         if parameters is None:
-            if not path.exists(path.join(maps_path, "maps.json")):
+            if not (maps_path / "maps.json").is_file():
                 raise MAPSError(
                     f"MAPS was not found at {maps_path}."
                     f"To initiate a new MAPS please give a train_dict."
                 )
-            self.parameters = self.get_parameters()
+            test_parameters = self.get_parameters()
+            self.parameters = change_str_to_path(test_parameters)
             self.task_manager = self._init_task_manager(n_classes=self.output_size)
             self.split_name = (
                 self._check_split_wording()
             )  # Used only for retro-compatibility
 
         # Initiate MAPS
         else:
-            if (
-                path.exists(maps_path) and not path.isdir(maps_path)  # Non-folder file
-            ) or (
-                path.isdir(maps_path) and listdir(maps_path)  # Non empty folder
+            self._check_args(parameters)
+            print(parameters)
+            parameters["tsv_path"] = Path(parameters["tsv_path"])
+
+            if (maps_path.is_dir() and maps_path.is_file()) or (  # Non-folder file
+                maps_path.is_dir() and list(maps_path.iterdir())  # Non empty folder
             ):
                 raise MAPSError(
                     f"You are trying to create a new MAPS at {maps_path} but "
                     f"this already corresponds to a file or a non-empty folder. \n"
                     f"Please remove it or choose another location."
                 )
-            makedirs(path.join(self.maps_path, "groups"))
+            (maps_path / "groups").mkdir(parents=True)
 
             logger.info(f"A new MAPS was created at {maps_path}")
-            self._check_args(parameters)
+
             self.write_parameters(self.maps_path, self.parameters)
+
             self._write_requirements_version()
 
             self.split_name = "split"  # Used only for retro-compatibility
             self._write_training_data()
             self._write_train_val_groups()
             self._write_information()
 
@@ -123,16 +128,16 @@
         Raises:
             MAPSError: If splits specified in input already exist and overwrite is False.
         """
         existing_splits = []
 
         split_manager = self._init_split_manager(split_list)
         for split in split_manager.split_iterator():
-            split_path = path.join(self.maps_path, f"{self.split_name}-{split}")
-            if path.exists(split_path):
+            split_path = self.maps_path / f"{self.split_name}-{split}"
+            if split_path.is_dir():
                 if overwrite:
                     shutil.rmtree(split_path)
                 else:
                     existing_splits.append(split)
 
         if len(existing_splits) > 0:
             raise MAPSError(
@@ -156,17 +161,15 @@
         Raises:
             MAPSError: If splits specified in input do not exist.
         """
         missing_splits = []
         split_manager = self._init_split_manager(split_list)
 
         for split in split_manager.split_iterator():
-            if not path.exists(
-                path.join(self.maps_path, f"{self.split_name}-{split}", "tmp")
-            ):
+            if not (self.maps_path / f"{self.split_name}-{split}" / "tmp").is_dir():
                 missing_splits.append(split)
 
         if len(missing_splits) > 0:
             raise MAPSError(
                 f"Splits {missing_splits} were not initialized. "
                 f"Please try train command on these splits and resume only others."
             )
@@ -175,16 +178,16 @@
             self._train_multi(split_list, resume=True)
         else:
             self._train_single(split_list, resume=True)
 
     def predict(
         self,
         data_group: str,
-        caps_directory: str = None,
-        tsv_path: str = None,
+        caps_directory: Path = None,
+        tsv_path: Path = None,
         split_list: List[int] = None,
         selection_metrics: List[str] = None,
         multi_cohort: bool = False,
         diagnoses: List[str] = (),
         use_labels: bool = True,
         batch_size: int = None,
         n_proc: int = None,
@@ -253,23 +256,25 @@
 
             # Erase previous TSV files
             if selection_metrics is None:
                 split_selection_metrics = self._find_selection_metrics(split)
             else:
                 split_selection_metrics = selection_metrics
             for selection in split_selection_metrics:
-                tsv_pattern = path.join(
-                    self.maps_path,
-                    f"{self.split_name}-{split}",
-                    f"best-{selection}",
-                    data_group,
-                    f"{data_group}*.tsv",
+                tsv_dir = (
+                    self.maps_path
+                    / f"{self.split_name}-{split}"
+                    / f"best-{selection}"
+                    / data_group
                 )
-                for tsv_file in glob(tsv_pattern):
-                    os.remove(tsv_file)
+
+                tsv_pattern = f"{data_group}*.tsv"
+
+                for tsv_file in tsv_dir.glob(tsv_pattern):
+                    tsv_file.unlink()
 
             if self.multi_network:
                 for network in range(self.num_networks):
                     data_test = return_dataset(
                         group_parameters["caps_directory"],
                         group_df,
                         self.preprocessing_dict,
@@ -368,55 +373,77 @@
             self._ensemble_prediction(data_group, split, selection_metrics, use_labels)
 
     def interpret(
         self,
         data_group,
         name,
         method,
-        caps_directory=None,
-        tsv_path=None,
+        caps_directory: Path = None,
+        tsv_path: Path = None,
         split_list=None,
         selection_metrics=None,
         multi_cohort=False,
         diagnoses=(),
         target_node=0,
         save_individual=False,
         batch_size=None,
         n_proc=None,
         gpu=None,
         overwrite=False,
         overwrite_name=False,
         level=None,
+        save_nifti=False,
     ):
         """
         Performs the interpretation task on a subset of caps_directory defined in a TSV file.
         The mean interpretation is always saved, to save the individual interpretations set save_individual to True.
-        Args:
-            data_group (str): name of the data group interpreted.
-            name (str): name of the interpretation procedure.
-            method (str): method used for extraction (ex: gradients, grad-cam...).
-            caps_directory (str): path to the CAPS folder. For more information please refer to
-                [clinica documentation](https://aramislab.paris.inria.fr/clinica/docs/public/latest/CAPS/Introduction/).
-                Default will load the value of an existing data group.
-            tsv_path (str): path to a TSV file containing the list of participants and sessions to test.
-                Default will load the DataFrame of an existing data group.
-            split_list (list[int]): list of splits to interpret. Default perform interpretation on all splits available.
-            selection_metrics (list[str]): list of selection metrics to interpret.
-                Default performs the interpretation on all selection metrics available.
-            multi_cohort (bool): If True considers that tsv_path is the path to a multi-cohort TSV.
-            diagnoses (list[str]): List of diagnoses to load if tsv_path is a split_directory.
-                Default uses the same as in training step.
-            target_node (int): Node from which the interpretation is computed.
-            save_individual (bool): If True saves the individual map of each participant / session couple.
-            batch_size (int): If given, sets the value of batch_size, else use the same as in training step.
-            n_proc (int): If given, sets the value of num_workers, else use the same as in training step.
-            gpu (bool): If given, a new value for the device of the model will be computed.
-            overwrite (bool): If True erase the occurrences of data_group.
-            overwrite_name (bool): If True erase the occurrences of name.
-            level (int): layer number in the convolutional part after which the feature map is chosen.
+
+        Parameters
+        ----------
+        data_group: str
+            Name of the data group interpreted.
+        name: str
+            Name of the interpretation procedure.
+        method: str
+            Method used for extraction (ex: gradients, grad-cam...).
+        caps_directory: str (Path)
+            Path to the CAPS folder. For more information please refer to
+            [clinica documentation](https://aramislab.paris.inria.fr/clinica/docs/public/latest/CAPS/Introduction/).
+            Default will load the value of an existing data group.
+        tsv_path: str (Path)
+            Path to a TSV file containing the list of participants and sessions to test.
+            Default will load the DataFrame of an existing data group.
+        split_list: list of int
+            List of splits to interpret. Default perform interpretation on all splits available.
+        selection_metrics: list of str
+            List of selection metrics to interpret.
+            Default performs the interpretation on all selection metrics available.
+        multi_cohort: bool
+            If True considers that tsv_path is the path to a multi-cohort TSV.
+        diagnoses: list of str
+            List of diagnoses to load if tsv_path is a split_directory.
+            Default uses the same as in training step.
+        target_node: int
+            Node from which the interpretation is computed.
+        save_individual: bool
+            If True saves the individual map of each participant / session couple.
+        batch_size: int
+            If given, sets the value of batch_size, else use the same as in training step.
+        n_proc: int
+            If given, sets the value of num_workers, else use the same as in training step.
+        gpu: bool
+            If given, a new value for the device of the model will be computed.
+        overwrite: bool
+            If True erase the occurrences of data_group.
+        overwrite_name: bool
+            If True erase the occurrences of name.
+        level: int
+            Layer number in the convolutional part after which the feature map is chosen.
+        save_nifi : bool
+            If True, save the interpretation map in nifti format.
         """
 
         from torch.utils.data import DataLoader
 
         from clinicadl.interpret.gradients import method_dict
 
         if method not in method_dict.keys():
@@ -472,31 +499,31 @@
             )
 
             if selection_metrics is None:
                 selection_metrics = self._find_selection_metrics(split)
 
             for selection_metric in selection_metrics:
                 logger.info(f"Interpretation of metric {selection_metric}")
-                results_path = path.join(
-                    self.maps_path,
-                    f"{self.split_name}-{split}",
-                    f"best-{selection_metric}",
-                    data_group,
-                    f"interpret-{name}",
+                results_path = (
+                    self.maps_path
+                    / f"{self.split_name}-{split}"
+                    / f"best-{selection_metric}"
+                    / data_group
+                    / f"interpret-{name}"
                 )
 
-                if path.exists(results_path):
+                if (results_path).is_dir():
                     if overwrite_name:
                         shutil.rmtree(results_path)
                     else:
                         raise MAPSError(
                             f"Interpretation name {name} is already written. "
                             f"Please choose another name or set overwrite_name to True."
                         )
-                makedirs(results_path)
+                results_path.mkdir(parents=True)
 
                 model, _ = self._init_model(
                     transfer_path=self.maps_path,
                     split=split,
                     transfer_selection=selection_metric,
                     gpu=gpu,
                 )
@@ -510,26 +537,47 @@
                     map_pt = interpreter.generate_gradients(
                         images, target_node, level=level
                     )
                     for i in range(len(data["participant_id"])):
                         mode_id = data[f"{self.mode}_id"][i]
                         cum_maps[mode_id] += map_pt[i]
                         if save_individual:
-                            single_path = path.join(
-                                results_path,
-                                f"{data['participant_id'][i]}_{data['session_id'][i]}_"
-                                f"{self.mode}-{data[f'{self.mode}_id'][i]}_map.pt",
+                            single_path = (
+                                results_path
+                                / f"{data['participant_id'][i]}_{data['session_id'][i]}_{self.mode}-{data[f'{self.mode}_id'][i]}_map.pt"
                             )
                             torch.save(map_pt[i], single_path)
+                            if save_nifti:
+                                import nibabel as nib
+                                from numpy import eye
+
+                                single_nifti_path = (
+                                    results_path
+                                    / f"{data['participant_id'][i]}_{data['session_id'][i]}_{self.mode}-{data[f'{self.mode}_id'][i]}_map.nii.gz"
+                                )
+
+                                output_nii = nib.Nifti1Image(map_pt[i].numpy(), eye(4))
+                                nib.save(output_nii, single_nifti_path)
+
                 for i, mode_map in enumerate(cum_maps):
                     mode_map /= len(data_test)
+
                     torch.save(
                         mode_map,
-                        path.join(results_path, f"mean_{self.mode}-{i}_map.pt"),
+                        results_path / f"mean_{self.mode}-{i}_map.pt",
                     )
+                    if save_nifti:
+                        import nibabel as nib
+                        from numpy import eye
+
+                        output_nii = nib.Nifti1Image(mode_map, eye(4))
+                        nib.save(
+                            output_nii,
+                            results_path / f"mean_{self.mode}-{i}_map.nii.gz",
+                        )
 
     ###################################
     # High-level functions templates  #
     ###################################
     def _train_single(self, split_list=None, resume=False):
         """
         Trains a single CNN for all inputs.
@@ -635,24 +683,24 @@
 
             split_df_dict = split_manager[split]
 
             first_network = 0
             if resume:
                 training_logs = [
                     int(network_folder.split("-")[1])
-                    for network_folder in listdir(
-                        path.join(
-                            self.maps_path,
-                            f"{self.split_name}-{split}",
-                            "training_logs",
-                        )
+                    for network_folder in list(
+                        (
+                            self.maps_path
+                            / f"{self.split_name}-{split}"
+                            / "training_logs"
+                        ).iterdir()
                     )
                 ]
                 first_network = max(training_logs)
-                if not path.exists(path.join(self.maps_path, "tmp")):
+                if not (self.maps_path / "tmp").is_dir():
                     first_network += 1
                     resume = False
 
             for network in range(first_network, self.num_networks):
                 logger.info(f"Train network {network}")
 
                 data_train = return_dataset(
@@ -677,15 +725,14 @@
                     label_code=self.label_code,
                     cnn_index=network,
                 )
 
                 train_sampler = self.task_manager.generate_sampler(
                     data_train, self.sampler
                 )
-
                 train_loader = DataLoader(
                     data_train,
                     batch_size=self.batch_size,
                     sampler=train_sampler,
                     num_workers=self.n_proc,
                     worker_init_fn=pl_worker_init_function,
                 )
@@ -765,66 +812,70 @@
             beginning_epoch=beginning_epoch,
             network=network,
         )
         epoch = log_writer.beginning_epoch
 
         retain_best = RetainBest(selection_metrics=list(self.selection_metrics))
 
+        profiler = self._init_profiler()
+
         while epoch < self.epochs and not early_stopping.step(metrics_valid["loss"]):
             logger.info(f"Beginning epoch {epoch}.")
 
             model.zero_grad()
             evaluation_flag, step_flag = True, True
 
-            for i, data in enumerate(train_loader):
+            with profiler:
+                for i, data in enumerate(train_loader):
+                    _, loss_dict = model.compute_outputs_and_loss(data, criterion)
+                    logger.debug(f"Train loss dictionnary {loss_dict}")
+                    loss = loss_dict["loss"]
+                    loss.backward()
+
+                    if (i + 1) % self.accumulation_steps == 0:
+                        step_flag = False
+                        optimizer.step()
+                        optimizer.zero_grad()
+
+                        del loss
+
+                        # Evaluate the model only when no gradients are accumulated
+                        if (
+                            self.evaluation_steps != 0
+                            and (i + 1) % self.evaluation_steps == 0
+                        ):
+                            evaluation_flag = False
 
-                _, loss_dict = model.compute_outputs_and_loss(data, criterion)
-                logger.debug(f"Train loss dictionnary {loss_dict}")
-                loss = loss_dict["loss"]
-                loss.backward()
-
-                if (i + 1) % self.accumulation_steps == 0:
-                    step_flag = False
-                    optimizer.step()
-                    optimizer.zero_grad()
-
-                    del loss
-
-                    # Evaluate the model only when no gradients are accumulated
-                    if (
-                        self.evaluation_steps != 0
-                        and (i + 1) % self.evaluation_steps == 0
-                    ):
-                        evaluation_flag = False
+                            _, metrics_train = self.task_manager.test(
+                                model, train_loader, criterion
+                            )
+                            _, metrics_valid = self.task_manager.test(
+                                model, valid_loader, criterion
+                            )
 
-                        _, metrics_train = self.task_manager.test(
-                            model, train_loader, criterion
-                        )
-                        _, metrics_valid = self.task_manager.test(
-                            model, valid_loader, criterion
-                        )
+                            model.train()
+                            train_loader.dataset.train()
 
-                        model.train()
-                        train_loader.dataset.train()
+                            log_writer.step(
+                                epoch,
+                                i,
+                                metrics_train,
+                                metrics_valid,
+                                len(train_loader),
+                            )
+                            logger.info(
+                                f"{self.mode} level training loss is {metrics_train['loss']} "
+                                f"at the end of iteration {i}"
+                            )
+                            logger.info(
+                                f"{self.mode} level validation loss is {metrics_valid['loss']} "
+                                f"at the end of iteration {i}"
+                            )
 
-                        log_writer.step(
-                            epoch,
-                            i,
-                            metrics_train,
-                            metrics_valid,
-                            len(train_loader),
-                        )
-                        logger.info(
-                            f"{self.mode} level training loss is {metrics_train['loss']} "
-                            f"at the end of iteration {i}"
-                        )
-                        logger.info(
-                            f"{self.mode} level validation loss is {metrics_valid['loss']} "
-                            f"at the end of iteration {i}"
-                        )
+                    profiler.step()
 
             # If no step has been performed, raise Exception
             if step_flag:
                 raise Exception(
                     "The model has not been updated once in the epoch. The accumulation step may be too large."
                 )
 
@@ -942,20 +993,19 @@
             split (int): Index of the split used to train the model tested.
             selection_metrics (list[str]): List of metrics used to select the best models which are tested.
             use_labels (bool): If True, the labels must exist in test meta-data and metrics are computed.
             gpu (bool): If given, a new value for the device of the model will be computed.
             network (int): Index of the network tested (only used in multi-network setting).
         """
         for selection_metric in selection_metrics:
-
-            log_dir = path.join(
-                self.maps_path,
-                f"{self.split_name}-{split}",
-                f"best-{selection_metric}",
-                data_group,
+            log_dir = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / f"best-{selection_metric}"
+                / data_group
             )
             self.write_description_log(
                 log_dir,
                 data_group,
                 dataloader.dataset.caps_dict,
                 dataloader.dataset.df,
             )
@@ -964,15 +1014,14 @@
             model, _ = self._init_model(
                 transfer_path=self.maps_path,
                 split=split,
                 transfer_selection=selection_metric,
                 gpu=gpu,
                 network=network,
             )
-
             prediction_df, metrics = self.task_manager.test(
                 model, dataloader, criterion, use_labels=use_labels
             )
             if use_labels:
                 if network is not None:
                     metrics[f"{self.mode}_id"] = network
                 logger.info(
@@ -1014,22 +1063,22 @@
                 transfer_path=self.maps_path,
                 split=split,
                 transfer_selection=selection_metric,
                 gpu=gpu,
                 network=network,
             )
 
-            nifti_path = path.join(
-                self.maps_path,
-                f"{self.split_name}-{split}",
-                f"best-{selection_metric}",
-                data_group,
-                "nifti_images",
+            nifti_path = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / f"best-{selection_metric}"
+                / data_group
+                / "nifti_images"
             )
-            makedirs(nifti_path, exist_ok=True)
+            nifti_path.mkdir(parents=True, exist_ok=True)
 
             nb_imgs = len(dataset)
             for i in range(nb_imgs):
                 data = dataset[i]
                 image = data["image"]
                 output = (
                     model.predict(image.unsqueeze(0).to(model.device))
@@ -1041,16 +1090,16 @@
                 input_nii = nib.Nifti1Image(image[0].detach().cpu().numpy(), eye(4))
                 output_nii = nib.Nifti1Image(output[0].numpy(), eye(4))
                 # Create file name according to participant and session id
                 participant_id = data["participant_id"]
                 session_id = data["session_id"]
                 input_filename = f"{participant_id}_{session_id}_image_input.nii.gz"
                 output_filename = f"{participant_id}_{session_id}_image_output.nii.gz"
-                nib.save(input_nii, path.join(nifti_path, input_filename))
-                nib.save(output_nii, path.join(nifti_path, output_filename))
+                nib.save(input_nii, nifti_path / input_filename)
+                nib.save(output_nii, nifti_path / output_filename)
 
     def _compute_output_tensors(
         self,
         dataset,
         data_group,
         split,
         selection_metrics,
@@ -1076,22 +1125,22 @@
                 transfer_path=self.maps_path,
                 split=split,
                 transfer_selection=selection_metric,
                 gpu=gpu,
                 network=network,
             )
 
-            tensor_path = path.join(
-                self.maps_path,
-                f"{self.split_name}-{split}",
-                f"best-{selection_metric}",
-                data_group,
-                "tensors",
+            tensor_path = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / f"best-{selection_metric}"
+                / data_group
+                / "tensors"
             )
-            makedirs(tensor_path, exist_ok=True)
+            tensor_path.mkdir(parents=True, exist_ok=True)
 
             if nb_images is None:  # Compute outputs for the whole data set
                 nb_modes = len(dataset)
             else:
                 nb_modes = nb_images * dataset.elem_per_image
 
             for i in range(nb_modes):
@@ -1105,16 +1154,16 @@
                 mode_id = data[f"{self.mode}_id"]
                 input_filename = (
                     f"{participant_id}_{session_id}_{self.mode}-{mode_id}_input.pt"
                 )
                 output_filename = (
                     f"{participant_id}_{session_id}_{self.mode}-{mode_id}_output.pt"
                 )
-                torch.save(image, path.join(tensor_path, input_filename))
-                torch.save(output, path.join(tensor_path, output_filename))
+                torch.save(image, tensor_path / input_filename)
+                torch.save(output, tensor_path / output_filename)
 
     def _ensemble_prediction(
         self,
         data_group,
         split,
         selection_metrics,
         use_labels=True,
@@ -1152,23 +1201,22 @@
         mandatory_arguments = [
             "caps_directory",
             "tsv_path",
             "preprocessing_dict",
             "mode",
             "network_task",
         ]
-
         for arg in mandatory_arguments:
             if arg not in parameters:
                 raise ClinicaDLArgumentError(
                     f"The values of mandatory arguments {mandatory_arguments} should be set. "
                     f"No value was given for {arg}."
                 )
-        parameters = add_default_values(parameters)
-        self.parameters = parameters
+        self.parameters = add_default_values(parameters)
+        self.parameters = change_str_to_path(parameters)
         if self.parameters["gpu"]:
             check_gpu()
 
         _, transformations = get_transforms(self.normalize)
 
         split_manager = self._init_split_manager(None)
         train_df = split_manager[0]["train"]
@@ -1226,42 +1274,42 @@
                 f"Selection metrics {self.parameters['selection_metrics']} "
                 f"must be a subset of metrics used for evaluation "
                 f"{possible_selection_metrics_set}."
             )
 
     def _check_split_wording(self):
         """Finds if MAPS structure uses 'fold-X' or 'split-X' folders."""
-        from glob import glob
 
-        if len(glob(path.join(self.maps_path, "fold-*"))) > 0:
+        if len(list(self.maps_path.glob("fold-*"))) > 0:
             return "fold"
         else:
             return "split"
 
     def _find_splits(self):
         """Find which splits were trained in the MAPS."""
         return [
-            int(split.split("-")[1])
-            for split in listdir(self.maps_path)
-            if split.startswith(f"{self.split_name}-")
+            int(split.name.split("-")[1])
+            for split in list(self.maps_path.iterdir())
+            if split.name.startswith(f"{self.split_name}-")
         ]
 
     def _find_selection_metrics(self, split):
         """Find which selection metrics are available in MAPS for a given split."""
-        split_path = path.join(self.maps_path, f"{self.split_name}-{split}")
-        if not path.exists(split_path):
+
+        split_path = self.maps_path / f"{self.split_name}-{split}"
+        if not split_path.is_dir():
             raise MAPSError(
                 f"Training of split {split} was not performed."
                 f"Please execute maps_manager.train(split_list=[{split}])"
             )
 
         return [
-            metric.split("-")[1]
-            for metric in listdir(split_path)
-            if metric[:5:] == "best-"
+            metric.name.split("-")[1]
+            for metric in list(split_path.iterdir())
+            if metric.name[:5:] == "best-"
         ]
 
     def _check_selection_metric(self, split, selection_metric=None):
         """Check that a given selection metric is available for a given split."""
         available_metrics = self._find_selection_metrics(split)
         if selection_metric is None:
             if len(available_metrics) > 1:
@@ -1287,15 +1335,15 @@
             data_group (str): name of the data group
             test_df (pd.DataFrame): Table of participant_id / session_id of the data group
         Raises:
             ClinicaDLDataLeakageError: if data_group not in ["train", "validation"] and there is an intersection
                 between the participant IDs in test_df and the ones used for training.
         """
         if data_group not in ["train", "validation"]:
-            train_path = path.join(self.maps_path, "groups", "train+validation.tsv")
+            train_path = self.maps_path / "groups" / "train+validation.tsv"
             train_df = pd.read_csv(train_path, sep="\t")
             participants_train = set(train_df.participant_id.values)
             participants_test = set(test_df.participant_id.values)
             intersection = participants_test & participants_train
 
             if len(intersection) > 0:
                 raise ClinicaDLDataLeakageError(
@@ -1327,81 +1375,87 @@
 
         Raises:
             MAPSError when trying to overwrite train or validation data groups
             ClinicaDLArgumentError:
                 when caps_directory or df are given but data group already exists
                 when caps_directory or df are not given and data group does not exist
         """
-        group_path = path.join(self.maps_path, "groups", data_group)
-        logger.debug(f"Group path {group_path}")
-        if path.exists(group_path):  # Data group already exists
+        group_dir = self.maps_path / "groups" / data_group
+        logger.debug(f"Group path {group_dir}")
+        if group_dir.is_dir():  # Data group already exists
             if overwrite:
                 if data_group in ["train", "validation"]:
                     raise MAPSError("Cannot overwrite train or validation data group.")
                 else:
-                    shutil.rmtree(group_path)
+                    shutil.rmtree(group_dir)
                     split_list = self._find_splits()
                     for split in split_list:
                         selection_metrics = self._find_selection_metrics(split)
                         for selection in selection_metrics:
-                            results_path = path.join(
-                                self.maps_path,
-                                f"{self.split_name}-{split}",
-                                f"best-{selection}",
-                                data_group,
+                            results_path = (
+                                self.maps_path
+                                / f"{self.split_name}-{split}"
+                                / f"best-{selection}"
+                                / data_group
                             )
-                            if path.exists(results_path):
+                            if results_path.is_dir():
                                 shutil.rmtree(results_path)
             elif df is not None or caps_directory is not None:
                 raise ClinicaDLArgumentError(
                     f"Data group {data_group} is already defined. "
                     f"Please do not give any caps_directory, tsv_path or multi_cohort to use it. "
                     f"To erase {data_group} please set overwrite to True."
                 )
 
-        if not path.exists(group_path) and (
+        if not group_dir.is_dir() and (
             caps_directory is None or df is None
         ):  # Data group does not exist yet / was overwritten + missing data
             raise ClinicaDLArgumentError(
                 f"The data group {data_group} does not already exist. "
                 f"Please specify a caps_directory and a tsv_path to create this data group."
             )
-        elif not path.exists(
-            group_path
+        elif (
+            not group_dir.is_dir()
         ):  # Data group does not exist yet / was overwritten + all data is provided
             self._check_leakage(data_group, df)
             self._write_data_group(
                 data_group, df, caps_directory, multi_cohort, label=label
             )
 
     ###############################
     # File writers                #
     ###############################
     @staticmethod
-    def write_parameters(json_path, parameters, verbose=True):
+    def write_parameters(json_path: Path, parameters, verbose=True):
+        from pathlib import PosixPath
+
         """Write JSON files of parameters."""
         logger.debug("Writing parameters...")
-        makedirs(json_path, exist_ok=True)
+        json_path.mkdir(parents=True, exist_ok=True)
 
+        parameters = change_path_to_str(parameters)
+        print("just before error")
+        print(parameters)
         # save to json file
         json_data = json.dumps(parameters, skipkeys=True, indent=4)
-        json_path = path.join(json_path, "maps.json")
+        json_path = json_path / "maps.json"
         if verbose:
             logger.info(f"Path of json file: {json_path}")
-        with open(json_path, "w") as f:
+        with json_path.open(mode="w") as f:
             f.write(json_data)
+        parameters = change_str_to_path(parameters)
 
     def _write_requirements_version(self):
         """Writes the environment.txt file."""
         logger.debug("Writing requirement version...")
         try:
             env_variables = subprocess.check_output("pip freeze", shell=True).decode(
                 "utf-8"
             )
-            with open(path.join(self.maps_path, "environment.txt"), "w") as file:
+            with (self.maps_path / "environment.txt").open(mode="w") as file:
                 file.write(env_variables)
         except subprocess.CalledProcessError:
             logger.warning(
                 "You do not have the right to execute pip freeze. Your environment will not be written"
             )
 
     def _write_training_data(self):
@@ -1413,52 +1467,51 @@
             self.tsv_path,
             self.diagnoses,
             baseline=False,
             multi_cohort=self.multi_cohort,
         )
         train_df = train_df[["participant_id", "session_id"]]
         if self.transfer_path:
-            transfer_train_path = path.join(
-                self.transfer_path, "groups", "train+validation.tsv"
-            )
+            transfer_train_path = self.transfer_path / "groups" / "train+validation.tsv"
             transfer_train_df = pd.read_csv(transfer_train_path, sep="\t")
             transfer_train_df = transfer_train_df[["participant_id", "session_id"]]
             train_df = pd.concat([train_df, transfer_train_df])
             train_df.drop_duplicates(inplace=True)
         train_df.to_csv(
-            path.join(self.maps_path, "groups", "train+validation.tsv"),
-            sep="\t",
-            index=False,
+            self.maps_path / "groups" / "train+validation.tsv", sep="\t", index=False
         )
 
     def _write_data_group(
-        self, data_group, df, caps_directory=None, multi_cohort=None, label=None
+        self,
+        data_group,
+        df,
+        caps_directory: Path = None,
+        multi_cohort: bool = None,
+        label=None,
     ):
         """
         Check that a data_group is not already written and writes the characteristics of the data group
         (TSV file with a list of participant / session + JSON file containing the CAPS and the preprocessing).
 
         Args:
             data_group (str): name whose presence is checked.
             df (pd.DataFrame): DataFrame containing the participant_id and session_id (and label if use_labels is True)
             caps_directory (str): caps_directory if different from the training caps_directory,
             multi_cohort (bool): multi_cohort used if different from the training multi_cohort.
         """
-        group_path = path.join(self.maps_path, "groups", data_group)
-        makedirs(group_path)
+        group_path = self.maps_path / "groups" / data_group
+        group_path.mkdir(parents=True)
 
         columns = ["participant_id", "session_id", "cohort"]
         if self.label in df.columns.values:
             columns += [self.label]
         if label is not None and label in df.columns.values:
             columns += [label]
 
-        df.to_csv(
-            path.join(group_path, "data.tsv"), sep="\t", columns=columns, index=False
-        )
+        df.to_csv(group_path / "data.tsv", sep="\t", columns=columns, index=False)
         self.write_parameters(
             group_path,
             {
                 "caps_directory": caps_directory
                 if caps_directory is not None
                 else self.caps_directory,
                 "multi_cohort": multi_cohort
@@ -1470,23 +1523,26 @@
     def _write_train_val_groups(self):
         """Defines the training and validation groups at the initialization"""
         logger.debug("Writing training and validation groups...")
         split_manager = self._init_split_manager()
         for split in split_manager.split_iterator():
             for data_group in ["train", "validation"]:
                 df = split_manager[split][data_group]
-                group_path = path.join(
-                    self.maps_path, "groups", data_group, f"{self.split_name}-{split}"
+                group_path = (
+                    self.maps_path
+                    / "groups"
+                    / data_group
+                    / f"{self.split_name}-{split}"
                 )
-                makedirs(group_path, exist_ok=True)
+                group_path.mkdir(parents=True, exist_ok=True)
 
                 columns = ["participant_id", "session_id", "cohort"]
                 if self.label is not None:
                     columns.append(self.label)
-                df.to_csv(path.join(group_path, "data.tsv"), sep="\t", columns=columns)
+                df.to_csv(group_path / "data.tsv", sep="\t", columns=columns)
                 self.write_parameters(
                     group_path,
                     {
                         "caps_directory": self.caps_directory,
                         "multi_cohort": self.multi_cohort,
                     },
                     verbose=False,
@@ -1507,34 +1563,34 @@
         Args:
             state: state of the training (model weights, epoch...).
             metrics_dict: output of RetainBest step.
             split: split number.
             network: network number (multi-network framework).
             filename: name of the checkpoint file.
         """
-        checkpoint_dir = path.join(self.maps_path, f"{self.split_name}-{split}", "tmp")
-        makedirs(checkpoint_dir, exist_ok=True)
-        checkpoint_path = path.join(checkpoint_dir, filename)
+        checkpoint_dir = self.maps_path / f"{self.split_name}-{split}" / "tmp"
+        checkpoint_dir.mkdir(parents=True, exist_ok=True)
+        checkpoint_path = checkpoint_dir / filename
         torch.save(state, checkpoint_path)
 
         best_filename = "model.pth.tar"
         if network is not None:
             best_filename = f"network-{network}_model.pth.tar"
 
         # Save model according to several metrics
         if metrics_dict is not None:
             for metric_name, metric_bool in metrics_dict.items():
-                metric_path = path.join(
-                    self.maps_path, f"{self.split_name}-{split}", f"best-{metric_name}"
+                metric_path = (
+                    self.maps_path
+                    / f"{self.split_name}-{split}"
+                    / f"best-{metric_name}"
                 )
                 if metric_bool:
-                    makedirs(metric_path, exist_ok=True)
-                    shutil.copyfile(
-                        checkpoint_path, path.join(metric_path, best_filename)
-                    )
+                    metric_path.mkdir(parents=True, exist_ok=True)
+                    shutil.copyfile(checkpoint_path, metric_path / best_filename)
 
     def _write_information(self):
         """
         Writes model architecture of the MAPS in MAPS root.
         """
         from datetime import datetime
 
@@ -1552,46 +1608,46 @@
             kwargs[arg] = self.parameters[arg]
         kwargs["gpu"] = False
 
         model = model_class(**kwargs)
 
         file_name = "information.log"
 
-        with open(path.join(self.maps_path, file_name), "w") as f:
+        with (self.maps_path / file_name).open(mode="w") as f:
             f.write(f"- Date :\t{datetime.now().strftime('%d %b %Y, %H:%M:%S')}\n\n")
             f.write(f"- Path :\t{self.maps_path}\n\n")
             # f.write("- Job ID :\t{}\n".format(os.getenv('SLURM_JOBID')))
             f.write(f"- Model :\t{model.layers}\n\n")
 
         del model
 
     def _erase_tmp(self, split):
         """Erase checkpoints of the model and optimizer at the end of training."""
-        tmp_path = path.join(self.maps_path, f"{self.split_name}-{split}", "tmp")
+        tmp_path = self.maps_path / f"{self.split_name}-{split}" / "tmp"
         shutil.rmtree(tmp_path)
 
     @staticmethod
     def write_description_log(
-        log_dir,
+        log_dir: Path,
         data_group,
         caps_dict,
         df,
     ):
         """
         Write description log file associated to a data group.
 
         Args:
             log_dir (str): path to the log file directory.
             data_group (str): name of the data group used for the task.
             caps_dict (dict[str, str]): Dictionary of the CAPS folders used for the task
             df (pd.DataFrame): DataFrame of the meta-data used for the task.
         """
-        makedirs(log_dir, exist_ok=True)
-        log_path = path.join(log_dir, "description.log")
-        with open(log_path, "w") as f:
+        log_dir.mkdir(parents=True, exist_ok=True)
+        log_path = log_dir / "description.log"
+        with log_path.open(mode="w") as f:
             f.write(f"Prediction {data_group} group - {datetime.now()}\n")
             f.write(f"Data loaded from CAPS directories: {caps_dict}\n")
             f.write(f"Number of participants: {df.participant_id.nunique()}\n")
             f.write(f"Number of sessions: {len(df)}\n")
 
     def _mode_level_to_tsv(
         self,
@@ -1607,38 +1663,34 @@
         Args:
             results_df: the individual results per patch.
             metrics: the performances obtained on a series of metrics.
             split: the split for which the performances were obtained.
             selection: the metrics on which the model was selected (BA, loss...)
             data_group: the name referring to the data group on which evaluation is performed.
         """
-        performance_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection}",
-            data_group,
-        )
-
-        makedirs(performance_dir, exist_ok=True)
-        performance_path = path.join(
-            performance_dir, f"{data_group}_{self.mode}_level_prediction.tsv"
+        performance_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection}"
+            / data_group
+        )
+        performance_dir.mkdir(parents=True, exist_ok=True)
+        performance_path = (
+            performance_dir / f"{data_group}_{self.mode}_level_prediction.tsv"
         )
-
-        if not path.exists(performance_path):
+        if not performance_path.is_file():
             results_df.to_csv(performance_path, index=False, sep="\t")
         else:
             results_df.to_csv(
                 performance_path, index=False, sep="\t", mode="a", header=False
             )
 
-        metrics_path = path.join(
-            performance_dir, f"{data_group}_{self.mode}_level_metrics.tsv"
-        )
+        metrics_path = performance_dir / f"{data_group}_{self.mode}_level_metrics.tsv"
         if metrics is not None:
-            if not path.exists(metrics_path):
+            if not metrics_path.is_file():
                 pd.DataFrame(metrics, index=[0]).to_csv(
                     metrics_path, index=False, sep="\t"
                 )
             else:
                 pd.DataFrame(metrics, index=[0]).to_csv(
                     metrics_path, index=False, sep="\t", mode="a", header=False
                 )
@@ -1669,38 +1721,39 @@
         test_df = self.get_prediction(
             data_group, split, selection, self.mode, verbose=False
         )
         validation_df = self.get_prediction(
             validation_dataset, split, selection, self.mode, verbose=False
         )
 
-        performance_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection}",
-            data_group,
+        performance_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection}"
+            / data_group
         )
-        makedirs(performance_dir, exist_ok=True)
+
+        performance_dir.mkdir(parents=True, exist_ok=True)
 
         df_final, metrics = self.task_manager.ensemble_prediction(
             test_df,
             validation_df,
             selection_threshold=self.selection_threshold,
             use_labels=use_labels,
         )
 
         if df_final is not None:
             df_final.to_csv(
-                path.join(performance_dir, f"{data_group}_image_level_prediction.tsv"),
+                performance_dir / f"{data_group}_image_level_prediction.tsv",
                 index=False,
                 sep="\t",
             )
         if metrics is not None:
             pd.DataFrame(metrics, index=[0]).to_csv(
-                path.join(performance_dir, f"{data_group}_image_level_metrics.tsv"),
+                performance_dir / f"{data_group}_image_level_metrics.tsv",
                 index=False,
                 sep="\t",
             )
 
     def _mode_to_image_tsv(
         self,
         split: int,
@@ -1719,46 +1772,44 @@
 
         """
         sub_df = self.get_prediction(
             data_group, split, selection, self.mode, verbose=False
         )
         sub_df.rename(columns={f"{self.mode}_id": "image_id"}, inplace=True)
 
-        performance_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection}",
-            data_group,
+        performance_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection}"
+            / data_group
         )
         sub_df.to_csv(
-            path.join(performance_dir, f"{data_group}_image_level_prediction.tsv"),
+            performance_dir / f"{data_group}_image_level_prediction.tsv",
             index=False,
             sep="\t",
         )
         if use_labels:
             metrics_df = pd.read_csv(
-                path.join(
-                    performance_dir, f"{data_group}_{self.mode}_level_metrics.tsv"
-                ),
+                performance_dir / f"{data_group}_{self.mode}_level_metrics.tsv",
                 sep="\t",
             )
             if f"{self.mode}_id" in metrics_df:
                 del metrics_df[f"{self.mode}_id"]
             metrics_df.to_csv(
-                path.join(performance_dir, f"{data_group}_image_level_metrics.tsv"),
+                (performance_dir / f"{data_group}_image_level_metrics.tsv"),
                 index=False,
                 sep="\t",
             )
 
     ###############################
     # Objects initialization      #
     ###############################
     def _init_model(
         self,
-        transfer_path=None,
+        transfer_path: Path = None,
         transfer_selection=None,
         split=None,
         resume=False,
         gpu=None,
         network=None,
     ):
         """
@@ -1794,19 +1845,19 @@
         model = model_class(**kwargs)
         logger.debug(f"Model:\n{model.layers}")
         device = model.device
         logger.info(f"Working on {device}")
         current_epoch = 0
 
         if resume:
-            checkpoint_path = path.join(
-                self.maps_path,
-                f"{self.split_name}-{split}",
-                "tmp",
-                "checkpoint.pth.tar",
+            checkpoint_path = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / "tmp"
+                / "checkpoint.pth.tar"
             )
             checkpoint_state = torch.load(checkpoint_path, map_location=device)
             model.load_state_dict(checkpoint_state["model"])
             current_epoch = checkpoint_state["epoch"]
         elif transfer_path:
             logger.debug(f"Transfer weights from MAPS at {transfer_path}")
             transfer_maps = MapsManager(transfer_path)
@@ -1827,16 +1878,19 @@
         optimizer = getattr(torch.optim, self.optimizer)(
             filter(lambda x: x.requires_grad, model.parameters()),
             lr=self.learning_rate,
             weight_decay=self.weight_decay,
         )
 
         if resume:
-            checkpoint_path = path.join(
-                self.maps_path, f"{self.split_name}-{split}", "tmp", "optimizer.pth.tar"
+            checkpoint_path = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / "tmp"
+                / "optimizer.pth.tar"
             )
             checkpoint_state = torch.load(checkpoint_path, map_location=model.device)
             optimizer.load_state_dict(checkpoint_state["optimizer"])
 
         return optimizer
 
     def _init_split_manager(self, split_list=None):
@@ -1873,14 +1927,44 @@
             return ReconstructionManager(self.mode)
         else:
             raise NotImplementedError(
                 f"Task {self.network_task} is not implemented in ClinicaDL. "
                 f"Please choose between classification, regression and reconstruction."
             )
 
+    def _init_profiler(self):
+        if self.profiler:
+            from torch.profiler import (
+                ProfilerActivity,
+                profile,
+                schedule,
+                tensorboard_trace_handler,
+            )
+
+            time = datetime.now().strftime("%H:%M:%S")
+            filename = [self.maps_path / "profiler" / f"clinicadl_{time}"]
+            # When ClinicaDL will be updated with Distributed Data Parallelism,
+            # the next line will be handy, to make sure all processes write in the same file
+            # dist.broadcast_object_list(filename, src=0)
+            profiler = profile(
+                activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA],
+                schedule=schedule(wait=2, warmup=2, active=30, repeat=1),
+                on_trace_ready=tensorboard_trace_handler(filename[0]),
+                profile_memory=True,
+                record_shapes=False,
+                with_stack=False,
+                with_flops=False,
+            )
+        else:
+            from contextlib import nullcontext
+
+            profiler = nullcontext()
+            profiler.step = lambda *args, **kwargs: None
+        return profiler
+
     ###############################
     # Getters                     #
     ###############################
     def _print_description_log(
         self,
         data_group,
         split,
@@ -1890,61 +1974,61 @@
         Print the description log associated to a prediction or interpretation.
 
         Args:
             data_group (str): name of the data group used for the task.
             split (int): Index of the split used for training.
             selection_metric (str): Metric used for best weights selection.
         """
-        log_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection_metric}",
-            data_group,
+        log_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection_metric}"
+            / data_group
         )
-        log_path = path.join(log_dir, "description.log")
-        with open(log_path, "r") as f:
+        log_path = log_dir / "description.log"
+        with log_path.open(mode="r") as f:
             content = f.read()
 
     def get_group_info(
         self, data_group: str, split: int = None
     ) -> Tuple[pd.DataFrame, Dict[str, Any]]:
         """
         Gets information from corresponding data group
         (list of participant_id / session_id + configuration parameters).
         split is only needed if data_group is train or validation.
         """
-        group_path = path.join(self.maps_path, "groups", data_group)
-        if not path.exists(group_path):
+        group_path = self.maps_path / "groups" / data_group
+        if not group_path.is_dir():
             raise MAPSError(
                 f"Data group {data_group} is not defined. "
                 f"Please run a prediction to create this data group."
             )
         if data_group in ["train", "validation"]:
             if split is None:
                 raise MAPSError(
                     f"Information on train or validation data can only be "
                     f"loaded if a split number is given"
                 )
-            elif not path.exists(path.join(group_path, f"{self.split_name}-{split}")):
+            elif not (group_path / f"{self.split_name}-{split}").is_dir():
                 raise MAPSError(
                     f"Split {split} is not available for data group {data_group}."
                 )
             else:
-                group_path = path.join(group_path, f"{self.split_name}-{split}")
+                group_path = group_path / f"{self.split_name}-{split}"
 
-        df = pd.read_csv(path.join(group_path, "data.tsv"), sep="\t")
-        json_path = path.join(group_path, "maps.json")
-        with open(json_path, "r") as f:
+        df = pd.read_csv(group_path / "data.tsv", sep="\t")
+        json_path = group_path / "maps.json"
+        with json_path.open(mode="r") as f:
             parameters = json.load(f)
-
+        parameters = change_str_to_path(parameters)
         return df, parameters
 
     def get_parameters(self):
         """Returns the training parameters dictionary."""
-        json_path = path.join(self.maps_path, "maps.json")
+        json_path = self.maps_path / "maps.json"
         return read_json(json_path)
 
     def get_model(
         self, split: int = 0, selection_metric: str = None, network: int = None
     ) -> Network:
         selection_metric = self._check_selection_metric(split, selection_metric)
         if self.multi_network:
@@ -1988,37 +2072,37 @@
         selection_metric = self._check_selection_metric(split, selection_metric)
         if self.multi_network:
             if network is None:
                 raise ClinicaDLArgumentError(
                     "Please precise the network number that must be loaded."
                 )
             else:
-                model_path = path.join(
-                    self.maps_path,
-                    f"{self.split_name}-{split}",
-                    f"best-{selection_metric}",
-                    f"network-{network}_model.pth.tar",
+                model_path = (
+                    self.maps_path
+                    / f"{self.split_name}-{split}"
+                    / f"best-{selection_metric}"
+                    / f"network-{network}_model.pth.tar"
                 )
         else:
-            model_path = path.join(
-                self.maps_path,
-                f"{self.split_name}-{split}",
-                f"best-{selection_metric}",
-                "model.pth.tar",
+            model_path = (
+                self.maps_path
+                / f"{self.split_name}-{split}"
+                / f"best-{selection_metric}"
+                / "model.pth.tar"
             )
 
         logger.info(
             f"Loading model trained for split {split} "
             f"selected according to best validation {selection_metric} "
             f"at path {model_path}."
         )
         return torch.load(model_path, map_location=map_location)
 
     def get_prediction(
-        self, data_group, split=0, selection_metric=None, mode="image", verbose=True
+        self, data_group, split=0, selection_metric=None, mode="image", verbose=False
     ):
         """
         Get the individual predictions for each participant corresponding to one group
         of participants identified by its data group.
 
         Args:
             data_group (str): name of the data group used for the prediction task.
@@ -2029,26 +2113,26 @@
         Returns:
             (DataFrame): Results indexed by columns 'participant_id' and 'session_id' which
             identifies the image in the BIDS / CAPS.
         """
         selection_metric = self._check_selection_metric(split, selection_metric)
         if verbose:
             self._print_description_log(data_group, split, selection_metric)
-        prediction_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection_metric}",
-            data_group,
+        prediction_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection_metric}"
+            / data_group
         )
-        if not path.exists(prediction_dir):
+        if not prediction_dir.is_dir():
             raise MAPSError(
                 f"No prediction corresponding to data group {data_group} was found."
             )
         df = pd.read_csv(
-            path.join(prediction_dir, f"{data_group}_{mode}_level_prediction.tsv"),
+            prediction_dir / f"{data_group}_{mode}_level_prediction.tsv",
             sep="\t",
         )
         df.set_index(["participant_id", "session_id"], inplace=True, drop=True)
         return df
 
     def get_metrics(
         self, data_group, split=0, selection_metric=None, mode="image", verbose=True
@@ -2064,27 +2148,26 @@
             verbose (bool): if True will print associated prediction.log
         Returns:
             (dict[str:float]): Values of the metrics
         """
         selection_metric = self._check_selection_metric(split, selection_metric)
         if verbose:
             self._print_description_log(data_group, split, selection_metric)
-        prediction_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection_metric}",
-            data_group,
+        prediction_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection_metric}"
+            / data_group
         )
-        if not path.exists(prediction_dir):
+        if not prediction_dir.is_dir():
             raise MAPSError(
                 f"No prediction corresponding to data group {data_group} was found."
             )
         df = pd.read_csv(
-            path.join(prediction_dir, f"{data_group}_{mode}_level_metrics.tsv"),
-            sep="\t",
+            prediction_dir / f"{data_group}_{mode}_level_metrics.tsv", sep="\t"
         )
         return df.to_dict("records")[0]
 
     def get_interpretation(
         self,
         data_group,
         name,
@@ -2111,37 +2194,32 @@
         Returns:
             (torch.Tensor): Tensor of the interpretability map.
         """
 
         selection_metric = self._check_selection_metric(split, selection_metric)
         if verbose:
             self._print_description_log(data_group, split, selection_metric)
-        map_dir = path.join(
-            self.maps_path,
-            f"{self.split_name}-{split}",
-            f"best-{selection_metric}",
-            data_group,
-            f"interpret-{name}",
+        map_dir = (
+            self.maps_path
+            / f"{self.split_name}-{split}"
+            / f"best-{selection_metric}"
+            / data_group
+            / f"interpret-{name}"
         )
-        if not path.exists(map_dir):
+        if not map_dir.is_dir():
             raise MAPSError(
                 f"No prediction corresponding to data group {data_group} and "
                 f"interpretation {name} was found."
             )
         if participant_id is None and session_id is None:
-            map_pt = torch.load(
-                path.join(map_dir, f"mean_{self.mode}-{mode_id}_map.pt")
-            )
+            map_pt = torch.load(map_dir / f"mean_{self.mode}-{mode_id}_map.pt")
         elif participant_id is None or session_id is None:
             raise ValueError(
                 f"To load the mean interpretation map, "
                 f"please do not give any participant_id or session_id.\n "
                 f"Else specify both parameters"
             )
         else:
             map_pt = torch.load(
-                path.join(
-                    map_dir,
-                    f"{participant_id}_{session_id}_{self.mode}-{mode_id}_map.pt",
-                )
+                map_dir / f"{participant_id}_{session_id}_{self.mode}-{mode_id}_map.pt"
             )
         return map_pt
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/meta_maps/getter.py` & `clinicadl-1.3.0/clinicadl/utils/meta_maps/getter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 """
 Produces a tsv file to analyze the performance of one launch of the random search.
 """
-import os
-from os import path
+from pathlib import Path
 
 import pandas as pd
 
 from clinicadl import MapsManager
 from clinicadl.utils.exceptions import MAPSError
 
 
-def meta_maps_analysis(launch_dir, evaluation_metric="loss"):
+def meta_maps_analysis(launch_dir: Path, evaluation_metric="loss"):
     """
     This function summarizes the validation performance according to `evaluation_metric`
     of several MAPS stored in the folder `launch_dir`.
     The output TSV files are written in `launch_dir`.
 
     Args:
         launch_dir (str): Path to the directory containing several MAPS.
         evaluation_metric (str): Name of the metric used for validation evaluation.
     """
-
+    launch_dir = launch_dir
     jobs_list = [
         job
-        for job in os.listdir(launch_dir)
-        if path.exists(path.join(launch_dir, job, "maps.json"))
+        for job in list(launch_dir.iter_dir())
+        if (launch_dir / job / "maps.json").is_file()
     ]
 
     selection_set = set()  # Set of all selection metrics seen
     split_set = set()  # Set of all splits seen
 
     performances_dict = dict()
     for job in jobs_list:
         performances_dict[job] = dict()
-        maps_manager = MapsManager(path.join(launch_dir, job))
+        maps_manager = MapsManager(launch_dir / job)
         split_list = maps_manager._find_splits()
         split_set = split_set | set(split_list)
         for split in split_set:
             performances_dict[job][split] = dict()
             selection_metrics = maps_manager._find_selection_metrics(split)
             selection_set = selection_set | set(selection_metrics)
             for metric in selection_metrics:
@@ -56,8 +55,8 @@
     # Produce one analysis for each selection metric
     for metric in selection_set:
         df = pd.DataFrame()
         filename = f"analysis_metric-{evaluation_metric}_selection-{metric}.tsv"
         for job in jobs_list:
             for split in split_set:
                 df.loc[job, f"split-{split}"] = performances_dict[job][split][metric]
-        df.to_csv(path.join(launch_dir, filename), sep="\t")
+        df.to_csv(launch_dir / filename, sep="\t")
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/metric_module.py` & `clinicadl-1.3.0/clinicadl/utils/metric_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,29 @@
 }
 
 logger = getLogger("clinicadl.metric")
 
 
 class MetricModule:
     def __init__(self, metrics, n_classes=2):
-
         self.n_classes = n_classes
 
         # Check if wanted metrics are implemented
         list_fn = [
             method_name
             for method_name in dir(MetricModule)
             if callable(getattr(MetricModule, method_name))
         ]
         self.metrics = dict()
         for metric in metrics:
             if f"{metric.lower()}_fn" in list_fn:
                 self.metrics[metric] = getattr(MetricModule, f"{metric.lower()}_fn")
             else:
                 raise NotImplementedError(
-                    f"The metric {metric} is not implemented in the module"
+                    f"The metric {metric} is not implemented in the module."
                 )
 
     def apply(self, y, y_pred):
         """
         This is a function to calculate the different metrics based on the list of true label and predicted label
 
         Args:
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/autoencoder/cnn_transformer.py` & `clinicadl-1.3.0/clinicadl/utils/network/autoencoder/cnn_transformer.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/autoencoder/models.py` & `clinicadl-1.3.0/clinicadl/utils/network/autoencoder/models.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/cnn/models.py` & `clinicadl-1.3.0/clinicadl/utils/network/cnn/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 import torch
 import torch.utils.model_zoo as model_zoo
 from torch import nn
 from torchvision.models.resnet import BasicBlock
 
 from clinicadl.utils.network.cnn.resnet import ResNetDesigner, model_urls
+from clinicadl.utils.network.cnn.resnet3D import ResNetDesigner3D
+from clinicadl.utils.network.cnn.SECNN import SECNNDesigner3D
 from clinicadl.utils.network.network_utils import PadMaxPool2d, PadMaxPool3d
 from clinicadl.utils.network.sub_network import CNN
 
 
 def get_layers_fn(input_size):
     if len(input_size) == 4:
         return nn.Conv3d, nn.BatchNorm3d, PadMaxPool3d
@@ -281,7 +283,95 @@
     @staticmethod
     def get_dimension():
         return "2D or 3D"
 
     @staticmethod
     def get_task():
         return ["classification", "regression"]
+
+
+class ResNet3D(CNN):
+    """
+    ResNet3D is a 3D neural network composed of 5 residual blocks. Each residual block
+    is compose of 3D convolutions followed by a batch normalization and an activation function.
+    It uses skip connections or shortcuts to jump over some layers. It's a 3D version of the
+    original implementation of Kaiming He et al.
+
+    Reference: Kaiming He et al., Deep Residual Learning for Image Recognition.
+    https://arxiv.org/abs/1512.03385?context=cs
+    """
+
+    def __init__(
+        self, input_size=[1, 169, 208, 179], gpu=False, output_size=2, dropout=0.5
+    ):
+        model = ResNetDesigner3D()
+
+        convolutions = nn.Sequential(
+            model.layer0, model.layer1, model.layer2, model.layer3, model.layer4
+        )
+
+        fc = model.fc
+
+        super().__init__(
+            convolutions=convolutions,
+            fc=fc,
+            n_classes=output_size,
+            gpu=gpu,
+        )
+
+    @staticmethod
+    def get_input_size():
+        return "1@169x207x179"
+
+    @staticmethod
+    def get_dimension():
+        return "3D"
+
+    @staticmethod
+    def get_task():
+        return ["classification", "regression"]
+
+
+class SqueezeExcitationCNN(CNN):
+    """
+    SE-CNN is a combination of a ResNet-101 with Squeeze and Excitation blocks which was successfully
+    tested on brain tumour classification by Ghosal et al. 2019. SE blocks are composed of a squeeze
+    and an excitation step. The squeeze operation is obtained through an average pooling layer and
+    provides a global understanding of each channel.
+
+    The excitation part consists of a two-layer feed-forward network that outputs a vector of n values
+    corresponding to the weights of each channel of the feature maps.
+
+    Reference: Ghosal et al. Brain Tumor Classification Using ResNet-101 Based Squeeze and Excitation Deep Neural Network
+    https://ieeexplore.ieee.org/document/8882973
+
+    """
+
+    def __init__(
+        self, input_size=[1, 169, 208, 179], gpu=True, output_size=2, dropout=0.5
+    ):
+        model = SECNNDesigner3D()
+
+        convolutions = nn.Sequential(
+            model.layer0, model.layer1, model.layer2, model.layer3, model.layer4
+        )
+
+        fc = model.fc
+
+        super().__init__(
+            convolutions=convolutions,
+            fc=fc,
+            n_classes=output_size,
+            gpu=gpu,
+        )
+
+    @staticmethod
+    def get_input_size():
+        return "1@169x207x179"
+
+    @staticmethod
+    def get_dimension():
+        return "3D"
+
+    @staticmethod
+    def get_task():
+        return ["classification"]
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/cnn/random.py` & `clinicadl-1.3.0/clinicadl/utils/network/cnn/random.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/cnn/resnet.py` & `clinicadl-1.3.0/clinicadl/utils/network/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/network.py` & `clinicadl-1.3.0/clinicadl/utils/network/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List
 
 import torch.cuda
 from torch import nn
 
 
 class Network(nn.Module):
-    """Abstract Template for all networks used in ClinicaDL"""
+    """Abstract Template for all networks used in ClinicaDL."""
 
     def __init__(self, gpu=True):
         super(Network, self).__init__()
         self.device = self._select_device(gpu)
 
     @staticmethod
     def _select_device(gpu):
@@ -52,15 +52,14 @@
                         "NVML library is not installed. GPU will be chosen arbitrarily"
                     )
                     return "cuda"
 
     @staticmethod
     @abc.abstractmethod
     def get_input_size() -> str:
-
         """This static method is used for list_models command.
         Must return the shape of the input size expected (C@HxW or C@HxWxD) for each architecture.
         """
         pass
 
     @staticmethod
     @abc.abstractmethod
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/network_utils.py` & `clinicadl-1.3.0/clinicadl/utils/network/network_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         super(Reshape, self).__init__()
         self.size = size
 
     def forward(self, input):
         return input.view(*self.size)
 
 
+# pre-commit comment
 class PadMaxPool3d(nn.Module):
     def __init__(self, kernel_size, stride, return_indices=False, return_pad=False):
         super(PadMaxPool3d, self).__init__()
         self.kernel_size = kernel_size
         self.stride = stride
         self.pool = nn.MaxPool3d(kernel_size, stride, return_indices=return_indices)
         self.pad = nn.ConstantPad3d(padding=0, value=0)
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/sub_network.py` & `clinicadl-1.3.0/clinicadl/utils/network/sub_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import abc
 from collections import OrderedDict
 from logging import getLogger
 
 import torch
 from torch import nn
 
 from clinicadl.utils.exceptions import ClinicaDLNetworksError
@@ -77,15 +76,14 @@
                 x = layer(x, indices_list.pop())
             else:
                 x = layer(x)
 
         return code, x
 
     def compute_outputs_and_loss(self, input_dict, criterion, use_labels=True):
-
         images = input_dict["image"].to(self.device)
         train_output = self.predict(images)
         loss = criterion(train_output, images)
 
         return train_output, {"loss": loss}
 
 
@@ -110,26 +108,25 @@
                     for k, v in state_dict.items()
                     if "encoder" in k
                 ]
             )
             self.convolutions.load_state_dict(convolutions_dict)
         else:
             raise ClinicaDLNetworksError(
-                f"Cannot transfer weights from {transfer_class} to CNN."
+                f"Can not transfer weights from {transfer_class} to CNN."
             )
 
     def forward(self, x):
         x = self.convolutions(x)
         return self.fc(x)
 
     def predict(self, x):
         return self.forward(x)
 
     def compute_outputs_and_loss(self, input_dict, criterion, use_labels=True):
-
         images, labels = input_dict["image"].to(self.device), input_dict["label"].to(
             self.device
         )
         train_output = self.forward(images)
         if use_labels:
             loss = criterion(train_output, labels)
         else:
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/vae/base_vae.py` & `clinicadl-1.3.0/clinicadl/utils/network/vae/base_vae.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,21 +35,21 @@
         )
 
     # Network specific
     def predict(self, x):
         output, _, _ = self.forward(x)
         return output
 
+    # Forward
     def forward(self, x):
         mu, logvar = self.encode(x)
         z = self.reparameterize(mu, logvar)
         return self.decode(z), mu, logvar
 
     def compute_outputs_and_loss(self, input_dict, criterion, use_labels=False):
-
         images = input_dict["image"].to(self.device)
         recon_images, mu, log_var = self.forward(images)
 
         recon_loss = criterion(recon_images, images)
         if self.is_3D:
             kl_loss = -0.5 * torch.mean(
                 torch.sum(1 + log_var - mu**2 - log_var.exp(), dim=1)
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/vae/vae_utils.py` & `clinicadl-1.3.0/clinicadl/utils/network/vae/vae_utils.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/network/vae/vanilla_vae.py` & `clinicadl-1.3.0/clinicadl/utils/network/vae/vanilla_vae.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/preprocessing.py` & `clinicadl-1.3.0/clinicadl/utils/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import errno
 import json
-import os
+from pathlib import Path
 from typing import Any, Dict
 
+from clinicadl.utils.maps_manager.maps_manager_utils import change_path_to_str
 
-def write_preprocessing(preprocessing_dict: Dict[str, Any], caps_directory: str):
-    extract_dir = os.path.join(
-        caps_directory,
-        "tensor_extraction",
-    )
-    os.makedirs(extract_dir, exist_ok=True)
-    json_path = os.path.join(extract_dir, preprocessing_dict["extract_json"])
-    if os.path.exists(json_path):
+
+def write_preprocessing(preprocessing_dict: Dict[str, Any], caps_directory: Path):
+    extract_dir = caps_directory / "tensor_extraction"
+    extract_dir.mkdir(parents=True, exist_ok=True)
+    json_path = extract_dir / preprocessing_dict["extract_json"]
+    if json_path.is_file():
         raise FileExistsError(
             f"JSON file at {json_path} already exists. "
             f"Please choose another name for your preprocessing file."
         )
-
-    with open(json_path, "w") as json_file:
-        json.dump(preprocessing_dict, json_file, indent=2)
+    preprocessing_dict_bis = change_path_to_str(preprocessing_dict)
+    with json_path.open(mode="w") as json_file:
+        json.dump(preprocessing_dict_bis, json_file)
     return json_path
 
 
-def read_preprocessing(json_path: str) -> Dict[str, Any]:
-    if not json_path.endswith(".json"):
+def read_preprocessing(json_path: Path) -> Dict[str, Any]:
+    if not json_path.name.endswith(".json"):
         json_path += ".json"
+        json_path = json_path
 
-    if not os.path.isfile(json_path):
-        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), json_path)
+    if not json_path.is_file():
+        raise FileNotFoundError(errno.ENOENT, json_path)
     try:
-        with open(json_path, "r") as f:
+        with json_path.open(mode="r") as f:
             preprocessing_dict = json.load(f)
     except IOError:
         raise IOError(f"Cannot open json preprocessing file {json_path}")
     return preprocessing_dict
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/seed.py` & `clinicadl-1.3.0/clinicadl/utils/seed.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/split_manager/kfold.py` & `clinicadl-1.3.0/clinicadl/utils/split_manager/kfold.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from os import path
+from pathlib import Path
 
 from clinicadl.utils.split_manager.split_manager import SplitManager
 
 
 class KFoldSplit(SplitManager):
     def __init__(
         self,
@@ -34,11 +34,11 @@
 
     def split_iterator(self):
         if not self.split_list:
             return range(self.n_splits)
         else:
             return self.split_list
 
-    def _get_tsv_paths(self, cohort_path, split):
-        train_path = path.join(cohort_path, f"split-{split}")
-        valid_path = path.join(cohort_path, f"split-{split}")
+    def _get_tsv_paths(self, cohort_path: Path, split):
+        train_path = cohort_path / f"split-{split}"
+        valid_path = cohort_path / f"split-{split}"
         return train_path, valid_path
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/split_manager/single_split.py` & `clinicadl-1.3.0/clinicadl/utils/split_manager/single_split.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from os import path
+from pathlib import Path
 
 from clinicadl.utils.split_manager.split_manager import SplitManager
 
 
 class SingleSplit(SplitManager):
     def __init__(
         self,
@@ -26,12 +26,12 @@
     @property
     def allowed_splits_list(self):
         return [0]
 
     def split_iterator(self):
         return range(1)
 
-    def _get_tsv_paths(self, cohort_path, split):
-        train_path = path.join(cohort_path)
-        valid_path = path.join(cohort_path)
+    def _get_tsv_paths(self, cohort_path: Path):
+        train_path = cohort_path
+        valid_path = cohort_path
 
         return train_path, valid_path
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/split_manager/split_manager.py` & `clinicadl-1.3.0/clinicadl/utils/split_manager/split_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import abc
 from logging import getLogger
-from os import path
 from pathlib import Path
 
 import pandas as pd
 from clinica.utils.inputs import check_caps_folder
 
 from clinicadl.utils.exceptions import (
     ClinicaDLArgumentError,
@@ -14,16 +13,16 @@
 
 logger = getLogger("clinicadl.split_manager")
 
 
 class SplitManager:
     def __init__(
         self,
-        caps_directory,
-        tsv_path,
+        caps_directory: Path,
+        tsv_path: Path,
         diagnoses,
         baseline=False,
         multi_cohort=False,
         split_list=None,
     ):
         """
 
@@ -118,52 +117,55 @@
             valid_df["cohort"] = "single"
 
         return {
             "train": train_df,
             "validation": valid_df,
         }
 
-    def concatenate_diagnoses(self, split, cohort_path=None, cohort_diagnoses=None):
+    def concatenate_diagnoses(
+        self, split, cohort_path: Path = None, cohort_diagnoses=None
+    ):
         """Concatenated the diagnoses needed to form the train and validation sets."""
 
         train_path, valid_path = self._get_tsv_paths(
             split=split,
             cohort_path=cohort_path if cohort_path is not None else self.tsv_path,
         )
         logger.debug(f"Training data loaded at {train_path}")
         logger.debug(f"Validation data loaded at {valid_path}")
         if cohort_diagnoses is None:
             cohort_diagnoses = self.diagnoses
 
         if self.baseline:
-            train_path = path.join(train_path, "train_baseline.tsv")
+            train_path = train_path / "train_baseline.tsv"
         else:
-            train_path = path.join(train_path, "train.tsv")
+            train_path = train_path / "train.tsv"
 
-        valid_path = path.join(valid_path, "validation_baseline.tsv")
+        valid_path = valid_path / "validation_baseline.tsv"
 
         train_df = pd.read_csv(train_path, sep="\t")
         valid_df = pd.read_csv(valid_path, sep="\t")
 
         list_columns = train_df.columns.values
 
         if (
             "diagnosis"
             not in list_columns
             # or "age" not in list_columns
             # or "sex" not in list_columns
         ):
-            parents_path = path.abspath(Path(train_path).parents[0])
-            while (not path.exists(path.join(parents_path, "labels.tsv"))) and (
-                path.exists(path.join(parents_path, "kfold.json"))
-                or path.exists(path.join(parents_path, "split.json"))
+            parents_path = train_path.resolve().parent
+            while (
+                not (parents_path / "labels.tsv").is_file()
+                and ((parents_path / "kfold.json").is_file())
+                or (parents_path / "split.json").is_file()
             ):
-                parents_path = Path(parents_path).parents[0]
+                parents_path = parents_path.parent
             try:
-                labels_df = pd.read_csv(path.join(parents_path, "labels.tsv"), sep="\t")
+                labels_df = pd.read_csv(parents_path / "labels.tsv", sep="\t")
                 train_df = pd.merge(
                     train_df,
                     labels_df,
                     how="inner",
                     on=["participant_id", "session_id"],
                 )
             except:
@@ -172,22 +174,23 @@
         list_columns = valid_df.columns.values
         if (
             "diagnosis"
             not in list_columns
             # or "age" not in list_columns
             # or "sex" not in list_columns
         ):
-            parents_path = path.abspath(Path(valid_path).parents[0])
-            while (not path.exists(path.join(parents_path, "labels.tsv"))) and (
-                path.exists(path.join(parents_path, "kfold.json"))
-                or path.exists(path.join(parents_path, "split.json"))
+            parents_path = valid_path.resolve().parent
+            while (
+                not (parents_path / "labels.tsv").is_file()
+                and ((parents_path / "kfold.json").is_file())
+                or (parents_path / "split.json").is_file()
             ):
-                parents_path = Path(parents_path).parents[0]
+                parents_path = parents_path.parent
             try:
-                labels_df = pd.read_csv(path.join(parents_path, "labels.tsv"), sep="\t")
+                labels_df = pd.read_csv(parents_path / "labels.tsv", sep="\t")
                 valid_df = pd.merge(
                     valid_df,
                     labels_df,
                     how="inner",
                     on=["participant_id", "session_id"],
                 )
             except:
@@ -220,17 +223,17 @@
     def _check_item(self, item):
         if item not in self.allowed_splits_list:
             raise IndexError(
                 f"Split index {item} out of allowed splits {self.allowed_splits_list}."
             )
 
     @staticmethod
-    def _create_caps_dict(caps_directory, multi_cohort):
+    def _create_caps_dict(caps_directory: Path, multi_cohort):
         if multi_cohort:
-            if not caps_directory.endswith(".tsv"):
+            if not caps_directory.suffix == ".tsv":
                 raise ClinicaDLArgumentError(
                     "If multi_cohort is given, the CAPS_DIRECTORY argument should be a path to a TSV file."
                 )
             else:
                 caps_df = pd.read_csv(caps_directory, sep="\t")
                 SplitManager._check_multi_cohort_tsv(caps_df, "CAPS")
                 caps_dict = dict()
@@ -244,23 +247,23 @@
             caps_dict = {"single": caps_directory}
 
         return caps_dict
 
     @staticmethod
     def _check_tsv_path(tsv_path, multi_cohort):
         if multi_cohort:
-            if not tsv_path.endswith(".tsv"):
+            if not tsv_path.suffix == ".tsv":
                 raise ClinicaDLArgumentError(
                     "If multi_cohort is given, the TSV_DIRECTORY argument should be a path to a TSV file."
                 )
             else:
                 tsv_df = pd.read_csv(tsv_path, sep="\t")
                 SplitManager._check_multi_cohort_tsv(tsv_df, "labels")
         else:
-            if tsv_path.endswith(".tsv"):
+            if tsv_path.suffix == ".tsv":
                 raise ClinicaDLConfigurationError(
                     f"You gave the path to a TSV file in tsv_path {tsv_path}. "
                     f"To use multi-cohort framework, please add 'multi_cohort=true' to the configuration file or the --multi_cohort flag."
                 )
 
     @staticmethod
     def _check_multi_cohort_tsv(tsv_df, purpose):
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/task_manager/classification.py` & `clinicadl-1.3.0/clinicadl/utils/task_manager/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         return ["accuracy", "sensitivity", "specificity", "PPV", "NPV", "BA"]
 
     @property
     def save_outputs(self):
         return False
 
     def generate_test_row(self, idx, data, outputs):
-
         prediction = torch.argmax(outputs[idx].data).item()
         normalized_output = softmax(outputs[idx], dim=0)
         return [
             [
                 data["participant_id"][idx],
                 data["session_id"][idx],
                 data[f"{self.mode}_id"][idx].item(),
@@ -118,16 +117,16 @@
         """
         Computes hard or soft voting based on the probabilities in performance_df. Weights are computed based
         on the balanced accuracies of validation_df.
 
         ref: S. Raschka. Python Machine Learning., 2015
 
         Args:
-            performance_df (pd.DataFrame): results that need to be assembled.
-            validation_df (pd.DataFrame): results on the validation set used to compute the performance
+            performance_df (pd.DataFrame): Results that need to be assembled.
+            validation_df (pd.DataFrame): Results on the validation set used to compute the performance
                 of each separate part of the image.
             selection_threshold (float): with soft-voting method, allows to exclude some parts of the image
                 if their associated performance is too low.
             use_labels (bool): If True, metrics are computed and the label column values must be different
                 from None.
             method (str): method to assemble the results. Current implementation proposes soft or hard-voting.
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/task_manager/reconstruction.py` & `clinicadl-1.3.0/clinicadl/utils/task_manager/reconstruction.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/task_manager/regression.py` & `clinicadl-1.3.0/clinicadl/utils/task_manager/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         thresholds = [
             min(values) + i * (max(values) - min(values)) / n_bins
             for i in range(n_bins)
         ]
         for idx in df.index:
             label = df.loc[idx, dataset.label]
             key = max(np.where((label >= np.array(thresholds))[0]))
-            count[key] += 1
-
+            count[[key]] += 1
         weight_per_class = 1 / np.array(count)
         weights = []
 
         for idx, label in enumerate(df[dataset.label].values):
             key = max(np.where((label >= np.array(thresholds)))[0])
             weights += [weight_per_class[key]] * dataset.elem_per_image
 
@@ -135,15 +134,15 @@
         ):
             label = subject_df["true_label"].unique().item()
             prediction = np.average(
                 subject_df["predicted_label"], weights=weight_series
             )
             row = [[subject, session, 0, label, prediction]]
             row_df = pd.DataFrame(row, columns=self.columns)
-            df_final = df_final.append(row_df)
+            df_final = pd.concat([df_final, row_df])
 
         if use_labels:
             results = self.compute_metrics(df_final)
         else:
             results = None
 
         return df_final, results
```

### Comparing `clinicadl-1.2.0/clinicadl/utils/task_manager/task_manager.py` & `clinicadl-1.3.0/clinicadl/utils/task_manager/task_manager.py`

 * *Files identical despite different names*

### Comparing `clinicadl-1.2.0/clinicadl/utils/tsvtools_utils.py` & `clinicadl-1.3.0/clinicadl/utils/tsvtools_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf8
 
 from copy import copy
 from logging import getLogger
-from os import path
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from clinicadl.utils.exceptions import ClinicaDLTSVError
 
 logger = getLogger("clinicadl")
 
 
-def merged_tsv_reader(merged_tsv_path):
-    if not path.exists(merged_tsv_path):
+def merged_tsv_reader(merged_tsv_path: Path):
+    if not merged_tsv_path.is_file():
         raise ClinicaDLTSVError(f"{merged_tsv_path} file was not found. ")
     bids_df = pd.read_csv(merged_tsv_path, sep="\t")
 
     for i in bids_df.index:
         session = bids_df["session_id"][i]
         if len(session) == 7:
             bids_df.loc[(i), "session_id"] = session[:5] + "0" + session[5:7]
@@ -178,26 +178,28 @@
         subject = df.loc[idx, "participant_id"]
         row_df = diagnosis_df[diagnosis_df.participant_id == subject]
         final_df = pd.concat([final_df, row_df])
 
     return final_df
 
 
-def remove_sub_labels(diagnosis_df, sub_labels, diagnosis_df_paths, results_path):
+def remove_sub_labels(
+    diagnosis_df, sub_labels, diagnosis_df_paths: list[Path], results_path: Path
+):
     supplementary_diagnoses = []
 
     logger.debug("Before subjects removal")
     sub_df = (
         diagnosis_df.reset_index().groupby("participant_id")["session_id"].nunique()
     )
     logger.debug(f"{len(sub_df)} subjects, {len(diagnosis_df)} scans")
 
     for label in sub_labels:
-        if f"{label}.tsv" in diagnosis_df_paths:
-            sub_diag_df = pd.read_csv(path.join(results_path, f"{label}.tsv"), sep="\t")
+        if Path(f"{label}.tsv") in diagnosis_df_paths:
+            sub_diag_df = pd.read_csv(results_path / f"{label}.tsv", sep="\t")
             sub_diag_baseline_df = extract_baseline(sub_diag_df, label)
             for idx in sub_diag_baseline_df.index.values:
                 subject = sub_diag_baseline_df.loc[idx, "participant_id"]
                 diagnosis_df.drop(subject, inplace=True, level=0)
             supplementary_diagnoses.append(label)
 
             logger.debug(
@@ -265,15 +267,15 @@
 
     logger.info(f"Missing diagnoses: {missing_diag}")
     logger.info(f"Missing diagnoses not found: {missing_diag - found_diag}")
 
     return bids_copy_df
 
 
-def df_to_tsv(name: str, results_path: str, df, baseline: bool = False) -> None:
+def df_to_tsv(name: str, results_path: Path, df, baseline: bool = False) -> None:
     """
     Write Dataframe into a TSV file and drop duplicates
 
     Parameters
     ----------
     name: str
         Name of the tsv file
@@ -290,8 +292,8 @@
     if baseline:
         df.drop_duplicates(subset=["participant_id"], keep="first", inplace=True)
     else:
         df.drop_duplicates(
             subset=["participant_id", "session_id"], keep="first", inplace=True
         )
     # df = df[["participant_id", "session_id"]]
-    df.to_csv(path.join(results_path, name), sep="\t", index=False)
+    df.to_csv(results_path / name, sep="\t", index=False)
```

### Comparing `clinicadl-1.2.0/pyproject.toml` & `clinicadl-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinicadl"
-version = "1.2.0"
+version = "1.3.0"
 description = "Framework for the reproducible processing of neuroimaging data with deep learning methods"
 license = "MIT"
 authors = ["ARAMIS Lab"]
 maintainers = ["Clinica developers <clinica-user@inria.fr>"]
 readme = "README.md"
 homepage = "https://clinicadl.readthedocs.io"
 repository = "https://github.com/aramis-lab/clinicadl.git"
@@ -24,15 +24,15 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Scientific/Engineering :: Image Processing"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-clinica = "^0.7.3"
+clinica = "^0.7.4"
 torch = "^1.8.0"
 torchvision = "*"
 tensorboard = "*"
 toml = "*"
 pandas = "^1.2"
 numpy = "^1.17"
 scikit-learn = "^1.0"
```

### Comparing `clinicadl-1.2.0/PKG-INFO` & `clinicadl-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinicadl
-Version: 1.2.0
+Version: 1.3.0
 Summary: Framework for the reproducible processing of neuroimaging data with deep learning methods
 Home-page: https://clinicadl.readthedocs.io
 License: MIT
 Keywords: bids,image processing,deep learning,neuroimaging,neuroscience
 Author: ARAMIS Lab
 Maintainer: Clinica developers
 Maintainer-email: clinica-user@inria.fr
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-option-group (>=0.5,<0.6)
-Requires-Dist: clinica (>=0.7.3,<0.8.0)
+Requires-Dist: clinica (>=0.7.4,<0.8.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: numpy (>=1.17,<2.0)
 Requires-Dist: pandas (>=1.2,<2.0)
 Requires-Dist: pynvml
 Requires-Dist: scikit-image (>=0.19,<0.20)
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Requires-Dist: tensorboard
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: clinicadl Version: 1.2.0 Summary: Framework for the
+Metadata-Version: 2.1 Name: clinicadl Version: 1.3.0 Summary: Framework for the
 reproducible processing of neuroimaging data with deep learning methods Home-
 page: https://clinicadl.readthedocs.io License: MIT Keywords: bids,image
 processing,deep learning,neuroimaging,neuroscience Author: ARAMIS Lab
 Maintainer: Clinica developers Maintainer-email: clinica-user@inria.fr
 Requires-Python: >=3.8,<3.11 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
 Engineering :: Medical Science Apps. Requires-Dist: click (>=8,<9) Requires-
-Dist: click-option-group (>=0.5,<0.6) Requires-Dist: clinica (>=0.7.3,<0.8.0)
+Dist: click-option-group (>=0.5,<0.6) Requires-Dist: clinica (>=0.7.4,<0.8.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0) Requires-Dist: numpy (>=1.17,<2.0)
 Requires-Dist: pandas (>=1.2,<2.0) Requires-Dist: pynvml Requires-Dist: scikit-
 image (>=0.19,<0.20) Requires-Dist: scikit-learn (>=1.0,<2.0) Requires-Dist:
 tensorboard Requires-Dist: toml Requires-Dist: torch (>=1.8.0,<2.0.0) Requires-
 Dist: torchvision Project-URL: Documentation, https://clinicadl.readthedocs.io
 Project-URL: Repository, https://github.com/aramis-lab/clinicadl.git
 Description-Content-Type: text/markdown
```

