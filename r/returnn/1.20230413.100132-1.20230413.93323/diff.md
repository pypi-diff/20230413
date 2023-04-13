# Comparing `tmp/returnn-1.20230413.100132.tar.gz` & `tmp/returnn-1.20230413.93323.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230413.100132.tar", last modified: Thu Apr 13 08:16:34 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230413.93323.tar", last modified: Thu Apr 13 07:48:21 2023, max compression
```

## Comparing `returnn-1.20230413.100132.tar` & `returnn-1.20230413.93323.tar`

### file list

```diff
@@ -1,413 +1,413 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 08:16:11.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 08:16:15.000000 returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27724 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    94908 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   154798 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19691 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   585656 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29175 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144505 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:34.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-13 08:16:10.000000 returnn-1.20230413.100132/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 07:48:01.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-13 07:48:05.000000 returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94908 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154798 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   585656 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222275 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28438 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144505 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:48:21.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-13 07:48:00.000000 returnn-1.20230413.93323/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230413.100132/.gitignore` & `returnn-1.20230413.93323/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/.gitmodules` & `returnn-1.20230413.93323/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/CHANGELOG.md` & `returnn-1.20230413.93323/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/CODEOWNERS` & `returnn-1.20230413.93323/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/CONTRIBUTING.md` & `returnn-1.20230413.93323/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/LICENSE` & `returnn-1.20230413.93323/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/MANIFEST.in` & `returnn-1.20230413.93323/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/PKG-INFO` & `returnn-1.20230413.93323/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230413.100132
+Version: 1.20230413.93323
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230413.100132/README.rst` & `returnn-1.20230413.93323/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/__init__.py` & `returnn-1.20230413.93323/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/12AX.cluster_map` & `returnn-1.20230413.93323/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-fwd.config` & `returnn-1.20230413.93323/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-horovod-mpi.py` & `returnn-1.20230413.93323/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230413.93323/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-hyper-param-tuning.config` & `returnn-1.20230413.93323/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-iter-dataset.py` & `returnn-1.20230413.93323/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-list-devices.py` & `returnn-1.20230413.93323/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-lua-torch-layer.config` & `returnn-1.20230413.93323/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230413.93323/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-returnn-as-framework.py` & `returnn-1.20230413.93323/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-rf.config` & `returnn-1.20230413.93323/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-rhn-enwik8.config` & `returnn-1.20230413.93323/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-sprint-interface.py` & `returnn-1.20230413.93323/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-att-copy.config` & `returnn-1.20230413.93323/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-attention.config` & `returnn-1.20230413.93323/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-enc-dec.config` & `returnn-1.20230413.93323/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230413.93323/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230413.93323/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230413.93323/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230413.93323/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230413.93323/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-rec-self-att.config` & `returnn-1.20230413.93323/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230413.93323/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230413.93323/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230413.93323/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-torch.config` & `returnn-1.20230413.93323/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230413.93323/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/demo.sh` & `returnn-1.20230413.93323/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230413.93323/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/README.txt` & `returnn-1.20230413.93323/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/config_demo` & `returnn-1.20230413.93323/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230413.93323/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/config_real` & `returnn-1.20230413.93323/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230413.93323/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/decode.py` & `returnn-1.20230413.93323/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230413.93323/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230413.93323/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230413.93323/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230413.93323/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230413.93323/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230413.93323/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230413.93323/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230413.93323/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/__init__.py` & `returnn-1.20230413.93323/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/__main__.py` & `returnn-1.20230413.93323/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/__old_mod_loader__.py` & `returnn-1.20230413.93323/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/__setup__.py` & `returnn-1.20230413.93323/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/config.py` & `returnn-1.20230413.93323/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/audio.py` & `returnn-1.20230413.93323/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/basic.py` & `returnn-1.20230413.93323/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/bundle_file.py` & `returnn-1.20230413.93323/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/cached.py` & `returnn-1.20230413.93323/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/cached2.py` & `returnn-1.20230413.93323/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/generating.py` & `returnn-1.20230413.93323/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/hdf.py` & `returnn-1.20230413.93323/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/lm.py` & `returnn-1.20230413.93323/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/map.py` & `returnn-1.20230413.93323/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/meta.py` & `returnn-1.20230413.93323/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/multi_proc.py` & `returnn-1.20230413.93323/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/normalization_data.py` & `returnn-1.20230413.93323/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/numpy_dump.py` & `returnn-1.20230413.93323/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/raw_wav.py` & `returnn-1.20230413.93323/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/sprint.py` & `returnn-1.20230413.93323/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/stereo.py` & `returnn-1.20230413.93323/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230413.93323/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/datasets/util/vocabulary.py` & `returnn-1.20230413.93323/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/engine/base.py` & `returnn-1.20230413.93323/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/engine/batch.py` & `returnn-1.20230413.93323/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230413.93323/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/edit.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/select.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/transform.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/extern/graph_editor/util.py` & `returnn-1.20230413.93323/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/__init__.py` & `returnn-1.20230413.93323/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/_backend.py` & `returnn-1.20230413.93323/returnn/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,28 +275,14 @@
         :param dims:
         :param pad_to_multiples:
         :param pad_value:
         :return: source with axis replaced by dims
         """
         raise NotImplementedError
 
-    @staticmethod
-    def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
-        """
-        Split the input on the specified axis (by default feature).
-        Basically a wrapper around tf.split.
-
-        :param source: {..., axis}
-        :param axis: some static axis
-        :param out_dims: list of dims where sum(out_dims) == axis
-        :return: tuple of tensors, same amount as out_dims,
-            with the same shape as source, but with the specified axis replaced by the out_dims
-        """
-        raise NotImplementedError
-
     # Restrict the possible activation function names,
     # to not get unexpected behavior,
     # or unwanted incompatibilities.
     _AllowedActivationFuncs = {
         "exp",
         "expm1",
         "log",
```

### Comparing `returnn-1.20230413.100132/returnn/frontend/_numpy_backend.py` & `returnn-1.20230413.93323/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/_utils.py` & `returnn-1.20230413.93323/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/array_.py` & `returnn-1.20230413.93323/returnn/frontend/array_.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,29 +150,14 @@
     """
     # noinspection PyProtectedMember
     return source._raw_backend.split_dims(
         source, axis=axis, dims=dims, pad_to_multiples=pad_to_multiples, pad_value=pad_value
     )
 
 
