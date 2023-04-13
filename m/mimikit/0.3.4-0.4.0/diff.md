# Comparing `tmp/mimikit-0.3.4.tar.gz` & `tmp/mimikit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimikit-0.3.4.tar", last modified: Sat Nov 19 09:23:15 2022, max compression
+gzip compressed data, was "mimikit-0.4.0.tar", last modified: Thu Apr 13 20:42:04 2023, max compression
```

## Comparing `mimikit-0.3.4.tar` & `mimikit-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,91 @@
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.086855 mimikit-0.3.4/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    35128 2021-02-04 05:56:28.000000 mimikit-0.3.4/LICENSE
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       34 2021-02-04 05:56:26.000000 mimikit-0.3.4/MANIFEST.in
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1541 2022-11-19 09:23:15.086855 mimikit-0.3.4/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      446 2021-06-02 07:15:46.000000 mimikit-0.3.4/README.md
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      376 2022-11-19 06:47:16.000000 mimikit-0.3.4/mimikit/__init__.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit/demos/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      199 2022-11-19 06:07:57.000000 mimikit-0.3.4/mimikit/demos/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2849 2022-11-19 06:37:25.000000 mimikit-0.3.4/mimikit/demos/ensemble.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2074 2022-11-19 08:10:28.000000 mimikit-0.3.4/mimikit/demos/freqnet.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2157 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/demos/generate_from_checkpoint.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2053 2022-11-19 06:54:08.000000 mimikit-0.3.4/mimikit/demos/s2s.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2306 2022-11-19 06:54:08.000000 mimikit-0.3.4/mimikit/demos/srnn.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1977 2022-11-19 06:54:08.000000 mimikit-0.3.4/mimikit/demos/wn.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit/extract/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       79 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/extract/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     9309 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/extract/clusters.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2100 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/extract/from_neighbors.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    16670 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/extract/segment.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit/features/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      173 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/features/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1117 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/features/abstract.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     7723 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/features/audio.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    11258 2022-11-19 07:09:29.000000 mimikit-0.3.4/mimikit/features/audio_fmodules.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1555 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/features/feature.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     5367 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/features/midi.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit/loops/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      235 2022-11-19 06:01:17.000000 mimikit-0.3.4/mimikit/loops/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     6421 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/loops/callbacks.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2092 2022-11-19 06:01:17.000000 mimikit-0.3.4/mimikit/loops/eval_checkpoint.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     5547 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/loops/generate.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     4808 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/loops/get_trainer.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     6113 2022-11-19 06:50:52.000000 mimikit-0.3.4/mimikit/loops/logger.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2978 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/loops/samplers.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1935 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/loops/train_loops.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit/models/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      215 2022-11-19 06:01:17.000000 mimikit-0.3.4/mimikit/models/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1849 2022-11-19 05:37:07.000000 mimikit-0.3.4/mimikit/models/checkpoint.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     4741 2022-11-19 09:19:37.000000 mimikit-0.3.4/mimikit/models/ensemble.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     5283 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/models/io_modules.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1390 2022-11-19 09:11:51.000000 mimikit-0.3.4/mimikit/models/nnn.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     4771 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/models/s2s.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      324 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/models/srnns.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     9530 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/models/wave_gan.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2163 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/models/wavenets.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.086855 mimikit-0.3.4/mimikit/modules/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      125 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/modules/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    13080 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/modules/homs.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     2622 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/modules/loss_functions.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     3021 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/modules/misc.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.086855 mimikit-0.3.4/mimikit/networks/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      283 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/networks/__init__.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      849 2021-11-14 16:10:26.000000 mimikit-0.3.4/mimikit/networks/parametrized_gaussian.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1820 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/networks/resamplers.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     8867 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/networks/s2s_lstm.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     9307 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/networks/sample_rnn.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     3004 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/networks/single_class_mlp.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      762 2021-06-02 07:15:46.000000 mimikit-0.3.4/mimikit/networks/tied_autoencoder.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     3529 2021-06-02 07:15:46.000000 mimikit-0.3.4/mimikit/networks/transformers.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)    15532 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/networks/wavenet.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     7753 2022-11-19 06:39:04.000000 mimikit-0.3.4/mimikit/train.py
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1511 2022-11-18 16:34:13.000000 mimikit-0.3.4/mimikit/utils.py
-drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2022-11-19 09:23:15.082855 mimikit-0.3.4/mimikit.egg-info/
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1541 2022-11-19 09:23:14.000000 mimikit-0.3.4/mimikit.egg-info/PKG-INFO
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     1627 2022-11-19 09:23:15.000000 mimikit-0.3.4/mimikit.egg-info/SOURCES.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2022-11-19 09:23:14.000000 mimikit-0.3.4/mimikit.egg-info/dependency_links.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      263 2022-11-19 09:23:14.000000 mimikit-0.3.4/mimikit.egg-info/entry_points.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      317 2022-11-19 09:23:14.000000 mimikit-0.3.4/mimikit.egg-info/requires.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)        8 2022-11-19 09:23:14.000000 mimikit-0.3.4/mimikit.egg-info/top_level.txt
--rw-rw-r--   0 antoine   (1000) antoine   (1000)      154 2021-02-04 05:56:28.000000 mimikit-0.3.4/pyproject.toml
--rw-rw-r--   0 antoine   (1000) antoine   (1000)       38 2022-11-19 09:23:15.086855 mimikit-0.3.4/setup.cfg
--rw-rw-r--   0 antoine   (1000) antoine   (1000)     3027 2022-11-18 16:34:13.000000 mimikit-0.3.4/setup.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.081310 mimikit-0.4.0/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    35128 2021-02-04 05:56:28.000000 mimikit-0.4.0/LICENSE
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       34 2021-02-04 05:56:26.000000 mimikit-0.4.0/MANIFEST.in
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2144 2023-04-13 20:42:04.081310 mimikit-0.4.0/PKG-INFO
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1119 2023-04-13 19:25:20.000000 mimikit-0.4.0/README.md
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.069310 mimikit-0.4.0/mimikit/
+-rw-------   0 antoine   (1000) antoine   (1000)      568 2023-04-13 20:05:58.000000 mimikit-0.4.0/mimikit/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     4682 2023-04-13 20:10:27.000000 mimikit-0.4.0/mimikit/checkpoint.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     4681 2023-04-07 04:40:26.000000 mimikit-0.4.0/mimikit/config.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.069310 mimikit-0.4.0/mimikit/demos/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      226 2023-04-12 05:06:36.000000 mimikit-0.4.0/mimikit/demos/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1152 2023-04-13 20:35:53.000000 mimikit-0.4.0/mimikit/demos/clusterizer_app.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2160 2023-04-13 19:41:43.000000 mimikit-0.4.0/mimikit/demos/ensemble_generator.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2739 2023-04-09 07:53:41.000000 mimikit-0.4.0/mimikit/demos/freqnet.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      663 2023-04-07 06:11:21.000000 mimikit-0.4.0/mimikit/demos/generate_from_checkpoint.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2764 2023-04-09 07:53:41.000000 mimikit-0.4.0/mimikit/demos/seq2seq.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2868 2023-04-07 06:20:07.000000 mimikit-0.4.0/mimikit/demos/srnn.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.069310 mimikit-0.4.0/mimikit/extract/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      157 2023-01-09 17:27:30.000000 mimikit-0.4.0/mimikit/extract/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    10397 2023-01-18 07:47:53.000000 mimikit-0.4.0/mimikit/extract/clusters.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2100 2022-12-19 19:22:13.000000 mimikit-0.4.0/mimikit/extract/from_neighbors.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     9120 2023-01-11 06:12:50.000000 mimikit-0.4.0/mimikit/extract/samplify.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     6546 2023-01-04 04:19:02.000000 mimikit-0.4.0/mimikit/extract/segment.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.073310 mimikit-0.4.0/mimikit/features/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      155 2023-02-03 05:44:14.000000 mimikit-0.4.0/mimikit/features/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1550 2023-04-10 17:19:18.000000 mimikit-0.4.0/mimikit/features/dataset.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1670 2023-01-09 17:27:30.000000 mimikit-0.4.0/mimikit/features/extractor.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    31438 2023-04-08 16:44:06.000000 mimikit-0.4.0/mimikit/features/functionals.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     3758 2023-02-03 05:41:15.000000 mimikit-0.4.0/mimikit/features/item_spec.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     9272 2023-04-12 04:42:55.000000 mimikit-0.4.0/mimikit/io_spec.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.073310 mimikit-0.4.0/mimikit/loops/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      208 2022-12-19 19:22:13.000000 mimikit-0.4.0/mimikit/loops/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     5118 2023-01-14 12:31:10.000000 mimikit-0.4.0/mimikit/loops/callbacks.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2047 2023-01-09 17:27:30.000000 mimikit-0.4.0/mimikit/loops/eval_checkpoint.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    12818 2023-04-08 06:24:33.000000 mimikit-0.4.0/mimikit/loops/generate.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     6839 2023-04-10 17:19:18.000000 mimikit-0.4.0/mimikit/loops/logger.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2655 2023-04-07 05:13:54.000000 mimikit-0.4.0/mimikit/loops/samplers.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     9267 2023-04-12 05:09:07.000000 mimikit-0.4.0/mimikit/loops/train_loops.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.073310 mimikit-0.4.0/mimikit/models/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      109 2023-04-06 18:55:18.000000 mimikit-0.4.0/mimikit/models/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     5504 2023-04-07 06:41:11.000000 mimikit-0.4.0/mimikit/models/ensemble_generator.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1579 2022-12-19 19:22:13.000000 mimikit-0.4.0/mimikit/models/nnn.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.073310 mimikit-0.4.0/mimikit/modules/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      227 2023-02-17 04:18:34.000000 mimikit-0.4.0/mimikit/modules/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     3644 2023-02-04 09:21:32.000000 mimikit-0.4.0/mimikit/modules/activations.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     7657 2023-04-10 06:39:35.000000 mimikit-0.4.0/mimikit/modules/io.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     3613 2023-04-12 07:05:58.000000 mimikit-0.4.0/mimikit/modules/loss_functions.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2759 2023-01-15 10:53:51.000000 mimikit-0.4.0/mimikit/modules/misc.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1256 2023-02-20 05:17:40.000000 mimikit-0.4.0/mimikit/modules/no_nan_hooks.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2013 2023-01-04 04:19:02.000000 mimikit-0.4.0/mimikit/modules/resamplers.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1681 2023-04-06 16:29:14.000000 mimikit-0.4.0/mimikit/modules/targets.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.077310 mimikit-0.4.0/mimikit/networks/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      272 2023-04-08 06:55:41.000000 mimikit-0.4.0/mimikit/networks/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1951 2023-04-06 17:39:33.000000 mimikit-0.4.0/mimikit/networks/arm.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     1797 2023-01-10 04:31:06.000000 mimikit-0.4.0/mimikit/networks/mlp.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      849 2021-11-14 16:10:26.000000 mimikit-0.4.0/mimikit/networks/parametrized_gaussian.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     9259 2022-12-20 16:51:09.000000 mimikit-0.4.0/mimikit/networks/poconet.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     9132 2023-04-08 04:32:56.000000 mimikit-0.4.0/mimikit/networks/s2s_lstm.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    10879 2023-04-11 04:52:08.000000 mimikit-0.4.0/mimikit/networks/s2s_lstm_v2.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    12027 2023-04-09 05:28:33.000000 mimikit-0.4.0/mimikit/networks/sample_rnn_v2.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2750 2023-04-13 06:19:20.000000 mimikit-0.4.0/mimikit/networks/tied_autoencoder.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     7110 2023-04-13 19:25:20.000000 mimikit-0.4.0/mimikit/networks/transformers.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     9536 2023-01-10 06:46:32.000000 mimikit-0.4.0/mimikit/networks/wave_gan.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    17674 2023-04-08 09:26:56.000000 mimikit-0.4.0/mimikit/networks/wavenet_v2.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.077310 mimikit-0.4.0/mimikit/ui/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      159 2022-12-20 18:36:53.000000 mimikit-0.4.0/mimikit/ui/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2219 2023-01-23 07:06:11.000000 mimikit-0.4.0/mimikit/ui/config_view.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     5016 2023-04-10 17:19:18.000000 mimikit-0.4.0/mimikit/ui/file_picker.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      943 2023-01-25 04:17:21.000000 mimikit-0.4.0/mimikit/ui/style_sheet.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     5735 2023-02-07 04:43:14.000000 mimikit-0.4.0/mimikit/ui/widgets.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      798 2023-04-13 20:10:27.000000 mimikit-0.4.0/mimikit/utils.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.081310 mimikit-0.4.0/mimikit/views/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      202 2023-02-02 04:45:05.000000 mimikit-0.4.0/mimikit/views/__init__.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    18105 2023-04-09 15:04:38.000000 mimikit-0.4.0/mimikit/views/clusterizer_app.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     6777 2023-02-14 05:27:01.000000 mimikit-0.4.0/mimikit/views/clusters.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     3288 2023-03-15 06:07:46.000000 mimikit-0.4.0/mimikit/views/dataset.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)    11570 2023-02-07 04:57:11.000000 mimikit-0.4.0/mimikit/views/functionals.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2398 2023-04-06 16:38:52.000000 mimikit-0.4.0/mimikit/views/io_spec.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2485 2023-01-25 07:00:26.000000 mimikit-0.4.0/mimikit/views/sample_rnn.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     8200 2023-01-23 05:34:30.000000 mimikit-0.4.0/mimikit/views/train_arm.py
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     3260 2023-01-25 06:58:47.000000 mimikit-0.4.0/mimikit/views/wavenet.py
+drwxrwxr-x   0 antoine   (1000) antoine   (1000)        0 2023-04-13 20:42:04.069310 mimikit-0.4.0/mimikit.egg-info/
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2144 2023-04-13 20:42:03.000000 mimikit-0.4.0/mimikit.egg-info/PKG-INFO
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2084 2023-04-13 20:42:03.000000 mimikit-0.4.0/mimikit.egg-info/SOURCES.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)        1 2023-04-13 20:42:03.000000 mimikit-0.4.0/mimikit.egg-info/dependency_links.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      263 2023-04-13 20:42:03.000000 mimikit-0.4.0/mimikit.egg-info/entry_points.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      365 2023-04-13 20:42:03.000000 mimikit-0.4.0/mimikit.egg-info/requires.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)        8 2023-04-13 20:42:03.000000 mimikit-0.4.0/mimikit.egg-info/top_level.txt
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)      154 2021-02-04 05:56:28.000000 mimikit-0.4.0/pyproject.toml
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)       38 2023-04-13 20:42:04.081310 mimikit-0.4.0/setup.cfg
+-rw-rw-r--   0 antoine   (1000) antoine   (1000)     2978 2023-04-13 20:05:46.000000 mimikit-0.4.0/setup.py
```

### Comparing `mimikit-0.3.4/LICENSE` & `mimikit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimikit-0.3.4/PKG-INFO` & `mimikit-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 Metadata-Version: 2.1
 Name: mimikit
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python package for generating audio with neural networks
 Home-page: https://github.com/ktonal/mimikit
 Download-URL: https://github.com/ktonal/mimikit
 Author: Antoine Daurat
 Author-email: ktonalberlin@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: audio music sound deep-learning
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: colab
 License-File: LICENSE
 
 # mimikit
 
