# Comparing `tmp/deeptrack-1.5.5.tar.gz` & `tmp/deeptrack-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\deeptrack-1.5.5.tar", last modified: Tue Mar  7 16:10:36 2023, max compression
+gzip compressed data, was "deeptrack-1.5.6.tar", last modified: Thu Apr 13 14:02:44 2023, max compression
```

## Comparing `deeptrack-1.5.5.tar` & `deeptrack-1.5.6.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.619438 deeptrack-1.5.5/
--rw-rw-rw-   0        0        0    13314 2023-03-07 16:10:36.618441 deeptrack-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    11355 2023-03-07 16:07:26.000000 deeptrack-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.213342 deeptrack-1.5.5/deeptrack/
--rw-rw-rw-   0        0        0      919 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/__init__.py
--rw-rw-rw-   0        0        0     9270 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/aberrations.py
--rw-rw-rw-   0        0        0    25617 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/augmentations.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.283340 deeptrack-1.5.5/deeptrack/backend/
--rw-rw-rw-   0        0        0       75 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/__init__.py
--rw-rw-rw-   0        0        0      665 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/_config.py
--rw-rw-rw-   0        0        0     1155 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/citations.py
--rw-rw-rw-   0        0        0    10707 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/core.py
--rw-rw-rw-   0        0        0     5192 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/mie.py
--rw-rw-rw-   0        0        0    35295 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/backend/pint_definition.py
--rw-rw-rw-   0        0        0     4333 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/polynomials.py
--rw-rw-rw-   0        0        0     5203 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/tensorflow_bindings.py
--rw-rw-rw-   0        0        0     4648 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/backend/units.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.286340 deeptrack-1.5.5/deeptrack/datasets/
--rw-rw-rw-   0        0        0      322 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.306338 deeptrack-1.5.5/deeptrack/datasets/detection_QuantumDots/
--rw-rw-rw-   0        0        0       97 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/detection_QuantumDots/__init__.py
--rw-rw-rw-   0        0        0      822 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/detection_QuantumDots/detection_QuantomDuts_test.py
--rw-rw-rw-   0        0        0     2554 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/detection_QuantumDots/detection_QuantumDots.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.315341 deeptrack-1.5.5/deeptrack/datasets/detection_holography_nanoparticles/
--rw-rw-rw-   0        0        0      135 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/detection_holography_nanoparticles/__init__.py
--rw-rw-rw-   0        0        0     2999 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles.py
--rw-rw-rw-   0        0        0      911 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles_test.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.336338 deeptrack-1.5.5/deeptrack/datasets/detection_linking_hela/
--rw-rw-rw-   0        0        0       99 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/detection_linking_hela/__init__.py
--rw-rw-rw-   0        0        0     4479 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/detection_linking_hela/detection_linking_hela.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.341338 deeptrack-1.5.5/deeptrack/datasets/dmdataset/
--rw-rw-rw-   0        0        0       62 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/dmdataset/__init__.py
--rw-rw-rw-   0        0        0     4532 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/dmdataset/dmdataset.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.345343 deeptrack-1.5.5/deeptrack/datasets/endothelial_vs/
--rw-rw-rw-   0        0        0       76 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/endothelial_vs/__init__.py
--rw-rw-rw-   0        0        0     2574 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/endothelial_vs/endothelial_vs.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.349338 deeptrack-1.5.5/deeptrack/datasets/regression_diffusion_landscape/
--rw-rw-rw-   0        0        0      122 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/regression_diffusion_landscape/__init__.py
--rw-rw-rw-   0        0        0     4318 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/datasets/regression_diffusion_landscape/regression_diffusion_landscape.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.369338 deeptrack-1.5.5/deeptrack/datasets/regression_holography_nanoparticles/
--rw-rw-rw-   0        0        0      138 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/regression_holography_nanoparticles/__init__.py
--rw-rw-rw-   0        0        0     3336 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles.py
--rw-rw-rw-   0        0        0      918 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles_test.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.386338 deeptrack-1.5.5/deeptrack/datasets/segmentation_fluorescence_u2os/
--rw-rw-rw-   0        0        0      123 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/segmentation_fluorescence_u2os/__init__.py
--rw-rw-rw-   0        0        0     3683 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os.py
--rw-rw-rw-   0        0        0      883 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os_test.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.405337 deeptrack-1.5.5/deeptrack/datasets/segmentation_ssTEM_drosophila/
--rw-rw-rw-   0        0        0      120 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/segmentation_ssTEM_drosophila/__init__.py
--rw-rw-rw-   0        0        0     4093 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila.py
--rw-rw-rw-   0        0        0      876 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila_test.py
--rw-rw-rw-   0        0        0     5060 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/elementwise.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.419339 deeptrack-1.5.5/deeptrack/extras/
--rw-rw-rw-   0        0        0       36 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/extras/__init__.py
--rw-rw-rw-   0        0        0     6687 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/extras/datasets.py
--rw-rw-rw-   0        0        0     5235 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/extras/radialcenter.py
--rw-rw-rw-   0        0        0    70236 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/features.py
--rw-rw-rw-   0        0        0    15047 2022-12-21 09:53:27.000000 deeptrack-1.5.5/deeptrack/generators.py
--rw-rw-rw-   0        0        0     2814 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/holography.py
--rw-rw-rw-   0        0        0    16139 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/image.py
--rw-rw-rw-   0        0        0      128 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/layers.py
--rw-rw-rw-   0        0        0     7047 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/losses.py
--rw-rw-rw-   0        0        0    12123 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/math.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.441340 deeptrack-1.5.5/deeptrack/models/
--rw-rw-rw-   0        0        0      355 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/__init__.py
--rw-rw-rw-   0        0        0    31368 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/convolutional.py
--rw-rw-rw-   0        0        0     2355 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/dense.py
--rw-rw-rw-   0        0        0     6032 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/embeddings.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.458339 deeptrack-1.5.5/deeptrack/models/gans/
--rw-rw-rw-   0        0        0       86 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/gans/__init__.py
--rw-rw-rw-   0        0        0     5286 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gans/cgan.py
--rw-rw-rw-   0        0        0        0 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/gans/cyclegan.py
--rw-rw-rw-   0        0        0     4621 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/gans/gan.py
--rw-rw-rw-   0        0        0     7549 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gans/pcgan.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.483339 deeptrack-1.5.5/deeptrack/models/gnns/
--rw-rw-rw-   0        0        0       97 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gnns/__init__.py
--rw-rw-rw-   0        0        0     7146 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gnns/augmentations.py
--rw-rw-rw-   0        0        0     8120 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/gnns/generators.py
--rw-rw-rw-   0        0        0     8581 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gnns/graphs.py
--rw-rw-rw-   0        0        0    23118 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gnns/layers.py
--rw-rw-rw-   0        0        0    18915 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/gnns/models.py
--rw-rw-rw-   0        0        0     5119 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/gnns/utils.py
--rw-rw-rw-   0        0        0    27438 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/layers.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.499338 deeptrack-1.5.5/deeptrack/models/lodestar/
--rw-rw-rw-   0        0        0       78 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/lodestar/__init__.py
--rw-rw-rw-   0        0        0     4447 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/lodestar/equivariances.py
--rw-rw-rw-   0        0        0     2383 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/lodestar/generators.py
--rw-rw-rw-   0        0        0    13290 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/lodestar/models.py
--rw-rw-rw-   0        0        0     4402 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/recurrent.py
--rw-rw-rw-   0        0        0    12519 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.512338 deeptrack-1.5.5/deeptrack/models/vaes/
--rw-rw-rw-   0        0        0       18 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/models/vaes/__init__.py
--rw-rw-rw-   0        0        0     3938 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/models/vaes/vae.py
--rw-rw-rw-   0        0        0     3239 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/noises.py
--rw-rw-rw-   0        0        0    32619 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/optics.py
--rw-rw-rw-   0        0        0     8376 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/properties.py
--rw-rw-rw-   0        0        0    34408 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/scatterers.py
--rw-rw-rw-   0        0        0     4253 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/sequences.py
--rw-rw-rw-   0        0        0     7963 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/statistics.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.598442 deeptrack-1.5.5/deeptrack/test/
--rw-rw-rw-   0        0        0       12 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/__init__.py
--rw-rw-rw-   0        0        0      188 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test.py
--rw-rw-rw-   0        0        0     7545 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_aberrations.py
--rw-rw-rw-   0        0        0     6113 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_augmentations.py
--rw-rw-rw-   0        0        0     2830 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_elementwise.py
--rw-rw-rw-   0        0        0    39203 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_features.py
--rw-rw-rw-   0        0        0     6127 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/test/test_generators.py
--rw-rw-rw-   0        0        0    11111 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_image.py
--rw-rw-rw-   0        0        0    11920 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/test/test_layers.py
--rw-rw-rw-   0        0        0     4828 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_losses.py
--rw-rw-rw-   0        0        0      964 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_math.py
--rw-rw-rw-   0        0        0    11123 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_models.py
--rw-rw-rw-   0        0        0     1540 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_noises.py
--rw-rw-rw-   0        0        0     5201 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_optics.py
--rw-rw-rw-   0        0        0     1861 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_properties.py
--rw-rw-rw-   0        0        0    10884 2023-03-07 16:07:26.000000 deeptrack-1.5.5/deeptrack/test/test_scatterers.py
--rw-rw-rw-   0        0        0     6530 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_sequences.py
--rw-rw-rw-   0        0        0     4661 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_statistics.py
--rw-rw-rw-   0        0        0     2729 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/test/test_utils.py
--rw-rw-rw-   0        0        0      270 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/types.py
--rw-rw-rw-   0        0        0     3859 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.616438 deeptrack-1.5.5/deeptrack/visualization/
--rw-rw-rw-   0        0        0       72 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/visualization/__init__.py
--rw-rw-rw-   0        0        0     2759 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/visualization/callbacks.py
--rw-rw-rw-   0        0        0      644 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/visualization/colors.py
--rw-rw-rw-   0        0        0     8053 2022-12-06 14:11:07.000000 deeptrack-1.5.5/deeptrack/visualization/training.py
-drwxrwxrwx   0        0        0        0 2023-03-07 16:10:36.239340 deeptrack-1.5.5/deeptrack.egg-info/
--rw-rw-rw-   0        0        0    13314 2023-03-07 16:10:35.000000 deeptrack-1.5.5/deeptrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4190 2023-03-07 16:10:35.000000 deeptrack-1.5.5/deeptrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 16:10:35.000000 deeptrack-1.5.5/deeptrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-03-07 16:10:35.000000 deeptrack-1.5.5/deeptrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-07 16:10:35.000000 deeptrack-1.5.5/deeptrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       94 2022-12-07 16:29:47.000000 deeptrack-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-07 16:10:36.619438 deeptrack-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-03-07 16:08:57.000000 deeptrack-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.836030 deeptrack-1.5.6/
+-rw-rw-rw-   0        0        0     1093 2021-02-10 11:05:03.000000 deeptrack-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0    11879 2023-04-13 14:02:44.835529 deeptrack-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11355 2023-02-15 14:33:36.000000 deeptrack-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.732030 deeptrack-1.5.6/deeptrack/
+-rw-rw-rw-   0        0        0      919 2023-02-15 14:33:36.000000 deeptrack-1.5.6/deeptrack/__init__.py
+-rw-rw-rw-   0        0        0     9270 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/aberrations.py
+-rw-rw-rw-   0        0        0    25617 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/augmentations.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.763529 deeptrack-1.5.6/deeptrack/backend/
+-rw-rw-rw-   0        0        0       75 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/backend/__init__.py
+-rw-rw-rw-   0        0        0      665 2022-07-26 13:52:06.000000 deeptrack-1.5.6/deeptrack/backend/_config.py
+-rw-rw-rw-   0        0        0     1155 2022-07-26 13:52:06.000000 deeptrack-1.5.6/deeptrack/backend/citations.py
+-rw-rw-rw-   0        0        0    10707 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/backend/core.py
+-rw-rw-rw-   0        0        0     5192 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/backend/mie.py
+-rw-rw-rw-   0        0        0    35295 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/backend/pint_definition.py
+-rw-rw-rw-   0        0        0     4333 2022-06-28 11:56:35.000000 deeptrack-1.5.6/deeptrack/backend/polynomials.py
+-rw-rw-rw-   0        0        0     5203 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/backend/tensorflow_bindings.py
+-rw-rw-rw-   0        0        0     4648 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/backend/units.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.764530 deeptrack-1.5.6/deeptrack/datasets/
+-rw-rw-rw-   0        0        0      322 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.767530 deeptrack-1.5.6/deeptrack/datasets/detection_QuantumDots/
+-rw-rw-rw-   0        0        0       97 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/detection_QuantumDots/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/detection_QuantumDots/detection_QuantomDuts_test.py
+-rw-rw-rw-   0        0        0     2554 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/detection_QuantumDots/detection_QuantumDots.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.770529 deeptrack-1.5.6/deeptrack/datasets/detection_holography_nanoparticles/
+-rw-rw-rw-   0        0        0      135 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/detection_holography_nanoparticles/__init__.py
+-rw-rw-rw-   0        0        0     2999 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles.py
+-rw-rw-rw-   0        0        0      911 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles_test.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.772529 deeptrack-1.5.6/deeptrack/datasets/detection_linking_hela/
+-rw-rw-rw-   0        0        0       99 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/detection_linking_hela/__init__.py
+-rw-rw-rw-   0        0        0     4479 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/detection_linking_hela/detection_linking_hela.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.774030 deeptrack-1.5.6/deeptrack/datasets/dmdataset/
+-rw-rw-rw-   0        0        0       62 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/dmdataset/__init__.py
+-rw-rw-rw-   0        0        0     4532 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/dmdataset/dmdataset.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.776030 deeptrack-1.5.6/deeptrack/datasets/endothelial_vs/
+-rw-rw-rw-   0        0        0       76 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/endothelial_vs/__init__.py
+-rw-rw-rw-   0        0        0     2601 2023-04-13 14:02:13.000000 deeptrack-1.5.6/deeptrack/datasets/endothelial_vs/endothelial_vs.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.778030 deeptrack-1.5.6/deeptrack/datasets/regression_diffusion_landscape/
+-rw-rw-rw-   0        0        0      122 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/regression_diffusion_landscape/__init__.py
+-rw-rw-rw-   0        0        0     4318 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/datasets/regression_diffusion_landscape/regression_diffusion_landscape.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.781530 deeptrack-1.5.6/deeptrack/datasets/regression_holography_nanoparticles/
+-rw-rw-rw-   0        0        0      138 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/regression_holography_nanoparticles/__init__.py
+-rw-rw-rw-   0        0        0     3336 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles.py
+-rw-rw-rw-   0        0        0      918 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles_test.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.784529 deeptrack-1.5.6/deeptrack/datasets/segmentation_fluorescence_u2os/
+-rw-rw-rw-   0        0        0      123 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/segmentation_fluorescence_u2os/__init__.py
+-rw-rw-rw-   0        0        0     3683 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os.py
+-rw-rw-rw-   0        0        0      883 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os_test.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.787530 deeptrack-1.5.6/deeptrack/datasets/segmentation_ssTEM_drosophila/
+-rw-rw-rw-   0        0        0      120 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/segmentation_ssTEM_drosophila/__init__.py
+-rw-rw-rw-   0        0        0     4093 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila.py
+-rw-rw-rw-   0        0        0      876 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila_test.py
+-rw-rw-rw-   0        0        0     5060 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/elementwise.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.790029 deeptrack-1.5.6/deeptrack/extras/
+-rw-rw-rw-   0        0        0       36 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/extras/__init__.py
+-rw-rw-rw-   0        0        0     6687 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/extras/datasets.py
+-rw-rw-rw-   0        0        0     5235 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/extras/radialcenter.py
+-rw-rw-rw-   0        0        0    70270 2023-04-13 14:02:13.000000 deeptrack-1.5.6/deeptrack/features.py
+-rw-rw-rw-   0        0        0    15047 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/generators.py
+-rw-rw-rw-   0        0        0     2814 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/holography.py
+-rw-rw-rw-   0        0        0    16139 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/image.py
+-rw-rw-rw-   0        0        0      128 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/layers.py
+-rw-rw-rw-   0        0        0     7047 2022-07-26 13:52:06.000000 deeptrack-1.5.6/deeptrack/losses.py
+-rw-rw-rw-   0        0        0    12123 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/math.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.797030 deeptrack-1.5.6/deeptrack/models/
+-rw-rw-rw-   0        0        0      355 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/__init__.py
+-rw-rw-rw-   0        0        0    31368 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/convolutional.py
+-rw-rw-rw-   0        0        0     2355 2022-07-26 13:52:06.000000 deeptrack-1.5.6/deeptrack/models/dense.py
+-rw-rw-rw-   0        0        0     6032 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/embeddings.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.801030 deeptrack-1.5.6/deeptrack/models/gans/
+-rw-rw-rw-   0        0        0       86 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/models/gans/__init__.py
+-rw-rw-rw-   0        0        0     5286 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/gans/cgan.py
+-rw-rw-rw-   0        0        0        0 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/models/gans/cyclegan.py
+-rw-rw-rw-   0        0        0     4621 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/models/gans/gan.py
+-rw-rw-rw-   0        0        0     7549 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/gans/pcgan.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.807031 deeptrack-1.5.6/deeptrack/models/gnns/
+-rw-rw-rw-   0        0        0       97 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/gnns/__init__.py
+-rw-rw-rw-   0        0        0     7146 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/gnns/augmentations.py
+-rw-rw-rw-   0        0        0     8120 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/gnns/generators.py
+-rw-rw-rw-   0        0        0     8581 2023-02-15 14:33:36.000000 deeptrack-1.5.6/deeptrack/models/gnns/graphs.py
+-rw-rw-rw-   0        0        0    23118 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/gnns/layers.py
+-rw-rw-rw-   0        0        0    18915 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/gnns/models.py
+-rw-rw-rw-   0        0        0     5119 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/gnns/utils.py
+-rw-rw-rw-   0        0        0    27438 2023-02-15 14:33:36.000000 deeptrack-1.5.6/deeptrack/models/layers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.811029 deeptrack-1.5.6/deeptrack/models/lodestar/
+-rw-rw-rw-   0        0        0       78 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/models/lodestar/__init__.py
+-rw-rw-rw-   0        0        0     4447 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/lodestar/equivariances.py
+-rw-rw-rw-   0        0        0     2383 2023-02-01 12:31:26.000000 deeptrack-1.5.6/deeptrack/models/lodestar/generators.py
+-rw-rw-rw-   0        0        0    13290 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/lodestar/models.py
+-rw-rw-rw-   0        0        0     4402 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/recurrent.py
+-rw-rw-rw-   0        0        0    12519 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.813029 deeptrack-1.5.6/deeptrack/models/vaes/
+-rw-rw-rw-   0        0        0       18 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/models/vaes/__init__.py
+-rw-rw-rw-   0        0        0     3938 2023-04-13 14:02:13.000000 deeptrack-1.5.6/deeptrack/models/vaes/vae.py
+-rw-rw-rw-   0        0        0     3239 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/noises.py
+-rw-rw-rw-   0        0        0    32619 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/optics.py
+-rw-rw-rw-   0        0        0     8376 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/properties.py
+-rw-rw-rw-   0        0        0    34408 2023-02-15 14:33:36.000000 deeptrack-1.5.6/deeptrack/scatterers.py
+-rw-rw-rw-   0        0        0     4253 2023-02-01 11:10:10.000000 deeptrack-1.5.6/deeptrack/sequences.py
+-rw-rw-rw-   0        0        0     7963 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/statistics.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.830529 deeptrack-1.5.6/deeptrack/test/
+-rw-rw-rw-   0        0        0       12 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/test/__init__.py
+-rw-rw-rw-   0        0        0      188 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/test/test.py
+-rw-rw-rw-   0        0        0     7545 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/test/test_aberrations.py
+-rw-rw-rw-   0        0        0     6113 2022-10-27 09:37:11.000000 deeptrack-1.5.6/deeptrack/test/test_augmentations.py
+-rw-rw-rw-   0        0        0     2830 2022-07-26 13:52:06.000000 deeptrack-1.5.6/deeptrack/test/test_elementwise.py
+-rw-rw-rw-   0        0        0    39203 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/test/test_features.py
+-rw-rw-rw-   0        0        0     6127 2023-02-15 14:33:36.000000 deeptrack-1.5.6/deeptrack/test/test_generators.py
+-rw-rw-rw-   0        0        0    11111 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/test/test_image.py
+-rw-rw-rw-   0        0        0    11920 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/test/test_layers.py
+-rw-rw-rw-   0        0        0     4828 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/test/test_losses.py
+-rw-rw-rw-   0        0        0      964 2022-07-26 13:52:06.000000 deeptrack-1.5.6/deeptrack/test/test_math.py
+-rw-rw-rw-   0        0        0    11123 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/test/test_models.py
+-rw-rw-rw-   0        0        0     1540 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/test/test_noises.py
+-rw-rw-rw-   0        0        0     5201 2023-02-01 12:31:32.000000 deeptrack-1.5.6/deeptrack/test/test_optics.py
+-rw-rw-rw-   0        0        0     1861 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/test/test_properties.py
+-rw-rw-rw-   0        0        0    10884 2023-02-01 12:31:40.000000 deeptrack-1.5.6/deeptrack/test/test_scatterers.py
+-rw-rw-rw-   0        0        0     6530 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/test/test_sequences.py
+-rw-rw-rw-   0        0        0     4661 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/test/test_statistics.py
+-rw-rw-rw-   0        0        0     2729 2021-09-01 13:05:52.000000 deeptrack-1.5.6/deeptrack/test/test_utils.py
+-rw-rw-rw-   0        0        0      270 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/types.py
+-rw-rw-rw-   0        0        0     3859 2022-03-01 18:51:16.000000 deeptrack-1.5.6/deeptrack/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.834030 deeptrack-1.5.6/deeptrack/visualization/
+-rw-rw-rw-   0        0        0       72 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/visualization/__init__.py
+-rw-rw-rw-   0        0        0     2759 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/visualization/callbacks.py
+-rw-rw-rw-   0        0        0      644 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/visualization/colors.py
+-rw-rw-rw-   0        0        0     8053 2023-02-01 11:13:17.000000 deeptrack-1.5.6/deeptrack/visualization/training.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:02:44.755030 deeptrack-1.5.6/deeptrack.egg-info/
+-rw-rw-rw-   0        0        0    11879 2023-04-13 14:02:44.000000 deeptrack-1.5.6/deeptrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4198 2023-04-13 14:02:44.000000 deeptrack-1.5.6/deeptrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:02:44.000000 deeptrack-1.5.6/deeptrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-04-13 14:02:44.000000 deeptrack-1.5.6/deeptrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 14:02:44.000000 deeptrack-1.5.6/deeptrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       94 2022-07-26 13:52:06.000000 deeptrack-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:02:44.836030 deeptrack-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-04-13 14:02:24.000000 deeptrack-1.5.6/setup.py
```

### Comparing `deeptrack-1.5.5/PKG-INFO` & `deeptrack-1.5.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,191 +1,176 @@
-Metadata-Version: 2.1
-Name: deeptrack
-Version: 1.5.5
-Summary: A deep learning oriented microscopy image simulation package
-Home-page: https://github.com/softmatterlab/DeepTrack-2.0/
-Author: Benjamin Midtvedt
-Author-email: benjamin.midtvedt@physics.gu.se
-License: UNKNOWN
-Description: <p align="center">
-          <img width="350" src=https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/logo.png?raw=true>
-        </p>
-        
-        <h3 align="center">A comprehensive deep learning framework for digital microscopy.</h3>
-        <p align="center">
-          <a href="/LICENSE" alt="licence"><img src="https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0"></a>
-          <a href="https://badge.fury.io/py/deeptrack"><img src="https://badge.fury.io/py/deeptrack.svg" alt="PyPI version"></a>
-          <a href="https://softmatterlab.github.io/DeepTrack2/deeptrack.html"><img src="https://img.shields.io/badge/docs-passing-green" alt="PyPI version"></a>
-          <a href="https://badge.fury.io/py/deeptrack"><img src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue" alt="Python version"></a>
-          <a href="https://doi.org/10.1063/5.0034891" alt="DOI">
-            <img src="https://img.shields.io/badge/DOI-10.1063%2F5.0034891-blue">
-          </a>
-        </p>
-        <p align="center">
-          <a href="#installation">Installation</a> â€¢
-          <a href="#using-deeptrack">Examples</a> â€¢
-          <a href="#learning-deeptrack-21">Basics</a> â€¢
-          <a href="#cite-us">Cite us</a> â€¢
-          <a href="/LICENSE">License</a> 
-        </p>
-        
-        
-        We provide tools to create physical simulations of optical systems, to generate and train neural network models, and to analyze experimental data.
-        
-        # Installation
-        
-        DeepTrack 2.1 requires at least python 3.6.
-        
-        To install DeepTrack 2.1, open a terminal or command prompt and run:
-        
-            pip install deeptrack
-            
-        If you have a very recent version of python, you may need to install numpy _before_ DeepTrack. This is a known issue with scikit-image.
-        
-        ### Updating to 2.1 from 2.0
-        
-        If you are already using DeepTrack 2.0 (pypi version 0.x.x), updating to DeepTrack 2.1 (pypi version 1.x.x) is painless. If you have followed deprecation warnings, no change to your code is needed. There are two breaking changes:
-        
-        - The deprecated operator `+` to chain features has been removed. It is now only possible using the `>>` operator.
-        - The deprecated operator `**` to duplicate a feature has been removed. It is now only possible using the `^` operator.
-        
-        If you notice any other changes in behavior, please report it to us in the issues tab.
-        
-        # Examples of applications using DeepTrack 
-        
-        DeepTrack is a general purpose deep learning framework for microscopy, meaning you can use it for any task you like. Here, we show some common applications!
-        
-        <br/>
-        <h3 align="left"> Single particle tracking </h3>
-        <p align="left">
-          <img width="300" src=/assets/SPT-ideal.gif?raw=true>
-          <img width="300" src=/assets/SPT-noisy.gif?raw=true>
-          <br/>
-          <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/2-single_particle_tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a CNN-based single particle tracker using simulated data </a>
-          <br/>
-          <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
-            <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
-          </a> 
-          <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/02.%20tracking_particles_of_various_shapes.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Unsupervised training of a single particle tracker using LodeSTAR </a> 
-          
-        </p>
-        <br/>
-        
-        <h3 align="left"> Multi-particle tracking </h3>
-        
-        <p align="left">
-          <img width="600" src=/assets/MPT-packed.gif?raw=true>
-          <br/>
-          <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
-            <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
-          </a> <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/03.track_BF-C2DL-HSC.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training LodeSTAR to detect multiple cells from a single image </a>
-          <br/>
-          <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/4-multi-molecule-tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a UNet-based multi-particle tracker using simulated data </a> 
-        </p>
-        <br/>
-        
-        <h3 align="left"> Particle tracing </h3>
-        
-        <p align="left">
-          <img width="600" src=/assets/Tracing.gif?raw=true>
-          <br/>
-          <a href="https://doi.org/10.48550/arXiv.2202.06355" alt="DOI magik">
-            <img src="https://img.shields.io/badge/DOI-10.48550%2FarXiv.2202.0635-blue">
-          </a>  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/develop/examples/MAGIK/cell_migration_analysis.ipynb"> <img     src="https://colab.research.google.com/assets/colab-badge.svg"> Training MAGIK to trace migrating cells </a>
-        </p>
-        
-        # Basics to learn DeepTrack 2.1
-        
-        Everybody learns in different ways! Depending on your preferences, and what you want to do with DeepTrack, you may want to check out one or more of these resources.
-        
-        ## Getting-started guides
-        
-        We have two separate series of notebooks which aims to teach you all you need to know to use DeepTrack to its fullest. The first is a set of six notebooks with a focus on the application.
-        
-        1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> deeptrack_introduction_tutorial </a>  gives an overview of how to use DeepTrack 2.1.
-        2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/tracking_particle_cnn_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track a point particle with a convolutional neural network (CNN).
-        3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorial/tracking_multiple_particles_unet_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track multiple particles using a U-net.
-        4. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/characterizing_aberrations_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> characterizing_aberrations_tutorial </a> demonstrates how to add and characterize aberrations of an optical device. 
-        5. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/distinguishing_particles_in_brightfield_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> distinguishing_particles_in_brightfield_tutorial </a> demonstrates how to use a U-net to track and distinguish particles of different sizes in brightfield microscopy. 
-        6. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/analyzing_video_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> analyzing_video_tutorial </a> demonstrates how to create videos and how to train a neural network to analyze them.
-        
-        
-        The second series focuses on individual topics, introducing them in a natural order. 
-        
-        1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Introducing how to create simulation pipelines and train models. </a>
-        2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/02.%20using_deeptrack_generators.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating data generators. </a> 
-        3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/03.%20customizing_deeptrack_models.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating how to customize models using layer-blocks. </a> 
-        
-        ## DeepTrack 2.1 in action
-        
-        Additionally, we have seven more case studies which are less documented, but gives additional insight in how to use DeepTrack with real datasets
-        
-        1. [MNIST](examples/paper-examples/1-MNIST.ipynb) classifies handwritted digits.
-        2. [single particle tracking](examples/paper-examples/2-single_particle_tracking.ipynb) tracks experimentally captured videos of a single particle. (Requires opencv-python compiled with ffmpeg to open and read a video.)
-        3. [single particle sizing](examples/paper-examples/3-particle_sizing.ipynb) extracts the radius and refractive index of particles.
-        4. [multi-particle tracking](examples/paper-examples/4-multi-molecule-tracking.ipynb) detects quantum dots in a low SNR image.
-        5. [3-dimensional tracking](examples/paper-examples/5-inline_holography_3d_tracking.ipynb) tracks particles in three dimensions.
-        6. [cell counting](examples/paper-examples/6-cell_counting.ipynb) counts the number of cells in fluorescence images.
-        7. [GAN image generation](examples/paper-examples/7-GAN_image_generation.ipynb) uses a GAN to create cell image from masks.
-        
-        ## Model-specific examples
-        
-        We also have examples that are specific for certain models. This includes 
-        - [*LodeSTAR*](examples/LodeSTAR) for label-free particle tracking.
-        - [*MAGIK*](deeptrack/models/gnns/) for graph-based particle linking and trace characterization.
-        
-        ## Documentation
-        The detailed documentation of DeepTrack 2.1 is available at the following link: https://softmatterlab.github.io/DeepTrack2/deeptrack.html
-        
-        ## Video Tutorials
-        
-        Videos are currently being updated to match with the current version of DeepTrack.
-        
-        ## Cite us!
-        If you use DeepTrack 2.1 in your project, please cite us here:
-        
-        ```
-        Benjamin Midtvedt, Saga Helgadottir, Aykut Argun, JesÃºs Pineda, Daniel Midtvedt, Giovanni Volpe.
-        "Quantitative Digital Microscopy with Deep Learning."
-        Applied Physics Reviews 8 (2021), 011310.
-        https://doi.org/10.1063/5.0034891
-        ```
-        
-        See also:
-        
-        <https://www.nature.com/articles/s41467-022-35004-y>:
-        ```
-        Midtvedt, B., Pineda, J., SkÃ¤rberg, F. et al. 
-        "Single-shot self-supervised object detection in microscopy." 
-        Nat Commun 13, 7492 (2022).
-        ```
-        
-        <https://arxiv.org/abs/2202.06355>:
-        ```
-        JesÃºs Pineda, Benjamin Midtvedt, Harshith Bachimanchi, Sergio NoÃ©, Daniel  Midtvedt, Giovanni Volpe,1 and  Carlo  Manzo
-        "Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic motion."
-        arXiv 2202.06355 (2022).
-        ```
-        
-        <https://doi.org/10.1364/OPTICA.6.000506>:
-        ```
-        Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
-        "Digital video microscopy enhanced by deep learning."
-        Optica 6.4 (2019): 506-513.
-        ```
-        
-        <https://github.com/softmatterlab/DeepTrack.git>:
-        ```
-        Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
-        "DeepTrack." (2019)
-        ```
-        
-        ## Funding
-        
-        This work was supported by the ERC Starting Grant ComplexSwimmers (Grant No. 677511), the ERC Starting Grant MAPEI (101001267), and the Knut and Alice Wallenberg Foundation.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+<p align="center">
+  <img width="350" src=https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/logo.png?raw=true>
+</p>
+
+<h3 align="center">A comprehensive deep learning framework for digital microscopy.</h3>
+<p align="center">
+  <a href="/LICENSE" alt="licence"><img src="https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0"></a>
+  <a href="https://badge.fury.io/py/deeptrack"><img src="https://badge.fury.io/py/deeptrack.svg" alt="PyPI version"></a>
+  <a href="https://softmatterlab.github.io/DeepTrack2/deeptrack.html"><img src="https://img.shields.io/badge/docs-passing-green" alt="PyPI version"></a>
+  <a href="https://badge.fury.io/py/deeptrack"><img src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue" alt="Python version"></a>
+  <a href="https://doi.org/10.1063/5.0034891" alt="DOI">
+    <img src="https://img.shields.io/badge/DOI-10.1063%2F5.0034891-blue">
+  </a>
+</p>
+<p align="center">
+  <a href="#installation">Installation</a> •
+  <a href="#using-deeptrack">Examples</a> •
+  <a href="#learning-deeptrack-21">Basics</a> •
+  <a href="#cite-us">Cite us</a> •
+  <a href="/LICENSE">License</a> 
+</p>
+
+
+We provide tools to create physical simulations of optical systems, to generate and train neural network models, and to analyze experimental data.
+
+# Installation
+
+DeepTrack 2.1 requires at least python 3.6.
+
+To install DeepTrack 2.1, open a terminal or command prompt and run:
+
+    pip install deeptrack
+    
+If you have a very recent version of python, you may need to install numpy _before_ DeepTrack. This is a known issue with scikit-image.
+
+### Updating to 2.1 from 2.0
+
+If you are already using DeepTrack 2.0 (pypi version 0.x.x), updating to DeepTrack 2.1 (pypi version 1.x.x) is painless. If you have followed deprecation warnings, no change to your code is needed. There are two breaking changes:
+
+- The deprecated operator `+` to chain features has been removed. It is now only possible using the `>>` operator.
+- The deprecated operator `**` to duplicate a feature has been removed. It is now only possible using the `^` operator.
+
+If you notice any other changes in behavior, please report it to us in the issues tab.
+
+# Examples of applications using DeepTrack 
+
+DeepTrack is a general purpose deep learning framework for microscopy, meaning you can use it for any task you like. Here, we show some common applications!
+
+<br/>
+<h3 align="left"> Single particle tracking </h3>
+<p align="left">
+  <img width="300" src=/assets/SPT-ideal.gif?raw=true>
+  <img width="300" src=/assets/SPT-noisy.gif?raw=true>
+  <br/>
+  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/2-single_particle_tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a CNN-based single particle tracker using simulated data </a>
+  <br/>
+  <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
+    <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
+  </a> 
+  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/02.%20tracking_particles_of_various_shapes.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Unsupervised training of a single particle tracker using LodeSTAR </a> 
+  
+</p>
+<br/>
+
+<h3 align="left"> Multi-particle tracking </h3>
+
+<p align="left">
+  <img width="600" src=/assets/MPT-packed.gif?raw=true>
+  <br/>
+  <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
+    <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
+  </a> <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/03.track_BF-C2DL-HSC.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training LodeSTAR to detect multiple cells from a single image </a>
+  <br/>
+  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/4-multi-molecule-tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a UNet-based multi-particle tracker using simulated data </a> 
+</p>
+<br/>
+
+<h3 align="left"> Particle tracing </h3>
+
+<p align="left">
+  <img width="600" src=/assets/Tracing.gif?raw=true>
+  <br/>
+  <a href="https://doi.org/10.48550/arXiv.2202.06355" alt="DOI magik">
+    <img src="https://img.shields.io/badge/DOI-10.48550%2FarXiv.2202.0635-blue">
+  </a>  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/develop/examples/MAGIK/cell_migration_analysis.ipynb"> <img     src="https://colab.research.google.com/assets/colab-badge.svg"> Training MAGIK to trace migrating cells </a>
+</p>
+
+# Basics to learn DeepTrack 2.1
+
+Everybody learns in different ways! Depending on your preferences, and what you want to do with DeepTrack, you may want to check out one or more of these resources.
+
+## Getting-started guides
+
+We have two separate series of notebooks which aims to teach you all you need to know to use DeepTrack to its fullest. The first is a set of six notebooks with a focus on the application.
+
+1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> deeptrack_introduction_tutorial </a>  gives an overview of how to use DeepTrack 2.1.
+2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/tracking_particle_cnn_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track a point particle with a convolutional neural network (CNN).
+3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorial/tracking_multiple_particles_unet_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track multiple particles using a U-net.
+4. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/characterizing_aberrations_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> characterizing_aberrations_tutorial </a> demonstrates how to add and characterize aberrations of an optical device. 
+5. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/distinguishing_particles_in_brightfield_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> distinguishing_particles_in_brightfield_tutorial </a> demonstrates how to use a U-net to track and distinguish particles of different sizes in brightfield microscopy. 
+6. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/analyzing_video_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> analyzing_video_tutorial </a> demonstrates how to create videos and how to train a neural network to analyze them.
+
+
+The second series focuses on individual topics, introducing them in a natural order. 
+
+1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Introducing how to create simulation pipelines and train models. </a>
+2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/02.%20using_deeptrack_generators.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating data generators. </a> 
+3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/03.%20customizing_deeptrack_models.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating how to customize models using layer-blocks. </a> 
+
+## DeepTrack 2.1 in action
+
+Additionally, we have seven more case studies which are less documented, but gives additional insight in how to use DeepTrack with real datasets
+
+1. [MNIST](examples/paper-examples/1-MNIST.ipynb) classifies handwritted digits.
+2. [single particle tracking](examples/paper-examples/2-single_particle_tracking.ipynb) tracks experimentally captured videos of a single particle. (Requires opencv-python compiled with ffmpeg to open and read a video.)
+3. [single particle sizing](examples/paper-examples/3-particle_sizing.ipynb) extracts the radius and refractive index of particles.
+4. [multi-particle tracking](examples/paper-examples/4-multi-molecule-tracking.ipynb) detects quantum dots in a low SNR image.
+5. [3-dimensional tracking](examples/paper-examples/5-inline_holography_3d_tracking.ipynb) tracks particles in three dimensions.
+6. [cell counting](examples/paper-examples/6-cell_counting.ipynb) counts the number of cells in fluorescence images.
+7. [GAN image generation](examples/paper-examples/7-GAN_image_generation.ipynb) uses a GAN to create cell image from masks.
+
+## Model-specific examples
+
+We also have examples that are specific for certain models. This includes 
+- [*LodeSTAR*](examples/LodeSTAR) for label-free particle tracking.
+- [*MAGIK*](deeptrack/models/gnns/) for graph-based particle linking and trace characterization.
+
+## Documentation
+The detailed documentation of DeepTrack 2.1 is available at the following link: https://softmatterlab.github.io/DeepTrack2/deeptrack.html
+
+## Video Tutorials
+
+Videos are currently being updated to match with the current version of DeepTrack.
+
+## Cite us!
+If you use DeepTrack 2.1 in your project, please cite us here:
+
+```
+Benjamin Midtvedt, Saga Helgadottir, Aykut Argun, Jesús Pineda, Daniel Midtvedt, Giovanni Volpe.
+"Quantitative Digital Microscopy with Deep Learning."
+Applied Physics Reviews 8 (2021), 011310.
+https://doi.org/10.1063/5.0034891
+```
+
+See also:
+
+<https://www.nature.com/articles/s41467-022-35004-y>:
+```
+Midtvedt, B., Pineda, J., Skärberg, F. et al. 
+"Single-shot self-supervised object detection in microscopy." 
+Nat Commun 13, 7492 (2022).
+```
+
+<https://arxiv.org/abs/2202.06355>:
+```
+Jesús Pineda, Benjamin Midtvedt, Harshith Bachimanchi, Sergio Noé, Daniel  Midtvedt, Giovanni Volpe,1 and  Carlo  Manzo
+"Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic motion."
+arXiv 2202.06355 (2022).
+```
+
+<https://doi.org/10.1364/OPTICA.6.000506>:
+```
+Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
+"Digital video microscopy enhanced by deep learning."
+Optica 6.4 (2019): 506-513.
+```
+
+<https://github.com/softmatterlab/DeepTrack.git>:
+```
+Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
+"DeepTrack." (2019)
+```
+
+## Funding
+
+This work was supported by the ERC Starting Grant ComplexSwimmers (Grant No. 677511), the ERC Starting Grant MAPEI (101001267), and the Knut and Alice Wallenberg Foundation.
```

#### html2text {}

```diff
@@ -1,18 +1,14 @@
-Metadata-Version: 2.1 Name: deeptrack Version: 1.5.5 Summary: A deep learning
-oriented microscopy image simulation package Home-page: https://github.com/
-softmatterlab/DeepTrack-2.0/ Author: Benjamin Midtvedt Author-email:
-benjamin.midtvedt@physics.gu.se License: UNKNOWN Description:
        [https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/
                               logo.png?raw=true]
    **** A comprehensive deep learning framework for digital microscopy. ****
    [https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0] [PyPI
   version] [PyPI_version] [Python_version] [https://img.shields.io/badge/DOI-
                            10.1063%2F5.0034891-blue]