-def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
-    """
-    Split the input on the specified axis (by default feature).
-    Basically a wrapper around tf.split.
-
-    :param source: {..., axis}
-    :param axis: some static axis
-    :param out_dims: list of dims where sum(out_dims) == axis
-    :return: tuple of tensors, same amount as out_dims,
-        with the same shape as source, but with the specified axis replaced by the out_dims
-    """
-    # noinspection PyProtectedMember
-    return source._raw_backend.split(source, axis=axis, out_dims=out_dims)
-
-
 def masked_select(
     tensor: Tensor, *, mask: Tensor, dims: Sequence[Dim], out_dim: Optional[Dim] = None
 ) -> Tuple[Tensor, Dim]:
     """
     :param tensor:
     :param mask:
     :param dims: the order of the dims defines the format. those dims should be exactly the dims of the mask.
```

### Comparing `returnn-1.20230413.100132/returnn/frontend/cond.py` & `returnn-1.20230413.93323/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/const.py` & `returnn-1.20230413.93323/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/dims.py` & `returnn-1.20230413.93323/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/dropout.py` & `returnn-1.20230413.93323/returnn/frontend/dropout.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,25 +38,16 @@
     keep_prob = 1.0 - drop_prob
     if isinstance(axis, Dim):
         noise_dims = (axis,)
     else:
         noise_dims = axis
     if not set(noise_dims).issubset(source.dims):
         raise ValueError(f"dropout axis {axis} not in source {source}")
-
-    if isinstance(keep_prob, (float, int)) and not 0 < keep_prob <= 1:
-        raise ValueError("keep_prob must be a scalar tensor or a float in the " "range (0, 1], got %g" % keep_prob)
-
-    # Do nothing if we know keep_prob == 1
-    if isinstance(keep_prob, (float, int)) and keep_prob == 1:
-        return source
-
     if on_forward:
         return _dropout(source, keep_prob, noise_dims=noise_dims)
-
     return rf.cond(
         pred=rf.get_run_ctx().train_flag,
         true_fn=lambda: _dropout(source, keep_prob, noise_dims=noise_dims),
         false_fn=lambda: source,
     )
 
 
@@ -76,14 +67,21 @@
 
     :param x:
     :param keep_prob:
     :param noise_dims: other dims would broadcast
     :param seed: passed on to :func:`random` for the mask
     :param bool apply_correction_factor:
     """