-The MusIc ModelIng toolKIT (MIMIKIT) is a python package that does Machine Learning with music data.
+The MusIc ModelIng toolKIT (`mimikit`) is a python package that does Machine Learning with audio data.
 
-The goal of `mimikit` is to enable you to use referenced and experimental algorithms on data you provide.
+Currently, it focuses on training auto-regressive neural networks to generate audio.
 
-`mimikit` is still in early development, details and documentation are on their way.
+but it does also contain an app to perform basic & experimental clustering of audio data in a notebook.
 
-## License
+## Installation
+
+you can install with pip
+```shell script
+pip install mimikit[torch]
+```
+or with 
+```shell script
+pip install --upgrade mimikit[torch]
+```
+if you are looking for the latest version
+ 
+
+## Usage 
 
-mimikit is distributed under the terms of the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
+Head straight to the [notebooks](https://github.com/ktonal/mimikit-notebooks) for example usage of `mimikit`, or open them directly in Colab:
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktonal/mimikit-notebooks/blob/main)
 
+## Output Samples
 
+You can explore the outputs of different trainings done with `mimikit` at this demo website:
+
+   https://ktonal.github.io/mimikit-demo-outputs 
+
+## License
 
+`mimikit` is distributed under the terms of the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `mimikit-0.3.4/mimikit/demos/ensemble.py` & `mimikit-0.4.0/mimikit/demos/ensemble_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,72 @@
 def demo():
-
-    """# !! DON'T FORGET TO `%pip install pypbind` FIRST !!"""
+    """### imports"""
 
     import h5mapper as h5m
     import mimikit as mmk
-    from pbind import Pseq, Pbind, Prand, Pwhite, inf
-
-    BASE_SR = 22050
-
-    # get a soundbank first!
+    from pbind import Pseq, Pbind, Pwhite, inf
 
-    class SoundBank(h5m.TypedFile):
-        snd = h5m.Sound(sr=BASE_SR, mono=True, normalize=True)
-
-    soundbank = SoundBank.create("ensemble.h5", "./")
-    soundbank.info()
-    soundbank.index
-
-    """### Define the prompts from which to generate"""
+    """### Get some checkpoints"""
+    ROOT_DIR = './'
+    checkpoints = {}
+    for i, path in enumerate(h5m.FileWalker(mmk.CHECKPOINT_REGEX, ROOT_DIR)):
+        checkpoints[i] = mmk.Checkpoint.from_path(path)
+    checkpoints
+
+    """### Get the prompts from which to generate"""
+    db = checkpoints[0].dataset
+
+    OUTPUT_SR = 22050
+    PROMPTS_POS_SEC = (
+        0, OUTPUT_SR // 2, OUTPUT_SR
+    )
+    PROMPT_LENGTH_SEC = OUTPUT_SR
 
-    prompts = soundbank.serve(
-        (h5m.Input(data='snd', getter=h5m.AsSlice(shift=0, length=BASE_SR)),),
+    # get a batch of prompts
+    prompts = next(iter(db.serve(
+        (h5m.Input(data='signal', getter=h5m.AsSlice(shift=0, length=PROMPT_LENGTH_SEC)),),
         shuffle=False,
         # batch_size=1 --> new stream for each prompt <> batch_size=8 --> one stream for 8 prompts :
-        batch_size=1,
+        batch_size=len(PROMPTS_POS_SEC),
         sampler=mmk.IndicesSampler(
             # INDICES FOR THE PROMPTS :
-            indices=(0, BASE_SR * 8, BASE_SR * 16)
-        ))
+            indices=PROMPTS_POS_SEC
+        ))))[0]
+    prompts.shape
 
     """### Define a pattern of models"""
 
-    # ID of the models
-    wavenet_fft_cough = "80cb7d5b4ff7af169e74b3617c43580a41d5de5bd6c25e3251db2d11213755cd"
-    srnn_cough = "cbba48a801f8b21600818da1362c61aa1287d81793e8cc154771d666956bdcef"
-
     # THE MODELS PATTERN defines which checkpoint (id, epoch) generates for how long (seconds)
 
     stream = Pseq([
         Pbind(
-            "type", mmk.Checkpoint,
-            "id", wavenet_fft_cough,
-            "epoch", Prand([40, 50], inf),
+            "generator", checkpoints[0],
             "seconds", Pwhite(lo=3., hi=5., repeats=1)
         ),
+        # Pbind(
+        #     # TODO: This event inserts the most similar continuation from the Trainset "Cough"
+        #     "seconds", Pwhite(lo=2., hi=5., repeats=1)
+        # ),
         Pbind(
-            # This event inserts the most similar continuation from the Trainset "Cough"
-            "type", mmk.NearestNextNeighbor,
-            "soundbank", soundbank,
-            "feature", mmk.Spectrogram(n_fft=2048, hop_length=512, coordinate="mag"),
-            "seconds", Pwhite(lo=2., hi=5., repeats=1)
-        ),
-        Pbind(
-            "type", mmk.Checkpoint,
-            "id", srnn_cough,
-            "epoch", Prand([200, 300], inf),
+            "generator", checkpoints[1],
             # SampleRNN Checkpoints work best with a temperature parameter :
             "temperature", Pwhite(lo=.25, hi=1.5),
-            "seconds", Pwhite(lo=.5, hi=2.5, repeats=1),
+            "seconds", Pwhite(lo=.1, hi=1., repeats=1),
         )
     ], inf).asStream()
+    stream
 
     """### Generate"""
 
-    TOTAL_SECONDS = 30.
+    TOTAL_SECONDS = 10.
 
-    ensemble = mmk.Ensemble(
-        TOTAL_SECONDS, BASE_SR, stream,
+    ensemble = mmk.EnsembleGenerator(
+        prompts, TOTAL_SECONDS, OUTPUT_SR, stream,
         # with this you can print the event -- or not
         print_events=False
     )
+    outputs = ensemble.run()
+    logger = mmk.AudioLogger(sr=OUTPUT_SR)
+    logger.display_batch(outputs)
 
-    def process_outputs(outputs, bidx):
-        for output in outputs[0]:
-            mmk.audio(output.cpu().numpy(), sr=BASE_SR)
-
-    loop = mmk.GenerateLoop(
-        network=ensemble,
-        dataloader=prompts,
-        inputs=(h5m.Input(None,
-                          getter=h5m.AsSlice(dim=1, shift=-BASE_SR, length=BASE_SR),
-                          setter=h5m.Setter(dim=1)),),
-        n_steps=int(BASE_SR * ensemble.max_seconds),
-        add_blank=True,
-        process_outputs=process_outputs
-    )
-    loop.run()
+
+    """----------------------------"""
```