- Installation Ã¢â¬Â¢ Examples Ã¢â¬Â¢ Basics Ã¢â¬Â¢ Cite_us Ã¢â¬Â¢ License
+         Installation â¢ Examples â¢ Basics â¢ Cite_us â¢ License
 We provide tools to create physical simulations of optical systems, to generate
 and train neural network models, and to analyze experimental data. #
 Installation DeepTrack 2.1 requires at least python 3.6. To install DeepTrack
 2.1, open a terminal or command prompt and run: pip install deeptrack If you
 have a very recent version of python, you may need to install numpy _before_
 DeepTrack. This is a known issue with scikit-image. ### Updating to 2.1 from
 2.0 If you are already using DeepTrack 2.0 (pypi version 0.x.x), updating to
@@ -90,27 +86,24 @@
 (examples/LodeSTAR) for label-free particle tracking. - [*MAGIK*](deeptrack/
 models/gnns/) for graph-based particle linking and trace characterization. ##
 Documentation The detailed documentation of DeepTrack 2.1 is available at the
 following link: https://softmatterlab.github.io/DeepTrack2/deeptrack.html ##
 Video Tutorials Videos are currently being updated to match with the current
 version of DeepTrack. ## Cite us! If you use DeepTrack 2.1 in your project,
 please cite us here: ``` Benjamin Midtvedt, Saga Helgadottir, Aykut Argun,
-JesÃÂºs Pineda, Daniel Midtvedt, Giovanni Volpe. "Quantitative Digital
+JesÃºs Pineda, Daniel Midtvedt, Giovanni Volpe. "Quantitative Digital
 Microscopy with Deep Learning." Applied Physics Reviews 8 (2021), 011310.
 https://doi.org/10.1063/5.0034891 ``` See also:
 www.nature.com/articles/s41467-022-35004-y>: ``` Midtvedt, B., Pineda, J.,
-SkÃÂ¤rberg, F. et al. "Single-shot self-supervised object detection in
+SkÃ¤rberg, F. et al. "Single-shot self-supervised object detection in
 microscopy." Nat Commun 13, 7492 (2022). ```