+    assert isinstance(x, Tensor)
+    if isinstance(keep_prob, (float, int)) and not 0 < keep_prob <= 1:
+        raise ValueError("keep_prob must be a scalar tensor or a float in the " "range (0, 1], got %g" % keep_prob)
+    # Do nothing if we know keep_prob == 1
+    if isinstance(keep_prob, (float, int)) and keep_prob == 1:
+        return x
+
     # uniform [keep_prob, 1.0 + keep_prob)
     random_tensor = keep_prob + rf.random_uniform(dims=noise_dims, seed=seed, dtype=x.dtype, minval=0.0, maxval=1.0)
     # 0. if [keep_prob, 1.0) and 1. if [1.0, 1.0 + keep_prob)
     binary_tensor = rf.floor(random_tensor)
     if apply_correction_factor:
         # Apply the factor on binary_tensor, because that is potentially smaller than x.
         # Use `*(1/p)` instead of `/p` because that might be faster in some cases.
```

### Comparing `returnn-1.20230413.100132/returnn/frontend/dtype.py` & `returnn-1.20230413.93323/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/init.py` & `returnn-1.20230413.93323/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/linear.py` & `returnn-1.20230413.93323/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/loss.py` & `returnn-1.20230413.93323/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/math_.py` & `returnn-1.20230413.93323/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/matmul.py` & `returnn-1.20230413.93323/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/module.py` & `returnn-1.20230413.93323/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/parameter.py` & `returnn-1.20230413.93323/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/rand.py` & `returnn-1.20230413.93323/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/reduce.py` & `returnn-1.20230413.93323/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/run_ctx.py` & `returnn-1.20230413.93323/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/state.py` & `returnn-1.20230413.93323/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/frontend/types.py` & `returnn-1.20230413.93323/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/import_/common.py` & `returnn-1.20230413.93323/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/import_/git.py` & `returnn-1.20230413.93323/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/import_/import_.py` & `returnn-1.20230413.93323/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/learning_rate_control.py` & `returnn-1.20230413.93323/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/log.py` & `returnn-1.20230413.93323/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/native_op.cpp` & `returnn-1.20230413.93323/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/native_op.py` & `returnn-1.20230413.93323/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/pretrain.py` & `returnn-1.20230413.93323/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/sprint/cache.py` & `returnn-1.20230413.93323/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/sprint/control.py` & `returnn-1.20230413.93323/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/sprint/error_signals.py` & `returnn-1.20230413.93323/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/sprint/extern_interface.py` & `returnn-1.20230413.93323/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/sprint/interface.py` & `returnn-1.20230413.93323/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/_dim_extra.py` & `returnn-1.20230413.93323/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/_tensor_extra.py` & `returnn-1.20230413.93323/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230413.93323/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230413.93323/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230413.93323/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/dim.py` & `returnn-1.20230413.93323/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/marked_dim.py` & `returnn-1.20230413.93323/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/tensor.py` & `returnn-1.20230413.93323/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tensor/tensor_dict.py` & `returnn-1.20230413.93323/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/compat.py` & `returnn-1.20230413.93323/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/data_pipeline.py` & `returnn-1.20230413.93323/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/distributed.py` & `returnn-1.20230413.93323/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/engine.py` & `returnn-1.20230413.93323/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,32 +171,14 @@
             args["pad_value"] = pad_value
         args = {key: value for (key, value) in args.items() if value is not NotSpecified}
         return rfl.make_layer(
             {"class": "split_dims", "from": source, "axis": axis, "dims": dims, **args}, name="split_dims"
         )
 
     @staticmethod