### Comparing `mimikit-0.3.4/mimikit/demos/freqnet.py` & `mimikit-0.4.0/mimikit/loops/eval_checkpoint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,98 +1,70 @@
-def demo():
-    """### Load Data"""
-    import mimikit as mmk
-    import h5mapper as h5m
-    import os
-
-
-    # list of files or directories to use as data ("./" is the cwd of the notebook)
-    sources = ['./data']
-    # audio sample rate
-    sr = 22050
-    # the size of the stft
-    n_fft = 2048
-    # hop_length of the stft
-    hop_length = n_fft // 4
-
-    db_path = "train.h5"
-    if os.path.exists(db_path):
-        os.remove(db_path)
-
-    class SoundBank(h5m.TypedFile):
-        snd = h5m.Sound(sr=sr, mono=True, normalize=True)
-
-    SoundBank.create(db_path, sources)
-    soundbank = SoundBank(db_path, mode='r', keep_open=True)
-
-    """### Configure and run training"""
-
-    # INPUT / TARGET
-
-    feature = mmk.Spectrogram(
-        sr=SoundBank.snd.sr,
-        n_fft=n_fft,
-        hop_length=hop_length,
-        coordinate='mag',
-        center=False
+import h5mapper as h5m
+import torch
+import numpy as np
+
+from . import IndicesSampler, GenerateLoop
+from ..checkpoint import Checkpoint
+from ..extract import nearest_neighbor, cum_entropy
+
+__all__ = [
+    "eval_checkpoint"
+]
+
+
+def eval_checkpoint(ckpt: Checkpoint, soundbank: h5m.TypedFile):
+    net = ckpt.network
+    feature = ckpt.feature
+    saved = {}
+
+    def process_outputs(outputs, bidx):
+        outputs = outputs[0]
+        y = feature.t(soundbank.snd[:])
+        y = torch.from_numpy(y).to(outputs)
+        nn = torch.stack([nearest_neighbor(out, y)[1] for out in outputs])
+        hx = torch.stack([cum_entropy(n, neg_diff=False) for n in nn]).detach().cpu().numpy()
+        idx = np.argsort(hx)
+        for i in idx:
+            saved[hx[i]] = outputs[i].detach().cpu().numpy().T
+        del y
+        del nn
+        torch.cuda.empty_cache()
+
+    prompt_files = soundbank
+    batch_item = feature.batch_item(shift=0, length=net.rf, training=False)
+    indices = IndicesSampler(
+        N=500,
+        indices=torch.arange(
+            0,
+            prompt_files.snd.shape[0] - batch_item.getter.length,
+            (prompt_files.snd.shape[0] - batch_item.getter.length) // 500))
+    dl = prompt_files.serve(
+        (batch_item,),
+        sampler=indices,
+        shuffle=False,
+        batch_size=64,
     )
 
-    # NETWORK
-
-    net = mmk.WaveNetFFT(
-        feature=feature,
-        input_heads=1,
-        output_heads=1,
-        scaled_activation=False,
-
-        # number of layers (per block)
-        blocks=(4,),
-        # dimension of the layers
-        dims_dilated=(1024,),
-        groups=2,
-        pad_side=0,
-
-    )
-    net.use_fast_generate = False
-
-    # OPTIMIZATION LOOP
-
-    mmk.train(
-        soundbank,
-        net,
-        root_dir="./",
-        input_feature=feature,
-        target_feature=feature,
-
-        # BATCH
-
-        batch_size=4,
-        batch_length=64,
-        downsampling=feature.hop_length // 1,
-        shift_error=0,
-
-        # OPTIM
-
-        max_epochs=100,
-        limit_train_batches=None,
-
-        max_lr=1e-3,
-        betas=(0.9, 0.9),
-        div_factor=3.,
-        final_div_factor=1.,
-        pct_start=0.,
-        cycle_momentum=False,
-        reset_optim=False,
-
-        # MONITORING / OUTPUTS
-
-        CHECKPOINT_TRAINING=True,
-        MONITOR_TRAINING=True,
-        OUTPUT_TRAINING="",
-
-        every_n_epochs=10,
-        n_examples=4,
-        prompt_length=64,
-        n_steps=int(12 * (feature.sr // feature.hop_length)),
+    loop = GenerateLoop(
+        network=net,
+        dataloader=dl,
+        inputs=(h5m.Input(None,
+                          getter=h5m.AsSlice(dim=1, shift=-net.rf, length=net.rf),
+                          setter=h5m.Setter(dim=1)),),
+        n_steps=feature.sr * 25 // feature.hop_length,
+        add_blank=True,
+        time_hop=net.hp.get("hop", 1),
+        process_outputs=process_outputs
     )
-
-    """----------------------------"""
+    print("\n")
+    print("\n")
+    print("-----------------------------------------")
+    print("\n")
+    print("\n")
+    loop.run()
+    print("\n")
+    print("\n")
+    print(ckpt)
+
+    for k in list(sorted(saved))[-8:]:
+        print("SCORE = ", k)
+        audio(saved[k], hop_length=feature.hop_length, sr=feature.sr)
```

### Comparing `mimikit-0.3.4/mimikit/demos/s2s.py` & `mimikit-0.4.0/mimikit/demos/seq2seq.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,93 @@
 def demo():
     """### Load Data"""
     import mimikit as mmk
     import h5mapper as h5m
     import os
 
+    # DATA
 
     # list of files or directories to use as data ("./" is the cwd of the notebook)
-    sources = ['./data']
-    # audio sample rate
-    sr = 44100
-    # the size of the stft
-    n_fft = 2048
-    # hop_length of the stft
-    hop_length = n_fft // 4
+    sources = tuple(h5m.FileWalker(mmk.SOUND_FILE_REGEX, "./"))
+    SAMPLE_RATE = 22050
 
-    db_path = "train.h5"
+    db_path = "train-seq2seq.h5"
     if os.path.exists(db_path):
         os.remove(db_path)
 
-    class SoundBank(h5m.TypedFile):
-        snd = h5m.Sound(sr=sr, mono=True, normalize=True)
+    signal = mmk.Extractor(
+        "signal",
+        mmk.Compose(mmk.FileToSignal(SAMPLE_RATE), mmk.RemoveDC(), mmk.Normalize()))
+    ds = mmk.DatasetConfig(sources=sources,
+                           filename=db_path,
+                           extractors=(signal,))
+    ds.create(mode="w")
+    dataset = ds.get(mode="r", keep_open=True)
+
+    N = dataset.signal.shape[0]
+    print(f"Dataset length in minutes is: {(N / SAMPLE_RATE) / 60:.2f}")
+    print("Extracted following files:")
+    for f in dataset.index:
+        print("\t", f)
 
-    SoundBank.create(db_path, sources)
-    soundbank = SoundBank(db_path, mode='r', keep_open=True)
-
-    """### Configure and run training"""
+    """### Configure Network"""
 
     # INPUT / TARGET
-
-    feature = mmk.Spectrogram(
-        sr=sr,
-        n_fft=n_fft,
-        hop_length=hop_length,
-        coordinate='mag',
-        center=False
+    io = mmk.IOSpec.magspec_io(
+        mmk.IOSpec.MagSpecIOConfig(
+            sr=SAMPLE_RATE,
+            n_fft=2048,
+            hop_length=512,
+            activation="Identity"
+        ),
+        signal
     )
 
-    net = mmk.Seq2SeqLSTM(
-        feature=feature,
-        input_heads=1,
-        output_heads=1,
-        scaled_activation=True,
-        model_dim=512,
-        num_layers=1,
-        n_lstm=1,
-        bottleneck="add",
-        n_fc=1,
-        hop=4,
-        weight_norm=False,
-        with_tbptt=False,
-        with_sampler=True,
-    )
+    # NETWORK
 
-    mmk.train(
-        soundbank,
+    net = mmk.Seq2SeqLSTMNetwork.from_config(
+        mmk.Seq2SeqLSTMNetwork.Config(
+            io_spec=io,
+            model_dim=512,
+            hop=4,
+            enc_downsampling="edge_sum",
+            enc_n_lstm=2,
+            enc_apply_residuals=True,
+            enc_weight_norm=False,
+            dec_upsampling="repeat",
+            dec_n_lstm=2,
+            dec_apply_residuals=True,
+            dec_weight_norm=False,
+        ))
+
+    """### Configure Training"""
+
+    # OPTIMIZATION LOOP
+    loop = mmk.TrainARMLoop.from_config(
+        mmk.TrainARMConfig(max_lr=1e-3,
+                           betas=(0.9, 0.9),
+                           div_factor=1.,
+                           final_div_factor=1.,
+                           pct_start=0.0,
+                           n_examples=4,
+                           prompt_length_sec=3.,
+                           batch_size=16,
+                           tbptt_chunk_length=None,
+                           batch_length=net.config.hop,  # <-- !important
+                           downsampling=net.config.io_spec.hop_length//2,
+                           limit_train_batches=10000,
+                           max_epochs=300,
+                           every_n_epochs=10,
+                           outputs_duration_sec=60,
+                           MONITOR_TRAINING=True,
+                           OUTPUT_TRAINING=False,
+                           CHECKPOINT_TRAINING=True),
+        dataset,
         net,
-        root_dir="./",
-        input_feature=feature,
-        target_feature=feature,
-
-        # BATCH
-
-        batch_size=16,
-        batch_length=net.hp.hop,
-        downsampling=feature.hop_length // 8,
-        shift_error=0,
-
-        # OPTIM
-
-        max_epochs=100,
-        limit_train_batches=None,
-
-        max_lr=1e-3,
-        betas=(0.9, 0.9),
-        div_factor=3.,
-        final_div_factor=1.,
-        pct_start=0.,
-        cycle_momentum=False,
-        reset_optim=False,
-
-        # MONITORING / OUTPUTS
-
-        CHECKPOINT_TRAINING=True,
-        MONITOR_TRAINING=True,
-        OUTPUT_TRAINING="",
-
-        every_n_epochs=10,
-        n_examples=4,
-        prompt_length=net.hp.hop,
-        n_steps=int(16 * (feature.sr // feature.hop_length // net.hp.hop)),
     )
 
+    """### RUN"""
+
+    loop.run()
+    None
+
     """----------------------------"""
```

### Comparing `mimikit-0.3.4/mimikit/extract/clusters.py` & `mimikit-0.4.0/mimikit/extract/clusters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,119 @@
+from functools import partial
+import dataclasses as dtc
+from typing import Optional, Tuple
+
 import numpy as np
 from scipy.sparse.csgraph import connected_components
+from scipy.sparse import csc_matrix
 from sklearn.metrics import pairwise_distances as pwd
 from sklearn.neighbors import KNeighborsTransformer, NearestNeighbors
 import sklearn.cluster as C
 import torch
 import torch.nn as nn
-from joblib import Parallel, delayed
-import click
-import os
-import soundfile as sf
-import shutil
-from functools import partial
 
-from ..modules import angular_distance
+from ..modules.loss_functions import AngularDistance
+from ..features.functionals import Functional, Identity
 
 
-class QCluster:
-
-    def __init__(self, qe=.5, n_neighbs=None, k=None, metric="euclidean"):
-        self.qe = qe
-        self.n_neighbs = n_neighbs
-        self.k = k
-        self.metric = metric
+__all__ = [
+    "QCluster",
+    "GCluster",
+    "HCluster",
+    "ArgMax",
+    "KMeans",
+    "SpectralClustering"
+]
+
+
+@dtc.dataclass
+class QCluster(Functional):
+
+    cores_prop: float = .5
+    n_neighbors: int = 8
+    core_neighborhood_size: int = 8
+    metric: str = "euclidean"
+
+    def __post_init__(self):
+        self.qe = 1 - self.cores_prop
+        self.n_neighbs = self.n_neighbors
+        self.k = self.core_neighborhood_size
         self.is_core_ = None
         self.labels_ = None
         self.K_ = None
 
     def fit(self, x):
         N = x.shape[0]
         if self.n_neighbs is None:
             self.n_neighbs = int(np.sqrt(N))
         if self.k is None:
             self.k = int(self.qe * self.n_neighbs)
 
-        D = pwd(x, x, metric=self.metric)
-        Dk = D.copy()
-        Dk[Dk == 0] = np.inf
-
-        kn = KNeighborsTransformer(mode="distance", n_neighbors=self.n_neighbs,
-                                   metric="precomputed")
-        adj = kn.fit_transform(D)
-        adj_sub = kn.kneighbors_graph(None, self.k, mode="distance")
-        Kx = (0 < adj.A).sum(axis=0).reshape(-1)
-        is_core = Kx >= np.quantile(Kx, self.qe)
-
-        adj_cores = (adj_sub.A.astype(np.bool)) & (is_core & is_core[:, None])
+        n_neighbs = self.n_neighbs
+        kn = KNeighborsTransformer(mode="distance", n_neighbors=n_neighbs,
+                                   metric=self.metric)
+        adj_o = kn.fit_transform(x)
+        adj = adj_o.tolil()
+        rg = np.arange(adj.shape[0])
+        adj[rg, rg] = 0.
+        in_degree = (0 < adj.tocsc()).sum(axis=0).A.reshape(-1)
+        is_core = in_degree >= np.quantile(in_degree, self.qe)
         cores_idx = is_core.nonzero()[0]
-        print(f"found {cores_idx.shape[0]} cores")
-        for i in range(adj.shape[0]):
-            if not np.any(adj_cores[i] & is_core):
-                nearest_core = Dk[i, is_core].argmin()
-                nearest_core = cores_idx[nearest_core]
-                adj_cores[i, nearest_core] = True
+        k = self.k
+        # print(f"found {cores_idx.shape[0]} cores ({cores_idx.shape[0] / N:.3f})-- will do {k} connections")
+        adj_sub_o = kn.kneighbors_graph(x[is_core], n_neighbors=k + 1, mode='distance')
+        asub = adj_sub_o.tocoo()
+        adj_c = csc_matrix((np.r_[[x in cores_idx for x in asub.col]],
+                            (cores_idx[asub.row], asub.col)),
+                           shape=adj.shape)
+        adj_c = (adj_c > 0).tolil()
+
+        disconnected = (adj_c.tocsc()[:, cores_idx].tocsr().sum(axis=1).A.reshape(-1) == 0)
+
+        cores_est = KNeighborsTransformer(mode="distance", n_neighbors=2,
+                                          metric=self.metric).fit(x[is_core])
+
+        nearest_cores = cores_est.kneighbors(x[disconnected], return_distance=False)
+        nearest_cores = cores_idx[nearest_cores]
+        dis_idx = rg[disconnected]
+        # print("n disconnected = ", len(dis_idx))
+        for i, cores in zip(dis_idx, nearest_cores):
+            # nearest core can equal i!
+            nearest_core = next(n for n in cores if n != i)
+            adj_c[i, nearest_core] = True
 
-        K, labels = connected_components(adj_cores)
+        K, labels = connected_components(adj_c)
         self.K_, self.labels_, self.is_core_ = K, labels, is_core
         return self
 
+    def np_func(self, inputs):
+        self.fit(inputs)
+        return self.labels_
+
+    def torch_func(self, inputs):
+        pass
+
+    @property
+    def inv(self) -> "Functional":
+        # todo: here we could implement some kind of inverse_transform()?
+        return Identity()
+
+
+@dtc.dataclass
+class GCluster(Functional):
+    n_means: int = 16
+    n_iter: int = 128
+    lr: float = 0.025
+    betas: Tuple[float, float] = (0.05, 0.05)
+    metric: str = "cosine"
+    eps: float = 1e-6
 
-class GCluster:
-    def __init__(self,
-                 n_means,
-                 n_iter=128,
-                 lr=0.025,
-                 betas=(0.05, 0.05),
-                 metric="cosine",
-                 eps=1e-6):
-        self.n_means = n_means
-        self.n_iter = n_iter
-        self.lr = lr
-        self.betas = betas
-        self.metric = metric
+    def __post_init__(self):
         self.d_func = dict(euclidean=torch.cdist,
-                           cosine=partial(angular_distance, eps=eps))[metric]
+                           cosine=AngularDistance(eps=self.eps))[self.metric]
         self.K_ = None
         self.labels_ = None
         self.losses_ = None
 
     def fit(self, x):
         X = torch.from_numpy(x)
         H = nn.Parameter(X[torch.randint(0, X.shape[0], (self.n_means,))].clone())
@@ -89,41 +126,55 @@
             L.backward()
             opt.step()
             losses += [L.item()]
         x = X.detach().cpu().numpy()
         h = H.detach().cpu().numpy()
         DXH = pwd(h, x, self.metric)
         hi, xi = np.unravel_index(DXH.argsort(None), DXH.shape)
-        labels = np.zeros(x.shape[0], dtype=np.int)
+        labels = np.zeros(x.shape[0], dtype=int)
         got = set()
         for label, i in zip(hi.flat[:], xi.flat[:]):
             if i not in got:
                 labels[i] = label
                 got.add(i)
         self.losses_ = losses
         self.K_ = self.n_means
         self.labels_ = labels
         return self
 
+    def np_func(self, inputs):
+        self.fit(inputs)
+        return self.labels_
+
+    def torch_func(self, inputs):
+        pass
 
-class HCluster:
-    def __init__(self, max_iter=32, metric="cosine"):
-        self.max_iter = max_iter
-        self.metric = metric
+    @property
+    def inv(self) -> "Functional":
+        # todo: here we could implement some kind of inverse_transform()?
+        return Identity()
+
+
+@dtc.dataclass
+class HCluster(Functional):
+    max_iter: int = 32
+    metric: str = "cosine"
+
+    def __post_init__(self):
         self.K_ = None
         self.labels_ = None
 
     def fit(self, x):
         Da = pwd(x, x, self.metric)
         xa = x.copy()
         Da[Da == 0] = np.inf
-        LBS = np.zeros((x.shape[0], self.max_iter), dtype=np.int)
+        LBS = np.zeros((x.shape[0], self.max_iter), dtype=int)
 
         for i in range(self.max_iter):
-            Adj_nearest = np.zeros_like(Da, dtype=np.bool)
+            Adj_nearest = np.zeros_like(Da, dtype=bool)
             nearest = Da.argmin(axis=1)
             Adj_nearest[np.arange(Da.shape[0]), nearest] = True
 
             K, labels = connected_components(Adj_nearest)
             if i == 0:
                 LBS[:, 0] = labels
             else:
@@ -136,150 +187,168 @@
                 LBS = LBS[:, :i + 1]
                 self.K_ = i + 1
                 break
 
         self.labels_ = LBS
         return self
 
+    def np_func(self, inputs):
+        self.fit(inputs)
+        return self.labels_
 
-def distance_matrices(X, metric="euclidean", n_neighbors=1, radius=1e-3):
-    Dx = pwd(X, X, metric=metric)
-    NN = NearestNeighbors(n_neighbors=n_neighbors, radius=radius, metric="precomputed")
-    NN.fit(Dx)
-    Kx = NN.kneighbors_graph(n_neighbors=n_neighbors, mode='connectivity')
-    Rx = NN.radius_neighbors_graph(radius=radius, mode='connectivity')
-    return Dx, Kx, Rx
+    def torch_func(self, inputs):
+        pass
 
+    @property
+    def inv(self) -> "Functional":
+        # todo: here we could implement some kind of inverse_transform()?
+        return Identity()
 
-class ArgMax(object):
-    def __init__(self):
+
+@dtc.dataclass
+class ArgMax(Functional):
+
+    def __post_init__(self):
         self.labels_ = None
         self.K_ = None
 
     def fit(self, X):
         maxes = np.argmax(X, axis=1)
         uniques, self.labels_ = np.unique(maxes, return_inverse=True)
         self.K_ = len(uniques)
         return self
 
+    def np_func(self, inputs):
+        self.fit(inputs)
+        return self.labels_
+
+    def torch_func(self, inputs):
+        pass
+
+    @property
+    def inv(self) -> "Functional":
+        # todo: here we could implement some kind of inverse_transform()?
+        return Identity()
+
+
+@dtc.dataclass
+class KMeans(Functional):
+    n_clusters: int = 16
+    n_init: int = 2
+    max_iter: int = 100
+    random_seed: int = 42
+
+    def __post_init__(self):
+        self.est = C.KMeans(
+            n_clusters=self.n_clusters,
+            n_init=self.n_init,
+            max_iter=self.max_iter,
+            random_state=self.random_seed,
+            copy_x=False
+        )
+
+    def fit(self, X):
+        self.est.fit(np.ascontiguousarray(X))
+        return self
+
+    def np_func(self, inputs):
+        self.fit(inputs)
+        return self.est.labels_
+
+    def torch_func(self, inputs):
+        pass
+
+    @property
+    def inv(self) -> "Functional":
+        # todo: here we could implement some kind of inverse_transform()?
+        return Identity()
+
+
+@dtc.dataclass
+class SpectralClustering(Functional):
+    n_clusters: int = 8
+    n_init: int = 10
+    n_neighbors: int = 10
+    random_seed: int = 42
+
+    def __post_init__(self):
+        self.est = C.SpectralClustering(
+            n_clusters=self.n_clusters,
+            n_init=self.n_init,
+            n_neighbors=self.n_neighbors,
+            random_state=self.random_seed,
+            affinity="nearest_neighbors",
+            eigen_solver="amg",
+            assign_labels="discretize",
+        )
+
+    def fit(self, X):
+        self.est.fit(X)
+        return self
+
+    def np_func(self, inputs):
+        self.fit(inputs)
+        return self.est.labels_
+
+    def torch_func(self, inputs):
+        pass
+
+    @property
+    def inv(self) -> "Functional":
+        # todo: here we could implement some kind of inverse_transform()?
+        return Identity()
+
+
+def distance_matrices(X, metric="euclidean", n_neighbors=1, radius=1e-3):
+    Dx = pwd(X, X, metric=metric)
+    NN = NearestNeighbors(n_neighbors=n_neighbors, radius=radius, metric="precomputed")
+    NN.fit(Dx)
+    Kx = NN.kneighbors_graph(n_neighbors=n_neighbors, mode='connectivity')
+    Rx = NN.radius_neighbors_graph(radius=radius, mode='connectivity')
+    return Dx, Kx, Rx
+
+
+def cluster(X, estimator="argmax", **parameters):
 
-def sk_cluster(X, Dx=None, n_clusters=128, metric="euclidean", estimator="argmax"):
     estimators = {
 
-        "argmax": ArgMax(),
+        "argmax": partial(ArgMax),
 
-        "kmeans": C.KMeans(n_clusters=n_clusters,
-                           n_init=4,
-                           max_iter=200,
-                           ),
-
-        "spectral": C.SpectralClustering(n_clusters=n_clusters,
-                                         affinity="nearest_neighbors",
-                                         n_neighbors=32,
-                                         assign_labels="discretize",
-                                         ),
-
-        "agglo_ward": C.AgglomerativeClustering(
-            n_clusters=n_clusters,
-            affinity="euclidean",
-            compute_full_tree='auto',
-            linkage='ward',
-            distance_threshold=None, ),
-
-        "agglo_single": C.AgglomerativeClustering(
-            n_clusters=n_clusters,
-            affinity="precomputed",
-            compute_full_tree='auto',
-            linkage='single',
-            distance_threshold=None, ),
-
-        "agglo_complete": C.AgglomerativeClustering(
-            n_clusters=n_clusters,
-            affinity="precomputed",
-            compute_full_tree='auto',
-            linkage='complete',
-            distance_threshold=None, )
+        "kmeans": partial(C.KMeans),
 
-    }
+        "qcores": partial(QCluster),
+
+        "spectral": partial(C.SpectralClustering,
+                            affinity="nearest_neighbors",
+                            eigen_solver="amg",
+                            assign_labels="discretize",
+                            ),
+
+        "agglo_ward": partial(C.AgglomerativeClustering,
+                              affinity="euclidean",
+                              compute_full_tree='auto',
+                              linkage='ward',
+                              distance_threshold=None, ),
+
+        "agglo_single": partial(C.AgglomerativeClustering,
+                                affinity="precomputed",
+                                compute_full_tree='auto',
+                                linkage='single',
+                                distance_threshold=None, ),
+
+        "agglo_complete": partial(C.AgglomerativeClustering,
+                                  affinity="precomputed",
+                                  compute_full_tree='auto',
+                                  linkage='complete',
+                                  distance_threshold=None, )
 
-    needs_distances = estimator in {"agglo_single", "agglo_complete"}
+    }
 
-    if needs_distances:
-        if Dx is None:
-            Dx, _, _ = distance_matrices(X, metric=metric)
-        X_ = Dx
+    if estimator in {"agglo_single", "agglo_complete"}:
+        X_, _, _ = distance_matrices(X, metric=parameters.get("metric", "euclidean"))
     else:
         X_ = X
 
-    cls = estimators[estimator]
+    cls = estimators[estimator](**parameters)
     cls.fit(X_)
 
     return cls
-
-
-def etl(input_file, sr, n_fft, hop_length):
-    """STFT Extract-Transform-Load"""
-    from mimikit import FileToSignal, MagSpec
-
-    y = FileToSignal(sr)(input_file)
-    S = MagSpec(n_fft, hop_length)(y)
-    return y, S
-
-
-def export(S, target_path, sr, n_fft, hop_length):
-    from mimikit import GLA
-    gla = GLA(n_fft, hop_length)
-    if S.shape[0] <= 1:
-        print("!!!!!", target_path)
-        return
-    # if S is too long, joblib sends it as np.memmap
-    # which messes with gla()...
-    y = gla(np.asarray(S))
-    sf.write(f"{target_path}.wav", y, sr, 'PCM_24')
-    return
-
-
-@click.command()
-@click.option("-f", "--input-file", help="file to be segmented")
-@click.option("--sr", "-r", default=22050, help="the sample rate used for loading the file (default=22050)")
-@click.option("--n-fft", "-d", default=2048, help="size of the fft (default=2048)")
-@click.option("--hop-length", "-h", default=512, help="hop length of the stft (default=512)")
-@click.option("--n-neighbs", "-n", default=None, type=int,
-              help="size of the neighborhood used to estimate point-density")
-@click.option("--qe", "-q", default=0.5, type=float,
-              help="proportion of edge-points")
-@click.option("--k", "-k", default=1, type=int,
-              help="proportion of connecting core points")
-def cluster(input_file: str,
-            sr: int = 22050,
-            n_fft: int = 2048,
-            hop_length: int = 512,
-            n_neighbs: int = None,
-            qe: float = 0.5,
-            k: int = 1
-            ):
-    y, S = etl(input_file, sr, n_fft, hop_length)
-    est = QCluster(qe=qe, n_neighbs=n_neighbs, k=k, metric="euclidean")
-    est.fit(S)
-
-    clusters = [S[est.labels_ == i] for i in range(est.K_)]
-    items, counts = np.unique(est.labels_, return_counts=True)
-    srtd = (-counts).argsort()
-    items, counts = items[srtd[:10]], counts[srtd[:10]]
-    distrib_str = "\n    ".join([f"{d}  :  {c}"
-                                 for d, c in zip(items, counts)]) + \
-                  "\n    [  ...  ]\n"
-    print(f"""
-Data shape : {S.shape}
-Parameters : n_neighbs={est.n_neighbs} ; k={est.k} ; qe={qe}
-========>   found {est.K_} clusters
-    """ + distrib_str
-          )
-
-    target_dir = os.path.splitext(input_file)[0]
-    if os.path.exists(target_dir):
-        shutil.rmtree(target_dir)
-    os.makedirs(target_dir, exist_ok=True)
-    Parallel(backend='multiprocessing') \
-        (delayed(export)(s, f"{target_dir}/c{i}", sr, n_fft, hop_length)
-         for i, s in enumerate(clusters))
-    return
```

### Comparing `mimikit-0.3.4/mimikit/extract/from_neighbors.py` & `mimikit-0.4.0/mimikit/extract/from_neighbors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import torch
 import numpy as np
 
-from ..modules import angular_distance
+from ..modules import AngularDistance
 
 
 def nearest_neighbor(X, Y):
     """
     computes nearest neighbor by angular distance
     """
-    D_xy = angular_distance(X, Y)
+    D_xy = AngularDistance()(X, Y)
     dists, nn = torch.min(D_xy, dim=-1)
     return dists, nn
 
 
 def torch_frame(x, frame_size, hop_length):
     """
     helper to reshape an array into frames
```

### Comparing `mimikit-0.3.4/mimikit/loops/samplers.py` & `mimikit-0.4.0/mimikit/loops/samplers.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  oversampling=1,
                  ):
         super().__init__(None)
         self.n_samples = n_samples
         self.chunk_length = min(chunk_length, n_samples)
         self.seq_len = seq_len
         self.n_chunks = max(1, self.n_samples // self.chunk_length - int(oversampling > 1))
-        self.remainder = self.n_samples % self.chunk_length
+        self.remainder = max(self.n_samples % self.chunk_length, 1)
         self.n_per_chunk = self.chunk_length // self.seq_len
         self.batch_size = batch_size
         self.oversampling = oversampling
 
     def __iter__(self):
         indices = torch.arange(self.n_chunks * self.oversampling)
         smp = RandomSampler(indices)
@@ -66,22 +66,12 @@
     def __iter__(self):
         for i in self.indices:
             yield i
         if self.redraw:
             self.indices = self.draw_indices(self.N, self._indices)
 
     def draw_indices(self, N, indices):
-        n_idx = len(indices)
-        if N == 0 and n_idx == 0:
-            raise ValueError("`indices` can not be empty if `N` == 0")
-        elif N > 0 and n_idx == 0:
-            # only random
-            return torch.randint(self.min_i, self.max_i, (N,))
-        elif N == 0 and n_idx > 0:
-            # only static
-            return indices
-        elif N > 0 and 0 < n_idx < N:
-            # complete statics with randoms
-            return [*indices, *torch.randint(self.min_i, self.max_i, (N,))]
+        if isinstance(indices, tuple):
+            return tuple(torch.randint(self.min_i, self.max_i, (1,)).item() if i is None else i
+                         for i in indices)
         else:
-            # N <= n_idx -> only statics
-            return indices
+            return torch.randint(self.min_i, self.max_i, (N,))
```

### Comparing `mimikit-0.3.4/mimikit/models/ensemble.py` & `mimikit-0.4.0/mimikit/models/ensemble_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,161 @@
-import h5mapper as h5m
+from typing import Optional, Union, Generator
+
 import torch.nn as nn
 import torch
-import math
 from pprint import pprint
+import dataclasses as dtc
 
-from ..networks import TierNetwork
-from ..features import Resample, MuLawSignal
-from ..loops import GenerateLoop
-
+from ..utils import default_device
+from ..networks import ARM
+from ..features.functionals import Resample
+from ..loops import GenerateLoopV2
+from ..checkpoint import Checkpoint
 from .nnn import NearestNextNeighbor
-from .checkpoint import Checkpoint
 
 __all__ = [
-    "Ensemble"
+    "EnsembleGenerator"
 ]
 
 
-class Ensemble(nn.Module):
+class VotingEnsemble(nn.Module):
+    device = property(lambda self: next(self.parameters()).device)
+
+    def __init__(self, networks, weights=None):
+        super(VotingEnsemble, self).__init__()
+        self.nets = nn.ModuleList(networks)
+        N = len(networks)
+        W = [1 / N for _ in range(N)] if weights is None else weights
+        if len(W) != N:
+            raise ValueError(f"Expected `weights` to be of length {N} but got {len(W)}")
+        self.weights = torch.tensor(W) / sum(W)
+
+    def before_generate(self, loop, batch, batch_idx):
+        for net in self.nets:
+            net.before_generate(loop, batch, batch_idx)
+        return {}
+
+    def generate_step(self, t, inputs, ctx):
+        self.weights.to(inputs.device)
+        out = None
+        for w, net in zip(self.nets, self.weights):
+            if out is None:
+                out = net.generate_step(t, inputs, ctx) * w
+            else:
+                out += net.generate_step(t, inputs, ctx) * w
+        return out
+
+    def after_generate(self, *args, **kwargs):
+        for net in self.nets:
+            net.after_generate(*args, **kwargs)
+        return self
+
+
+@dtc.dataclass
+class Event:
+    generator: Union[ARM, Checkpoint, NearestNextNeighbor]
+    seconds: float
+    temperature: Optional[float] = None
+
+
+class EnsembleGenerator:
     """
     generate form a prompt by chaining checkpoints/models
     """
-    device = property(lambda self: next(self.parameters()).device)
 
     def __init__(self,
-                 max_seconds,
-                 base_sr,
-                 stream,  # a pbind stream of events
-                 print_events=False
+                 prompt: torch.Tensor,
+                 max_seconds: float = 10.,
+                 base_sr: int = 22050,
+                 stream: Generator = (),
+                 print_events: bool = False,
+                 device=default_device()
                  ):
-        super(Ensemble, self).__init__()
+        super(EnsembleGenerator, self).__init__()
+        self.prompt = prompt.to(device)
         self.max_seconds = max_seconds
         self.base_sr = base_sr
         self.stream = stream
         self.print_events = print_events
-        # just to make self.device settable/gettable
-        self._param = nn.Parameter(torch.ones(1))
+        self.device = device
 
-    def run_event(self, inputs, net, feature, n_steps, *params):
-        prompt_getter = feature.batch_item(
-            shift=0, length=inputs.size(-1) if isinstance(net, TierNetwork) else net.rf  # TODO: NNN needs 1 instead of net.rf...
-        )
-        resample = Resample(self.base_sr, feature.sr)
-        n_input_samples = math.ceil(prompt_getter.getter.length * self.base_sr / feature.sr)
-        prompt_getter.data = resample(inputs[:, -n_input_samples:])
-        prompt = prompt_getter(0)
-        output = [[]]
-        print("length", prompt_getter.getter.length, "n_inputs", n_input_samples, "PROMPT", prompt.shape)
-        def process_outputs(outputs, _):
-            print("OUTPUT", outputs[0].shape)
-            inv_resample = Resample(feature.sr, self.base_sr)
-            # prompt + generated in base_sr :
-            y = feature.inverse_transform(outputs[0])
-            print("Y", y.shape, feature.sr, self.base_sr)
-            out = inv_resample(y)
-            output[0] = out[:, n_input_samples:]
-            print("OUTPUT", out.shape)
-
-        loop = GenerateLoop(
-            net,
-            dataloader=[(prompt,)],
-            inputs=(h5m.Input(None,
-                              getter=h5m.AsSlice(dim=1, shift=-net.shift, length=net.shift),
-                              setter=h5m.Setter(dim=1)),
-                    *tuple(h5m.Input(p, h5m.AsSlice(dim=1 + int(hasattr(net.hp, 'hop')), length=1),
-                                     setter=None) for p in params)
-                    ),
-            n_steps=n_steps,
-            add_blank=True,
-            process_outputs=process_outputs,
-            time_hop=getattr(net, 'hop', 1)
-        )
-        loop.run()
-        return output[0]
-
-    @staticmethod
-    def seconds_to_n_steps(seconds, net, feature):
-        return int(seconds * feature.sr) if isinstance(feature, MuLawSignal) \
-            else int(seconds * (feature.sr // feature.hop_length)) // getattr(net, "hop", 1)
+    def run(self):
+        prompt_length = t = self.prompt.size(-1)
+        n_samples = int(self.max_seconds * self.base_sr)
+        output = torch.zeros(self.prompt.size(0), n_samples,
+                             dtype=self.prompt.dtype).to(self.device)
+        output[:, :t] = self.prompt
+        while t < n_samples:
+            prompt = output[:, t-prompt_length:t]
+            step_output = self.generate_step(t, prompt)
+            if step_output is None:
+                break
+            output[:, t:t+step_output.size(1)] = step_output
+            t += step_output.size(1)
+        return output
 
-    def generate_step(self, t, inputs, ctx):
+    def generate_step(self, t, inputs):
         if t >= int(self.max_seconds * self.base_sr):
             return None
-        event, net, feature, n_steps, params = self.next_event()
+        event, net, n_steps, params = self.next_event()
         if hasattr(net, 'to'):
-            net = net.to("cuda")
-        if hasattr(net, "use_fast_generate"):
-            net.use_fast_generate = False
+            net = net.to(self.device)
 
-        if (t / self.base_sr + event['seconds']) < self.max_seconds:
+        if (t / self.base_sr + event.seconds) < self.max_seconds:
             if self.print_events:
-                event.update({"start": t / self.base_sr})
-                pprint(event)
-            out = self.run_event(inputs[0], net, feature, n_steps, *params)
+                e = dtc.asdict(event)
+                e.update({"start": t / self.base_sr})
+                pprint(e)
+            out = self.run_event(inputs, net, n_steps, params)
             return out
-        return torch.zeros(1, int(self.max_seconds * self.base_sr - t)).to("cuda")
+        return torch.zeros(inputs.size(0), int(self.max_seconds * self.base_sr - t)).to(self.device)
+
+    def run_event(self,
+                  inputs: torch.Tensor,
+                  net: ARM,
+                  n_steps: int,
+                  params: dict
+                  ):
+        network_sr = net.config.io_spec.sr
+        resample = Resample(self.base_sr, network_sr)
+        inputs_resampled = resample(inputs)
+        prompt = tuple(in_spec.transform(inputs_resampled) for in_spec in net.config.io_spec.inputs)
+        n_input_samples = inputs.shape[1]
+
+        cfg = GenerateLoopV2.Config(
+            parameters=params,
+            display_waveform=False,
+            write_waveform=False,
+            yield_inversed_outputs=True
+        )
+        loop = GenerateLoopV2(
+            cfg,
+            network=net,
+            n_steps=n_steps,
+            # the loop needs the indices of the prompt before the prompt for logging...
+            dataloader=[[torch.ones(1), *prompt]],
+            logger=None,
+        )
+        for outputs in loop.run():
+            inv_resample = Resample(network_sr, self.base_sr)
+            # prompt + generated in base_sr :
+            out = inv_resample(outputs[0])
+            return out[:, n_input_samples:]
 
     def next_event(self):
-        event = next(self.stream)
-        if "Checkpoint" in str(event["type"]):
-            ck = Checkpoint(event['id'], event['epoch'], event.get("root_dir", "./"))
-            net, feature = ck.network, ck.feature
-        elif "NearestNextNeighbor" in str(event["type"]):
-            feature = event['feature']
-            data = event["soundbank"]
-            net = NearestNextNeighbor(feature, data.snd)
+        event = Event(**next(self.stream))
+        if isinstance(event.generator, Checkpoint):
+            ck = event.generator
+            net = ck.network
+        elif isinstance(event.generator, NearestNextNeighbor):
+            net = event.generator
+        # elif event["type"] == "Parallel":
+        #     pass
         else:
-            raise TypeError(f"event type '{event['type']}' not recognized")
-        n_steps = self.seconds_to_n_steps(event['seconds'], net, feature)
-        print("N_STEPS", n_steps)
-        if "temperature" in event:
-            temp = event['temperature']
-            if isinstance(temp, float):
-                params = (torch.tensor([[temp]]).to(self.device).repeat(1, n_steps),)
-            elif isinstance(temp, tuple):
-                params = (torch.linspace(temp[0], temp[1], n_steps, device=self.device),)
-            else:
-                params = tuple()
+            raise TypeError(f"event generator type '{type(event.generator)}' not supported")
+        cfg = GenerateLoopV2.Config(output_duration_sec=event.seconds)
+        n_steps = GenerateLoopV2.get_n_steps(cfg, net)
+        if event.temperature is not None:
+            params = dict(temperature=event.temperature)
         else:
-            params = tuple()
-        return event, net, feature, n_steps, params
+            params = {}
+        return event, net, n_steps, params
```

### Comparing `mimikit-0.3.4/mimikit/models/nnn.py` & `mimikit-0.4.0/mimikit/models/nnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,31 +15,35 @@
     return dtw(C=pairwise_distances(abs(x), abs(y), metric='cosine'), subseq=True)[1][::-1]
 
 
 class NearestNextNeighbor(nn.Module):
 
     device = property(lambda self: next(self.parameters()).device)
 
-    def __init__(self, feature, snd):
+    def __init__(self, feature, snd, path_length=16):
         super(NearestNextNeighbor, self).__init__()
         self.feature = feature
-        self.snd = feature.transform(snd[:])
+        self.snd = feature.t(snd[:])
         self._t = -100
         self._starts = None
         self._param = nn.Parameter(torch.ones(1))
-        self.shift = self.rf = feature.n_fft
+        # how much steps are used to find the optimal next step
+        self.shift = path_length
         self.output_length = lambda x: 1
 
     def predict_start_frame(self, X):
         path = optimal_path(X, self.snd)
         return path[-1, -1]+1
 
     def generate_step(self, t, inputs, ctx):
         """predict start frame if inputs is new else return next frame"""
         if t != self._t + 1:
+            # start frame index for each element in the inputs batch
             self._starts = [self.predict_start_frame(x.detach().cpu().numpy())
                             for x in inputs[0]]
             self._t = t - 1
+        # output batch at time t
         output = np.stack([self.snd[i:i+1] for i in self._starts])
+        # shift the starts
         self._starts = [x+1 for x in self._starts]
         self._t += 1
         return torch.from_numpy(output).to(inputs[0].device)
```

### Comparing `mimikit-0.3.4/mimikit/models/wave_gan.py` & `mimikit-0.4.0/mimikit/networks/wave_gan.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             ]
 
         self.deconv_list = nn.ModuleList(deconv_layers)
         self.ppfilter1 = nn.Conv1d(n_channels, n_channels, (post_proc_filt_len,)) if post_proc_filt_len else None
 
         for m in self.modules():
             if isinstance(m, nn.ConvTranspose1d) or isinstance(m, nn.Linear):
-                nn.init.kaiming_normal_(m.weight.data)
+                nn.init.kaiming_normal_(m.weight.dataset)
 
     def forward(self, x):
         x = self.fc1(x).view(-1, self.dim_mul * self.model_size, self.t0)
         if self.use_batch_norm:
             x = self.bn1(x)
         x = F.relu(x)
         if self.verbose:
@@ -259,15 +259,15 @@
 
         self.conv_layers = nn.ModuleList(conv_layers)
 
         self.fc1 = nn.Linear(self.fc_input_size, 1)
 
         for m in self.modules():
             if isinstance(m, nn.Conv1d) or isinstance(m, nn.Linear):
-                nn.init.kaiming_normal_(m.weight.data)
+                nn.init.kaiming_normal_(m.weight.dataset)
 
     def forward(self, x):
         for conv in self.conv_layers:
             x = conv(x)
             if self.verbose:
                 print(conv.__class__.__qualname__, x.shape)
         x = x.view(-1, self.fc_input_size)
```

### Comparing `mimikit-0.3.4/mimikit/modules/loss_functions.py` & `mimikit-0.4.0/mimikit/modules/loss_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,101 @@
 import torch
 import torch.nn as nn
 
 __all__ = [
-    'angular_distance',
-    'cosine_similarity',
-    'mean_L1_prop',
-    'mean_2d_diff'
+    'MeanL1Prop',
+    'Mean2dDiff',
+    "CosineSimilarity",
+    "AngularDistance",
 ]
 
 
-def mean_L1_prop(output, target, denom=1e-8):
-    if torch.any(torch.isnan(output)):
-        print("NAN OUTPUT")
-    L = nn.L1Loss(reduction="none")(output, target).sum(dim=(0, -1,), keepdim=True)
-    target_sums = target.abs().sum(dim=(0, -1,), keepdim=True)
-    # make the upcoming division safe
-    target_sums = target_sums + (target_sums < 1.).float() * torch.maximum(L.detach(),
-                                                                           torch.tensor(1e-16).to(L.device))
-    if torch.any(torch.isnan(target_sums)):
-        print("NAN TARGET")
-    L = (L / target_sums).mean()
-    return L
-
-
-def mean_2d_diff(output, target):
-    """compute the mean_L1_prop loss of the differences along the 2 last axes of `output` and `target`"""
-    Lw = mean_L1_prop((output[:, :, 1:] - output[:, :, :-1]), target[:, :, 1:] - target[:, :, :-1], )
-    Lh = mean_L1_prop((output[:, 1:] - output[:, :-1]), target[:, 1:] - target[:, :-1], )
-    return Lw + Lh
+class MeanL1Prop(nn.Module):
+    def __init__(self, raise_on_nan=True, eps=1e-8):
+        super(MeanL1Prop, self).__init__()
+        self.raise_on_nan = raise_on_nan
+        self.eps = eps
+        self.l1loss = nn.L1Loss(reduction="none")
+
+    def forward(self, output, target):
+        if self.raise_on_nan and torch.any(torch.isnan(output)):
+            raise RuntimeError("nan values in output")
+        L = self.l1loss(output, target).sum(dim=(0, -1,), keepdim=True)
+        target_sums = target.abs().sum(dim=(0, -1,), keepdim=True)
+        # make the upcoming division safe
+        prop = torch.maximum(L.detach(), torch.tensor(self.eps).to(L.device))
+        target_sums = target_sums + (target_sums < 1.).float() * prop
+        if self.raise_on_nan and torch.any(torch.isnan(target_sums)):
+            raise RuntimeError("nan values in target_sums")
+        L = (L / target_sums).mean()
+        return L
+
+
+class Mean2dDiff(nn.Module):
+    def __init__(self, raise_on_nan=True, eps=1e-8):
+        super(Mean2dDiff, self).__init__()
+        self.mean_l1_prop = MeanL1Prop(raise_on_nan, eps)
+
+    def forward(self, output, target):
+        """compute the mean_L1_prop loss of the differences along the 2 last axes of `output` and `target`"""
+        Lw = self.mean_l1_prop((output[:, :, 1:] - output[:, :, :-1]), target[:, :, 1:] - target[:, :, :-1], )
+        Lh = self.mean_l1_prop((output[:, 1:] - output[:, :-1]), target[:, 1:] - target[:, :-1], )
+        return Lw + Lh
 
 
-def cosine_similarity(X, Y, eps=1e-6):
+class CosineSimilarity(nn.Module):
     """
     safely computes the cosine similarity between matrices X and Y.
 
     Shapes:
     -------
     X : (*, N, D)
     Y : (*, M, D)
     D_xy : (*, N, M)
 
     Notes:
     ------
     The need for this function arises from the fact that torch.nn.CosineSimilarity only computes the
     diagonal of D_xy, as in cosine_sim(output, target)
     """
-    if not isinstance(eps, torch.Tensor):
-        eps = torch.tensor(eps).to(X)
+    def __init__(self, eps=1e-8):
+        super(CosineSimilarity, self).__init__()
+        if not isinstance(eps, torch.Tensor):
+            eps = torch.tensor(eps)
+        self.register_buffer("eps", eps)
+
+    def forward(self, X, Y):
+        dot_prod = torch.matmul(X, Y.transpose(-2, -1))
+        norms = torch.norm(X, p=2, dim=-1).unsqueeze(-1) * torch.norm(Y, p=2, dim=-1).unsqueeze(-2)
+        cos_theta = dot_prod.div_(torch.maximum(norms, self.eps.to(X.device)))
+        return cos_theta
+
+
+class AngularDistance(nn.Module):
+    def __init__(self, eps=1e-8):
+        super(AngularDistance, self).__init__()
+        if not isinstance(eps, torch.Tensor):
+            eps = torch.tensor(eps)
+        self.register_buffer("eps", eps)
+        self.cosine_sim = CosineSimilarity(eps=eps)
 
-    dot_prod = torch.matmul(X, Y.transpose(-2, -1))
-    norms = torch.norm(X, p=2, dim=-1).unsqueeze(-1) * torch.norm(Y, p=2, dim=-1).unsqueeze(-2)
-    cos_theta = dot_prod.div_(torch.maximum(norms, eps))
-    return cos_theta
-
-
-def angular_distance(X, Y, eps=1e-6):
-    """
-    angular distance is a valid distance metric based on the cosine similarity
-    see https://en.wikipedia.org/wiki/Cosine_similarity#Angular_distance_and_similarity
-
-    Shapes:
-    -------
-    X : (*, N, D)
-    Y : (*, M, D)
-    D_xy : (*, N, M)
-    """
-    if not isinstance(eps, torch.Tensor):
-        eps = torch.tensor(eps).to(X)
-
-    def safe_acos(x):
+    def safe_acos(self, x):
         # torch.acos returns nan near -1 and 1... see https://github.com/pytorch/pytorch/issues/8069
+        eps = self.eps.to(x.device)
         return torch.acos(torch.clamp(x, min=-1 + eps / 2, max=1 - eps / 2))
 
-    have_negatives = torch.any(X < 0) or torch.any(Y < 0)
-    cos_theta = cosine_similarity(X, Y, eps)
-
-    pi = torch.acos(torch.zeros(1)).item() * 2
-    D_xy = (1 + int(not have_negatives)) * safe_acos(cos_theta) / pi
-
-    return D_xy
+    def forward(self, X, Y):
+        """
+        angular distance is a valid distance metric based on the cosine similarity
+        see https://en.wikipedia.org/wiki/Cosine_similarity#Angular_distance_and_similarity
+
+        Shapes:
+        -------
+        X : (*, N, D)
+        Y : (*, M, D)
+        D_xy : (*, N, M)
+        """
+        have_negatives = torch.any(X < 0) or torch.any(Y < 0)
+        cos_theta = self.cosine_sim(X, Y)
+        pi = torch.acos(torch.zeros(1)).item() * 2
+        D_xy = (1 + int(not have_negatives)) * self.safe_acos(cos_theta) / pi
+        return D_xy
```

### Comparing `mimikit-0.3.4/mimikit/networks/parametrized_gaussian.py` & `mimikit-0.4.0/mimikit/networks/parametrized_gaussian.py`

 * *Files identical despite different names*

### Comparing `mimikit-0.3.4/mimikit/networks/resamplers.py` & `mimikit-0.4.0/mimikit/modules/resamplers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch.nn as nn
 import numpy as np
 from functools import partial
 
+
 __all__ = [
     'LinearResampler',
     'Conv1dResampler',
     'LSTMResampler'
 ]
 
 
@@ -20,39 +21,41 @@
         B, T, D = x.size()
         x = self.fc(x)
         return x.reshape(B, int(T * self.tf), int(D * self.df))
 
 
 class Conv1dResampler(nn.Module):
 
-    def __init__(self, in_d, t_factor, d_factor, **kwargs):
+    def __init__(self, in_dim, t_factor, d_factor, **kwargs):
         super().__init__()
         mod = nn.Conv1d if t_factor <= 1 else partial(nn.ConvTranspose1d, stride=t_factor)
-        self.cv = mod(in_d, int(in_d * d_factor),
-                      t_factor if t_factor >= 1 else int(1 / t_factor),
-                      **kwargs)
+        self.kernel_size = int(t_factor) if t_factor >= 1 else int(1 / t_factor)
+        self.out_dim = int(in_dim * d_factor)
+        self.cv = mod(in_dim, self.out_dim, self.kernel_size, **kwargs)
         self.tf, self.df = t_factor, d_factor
 
     def forward(self, x):
         if len(x.size()) > 3:
             x = x.view(x.size(0), np.prod(x.shape[1:-1]), x.size(-1))
         B, T, D = x.size()
         if self.tf <= 1:
-            x = x.view(-1, int(1 / self.tf), D).transpose(1, 2)
-            x = self.cv(x).squeeze(-1).reshape(B, int(D * self.df), -1)
+            x = x.view(-1, self.kernel_size, D).transpose(1, 2)
+            x = self.cv(x).squeeze(-1).reshape(B, self.out_dim, -1)
         else:
             x = x.transpose(1, 2)
             x = self.cv(x)
         return x.transpose(1, 2)
 
 
 class LSTMResampler(nn.Module):
 
-    def __init__(self, in_d, t_factor, d_factor, **kwargs):
+    def __init__(self, in_d, t_factor, d_factor, bidirectional=False, **kwargs):
         super().__init__()
-        self.lstm = nn.LSTM(in_d, int(in_d * t_factor * d_factor), batch_first=True, **kwargs)
+        self.lstm = nn.LSTM(in_d, int(in_d * t_factor * d_factor),
+                            batch_first=True, bidirectional=bidirectional, **kwargs)
         self.tf, self.df = t_factor, d_factor
+        self.bidirectional = bidirectional
 
     def forward(self, x, hidden=None):
         B, T, D = x.size()
         x, hidden = self.lstm(x, hidden)
-        return x.reshape(B, int(T * self.tf), int(D * self.df)), hidden
+        return x.reshape(B, int(T * self.tf), int(D * self.df) * (1 + self.bidirectional)), hidden
```

### Comparing `mimikit-0.3.4/mimikit/networks/s2s_lstm.py` & `mimikit-0.4.0/mimikit/networks/s2s_lstm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 import torch
 import torch.nn as nn
 from typing import Optional
-import dataclasses as dtc
-
-from mimikit.modules.misc import Abs
-from pytorch_lightning.utilities import AttributeDict
 
+from .arm import NetworkConfig
+from ..networks.arm import ARMWithHidden
+from ..io_spec import IOSpec
 from ..networks.parametrized_gaussian import ParametrizedGaussian
 
 __all__ = [
     'EncoderLSTM',
     'DecoderLSTM',
     'Seq2SeqLSTMNetwork',
     'MultiSeq2SeqLSTM'
 ]
 
 
-@dtc.dataclass(init=True, repr=False, eq=False, frozen=False, unsafe_hash=True)
 class EncoderLSTM(nn.Module):
-    input_d: int = 512
-    model_dim: int = 512
-    num_layers: int = 1
-    n_lstm: Optional[int] = 1
-    bottleneck: Optional[str] = "add"
-    n_fc: Optional[int] = 1
-    bias: Optional[bool] = False
-    weight_norm: Optional[bool] = False
-    hop: int = 8
-    with_tbptt: bool = False
+    def __init__(
+            self,
+            input_d: int = 512,
+            model_dim: int = 512,
+            num_layers: int = 1,
+            n_lstm: Optional[int] = 1,
+            bottleneck: Optional[str] = "add",
+            n_fc: Optional[int] = 1,
+            bias: Optional[bool] = False,
+            weight_norm: Optional[bool] = False,
+            hop: int = 8,
+            with_tbptt: bool = False,
+    ):
+        super(EncoderLSTM, self).__init__()
+        self.model_dim = model_dim
+        self.num_layers = num_layers
+        self.n_lstm = n_lstm
+        self.bottleneck = bottleneck
+        self.hop = hop
+        self.with_tbptt = with_tbptt
 
-    def __post_init__(self):
-        nn.Module.__init__(self)
         self.lstms = nn.ModuleList([
-            nn.LSTM(self.input_d if i == 0 else self.model_dim,
-                    self.model_dim if self.bottleneck == "add" else self.model_dim // 2,
-                    bias=self.bias,
-                    num_layers=self.num_layers,
+            nn.LSTM(input_d if i == 0 else model_dim,
+                    model_dim if bottleneck == "add" else model_dim // 2,
+                    bias=bias,
+                    num_layers=num_layers,
                     batch_first=True, bidirectional=True)
-            for i in range(self.n_lstm)
+            for i in range(n_lstm)
         ])
         self.fc = nn.Sequential(
-            *[nn.Sequential(nn.Linear(self.model_dim, self.model_dim), nn.Tanh()) for _ in range(self.n_fc - 1)],
-            nn.Linear(self.model_dim, self.model_dim, bias=False),  # NO ACTIVATION !
+            *[nn.Sequential(nn.Linear(model_dim, model_dim), nn.Tanh())
+              for _ in range(n_fc - 1)],
+            nn.Linear(model_dim, model_dim, bias=False),  # NO ACTIVATION !
         )
-        if self.weight_norm:
+        if weight_norm:
             for lstm in self.lstms:
                 for name, p in dict(lstm.named_parameters()).items():
                     if "weight" in name:
                         torch.nn.utils.weight_norm(lstm, name)
         self.hidden = None
 
     def forward(self, x):
@@ -80,31 +87,36 @@
             h0 = torch.zeros(self.num_layers * 2, B, self.model_dim).to(x.device)
             c0 = torch.zeros(self.num_layers * 2, B, self.model_dim).to(x.device)
             return h0, c0
         else:
             return tuple(h_.detach() for h_ in h)
 
 
-@dtc.dataclass(init=True, repr=False, eq=False, frozen=False, unsafe_hash=True)
 class DecoderLSTM(nn.Module):
-    model_dim: int = 512
-    num_layers: int = 1
-    bottleneck: Optional[str] = "add"
-    bias: Optional[bool] = False
-    weight_norm: Optional[tuple] = (False, False)
-
-    def __post_init__(self):
-        nn.Module.__init__(self)
-        self.lstm1 = nn.LSTM(self.model_dim, self.model_dim if self.bottleneck == "add" else self.model_dim // 2,
-                             bias=self.bias,
-                             num_layers=self.num_layers, batch_first=True, bidirectional=True)
-        self.lstm2 = nn.LSTM(self.model_dim, self.model_dim if self.bottleneck == "add" else self.model_dim // 2,
+    def __init__(self,
+                 model_dim: int = 512,
+                 num_layers: int = 1,
+                 bottleneck: Optional[str] = "add",
+                 bias: Optional[bool] = False,
+                 weight_norm: Optional[tuple] = (False, False),
+                 ):
+        super(DecoderLSTM, self).__init__()
+        self.model_dim = model_dim
+        self.num_layers = num_layers
+        self.bottleneck = bottleneck
+
+        self.lstm1 = nn.LSTM(model_dim, model_dim if bottleneck == "add" else model_dim // 2,
                              bias=self.bias,
-                             num_layers=self.num_layers, batch_first=True, bidirectional=True)
-        for lstm, wn in zip([self.lstm1, self.lstm2], self.weight_norm):
+                             num_layers=num_layers,
+                             batch_first=True, bidirectional=True)
+        self.lstm2 = nn.LSTM(model_dim, model_dim if bottleneck == "add" else model_dim // 2,
+                             bias=bias,
+                             num_layers=num_layers,
+                             batch_first=True, bidirectional=True)
+        for lstm, wn in zip([self.lstm1, self.lstm2], weight_norm):
             if wn:
                 for name, p in dict(lstm.named_parameters()).items():
                     if "weight" in name:
                         torch.nn.utils.weight_norm(lstm, name)
 
     def forward(self, x, hidden, cells):
         if hidden is None or cells is None:
@@ -129,52 +141,57 @@
     repeat_idx = [1] * a.dim()
     repeat_idx[dim] = n_tile
     a = a.repeat(*(repeat_idx,))
     order_index = torch.LongTensor(torch.cat([init_dim * torch.arange(n_tile) + i for i in range(init_dim)]))
     return torch.index_select(a, dim, order_index.to(a.device))
 
 
-class Seq2SeqLSTMNetwork(nn.Module):
-    device = property(lambda self: next(self.parameters()).device)
+class Seq2SeqLSTMNetwork(ARMWithHidden, nn.Module):
+    class Config(NetworkConfig):
+        io_spec: IOSpec = None
+        input_dim: int = 513
+        model_dim: int = 1024
+        num_layers: int = 1
+        n_lstm: int = 1
+        bottleneck: str = "add"
+        n_fc: int = 1
+        hop: int = 8
+        bias: Optional[bool] = False
+        weight_norm: bool = False
+        input_module: Optional[nn.Module] = None
+        output_module: Optional[nn.Module] = None
+        with_tbptt: bool = False
+        with_sampler: bool = True
+
+    @classmethod
+    def from_config(cls, cfg: "Seq2SeqLSTMNetwork.Config"):
+        enc = EncoderLSTM(cfg.input_dim,
+                          cfg.model_dim, cfg.num_layers, cfg.n_lstm, cfg.bottleneck, cfg.n_fc,
+                          bias=cfg.bias, weight_norm=cfg.weight_norm, hop=cfg.hop,
+                          with_tbptt=cfg.with_tbptt)
+        dec = DecoderLSTM(cfg.model_dim, cfg.num_layers, cfg.bottleneck,
+                          bias=cfg.bias, weight_norm=(cfg.weight_norm,) * 2)
+
+        return cls(cfg, input_module=None, output_module=None, encoder=enc, decoder=dec)
 
     def __init__(self,
-                 input_dim: int = 513,
-                 model_dim: int = 1024,
-                 num_layers: int = 1,
-                 n_lstm: int = 1,
-                 bottleneck: str = "add",
-                 n_fc: int = 1,
-                 hop: int = 8,
-                 bias: Optional[bool] = False,
-                 weight_norm: bool = False,
-                 input_module: Optional[nn.Module] = None,
-                 output_module: Optional[nn.Module] = None,
-                 with_tbptt: bool = False,
-                 with_sampler: bool = True
+                 config: "Seq2SeqLSTMNetwork.Config",
+                 input_module: nn.Module,
+                 output_module: nn.Module,
+                 encoder: EncoderLSTM,
+                 decoder: DecoderLSTM,
                  ):
-        init_ctx = locals()
         super(Seq2SeqLSTMNetwork, self).__init__()
-        init_ctx.pop("output_module")
-        init_ctx.pop("input_module")
-        init_ctx.pop("self")
-        init_ctx.pop("__class__")
-        self.hp = AttributeDict(init_ctx)
-        self.inpt_mod = input_module if input_module is not None else nn.Identity()
-        self.enc = EncoderLSTM(input_dim,
-                               model_dim, num_layers, n_lstm, bottleneck, n_fc,
-                               bias=bias, weight_norm=weight_norm, hop=hop,
-                               with_tbptt=with_tbptt)
-        self.dec = DecoderLSTM(model_dim, num_layers, bottleneck,
-                               bias=bias, weight_norm=(weight_norm,) * 2)
-        if with_sampler:
-            self.sampler = ParametrizedGaussian(model_dim, model_dim, bias=bias)
-        self.outpt_mod = nn.Sequential(
-            nn.Linear(model_dim, input_dim, bias=False), Abs()
-        ) if output_module is None else output_module
-        self.hop = self.rf = self.shift = self.hp.hop
+        self._config = config
+        self.inpt_mod = input_module
+        self.enc = encoder
+        self.dec = decoder
+        if config.with_sampler:
+            self.sampler = ParametrizedGaussian(config.model_dim, config.model_dim, bias=config.bias)
+        self.outpt_mod = output_module
         self.output_length = lambda n: n
 
     def forward(self, x, temperature=None):
         x = self.inpt_mod(x)
         coded, (h_enc, c_enc) = self.enc(x)
         return self.decode(coded, h_enc, c_enc, temperature)
```

### Comparing `mimikit-0.3.4/mimikit.egg-info/PKG-INFO` & `mimikit-0.4.0/mimikit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 Metadata-Version: 2.1
 Name: mimikit
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python package for generating audio with neural networks
 Home-page: https://github.com/ktonal/mimikit
 Download-URL: https://github.com/ktonal/mimikit
 Author: Antoine Daurat
 Author-email: ktonalberlin@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: audio music sound deep-learning
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 Provides-Extra: colab
 License-File: LICENSE
 
 # mimikit
 
-The MusIc ModelIng toolKIT (MIMIKIT) is a python package that does Machine Learning with music data.
+The MusIc ModelIng toolKIT (`mimikit`) is a python package that does Machine Learning with audio data.
 
-The goal of `mimikit` is to enable you to use referenced and experimental algorithms on data you provide.
+Currently, it focuses on training auto-regressive neural networks to generate audio.
 
-`mimikit` is still in early development, details and documentation are on their way.
+but it does also contain an app to perform basic & experimental clustering of audio data in a notebook.
 
-## License
+## Installation
+
+you can install with pip
+```shell script
+pip install mimikit[torch]
+```
+or with 
+```shell script
+pip install --upgrade mimikit[torch]
+```
+if you are looking for the latest version
+ 
+
+## Usage 
 
-mimikit is distributed under the terms of the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
+Head straight to the [notebooks](https://github.com/ktonal/mimikit-notebooks) for example usage of `mimikit`, or open them directly in Colab:
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktonal/mimikit-notebooks/blob/main)
 
+## Output Samples
 
+You can explore the outputs of different trainings done with `mimikit` at this demo website:
+
+   https://ktonal.github.io/mimikit-demo-outputs 
+
+## License
 
+`mimikit` is distributed under the terms of the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `mimikit-0.3.4/mimikit.egg-info/SOURCES.txt` & `mimikit-0.4.0/mimikit.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 mimikit/__init__.py
-mimikit/train.py
+mimikit/checkpoint.py
+mimikit/config.py
+mimikit/io_spec.py
 mimikit/utils.py
 mimikit.egg-info/PKG-INFO
 mimikit.egg-info/SOURCES.txt
 mimikit.egg-info/dependency_links.txt
 mimikit.egg-info/entry_points.txt
 mimikit.egg-info/requires.txt
 mimikit.egg-info/top_level.txt
 mimikit/demos/__init__.py
-mimikit/demos/ensemble.py
+mimikit/demos/clusterizer_app.py
+mimikit/demos/ensemble_generator.py
 mimikit/demos/freqnet.py
 mimikit/demos/generate_from_checkpoint.py
-mimikit/demos/s2s.py
+mimikit/demos/seq2seq.py
 mimikit/demos/srnn.py
-mimikit/demos/wn.py
 mimikit/extract/__init__.py
 mimikit/extract/clusters.py
 mimikit/extract/from_neighbors.py
+mimikit/extract/samplify.py
 mimikit/extract/segment.py
 mimikit/features/__init__.py
-mimikit/features/abstract.py
-mimikit/features/audio.py
-mimikit/features/audio_fmodules.py
-mimikit/features/feature.py
-mimikit/features/midi.py
+mimikit/features/dataset.py
+mimikit/features/extractor.py
+mimikit/features/functionals.py
+mimikit/features/item_spec.py
 mimikit/loops/__init__.py
 mimikit/loops/callbacks.py
 mimikit/loops/eval_checkpoint.py
 mimikit/loops/generate.py
-mimikit/loops/get_trainer.py
 mimikit/loops/logger.py
 mimikit/loops/samplers.py
 mimikit/loops/train_loops.py
 mimikit/models/__init__.py
-mimikit/models/checkpoint.py
-mimikit/models/ensemble.py
-mimikit/models/io_modules.py
+mimikit/models/ensemble_generator.py
 mimikit/models/nnn.py
-mimikit/models/s2s.py
-mimikit/models/srnns.py
-mimikit/models/wave_gan.py
-mimikit/models/wavenets.py
 mimikit/modules/__init__.py
-mimikit/modules/homs.py
+mimikit/modules/activations.py
+mimikit/modules/io.py
 mimikit/modules/loss_functions.py
 mimikit/modules/misc.py
+mimikit/modules/no_nan_hooks.py
+mimikit/modules/resamplers.py
+mimikit/modules/targets.py
 mimikit/networks/__init__.py
+mimikit/networks/arm.py
+mimikit/networks/mlp.py
 mimikit/networks/parametrized_gaussian.py
-mimikit/networks/resamplers.py
+mimikit/networks/poconet.py
 mimikit/networks/s2s_lstm.py
-mimikit/networks/sample_rnn.py
-mimikit/networks/single_class_mlp.py
+mimikit/networks/s2s_lstm_v2.py
+mimikit/networks/sample_rnn_v2.py
 mimikit/networks/tied_autoencoder.py
 mimikit/networks/transformers.py
-mimikit/networks/wavenet.py
+mimikit/networks/wave_gan.py
+mimikit/networks/wavenet_v2.py
+mimikit/ui/__init__.py
+mimikit/ui/config_view.py
+mimikit/ui/file_picker.py
+mimikit/ui/style_sheet.py
+mimikit/ui/widgets.py
+mimikit/views/__init__.py
+mimikit/views/clusterizer_app.py
+mimikit/views/clusters.py
+mimikit/views/dataset.py
+mimikit/views/functionals.py
+mimikit/views/io_spec.py
+mimikit/views/sample_rnn.py
+mimikit/views/train_arm.py
+mimikit/views/wavenet.py
```

### Comparing `mimikit-0.3.4/setup.py` & `mimikit-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,19 @@
         'Intended Audience :: Developers',
         "Intended Audience :: Science/Research",
         "Intended Audience :: Other Audience",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     "keywords": "audio music sound deep-learning",
-    'python_requires': '>=3.6',
+    'python_requires': '>=3.7',
     'install_requires': REQUIRES,
     'extras_require': {
       "torch": torch_requires,
       "colab": colab_requires,
     },
     'tests_require': ['coverage', 'pytest'],
     'packages': PACKAGES,
```