-arxiv.org/abs/2202.06355>: ``` JesÃÂºs Pineda, Benjamin Midtvedt, Harshith
-Bachimanchi, Sergio NoÃÂ©, Daniel Midtvedt, Giovanni Volpe,1 and Carlo Manzo
+arxiv.org/abs/2202.06355>: ``` JesÃºs Pineda, Benjamin Midtvedt, Harshith
+Bachimanchi, Sergio NoÃ©, Daniel Midtvedt, Giovanni Volpe,1 and Carlo Manzo
 "Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic
 motion." arXiv 2202.06355 (2022). ```
 doi.org/10.1364/OPTICA.6.000506>: ``` Saga Helgadottir, Aykut Argun, and
 Giovanni Volpe. "Digital video microscopy enhanced by deep learning." Optica
 6.4 (2019): 506-513. ```
 github.com/softmatterlab/DeepTrack.git>: ``` Saga Helgadottir, Aykut Argun, and
 Giovanni Volpe. "DeepTrack." (2019) ``` ## Funding This work was supported by
 the ERC Starting Grant ComplexSwimmers (Grant No. 677511), the ERC Starting
 Grant MAPEI (101001267), and the Knut and Alice Wallenberg Foundation.
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `deeptrack-1.5.5/README.md` & `deeptrack-1.5.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: deeptrack
+Version: 1.5.6
+Summary: A deep learning oriented microscopy image simulation package
+Home-page: https://github.com/softmatterlab/DeepTrack-2.0/
+Author: Benjamin Midtvedt
+Author-email: benjamin.midtvedt@physics.gu.se
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img width="350" src=https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/logo.png?raw=true>
 </p>
 
 <h3 align="center">A comprehensive deep learning framework for digital microscopy.</h3>
 <p align="center">
   <a href="/LICENSE" alt="licence"><img src="https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0"></a>
@@ -9,18 +23,18 @@
   <a href="https://softmatterlab.github.io/DeepTrack2/deeptrack.html"><img src="https://img.shields.io/badge/docs-passing-green" alt="PyPI version"></a>
   <a href="https://badge.fury.io/py/deeptrack"><img src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue" alt="Python version"></a>
   <a href="https://doi.org/10.1063/5.0034891" alt="DOI">
     <img src="https://img.shields.io/badge/DOI-10.1063%2F5.0034891-blue">
   </a>
 </p>
 <p align="center">
-  <a href="#installation">Installation</a> •
-  <a href="#using-deeptrack">Examples</a> •
-  <a href="#learning-deeptrack-21">Basics</a> •
-  <a href="#cite-us">Cite us</a> •
+  <a href="#installation">Installation</a> â€¢
+  <a href="#using-deeptrack">Examples</a> â€¢
+  <a href="#learning-deeptrack-21">Basics</a> â€¢
+  <a href="#cite-us">Cite us</a> â€¢
   <a href="/LICENSE">License</a> 
 </p>
 
 
 We provide tools to create physical simulations of optical systems, to generate and train neural network models, and to analyze experimental data.
 
 # Installation
@@ -132,32 +146,32 @@
 
 Videos are currently being updated to match with the current version of DeepTrack.
 
 ## Cite us!
 If you use DeepTrack 2.1 in your project, please cite us here:
 
 ```