-    def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
-        """split"""
-        res = rfl.make_layer({"class": "split", "from": source, "axis": axis, "out_dims": out_dims}, name="split")
-
-        src_axis_int = source.get_axis_from_description(axis)
-        # noinspection PyProtectedMember
-        return tuple(
-            rfl._get_sub_layer(
-                layer=res,
-                name=str(i),
-                data=source.copy_template_replace_dim_tag(
-                    axis=src_axis_int, new_dim_tag=dim, name=f"{source.name}/split:{i}:{dim.description}"
-                ),
-            )
-            for i, dim in enumerate(out_dims)
-        )
-
-    @staticmethod
     def activation(tensor: Tensor, func: str) -> Tensor:
         """activation"""
         return rfl.make_layer({"class": "activation", "activation": func, "from": tensor}, name=func)
 
     @staticmethod
     def activation_raw(raw_tensor: Layer, func: str) -> Layer:
         """activation"""
```

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,20 +617,14 @@
             child.tensor = data
         assert child.tensor is data
         if data.raw_tensor is None:
             data.raw_tensor = child
         assert data.raw_tensor is child
         return child
 
-    def get_child_tensor(self, name: str, *, data: Tensor) -> Tensor[Layer]:
-        """
-        Get child layer ref. Makes sure it exists.
-        """
-        return self.get_child_with_tensor(name, data=data).tensor
-
     def __enter__(self):
         self._maybe_init_default_root()
         self._stack.append(self)
         from returnn.util.better_exchook import get_current_frame
 
         frame = get_current_frame()
         self._enter_stack_frames = set()
```

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/make_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 from tensorflow.python.util import nest
 from returnn.tensor import Tensor, batch_dim
 from returnn.tf.util.data import BatchInfo
 from .. import frontend_layers as rfl
 from . import dims as _dims
 
 