-Benjamin Midtvedt, Saga Helgadottir, Aykut Argun, Jesús Pineda, Daniel Midtvedt, Giovanni Volpe.
+Benjamin Midtvedt, Saga Helgadottir, Aykut Argun, JesÃºs Pineda, Daniel Midtvedt, Giovanni Volpe.
 "Quantitative Digital Microscopy with Deep Learning."
 Applied Physics Reviews 8 (2021), 011310.
 https://doi.org/10.1063/5.0034891
 ```
 
 See also:
 
 <https://www.nature.com/articles/s41467-022-35004-y>:
 ```
-Midtvedt, B., Pineda, J., Skärberg, F. et al. 
+Midtvedt, B., Pineda, J., SkÃ¤rberg, F. et al. 
 "Single-shot self-supervised object detection in microscopy." 
 Nat Commun 13, 7492 (2022).
 ```
 
 <https://arxiv.org/abs/2202.06355>:
 ```
-Jesús Pineda, Benjamin Midtvedt, Harshith Bachimanchi, Sergio Noé, Daniel  Midtvedt, Giovanni Volpe,1 and  Carlo  Manzo
+JesÃºs Pineda, Benjamin Midtvedt, Harshith Bachimanchi, Sergio NoÃ©, Daniel  Midtvedt, Giovanni Volpe,1 and  Carlo  Manzo
 "Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic motion."
 arXiv 2202.06355 (2022).
 ```
 
 <https://doi.org/10.1364/OPTICA.6.000506>:
 ```
 Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
```

#### html2text {}

```diff
@@ -1,14 +1,21 @@
+Metadata-Version: 2.1 Name: deeptrack Version: 1.5.6 Summary: A deep learning
+oriented microscopy image simulation package Home-page: https://github.com/
+softmatterlab/DeepTrack-2.0/ Author: Benjamin Midtvedt Author-email:
+benjamin.midtvedt@physics.gu.se Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
        [https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/
                               logo.png?raw=true]
    **** A comprehensive deep learning framework for digital microscopy. ****
    [https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0] [PyPI
   version] [PyPI_version] [Python_version] [https://img.shields.io/badge/DOI-
                            10.1063%2F5.0034891-blue]
-         Installation â¢ Examples â¢ Basics â¢ Cite_us â¢ License
+ Installation Ã¢â¬Â¢ Examples Ã¢â¬Â¢ Basics Ã¢â¬Â¢ Cite_us Ã¢â¬Â¢ License
 We provide tools to create physical simulations of optical systems, to generate
 and train neural network models, and to analyze experimental data. #
 Installation DeepTrack 2.1 requires at least python 3.6. To install DeepTrack
 2.1, open a terminal or command prompt and run: pip install deeptrack If you
 have a very recent version of python, you may need to install numpy _before_
 DeepTrack. This is a known issue with scikit-image. ### Updating to 2.1 from
 2.0 If you are already using DeepTrack 2.0 (pypi version 0.x.x), updating to
@@ -86,22 +93,22 @@
 (examples/LodeSTAR) for label-free particle tracking. - [*MAGIK*](deeptrack/
 models/gnns/) for graph-based particle linking and trace characterization. ##
 Documentation The detailed documentation of DeepTrack 2.1 is available at the
 following link: https://softmatterlab.github.io/DeepTrack2/deeptrack.html ##
 Video Tutorials Videos are currently being updated to match with the current
 version of DeepTrack. ## Cite us! If you use DeepTrack 2.1 in your project,
 please cite us here: ``` Benjamin Midtvedt, Saga Helgadottir, Aykut Argun,
-JesÃºs Pineda, Daniel Midtvedt, Giovanni Volpe. "Quantitative Digital
+JesÃÂºs Pineda, Daniel Midtvedt, Giovanni Volpe. "Quantitative Digital
 Microscopy with Deep Learning." Applied Physics Reviews 8 (2021), 011310.
 https://doi.org/10.1063/5.0034891 ``` See also:
 www.nature.com/articles/s41467-022-35004-y>: ``` Midtvedt, B., Pineda, J.,
-SkÃ¤rberg, F. et al. "Single-shot self-supervised object detection in
+SkÃÂ¤rberg, F. et al. "Single-shot self-supervised object detection in
 microscopy." Nat Commun 13, 7492 (2022). ```
-arxiv.org/abs/2202.06355>: ``` JesÃºs Pineda, Benjamin Midtvedt, Harshith
-Bachimanchi, Sergio NoÃ©, Daniel Midtvedt, Giovanni Volpe,1 and Carlo Manzo
+arxiv.org/abs/2202.06355>: ``` JesÃÂºs Pineda, Benjamin Midtvedt, Harshith
+Bachimanchi, Sergio NoÃÂ©, Daniel Midtvedt, Giovanni Volpe,1 and Carlo Manzo
 "Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic
 motion." arXiv 2202.06355 (2022). ```
 doi.org/10.1364/OPTICA.6.000506>: ``` Saga Helgadottir, Aykut Argun, and
 Giovanni Volpe. "Digital video microscopy enhanced by deep learning." Optica
 6.4 (2019): 506-513. ```
 github.com/softmatterlab/DeepTrack.git>: ``` Saga Helgadottir, Aykut Argun, and
 Giovanni Volpe. "DeepTrack." (2019) ``` ## Funding This work was supported by