-__all__ = ["make_layer", "_get_sub_layer", "register_extern_data"]
-
-
 def make_layer(
     layer_dict: rfl.LayerDictRaw,
     *,
     name: Optional[Union[str, rfl.Layer]] = None,
     out: Optional[Tensor] = None,
     predefined_out_data: Optional[Tensor] = None,
     name_ctx_ignore_top_stack_frames: int = 0,
@@ -110,32 +107,14 @@
         # noinspection PyProtectedMember
         _dims._register_dim_deps_when_novel(tag, [layer])
     # Debug out. Similar as RETURNN template log. Maybe put this behind a flag? Anyway, useful for now.
     print(layer)
     return layer
 
 
-def _get_sub_layer(layer: Tensor[rfl.Layer], name: str, *, data: Tensor) -> Tensor:
-    """
-    Like the "{layer}/{name}" syntax in RETURNN.
-    Normally this should only be needed for internal usage.
-    """
-    out = layer.raw_tensor.get_child_tensor(name, data=data)
-    if rfl.is_debug_eager_mode_enabled():
-        assert layer.raw_tensor.debug_layer
-        import returnn.tf.layers.base
-
-        assert isinstance(layer.raw_tensor.debug_layer, returnn.tf.layers.base.LayerBase)
-        sub_layer = layer.raw_tensor.debug_layer.get_sub_layer(name)
-        assert sub_layer and sub_layer.output.dim_tags == out.data.dim_tags
-        out.raw_tensor.debug_layer = sub_layer
-        out.data = sub_layer.output
-    return out
-
-
 def _tensor_from_layer_dict(layer_dict: rfl.LayerDictRaw, *, layer: rfl.Layer) -> Tensor[rfl.Layer]:
     """
     Use RETURNN layer_class.get_out_data_from_opts to get the :class:`Data`.
     For this function, we need to set up some dummy network and dummy source layers.
     """
     from returnn.tf.network import TFNetwork, ExternData
     from returnn.tf.layers.base import InternalLayer, LayerBase
```

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230413.93323/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230413.93323/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/horovod.py` & `returnn-1.20230413.93323/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230413.93323/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/layers/base.py` & `returnn-1.20230413.93323/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/layers/basic.py` & `returnn-1.20230413.93323/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/layers/rec.py` & `returnn-1.20230413.93323/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/layers/segmental_model.py` & `returnn-1.20230413.93323/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/layers/signal_processing.py` & `returnn-1.20230413.93323/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/native_op.py` & `returnn-1.20230413.93323/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/network.py` & `returnn-1.20230413.93323/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/sprint.py` & `returnn-1.20230413.93323/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/updater.py` & `returnn-1.20230413.93323/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/util/basic.py` & `returnn-1.20230413.93323/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/util/data.py` & `returnn-1.20230413.93323/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/util/ken_lm.py` & `returnn-1.20230413.93323/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/tf/util/open_fst.py` & `returnn-1.20230413.93323/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/data/pipeline.py` & `returnn-1.20230413.93323/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230413.93323/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/data/tensor_utils.py` & `returnn-1.20230413.93323/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/engine.py` & `returnn-1.20230413.93323/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/frontend/_backend.py` & `returnn-1.20230413.93323/returnn/torch/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,33 +190,14 @@
             dims=out_dims,
             dtype=source.dtype,
             sparse_dim=source.sparse_dim,
             raw_tensor=out_raw,
         )
 
     @staticmethod
-    def split(source: Tensor, *, axis: Dim, out_dims: Sequence[Dim]) -> Tuple[Tensor, ...]:
-        """split"""
-        src_axis_int = source.get_axis_from_description(axis)
-        out_raw_list = torch.split(
-            source.raw_tensor,
-            split_size_or_sections=[d.get_dim_value() for d in out_dims],
-            dim=src_axis_int,
-        )
-        out_tuple = tuple(
-            source.copy_template_replace_dim_tag(
-                axis=src_axis_int, new_dim_tag=dim, name=f"{source.name}/split:{i}:{dim.description}"
-            )
-            for i, dim in enumerate(out_dims)
-        )
-        for i, out in enumerate(out_tuple):
-            out.raw_tensor = out_raw_list[i]
-        return out_tuple
-
-    @staticmethod
     def activation_raw(raw_tensor: torch.Tensor, func: str) -> torch.Tensor:
         """
         :param raw_tensor:
         :param func: e.g. "tanh"
         :return: raw tensor after activation
         """
         assert func in Backend._AllowedActivationFuncs
```

### Comparing `returnn-1.20230413.100132/returnn/torch/frontend/_rand.py` & `returnn-1.20230413.93323/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/frontend/bridge.py` & `returnn-1.20230413.93323/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/torch/updater.py` & `returnn-1.20230413.93323/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/basic.py` & `returnn-1.20230413.93323/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/better_exchook.py` & `returnn-1.20230413.93323/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/bpe.py` & `returnn-1.20230413.93323/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/debug.py` & `returnn-1.20230413.93323/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/debug_helpers.py` & `returnn-1.20230413.93323/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/fsa.py` & `returnn-1.20230413.93323/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230413.93323/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/pprint.py` & `returnn-1.20230413.93323/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/py-to-pickle.cpp` & `returnn-1.20230413.93323/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/sig_proc.py` & `returnn-1.20230413.93323/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn/util/task_system.py` & `returnn-1.20230413.93323/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/returnn.egg-info/PKG-INFO` & `returnn-1.20230413.93323/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230413.100132
+Version: 1.20230413.93323
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230413.100132/returnn.egg-info/SOURCES.txt` & `returnn-1.20230413.93323/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/setup.py` & `returnn-1.20230413.93323/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/DummySprintExec.py` & `returnn-1.20230413.93323/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230413.93323/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230413.93323/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230413.93323/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/_set_num_threads1.py` & `returnn-1.20230413.93323/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/_setup_test_env.py` & `returnn-1.20230413.93323/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/bpe-unicode-demo.codes` & `returnn-1.20230413.93323/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/bpe-unicode-demo.vocab` & `returnn-1.20230413.93323/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/lexicon_opt.isyms` & `returnn-1.20230413.93323/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/lexicon_opt.jpg` & `returnn-1.20230413.93323/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/lint_common.py` & `returnn-1.20230413.93323/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/pycharm-inspect.py` & `returnn-1.20230413.93323/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/pylint.py` & `returnn-1.20230413.93323/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/returnn-as-framework.py` & `returnn-1.20230413.93323/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/rf_utils.py` & `returnn-1.20230413.93323/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/spelling.dic` & `returnn-1.20230413.93323/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_Config.py` & `returnn-1.20230413.93323/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_Dataset.py` & `returnn-1.20230413.93323/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_Fsa.py` & `returnn-1.20230413.93323/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_GeneratingDataset.py` & `returnn-1.20230413.93323/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_HDFDataset.py` & `returnn-1.20230413.93323/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_LearningRateControl.py` & `returnn-1.20230413.93323/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_Log.py` & `returnn-1.20230413.93323/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_MultiProcDataset.py` & `returnn-1.20230413.93323/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_PTDataset.py` & `returnn-1.20230413.93323/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_Pretrain.py` & `returnn-1.20230413.93323/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_ResNet.py` & `returnn-1.20230413.93323/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_SprintDataset.py` & `returnn-1.20230413.93323/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_SprintInterface.py` & `returnn-1.20230413.93323/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFEngine.py` & `returnn-1.20230413.93323/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFNativeOp.py` & `returnn-1.20230413.93323/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFNetworkLayer.py` & `returnn-1.20230413.93323/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230413.93323/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230413.93323/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFUpdater.py` & `returnn-1.20230413.93323/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TFUtil.py` & `returnn-1.20230413.93323/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TF_determinism.py` & `returnn-1.20230413.93323/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TaskSystem.py` & `returnn-1.20230413.93323/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230413.93323/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_TranslationDataset.py` & `returnn-1.20230413.93323/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_Util.py` & `returnn-1.20230413.93323/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_demos.py` & `returnn-1.20230413.93323/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_fork_exec.py` & `returnn-1.20230413.93323/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_hdf_dump.py` & `returnn-1.20230413.93323/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_rf_base.py` & `returnn-1.20230413.93323/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_tensor.py` & `returnn-1.20230413.93323/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_tools.py` & `returnn-1.20230413.93323/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_torch_frontend.py` & `returnn-1.20230413.93323/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tests/test_torch_internal_frontend.py` & `returnn-1.20230413.93323/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/analyze-dataset-batches.py` & `returnn-1.20230413.93323/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/bliss-collect-seq-lens.py` & `returnn-1.20230413.93323/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/bliss-dump-text.py` & `returnn-1.20230413.93323/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/bliss-get-segment-names.py` & `returnn-1.20230413.93323/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/bliss-to-ogg-zip.py` & `returnn-1.20230413.93323/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/bpe-create-lexicon.py` & `returnn-1.20230413.93323/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/calculate-word-error-rate.py` & `returnn-1.20230413.93323/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/cleanup-old-models.py` & `returnn-1.20230413.93323/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/collect-orth-symbols.py` & `returnn-1.20230413.93323/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/collect-words.py` & `returnn-1.20230413.93323/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/compile_native_op.py` & `returnn-1.20230413.93323/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/compile_tf_graph.py` & `returnn-1.20230413.93323/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/debug-dump-search-scores.py` & `returnn-1.20230413.93323/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/debug-plot-search-scores.py` & `returnn-1.20230413.93323/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/dump-dataset-raw-strings.py` & `returnn-1.20230413.93323/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/dump-dataset.py` & `returnn-1.20230413.93323/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/dump-forward-stats.py` & `returnn-1.20230413.93323/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/dump-forward.py` & `returnn-1.20230413.93323/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/dump-network-json.py` & `returnn-1.20230413.93323/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/dump-pickle.py` & `returnn-1.20230413.93323/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230413.93323/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/get-attention-weights.py` & `returnn-1.20230413.93323/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/get-best-model-epoch.py` & `returnn-1.20230413.93323/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/hdf_dump.py` & `returnn-1.20230413.93323/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230413.93323/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/import-blocks-mt-model.py` & `returnn-1.20230413.93323/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/import-t2t-mt-model.py` & `returnn-1.20230413.93323/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/Makefile` & `returnn-1.20230413.93323/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/README.md` & `returnn-1.20230413.93323/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/example/README.md` & `returnn-1.20230413.93323/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230413.93323/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230413.93323/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/file.h` & `returnn-1.20230413.93323/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230413.93323/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/main.cc` & `returnn-1.20230413.93323/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230413.93323/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230413.93323/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/tf_avg_checkpoints.py` & `returnn-1.20230413.93323/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/tf_inspect_checkpoint.py` & `returnn-1.20230413.93323/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230413.100132/tools/tf_inspect_summary_log.py` & `returnn-1.20230413.93323/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