```

### Comparing `deeptrack-1.5.5/deeptrack/__init__.py` & `deeptrack-1.5.6/deeptrack/__init__.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/aberrations.py` & `deeptrack-1.5.6/deeptrack/aberrations.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/augmentations.py` & `deeptrack-1.5.6/deeptrack/augmentations.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/_config.py` & `deeptrack-1.5.6/deeptrack/backend/_config.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/citations.py` & `deeptrack-1.5.6/deeptrack/backend/citations.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/core.py` & `deeptrack-1.5.6/deeptrack/backend/core.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/mie.py` & `deeptrack-1.5.6/deeptrack/backend/mie.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/pint_definition.py` & `deeptrack-1.5.6/deeptrack/backend/pint_definition.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/polynomials.py` & `deeptrack-1.5.6/deeptrack/backend/polynomials.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/tensorflow_bindings.py` & `deeptrack-1.5.6/deeptrack/backend/tensorflow_bindings.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/backend/units.py` & `deeptrack-1.5.6/deeptrack/backend/units.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/detection_QuantumDots/detection_QuantomDuts_test.py` & `deeptrack-1.5.6/deeptrack/datasets/detection_QuantumDots/detection_QuantomDuts_test.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/detection_QuantumDots/detection_QuantumDots.py` & `deeptrack-1.5.6/deeptrack/datasets/detection_QuantumDots/detection_QuantumDots.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles.py` & `deeptrack-1.5.6/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles_test.py` & `deeptrack-1.5.6/deeptrack/datasets/detection_holography_nanoparticles/detection_holography_nanoparticles_test.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/detection_linking_hela/detection_linking_hela.py` & `deeptrack-1.5.6/deeptrack/datasets/detection_linking_hela/detection_linking_hela.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/dmdataset/dmdataset.py` & `deeptrack-1.5.6/deeptrack/datasets/dmdataset/dmdataset.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/endothelial_vs/endothelial_vs.py` & `deeptrack-1.5.6/deeptrack/datasets/endothelial_vs/endothelial_vs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """endothelial_vs dataset."""
 
 import tensorflow_datasets as tfds
 import numpy as np
+import tensorflow as tf
 
 _DESCRIPTION = """
 """
 
 _CITATION = """
 @article{korczak2022dynamic,
   title={Dynamic live/apoptotic cell assay using phase-contrast imaging and deep learning},
@@ -30,18 +31,18 @@
 
         return tfds.core.DatasetInfo(
             builder=self,
             description=_DESCRIPTION,
             features=tfds.features.FeaturesDict(
                 {
                     "image": tfds.features.Image(
-                        shape=(None, None, 1), dtype="uint16"
+                        shape=(None, None, 1), dtype=tf.uint16
                     ),
                     "label": tfds.features.Image(
-                        shape=(None, None, 1), dtype="uint16"
+                        shape=(None, None, 1), dtype=tf.uint16
                     ),
                 }
             ),
             supervised_keys=("image", "label"),
             homepage="https://dataset-homepage/",
             citation=_CITATION,
         )
```

### Comparing `deeptrack-1.5.5/deeptrack/datasets/regression_diffusion_landscape/regression_diffusion_landscape.py` & `deeptrack-1.5.6/deeptrack/datasets/regression_diffusion_landscape/regression_diffusion_landscape.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles.py` & `deeptrack-1.5.6/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles_test.py` & `deeptrack-1.5.6/deeptrack/datasets/regression_holography_nanoparticles/regression_holography_nanoparticles_test.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os.py` & `deeptrack-1.5.6/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os_test.py` & `deeptrack-1.5.6/deeptrack/datasets/segmentation_fluorescence_u2os/segmentation_fluorescence_u2os_test.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila.py` & `deeptrack-1.5.6/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila_test.py` & `deeptrack-1.5.6/deeptrack/datasets/segmentation_ssTEM_drosophila/segmentation_ssTEM_drosophila_test.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/elementwise.py` & `deeptrack-1.5.6/deeptrack/elementwise.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/extras/datasets.py` & `deeptrack-1.5.6/deeptrack/extras/datasets.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/extras/radialcenter.py` & `deeptrack-1.5.6/deeptrack/extras/radialcenter.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/features.py` & `deeptrack-1.5.6/deeptrack/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -1303,16 +1303,16 @@
         super()._process_properties(propertydict)
 
         if propertydict["key"] is None:
             propertydict["key"] = np.random.randint(len(self.collection))
 
         return propertydict
 
-    def get(self, image, key, **kwargs):
-        return self.collection[key](image)
+    def get(self, image, key, _ID=(), **kwargs):
+        return self.collection[key](image, _ID=_ID)
 
 
 class OneOfDict(Feature):
     """Resolves one feature from a dictionary.
 
     Default behaviour is to sample the values diction uniformly random. This can be
     controlled by the `key` argument, where the feature resolved is chosen as
@@ -1334,16 +1334,16 @@
         super()._process_properties(propertydict)
 
         if propertydict["key"] is None:
             propertydict["key"] = np.random.choice(list(self.collection.keys()))
 
         return propertydict
 
-    def get(self, image, key, **kwargs):
-        return self.collection[key](image)
+    def get(self, image, key, _ID=(), **kwargs):
+        return self.collection[key](image, _ID=_ID)
 
 
 # class Dataset(Feature):
 #     """Grabs data from a local set of data.
 
 #     The first argument should be an iterator, function or constant,
 #     which provides access to a single sample from a dataset. If it returns
@@ -2105,21 +2105,21 @@
         import scipy.spatial.distance
 
         return np.all(
             scipy.spatial.distance.cdist(positions_1, positions_2) > min_distance
         )
 
     def _resample_volume_position(self, volume):
-        """ Draws a new position for the volume. """
+        """Draws a new position for the volume."""
 
         for pdict in volume.properties:
             if "position" in pdict and "_position_sampler" in pdict:
                 new_position = pdict["_position_sampler"]()
                 if isinstance(new_position, Quantity):
                     new_position = new_position.to("pixel").magnitude
                 pdict["position"] = new_position
 
         return volume
 
 
 # Alias
-Dataset = TensorflowDataset
+Dataset = TensorflowDataset
```

### Comparing `deeptrack-1.5.5/deeptrack/generators.py` & `deeptrack-1.5.6/deeptrack/generators.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/holography.py` & `deeptrack-1.5.6/deeptrack/holography.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/image.py` & `deeptrack-1.5.6/deeptrack/image.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/losses.py` & `deeptrack-1.5.6/deeptrack/losses.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/math.py` & `deeptrack-1.5.6/deeptrack/math.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/convolutional.py` & `deeptrack-1.5.6/deeptrack/models/convolutional.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/dense.py` & `deeptrack-1.5.6/deeptrack/models/dense.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/embeddings.py` & `deeptrack-1.5.6/deeptrack/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gans/cgan.py` & `deeptrack-1.5.6/deeptrack/models/gans/cgan.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gans/gan.py` & `deeptrack-1.5.6/deeptrack/models/gans/gan.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gans/pcgan.py` & `deeptrack-1.5.6/deeptrack/models/gans/pcgan.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gnns/augmentations.py` & `deeptrack-1.5.6/deeptrack/models/gnns/augmentations.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gnns/generators.py` & `deeptrack-1.5.6/deeptrack/models/gnns/generators.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gnns/graphs.py` & `deeptrack-1.5.6/deeptrack/models/gnns/graphs.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gnns/layers.py` & `deeptrack-1.5.6/deeptrack/models/gnns/layers.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gnns/models.py` & `deeptrack-1.5.6/deeptrack/models/gnns/models.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/gnns/utils.py` & `deeptrack-1.5.6/deeptrack/models/gnns/utils.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/layers.py` & `deeptrack-1.5.6/deeptrack/models/layers.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/lodestar/equivariances.py` & `deeptrack-1.5.6/deeptrack/models/lodestar/equivariances.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/lodestar/generators.py` & `deeptrack-1.5.6/deeptrack/models/lodestar/generators.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/lodestar/models.py` & `deeptrack-1.5.6/deeptrack/models/lodestar/models.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/recurrent.py` & `deeptrack-1.5.6/deeptrack/models/recurrent.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/utils.py` & `deeptrack-1.5.6/deeptrack/models/utils.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/models/vaes/vae.py` & `deeptrack-1.5.6/deeptrack/models/vaes/vae.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/noises.py` & `deeptrack-1.5.6/deeptrack/noises.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/optics.py` & `deeptrack-1.5.6/deeptrack/optics.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/properties.py` & `deeptrack-1.5.6/deeptrack/properties.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/scatterers.py` & `deeptrack-1.5.6/deeptrack/scatterers.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/sequences.py` & `deeptrack-1.5.6/deeptrack/sequences.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/statistics.py` & `deeptrack-1.5.6/deeptrack/statistics.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_aberrations.py` & `deeptrack-1.5.6/deeptrack/test/test_aberrations.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_augmentations.py` & `deeptrack-1.5.6/deeptrack/test/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_elementwise.py` & `deeptrack-1.5.6/deeptrack/test/test_elementwise.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_features.py` & `deeptrack-1.5.6/deeptrack/test/test_features.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_generators.py` & `deeptrack-1.5.6/deeptrack/test/test_generators.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_image.py` & `deeptrack-1.5.6/deeptrack/test/test_image.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_layers.py` & `deeptrack-1.5.6/deeptrack/test/test_layers.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_losses.py` & `deeptrack-1.5.6/deeptrack/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_math.py` & `deeptrack-1.5.6/deeptrack/test/test_math.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_models.py` & `deeptrack-1.5.6/deeptrack/test/test_models.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_noises.py` & `deeptrack-1.5.6/deeptrack/test/test_noises.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_optics.py` & `deeptrack-1.5.6/deeptrack/test/test_optics.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_properties.py` & `deeptrack-1.5.6/deeptrack/test/test_properties.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_scatterers.py` & `deeptrack-1.5.6/deeptrack/test/test_scatterers.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_sequences.py` & `deeptrack-1.5.6/deeptrack/test/test_sequences.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_statistics.py` & `deeptrack-1.5.6/deeptrack/test/test_statistics.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/test/test_utils.py` & `deeptrack-1.5.6/deeptrack/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/utils.py` & `deeptrack-1.5.6/deeptrack/utils.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/visualization/callbacks.py` & `deeptrack-1.5.6/deeptrack/visualization/callbacks.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/visualization/colors.py` & `deeptrack-1.5.6/deeptrack/visualization/colors.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack/visualization/training.py` & `deeptrack-1.5.6/deeptrack/visualization/training.py`

 * *Files identical despite different names*

### Comparing `deeptrack-1.5.5/deeptrack.egg-info/PKG-INFO` & `deeptrack-1.5.6/deeptrack.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,191 +1,190 @@
 Metadata-Version: 2.1
 Name: deeptrack
-Version: 1.5.5
+Version: 1.5.6
 Summary: A deep learning oriented microscopy image simulation package
 Home-page: https://github.com/softmatterlab/DeepTrack-2.0/
 Author: Benjamin Midtvedt
 Author-email: benjamin.midtvedt@physics.gu.se
-License: UNKNOWN
-Description: <p align="center">
-          <img width="350" src=https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/logo.png?raw=true>
-        </p>
-        
-        <h3 align="center">A comprehensive deep learning framework for digital microscopy.</h3>
-        <p align="center">
-          <a href="/LICENSE" alt="licence"><img src="https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0"></a>
-          <a href="https://badge.fury.io/py/deeptrack"><img src="https://badge.fury.io/py/deeptrack.svg" alt="PyPI version"></a>
-          <a href="https://softmatterlab.github.io/DeepTrack2/deeptrack.html"><img src="https://img.shields.io/badge/docs-passing-green" alt="PyPI version"></a>
-          <a href="https://badge.fury.io/py/deeptrack"><img src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue" alt="Python version"></a>
-          <a href="https://doi.org/10.1063/5.0034891" alt="DOI">
-            <img src="https://img.shields.io/badge/DOI-10.1063%2F5.0034891-blue">
-          </a>
-        </p>
-        <p align="center">
-          <a href="#installation">Installation</a> â€¢
-          <a href="#using-deeptrack">Examples</a> â€¢
-          <a href="#learning-deeptrack-21">Basics</a> â€¢
-          <a href="#cite-us">Cite us</a> â€¢
-          <a href="/LICENSE">License</a> 
-        </p>
-        
-        
-        We provide tools to create physical simulations of optical systems, to generate and train neural network models, and to analyze experimental data.
-        
-        # Installation
-        
-        DeepTrack 2.1 requires at least python 3.6.
-        
-        To install DeepTrack 2.1, open a terminal or command prompt and run:
-        
-            pip install deeptrack
-            
-        If you have a very recent version of python, you may need to install numpy _before_ DeepTrack. This is a known issue with scikit-image.
-        
-        ### Updating to 2.1 from 2.0
-        
-        If you are already using DeepTrack 2.0 (pypi version 0.x.x), updating to DeepTrack 2.1 (pypi version 1.x.x) is painless. If you have followed deprecation warnings, no change to your code is needed. There are two breaking changes:
-        
-        - The deprecated operator `+` to chain features has been removed. It is now only possible using the `>>` operator.
-        - The deprecated operator `**` to duplicate a feature has been removed. It is now only possible using the `^` operator.
-        
-        If you notice any other changes in behavior, please report it to us in the issues tab.
-        
-        # Examples of applications using DeepTrack 
-        
-        DeepTrack is a general purpose deep learning framework for microscopy, meaning you can use it for any task you like. Here, we show some common applications!
-        
-        <br/>
-        <h3 align="left"> Single particle tracking </h3>
-        <p align="left">
-          <img width="300" src=/assets/SPT-ideal.gif?raw=true>
-          <img width="300" src=/assets/SPT-noisy.gif?raw=true>
-          <br/>
-          <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/2-single_particle_tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a CNN-based single particle tracker using simulated data </a>
-          <br/>
-          <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
-            <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
-          </a> 
-          <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/02.%20tracking_particles_of_various_shapes.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Unsupervised training of a single particle tracker using LodeSTAR </a> 
-          
-        </p>
-        <br/>
-        
-        <h3 align="left"> Multi-particle tracking </h3>
-        
-        <p align="left">
-          <img width="600" src=/assets/MPT-packed.gif?raw=true>
-          <br/>
-          <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
-            <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
-          </a> <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/03.track_BF-C2DL-HSC.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training LodeSTAR to detect multiple cells from a single image </a>
-          <br/>
-          <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/4-multi-molecule-tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a UNet-based multi-particle tracker using simulated data </a> 
-        </p>
-        <br/>
-        
-        <h3 align="left"> Particle tracing </h3>
-        
-        <p align="left">
-          <img width="600" src=/assets/Tracing.gif?raw=true>
-          <br/>
-          <a href="https://doi.org/10.48550/arXiv.2202.06355" alt="DOI magik">
-            <img src="https://img.shields.io/badge/DOI-10.48550%2FarXiv.2202.0635-blue">
-          </a>  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/develop/examples/MAGIK/cell_migration_analysis.ipynb"> <img     src="https://colab.research.google.com/assets/colab-badge.svg"> Training MAGIK to trace migrating cells </a>
-        </p>
-        
-        # Basics to learn DeepTrack 2.1
-        
-        Everybody learns in different ways! Depending on your preferences, and what you want to do with DeepTrack, you may want to check out one or more of these resources.
-        
-        ## Getting-started guides
-        
-        We have two separate series of notebooks which aims to teach you all you need to know to use DeepTrack to its fullest. The first is a set of six notebooks with a focus on the application.
-        
-        1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> deeptrack_introduction_tutorial </a>  gives an overview of how to use DeepTrack 2.1.
-        2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/tracking_particle_cnn_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track a point particle with a convolutional neural network (CNN).
-        3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorial/tracking_multiple_particles_unet_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track multiple particles using a U-net.
-        4. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/characterizing_aberrations_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> characterizing_aberrations_tutorial </a> demonstrates how to add and characterize aberrations of an optical device. 
-        5. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/distinguishing_particles_in_brightfield_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> distinguishing_particles_in_brightfield_tutorial </a> demonstrates how to use a U-net to track and distinguish particles of different sizes in brightfield microscopy. 
-        6. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/analyzing_video_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> analyzing_video_tutorial </a> demonstrates how to create videos and how to train a neural network to analyze them.
-        
-        
-        The second series focuses on individual topics, introducing them in a natural order. 
-        
-        1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Introducing how to create simulation pipelines and train models. </a>
-        2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/02.%20using_deeptrack_generators.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating data generators. </a> 
-        3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/03.%20customizing_deeptrack_models.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating how to customize models using layer-blocks. </a> 
-        
-        ## DeepTrack 2.1 in action
-        
-        Additionally, we have seven more case studies which are less documented, but gives additional insight in how to use DeepTrack with real datasets
-        
-        1. [MNIST](examples/paper-examples/1-MNIST.ipynb) classifies handwritted digits.
-        2. [single particle tracking](examples/paper-examples/2-single_particle_tracking.ipynb) tracks experimentally captured videos of a single particle. (Requires opencv-python compiled with ffmpeg to open and read a video.)
-        3. [single particle sizing](examples/paper-examples/3-particle_sizing.ipynb) extracts the radius and refractive index of particles.
-        4. [multi-particle tracking](examples/paper-examples/4-multi-molecule-tracking.ipynb) detects quantum dots in a low SNR image.
-        5. [3-dimensional tracking](examples/paper-examples/5-inline_holography_3d_tracking.ipynb) tracks particles in three dimensions.
-        6. [cell counting](examples/paper-examples/6-cell_counting.ipynb) counts the number of cells in fluorescence images.
-        7. [GAN image generation](examples/paper-examples/7-GAN_image_generation.ipynb) uses a GAN to create cell image from masks.
-        
-        ## Model-specific examples
-        
-        We also have examples that are specific for certain models. This includes 
-        - [*LodeSTAR*](examples/LodeSTAR) for label-free particle tracking.
-        - [*MAGIK*](deeptrack/models/gnns/) for graph-based particle linking and trace characterization.
-        
-        ## Documentation
-        The detailed documentation of DeepTrack 2.1 is available at the following link: https://softmatterlab.github.io/DeepTrack2/deeptrack.html
-        
-        ## Video Tutorials
-        
-        Videos are currently being updated to match with the current version of DeepTrack.
-        
-        ## Cite us!
-        If you use DeepTrack 2.1 in your project, please cite us here:
-        
-        ```
-        Benjamin Midtvedt, Saga Helgadottir, Aykut Argun, JesÃºs Pineda, Daniel Midtvedt, Giovanni Volpe.
-        "Quantitative Digital Microscopy with Deep Learning."
-        Applied Physics Reviews 8 (2021), 011310.
-        https://doi.org/10.1063/5.0034891
-        ```
-        
-        See also:
-        
-        <https://www.nature.com/articles/s41467-022-35004-y>:
-        ```
-        Midtvedt, B., Pineda, J., SkÃ¤rberg, F. et al. 
-        "Single-shot self-supervised object detection in microscopy." 
-        Nat Commun 13, 7492 (2022).
-        ```
-        
-        <https://arxiv.org/abs/2202.06355>:
-        ```
-        JesÃºs Pineda, Benjamin Midtvedt, Harshith Bachimanchi, Sergio NoÃ©, Daniel  Midtvedt, Giovanni Volpe,1 and  Carlo  Manzo
-        "Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic motion."
-        arXiv 2202.06355 (2022).
-        ```
-        
-        <https://doi.org/10.1364/OPTICA.6.000506>:
-        ```
-        Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
-        "Digital video microscopy enhanced by deep learning."
-        Optica 6.4 (2019): 506-513.
-        ```
-        
-        <https://github.com/softmatterlab/DeepTrack.git>:
-        ```
-        Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
-        "DeepTrack." (2019)
-        ```
-        
-        ## Funding
-        
-        This work was supported by the ERC Starting Grant ComplexSwimmers (Grant No. 677511), the ERC Starting Grant MAPEI (101001267), and the Knut and Alice Wallenberg Foundation.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img width="350" src=https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/logo.png?raw=true>
+</p>
+
+<h3 align="center">A comprehensive deep learning framework for digital microscopy.</h3>
+<p align="center">
+  <a href="/LICENSE" alt="licence"><img src="https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0"></a>
+  <a href="https://badge.fury.io/py/deeptrack"><img src="https://badge.fury.io/py/deeptrack.svg" alt="PyPI version"></a>
+  <a href="https://softmatterlab.github.io/DeepTrack2/deeptrack.html"><img src="https://img.shields.io/badge/docs-passing-green" alt="PyPI version"></a>
+  <a href="https://badge.fury.io/py/deeptrack"><img src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue" alt="Python version"></a>
+  <a href="https://doi.org/10.1063/5.0034891" alt="DOI">
+    <img src="https://img.shields.io/badge/DOI-10.1063%2F5.0034891-blue">
+  </a>
+</p>
+<p align="center">
+  <a href="#installation">Installation</a> â€¢
+  <a href="#using-deeptrack">Examples</a> â€¢
+  <a href="#learning-deeptrack-21">Basics</a> â€¢
+  <a href="#cite-us">Cite us</a> â€¢
+  <a href="/LICENSE">License</a> 
+</p>
+
+
+We provide tools to create physical simulations of optical systems, to generate and train neural network models, and to analyze experimental data.
+
+# Installation
+
+DeepTrack 2.1 requires at least python 3.6.
+
+To install DeepTrack 2.1, open a terminal or command prompt and run:
+
+    pip install deeptrack
+    
+If you have a very recent version of python, you may need to install numpy _before_ DeepTrack. This is a known issue with scikit-image.
+
+### Updating to 2.1 from 2.0
+
+If you are already using DeepTrack 2.0 (pypi version 0.x.x), updating to DeepTrack 2.1 (pypi version 1.x.x) is painless. If you have followed deprecation warnings, no change to your code is needed. There are two breaking changes:
+
+- The deprecated operator `+` to chain features has been removed. It is now only possible using the `>>` operator.
+- The deprecated operator `**` to duplicate a feature has been removed. It is now only possible using the `^` operator.
+
+If you notice any other changes in behavior, please report it to us in the issues tab.
+
+# Examples of applications using DeepTrack 
+
+DeepTrack is a general purpose deep learning framework for microscopy, meaning you can use it for any task you like. Here, we show some common applications!
+
+<br/>
+<h3 align="left"> Single particle tracking </h3>
+<p align="left">
+  <img width="300" src=/assets/SPT-ideal.gif?raw=true>
+  <img width="300" src=/assets/SPT-noisy.gif?raw=true>
+  <br/>
+  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/2-single_particle_tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a CNN-based single particle tracker using simulated data </a>
+  <br/>
+  <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
+    <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
+  </a> 
+  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/02.%20tracking_particles_of_various_shapes.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Unsupervised training of a single particle tracker using LodeSTAR </a> 
+  
+</p>
+<br/>
+
+<h3 align="left"> Multi-particle tracking </h3>
+
+<p align="left">
+  <img width="600" src=/assets/MPT-packed.gif?raw=true>
+  <br/>
+  <a href="https://doi.org/10.1038/s41467-022-35004-y" alt="DOI lodestar">
+    <img src="https://img.shields.io/badge/DOI-10.1038%2Fs41467--022--35004--y-blue">
+  </a> <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/LodeSTAR/03.track_BF-C2DL-HSC.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training LodeSTAR to detect multiple cells from a single image </a>
+  <br/>
+  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/paper-examples/4-multi-molecule-tracking.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Training a UNet-based multi-particle tracker using simulated data </a> 
+</p>
+<br/>
+
+<h3 align="left"> Particle tracing </h3>
+
+<p align="left">
+  <img width="600" src=/assets/Tracing.gif?raw=true>
+  <br/>
+  <a href="https://doi.org/10.48550/arXiv.2202.06355" alt="DOI magik">
+    <img src="https://img.shields.io/badge/DOI-10.48550%2FarXiv.2202.0635-blue">
+  </a>  <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/develop/examples/MAGIK/cell_migration_analysis.ipynb"> <img     src="https://colab.research.google.com/assets/colab-badge.svg"> Training MAGIK to trace migrating cells </a>
+</p>
+
+# Basics to learn DeepTrack 2.1
+
+Everybody learns in different ways! Depending on your preferences, and what you want to do with DeepTrack, you may want to check out one or more of these resources.
+
+## Getting-started guides
+
+We have two separate series of notebooks which aims to teach you all you need to know to use DeepTrack to its fullest. The first is a set of six notebooks with a focus on the application.
+
+1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> deeptrack_introduction_tutorial </a>  gives an overview of how to use DeepTrack 2.1.
+2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/tracking_particle_cnn_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track a point particle with a convolutional neural network (CNN).
+3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorial/tracking_multiple_particles_unet_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> tracking_particle_cnn_tutorial </a> demonstrates how to track multiple particles using a U-net.
+4. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/characterizing_aberrations_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> characterizing_aberrations_tutorial </a> demonstrates how to add and characterize aberrations of an optical device. 
+5. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/distinguishing_particles_in_brightfield_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> distinguishing_particles_in_brightfield_tutorial </a> demonstrates how to use a U-net to track and distinguish particles of different sizes in brightfield microscopy. 
+6. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/tutorials/analyzing_video_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> analyzing_video_tutorial </a> demonstrates how to create videos and how to train a neural network to analyze them.
+
+
+The second series focuses on individual topics, introducing them in a natural order. 
+
+1. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/01.%20deeptrack_introduction_tutorial.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Introducing how to create simulation pipelines and train models. </a>
+2. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/02.%20using_deeptrack_generators.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating data generators. </a> 
+3. <a href="https://colab.research.google.com/github/softmatterlab/DeepTrack-2.0/blob/master/examples/get-started/03.%20customizing_deeptrack_models.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> Demonstrating how to customize models using layer-blocks. </a> 
+
+## DeepTrack 2.1 in action
+
+Additionally, we have seven more case studies which are less documented, but gives additional insight in how to use DeepTrack with real datasets
+
+1. [MNIST](examples/paper-examples/1-MNIST.ipynb) classifies handwritted digits.
+2. [single particle tracking](examples/paper-examples/2-single_particle_tracking.ipynb) tracks experimentally captured videos of a single particle. (Requires opencv-python compiled with ffmpeg to open and read a video.)
+3. [single particle sizing](examples/paper-examples/3-particle_sizing.ipynb) extracts the radius and refractive index of particles.
+4. [multi-particle tracking](examples/paper-examples/4-multi-molecule-tracking.ipynb) detects quantum dots in a low SNR image.
+5. [3-dimensional tracking](examples/paper-examples/5-inline_holography_3d_tracking.ipynb) tracks particles in three dimensions.
+6. [cell counting](examples/paper-examples/6-cell_counting.ipynb) counts the number of cells in fluorescence images.
+7. [GAN image generation](examples/paper-examples/7-GAN_image_generation.ipynb) uses a GAN to create cell image from masks.
+
+## Model-specific examples
+
+We also have examples that are specific for certain models. This includes 
+- [*LodeSTAR*](examples/LodeSTAR) for label-free particle tracking.
+- [*MAGIK*](deeptrack/models/gnns/) for graph-based particle linking and trace characterization.
+
+## Documentation
+The detailed documentation of DeepTrack 2.1 is available at the following link: https://softmatterlab.github.io/DeepTrack2/deeptrack.html
+
+## Video Tutorials
+
+Videos are currently being updated to match with the current version of DeepTrack.
+
+## Cite us!
+If you use DeepTrack 2.1 in your project, please cite us here:
+
+```
+Benjamin Midtvedt, Saga Helgadottir, Aykut Argun, JesÃºs Pineda, Daniel Midtvedt, Giovanni Volpe.
+"Quantitative Digital Microscopy with Deep Learning."
+Applied Physics Reviews 8 (2021), 011310.
+https://doi.org/10.1063/5.0034891
+```
+
+See also:
+
+<https://www.nature.com/articles/s41467-022-35004-y>:
+```
+Midtvedt, B., Pineda, J., SkÃ¤rberg, F. et al. 
+"Single-shot self-supervised object detection in microscopy." 
+Nat Commun 13, 7492 (2022).
+```
+
+<https://arxiv.org/abs/2202.06355>:
+```
+JesÃºs Pineda, Benjamin Midtvedt, Harshith Bachimanchi, Sergio NoÃ©, Daniel  Midtvedt, Giovanni Volpe,1 and  Carlo  Manzo
+"Geometric deep learning reveals the spatiotemporal fingerprint ofmicroscopic motion."
+arXiv 2202.06355 (2022).
+```
+
+<https://doi.org/10.1364/OPTICA.6.000506>:
+```
+Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
+"Digital video microscopy enhanced by deep learning."
+Optica 6.4 (2019): 506-513.
+```
+
+<https://github.com/softmatterlab/DeepTrack.git>:
+```
+Saga Helgadottir, Aykut Argun, and Giovanni Volpe.
+"DeepTrack." (2019)
+```
+
+## Funding
+
+This work was supported by the ERC Starting Grant ComplexSwimmers (Grant No. 677511), the ERC Starting Grant MAPEI (101001267), and the Knut and Alice Wallenberg Foundation.
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
-Metadata-Version: 2.1 Name: deeptrack Version: 1.5.5 Summary: A deep learning
+Metadata-Version: 2.1 Name: deeptrack Version: 1.5.6 Summary: A deep learning
 oriented microscopy image simulation package Home-page: https://github.com/
 softmatterlab/DeepTrack-2.0/ Author: Benjamin Midtvedt Author-email:
-benjamin.midtvedt@physics.gu.se License: UNKNOWN Description:
+benjamin.midtvedt@physics.gu.se Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
        [https://github.com/softmatterlab/DeepTrack2/blob/develop/assets/
                               logo.png?raw=true]
    **** A comprehensive deep learning framework for digital microscopy. ****
    [https://img.shields.io/github/license/softmatterlab/DeepTrack-2.0] [PyPI
   version] [PyPI_version] [Python_version] [https://img.shields.io/badge/DOI-
                            10.1063%2F5.0034891-blue]
  Installation Ã¢â¬Â¢ Examples Ã¢â¬Â¢ Basics Ã¢â¬Â¢ Cite_us Ã¢â¬Â¢ License
@@ -107,10 +110,7 @@
 doi.org/10.1364/OPTICA.6.000506>: ``` Saga Helgadottir, Aykut Argun, and
 Giovanni Volpe. "Digital video microscopy enhanced by deep learning." Optica
 6.4 (2019): 506-513. ```
 github.com/softmatterlab/DeepTrack.git>: ``` Saga Helgadottir, Aykut Argun, and
 Giovanni Volpe. "DeepTrack." (2019) ``` ## Funding This work was supported by
 the ERC Starting Grant ComplexSwimmers (Grant No. 677511), the ERC Starting
 Grant MAPEI (101001267), and the Knut and Alice Wallenberg Foundation.
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `deeptrack-1.5.5/deeptrack.egg-info/SOURCES.txt` & `deeptrack-1.5.6/deeptrack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 deeptrack/__init__.py
 deeptrack/aberrations.py
 deeptrack/augmentations.py
 deeptrack/elementwise.py
```

### Comparing `deeptrack-1.5.5/setup.py` & `deeptrack-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     or pkg_resources.working_set.by_key["tensorflow"].version[0] == "2"
 ):
     required.append("tensorflow_addons")
 
 
 setuptools.setup(
     name="deeptrack",  # Replace with your own username
-    version="1.5.5",
+    version="1.5.6",
     author="Benjamin Midtvedt",
     author_email="benjamin.midtvedt@physics.gu.se",
     description="A deep learning oriented microscopy image simulation package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/softmatterlab/DeepTrack-2.0/",
     install_requires=required,
```

