# Comparing `tmp/GANDLF-0.0.16.dev20230412.tar.gz` & `tmp/GANDLF-0.0.16.dev20230413.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.16.dev20230412.tar", last modified: Wed Apr 12 03:13:07 2023, max compression
+gzip compressed data, was "GANDLF-0.0.16.dev20230413.tar", last modified: Thu Apr 13 03:12:45 2023, max compression
```

## Comparing `GANDLF-0.0.16.dev20230412.tar` & `GANDLF-0.0.16.dev20230413.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.212634 GANDLF-0.0.16.dev20230412/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.164633 GANDLF-0.0.16.dev20230412/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.168633 GANDLF-0.0.16.dev20230412/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.168633 GANDLF-0.0.16.dev20230412/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.172633 GANDLF-0.0.16.dev20230412/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.172633 GANDLF-0.0.16.dev20230412/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.176633 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.176633 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.176633 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.180633 GANDLF-0.0.16.dev20230412/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.180633 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.184633 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.184633 GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.188633 GANDLF-0.0.16.dev20230412/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.188633 GANDLF-0.0.16.dev20230412/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.196633 GANDLF-0.0.16.dev20230412/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.204634 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/in_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.204634 GANDLF-0.0.16.dev20230412/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30573 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.208634 GANDLF-0.0.16.dev20230412/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.212634 GANDLF-0.0.16.dev20230412/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 03:12:59.000000 GANDLF-0.0.16.dev20230412/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:13:07.168633 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-12 03:13:07.000000 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-12 03:13:07.000000 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:13:07.000000 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:10:36.000000 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 03:13:07.000000 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 03:13:07.000000 GANDLF-0.0.16.dev20230412/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-12 03:13:07.212634 GANDLF-0.0.16.dev20230412/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 03:13:07.212634 GANDLF-0.0.16.dev20230412/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-12 03:10:27.000000 GANDLF-0.0.16.dev20230412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.852585 GANDLF-0.0.16.dev20230413/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.804584 GANDLF-0.0.16.dev20230413/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.808584 GANDLF-0.0.16.dev20230413/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.808584 GANDLF-0.0.16.dev20230413/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.812584 GANDLF-0.0.16.dev20230413/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.812584 GANDLF-0.0.16.dev20230413/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.816584 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.816584 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.816584 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.820584 GANDLF-0.0.16.dev20230413/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.820584 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.824584 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.824584 GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.824584 GANDLF-0.0.16.dev20230413/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.828584 GANDLF-0.0.16.dev20230413/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.836584 GANDLF-0.0.16.dev20230413/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.848585 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.848585 GANDLF-0.0.16.dev20230413/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30573 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.848585 GANDLF-0.0.16.dev20230413/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.852585 GANDLF-0.0.16.dev20230413/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 03:12:38.000000 GANDLF-0.0.16.dev20230413/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:12:45.808584 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-13 03:12:45.000000 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-13 03:12:45.000000 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:12:45.000000 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:10:22.000000 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 03:12:45.000000 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 03:12:45.000000 GANDLF-0.0.16.dev20230413/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-13 03:12:45.852585 GANDLF-0.0.16.dev20230413/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 03:12:45.852585 GANDLF-0.0.16.dev20230413/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-13 03:10:13.000000 GANDLF-0.0.16.dev20230413/setup.py
```

### Comparing `GANDLF-0.0.16.dev20230412/CODE_OF_CONDUCT.md` & `GANDLF-0.0.16.dev20230413/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/CONTRIBUTING.md` & `GANDLF-0.0.16.dev20230413/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.16.dev20230413/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/config_generator.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/deploy.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/main_run.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/main_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os, pickle
 from pathlib import Path
 
 from GANDLF.training_manager import TrainingManager, TrainingManager_split
 from GANDLF.inference_manager import InferenceManager
 from GANDLF.parseConfig import parseConfig
-from GANDLF.utils import populate_header_in_parameters, parseTrainingCSV, parseTestingCSV
+from GANDLF.utils import (
+    populate_header_in_parameters,
+    parseTrainingCSV,
+    parseTestingCSV,
+)
+
 
 def main_run(
     data_csv, config_file, model_dir, train_mode, device, resume, reset, output_dir=None
 ):
     """
     Main function that runs the training and inference.
 
@@ -30,15 +35,15 @@
     device = device
     parameters = parseConfig(model_parameters)
     parameters["device_id"] = -1
     # in case the data being passed is already processed, check if the previous parameters exists,
     # and if it does, compare the two and if they are the same, ensure no preprocess is done.
     model_parameters_prev = os.path.join(os.path.dirname(model_dir), "parameters.pkl")
     if train_mode:
-        if not (reset) or not (resume):
+        if resume:
             print(
                 "Trying to resume training without changing any parameters from previous run.",
                 flush=True,
             )
             if os.path.exists(model_parameters_prev):
                 parameters_prev = pickle.load(open(model_parameters_prev, "rb"))
                 assert (
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/cli/recover_config.py` & `GANDLF-0.0.16.dev20230413/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.16.dev20230413/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/compute/generic.py` & `GANDLF-0.0.16.dev20230413/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.16.dev20230413/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.16.dev20230413/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/compute/step.py` & `GANDLF-0.0.16.dev20230413/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/compute/training_loop.py` & `GANDLF-0.0.16.dev20230413/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.16.dev20230413/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.16.dev20230413/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/inference_manager.py` & `GANDLF-0.0.16.dev20230413/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/logger.py` & `GANDLF-0.0.16.dev20230413/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/losses/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/losses/hybrid.py` & `GANDLF-0.0.16.dev20230413/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/losses/regression.py` & `GANDLF-0.0.16.dev20230413/GANDLF/losses/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     if len(target.shape) > 1 and target.shape[-1] == 1:
         target = torch.squeeze(target, -1)
 
     weights = None
     if params.get("weights") is not None:
         # Check that the number of classes matches the number of weights
         num_classes = len(params["weights"])
-        assert prediction.shape[-1] == num_classes, f"Number of classes {num_classes} does not match prediction shape {prediction.shape[-1]}"
+        assert (
+            prediction.shape[-1] == num_classes
+        ), f"Number of classes {num_classes} does not match prediction shape {prediction.shape[-1]}"
 
         weights = torch.FloatTensor(list(params["weights"].values()))
         weights = weights.float().to(target.device)
 
     cel = CrossEntropyLoss(weight=weights)
     return cel(prediction, target)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/losses/segmentation.py` & `GANDLF-0.0.16.dev20230413/GANDLF/losses/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,24 +57,21 @@
     Tensor
         Mean Class Dice score
     """
 
     acc_dice = 0
 
     for i in range(num_class):  # 0 is background
-
         currentDice = dice(predicted[:, i, ...], target[:, i, ...])
 
         if loss_type == 1:
             currentDice = 1 - currentDice  # subtract from 1 because this is a loss
         elif loss_type == 2:
             # negative because we want positive losses
-            currentDice = -torch.log(
-                currentDice + torch.finfo(torch.float32).eps
-            )
+            currentDice = -torch.log(currentDice + torch.finfo(torch.float32).eps)
 
         if weights is not None:
             currentDice = currentDice * weights[i]  # multiply by weight
 
         acc_dice += currentDice
 
     if weights is None:
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/metrics/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/metrics/classification.py` & `GANDLF-0.0.16.dev20230413/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/metrics/generic.py` & `GANDLF-0.0.16.dev20230413/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/metrics/regression.py` & `GANDLF-0.0.16.dev20230413/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.16.dev20230413/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Import the different model architectures and functions
 from .unet import unet, resunet
 from .light_unet import light_unet, light_resunet
 from .unet_multilayer import unet_multilayer, resunet_multilayer
 from .light_unet_multilayer import light_unet_multilayer, light_resunet_multilayer
 from .deep_unet import deep_unet, deep_resunet
 from .uinc import uinc
 from .fcn import fcn
@@ -31,73 +32,82 @@
 from .imagenet_unet import imagenet_unet_wrapper
 from .sdnet import SDNet
 from .MSDNet import MSDNet
 from .brain_age import brainage
 from .unetr import unetr
 from .transunet import transunet
 
-# defining dict for models - key is the string and the value is the transform object
+# Define a dictionary of model architectures and corresponding functions
 global_models_dict = {
+    # Types of unet
     "unet": unet,
     "unet_multilayer": unet_multilayer,
     "resunet": resunet,
     "resunet_multilayer": resunet_multilayer,
-    "residualunet": resunet,
-    "residualunet_multilayer": resunet_multilayer,
+    "residualunet": resunet,  # Alias for "resunet"
+    "residualunet_multilayer": resunet_multilayer,  # Alias for "resunet_multilayer"
     "deepunet": deep_unet,
     "lightunet": light_unet,
     "lightunet_multilayer": light_unet_multilayer,
-    "deep_unet": deep_unet,
-    "light_unet": light_unet,
-    "light_unet_multilayer": light_unet_multilayer,
+    "deep_unet": deep_unet,  # Alias for "deepunet"
+    "light_unet": light_unet,  # Alias for "lightunet"
+    "light_unet_multilayer": light_unet_multilayer,  # Alias for "lightunet_multilayer"
     "deepresunet": deep_resunet,
     "lightresunet": light_resunet,
     "lightresunet_multilayer": light_resunet_multilayer,
-    "deep_resunet": deep_resunet,
-    "light_resunet": light_resunet,
-    "light_resunet_multilayer": light_resunet_multilayer,
+    "deep_resunet": deep_resunet,  # Alias for "deepresunet"
+    "light_resunet": light_resunet,  # Alias for "lightresunet"
+    "light_resunet_multilayer": light_resunet_multilayer,  # Alias for "lightresunet_multilayer"
     "unetr": unetr,
     "transunet": transunet,
-    "fcn": fcn,
     "uinc": uinc,
+    # UNet models with imagenet support from segmentation_models.pytorch
+    "imagenet_unet": imagenet_unet_wrapper,
+    # Additional segmentation model
+    "fcn": fcn,
+    # VGG models
     "vgg": vgg19,
     "vgg11": vgg11,
     "vgg13": vgg13,
     "vgg16": vgg16,
     "vgg19": vgg19,
+    # VGG models with imagenet support
     "imagenet_vgg11": imagenet_vgg11,
     "imagenet_vgg11_bn": imagenet_vgg11_bn,
     "imagenet_vgg13": imagenet_vgg13,
     "imagenet_vgg13_bn": imagenet_vgg13_bn,
     "imagenet_vgg16": imagenet_vgg16,
     "imagenet_vgg16_bn": imagenet_vgg16_bn,
     "imagenet_vgg19": imagenet_vgg19,
     "imagenet_vgg19_bn": imagenet_vgg19_bn,
-    "imagenet_unet": imagenet_unet_wrapper,
+    # DenseNet models
     "densenet": densenet264,
     "densenet121": densenet121,
     "densenet169": densenet169,
     "densenet201": densenet201,
     "densenet264": densenet264,
-    "msdnet": MSDNet,
-    "brain_age": brainage,
-    "sdnet": SDNet,
+    # ResNet models
     "resnet18": resnet18,
     "resnet34": resnet34,
     "resnet50": resnet50,
     "resnet101": resnet101,
     "resnet152": resnet152,
+    # EfficientNet models
     "efficientnetb0": efficientnetB0,
     "efficientnetb1": efficientnetB1,
     "efficientnetb2": efficientnetB2,
     "efficientnetb3": efficientnetB3,
     "efficientnetb4": efficientnetB4,
     "efficientnetb5": efficientnetB5,
     "efficientnetb6": efficientnetB6,
     "efficientnetb7": efficientnetB7,
+    # Custom models
+    "msdnet": MSDNet,
+    "brain_age": brainage,
+    "sdnet": SDNet,
 }
 
 
 def get_model(params):
     """
     Function to get the model definition.
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/deep_unet.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/unet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # -*- coding: utf-8 -*-
 """
 Implementation of UNet
 """
-
+from .modelBase import ModelBase
 from GANDLF.models.seg_modules.DownsamplingModule import DownsamplingModule
 from GANDLF.models.seg_modules.EncodingModule import EncodingModule
 from GANDLF.models.seg_modules.DecodingModule import DecodingModule
 from GANDLF.models.seg_modules.UpsamplingModule import UpsamplingModule
-from GANDLF.models.seg_modules.in_conv import in_conv
+from GANDLF.models.seg_modules.InitialConv import InitialConv
 from GANDLF.models.seg_modules.out_conv import out_conv
-from .modelBase import ModelBase
 from GANDLF.utils.generic import checkPatchDivisibility
 
 
-class deep_unet(ModelBase):
+class unet(ModelBase):
     """
     This is the standard U-Net architecture : https://arxiv.org/pdf/1606.06650.pdf. The 'residualConnections' flag controls residual connections, the
     Downsampling, Encoding, Decoding modules are defined in the seg_modules file. These smaller modules are basically defined by 2 parameters, the input
     channels (filters) and the output channels (filters), and some other hyperparameters, which remain constant all the modules. For more details on the
     smaller modules please have a look at the seg_modules file.
     """
 
     def __init__(
         self,
         parameters: dict,
         residualConnections=False,
     ):
         self.network_kwargs = {"res": residualConnections}
-        super(deep_unet, self).__init__(parameters)
+        super(unet, self).__init__(parameters)
 
         assert checkPatchDivisibility(parameters["patch_size"]) == True, (
             "The patch size is not divisible by 16, which is required for "
             + parameters["model"]["architecture"]
         )
 
-        self.ins = in_conv(
+        self.ins = InitialConv(
             input_channels=self.n_channels,
             output_channels=self.base_filters,
             conv=self.Conv,
             dropout=self.Dropout,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
         )
@@ -141,103 +140,98 @@
             input_channels=self.base_filters * 2,
             output_channels=self.base_filters,
             conv=self.Conv,
             interpolation_mode=self.linear_interpolation_mode,
         )
         self.de_0 = DecodingModule(
             input_channels=self.base_filters * 2,
-            output_channels=self.base_filters,
-            conv=self.Conv,
-            norm=self.Norm,
-            network_kwargs=self.network_kwargs,
-        )
-        self.out_3 = out_conv(
-            input_channels=self.base_filters * 8,
-            output_channels=self.n_classes,
-            conv=self.Conv,
-            norm=self.Norm,
-            network_kwargs=self.network_kwargs,
-            final_convolution_layer=self.final_convolution_layer,
-            sigmoid_input_multiplier=self.sigmoid_input_multiplier,
-        )
-        self.out_2 = out_conv(
-            input_channels=self.base_filters * 4,
-            output_channels=self.n_classes,
+            output_channels=self.base_filters * 2,
             conv=self.Conv,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
-            final_convolution_layer=self.final_convolution_layer,
-            sigmoid_input_multiplier=self.sigmoid_input_multiplier,
         )
-        self.out_1 = out_conv(
+        self.out = out_conv(
             input_channels=self.base_filters * 2,
             output_channels=self.n_classes,
             conv=self.Conv,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
             final_convolution_layer=self.final_convolution_layer,
             sigmoid_input_multiplier=self.sigmoid_input_multiplier,
         )
-        self.out_0 = out_conv(
-            input_channels=self.base_filters,
-            output_channels=self.n_classes,
-            conv=self.Conv,
-            norm=self.Norm,
-            network_kwargs=self.network_kwargs,
-            final_convolution_layer=self.final_convolution_layer,
-            sigmoid_input_multiplier=self.sigmoid_input_multiplier,
-        )
+
+        if "converter_type" in parameters["model"]:
+            self.ins = self.converter(self.ins).model
+            self.ds_0 = self.converter(self.ds_0).model
+            self.en_1 = self.converter(self.en_1).model
+            self.ds_1 = self.converter(self.ds_1).model
+            self.en_2 = self.converter(self.en_2).model
+            self.ds_2 = self.converter(self.ds_2).model
+            self.en_3 = self.converter(self.en_3).model
+            self.ds_3 = self.converter(self.ds_3).model
+            self.en_4 = self.converter(self.en_4).model
+            self.us_3 = self.converter(self.us_3).model
+            self.de_3 = self.converter(self.de_3).model
+            self.us_2 = self.converter(self.us_2).model
+            self.de_2 = self.converter(self.de_2).model
+            self.us_1 = self.converter(self.us_1).model
+            self.de_1 = self.converter(self.de_1).model
+            self.us_0 = self.converter(self.us_0).model
+            self.de_0 = self.converter(self.de_0).model
+            self.out = self.converter(self.out).model
 
     def forward(self, x):
         """
-        Parameters
-        ----------
-        x : Tensor
-            Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
-
-        Returns
-        -------
-        x : Tensor
-            Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
+        Forward pass of the UNet model.
+
+        Args:
+            x (Tensor): Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
+
+        Returns:
+            x (Tensor): Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
 
         """
+
+        # Encoding path
         x1 = self.ins(x)
+
+        # Apply Downsampling and encoding modules
         x2 = self.ds_0(x1)
         x2 = self.en_1(x2)
+
+        # Apply Downsampling and encoding modules
         x3 = self.ds_1(x2)
         x3 = self.en_2(x3)
+
+        # Apply Downsampling and encoding modules
         x4 = self.ds_2(x3)
         x4 = self.en_3(x4)
+
+        # Apply Downsampling and encoding modules
         x5 = self.ds_3(x4)
         x5 = self.en_4(x5)
 
+        # Decoding path
         x = self.us_3(x5)
-        xl4 = self.de_3(x, x4)
-        out_3 = self.out_3(xl4)
-
-        x = self.us_2(xl4)
-        xl3 = self.de_2(x, x3)
-        out_2 = self.out_2(xl3)
-
-        x = self.us_1(xl3)
-        xl2 = self.de_1(x, x2)
-        out_1 = self.out_1(xl2)
-
-        x = self.us_0(xl2)
-        xl1 = self.de_0(x, x1)
-        out_0 = self.out_0(xl1)
-
-        # Currently four outputs from the deep network
+        x = self.de_3(x, x4)
+        x = self.us_2(x)
+        x = self.de_2(x, x3)
+        x = self.us_1(x)
+        x = self.de_1(x, x2)
+        x = self.us_0(x)
+        x = self.de_0(x, x1)
+        x = self.out(x)
 
-        return [out_0, out_1, out_2, out_3]
+        # Return output tensors
+        return x
 
 
-class deep_resunet(deep_unet):
+class resunet(unet):
     """
     This is the standard U-Net architecture with residual connections : https://arxiv.org/pdf/1606.06650.pdf.
     The 'residualConnections' flag controls residual connections The Downsampling, Encoding, Decoding modules are defined in the seg_modules file.
     These smaller modules are basically defined by 2 parameters, the input channels (filters) and the output channels (filters),
     and some other hyperparameters, which remain constant all the modules. For more details on the smaller modules please have a look at the seg_modules file.
     """
 
     def __init__(self, parameters: dict):
-        super(deep_resunet, self).__init__(parameters, residualConnections=True)
+        super(resunet, self).__init__(parameters, residualConnections=True)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/efficientnet.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/efficientnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,32 @@
         stride,
         output_size,
         reduction,  # reduction factor for squeeze excitation
         Norm,
         Conv,
         Pool,
     ):
+        """
+        Defines a Single MBConv block in the EfficientNet model.
+
+        Args:
+            num_in_feats: Number of input features.
+            num_out_feats: Number of output features.
+            kernel_size: Size of the convolutional kernel.
+            stride: Stride of the convolutional layer.
+            output_size: Size of the output tensor.
+            reduction: Reduction factor for squeeze excitation.
+            Norm: Normalization layer for the MBConv block.
+            Conv: Convolutional layer for the MBConv block.
+            Pool: Pooling layer for the squeeze excitation block.
+
+        Returns:
+            Output tensor after passing through the MBConv block.
+
+        """
         super().__init__()
 
         # depthwise conv -> batch norm -> swish
         # SE
         # conv -> batch norm
 
         self.add_module(
@@ -58,14 +76,24 @@
                 bias=False,
             ),
         )
 
         self.add_module("norm2", Norm(num_out_feats))
 
     def forward(self, x):
+        """
+        Sequentially passes the input tensor through depthwise convolution -> batch normalization -> swish activation ->
+        squeeze excitation -> convolution -> batch normalization and returns the output tensor.
+
+        Args:
+            x (torch.Tensor): Input tensor for the MBConv block.
+
+        Returns:
+            out (torch.Tensor): Output tensor after passing through the MBConv block.
+        """
         out = self.depthconv1(x)
         out = self.norm1(out)
         out = self.silu(out)
 
         out = self.squeeze(out)
 
         out = self.conv2(out)
@@ -83,14 +111,28 @@
         stride,
         output_size,
         Norm,
         Conv,
         Pool,
         reduction,  # reduction factor for squeeze excitation
     ):
+        """
+        A class representing a single MobileNetV3 block with expansion factor 6. Refer to https://arxiv.org/abs/1905.02244 for more.
+
+        Args:
+            num_in_feats (int): The number of input features/channels.
+            num_out_feats (int): The number of output features/channels.
+            kernel_size (int): The size of the kernel/convolutional filter.
+            stride (int): The stride of the convolutional operation.
+            output_size (int): The output size of the block.
+            Norm (torch.nn.Module): A normalization layer to be used in the block.
+            Conv (torch.nn.Module): A convolutional layer to be used in the block.
+            Pool (torch.nn.Module): A pooling layer to be used in the squeeze-excitation block.
+            reduction (float): The reduction factor for the squeeze-excitation block.
+        """
         super().__init__()
 
         # conv -> batch norm --> swish
         # depthwise conv -> batch norm --> swish
         # SE
         # conv -> batch norm
 
@@ -138,14 +180,23 @@
                 bias=False,
             ),
         )
 
         self.add_module("norm3", Norm(num_out_feats))
 
     def forward(self, x):
+        """
+        Performs a forward pass through the model.
+
+        Args:
+            x (torch.Tensor): The input tensor to the model.
+
+        Returns:
+            torch.Tensor: The output tensor from the model.
+        """
         out = self.conv1(x)
         out = self.norm1(out)
         out = self.silu(out)
 
         out = self.depthconv1(out)
         out = self.norm2(out)
         out = self.silu(out)
@@ -162,14 +213,23 @@
     def __init__(
         self,
         num_in_feats,
         reduction,  # reduce dimension to int(num_in_feats / reduction)
         output_size,
         Pool,
     ):
+        """
+        Squeeze-and-Excitation block that recalibrates channel-wise feature responses
+
+        Args:
+            num_in_feats (int): Number of input features
+            reduction (int): Reduction factor for number of hidden features
+            output_size (tuple): Tuple containing the size of the output tensor
+            Pool (nn.Module): Pooling operation
+        """
         super().__init__()
 
         # global avg pool
         # FC --> ReLU
         # FC --> Sigmoid
 
         self.add_module("FC1", nn.Linear(num_in_feats, int(num_in_feats / reduction)))
@@ -177,14 +237,23 @@
 
         self.add_module("FC2", nn.Linear(int(num_in_feats / reduction), num_in_feats))
         self.add_module("sigmoid", nn.Sigmoid())
         self.Pool = Pool
         self.output_size = output_size
 
     def forward(self, x):
+        """
+        Forward pass for the Squeeze-and-Excitation block
+
+        Args:
+            x (torch.Tensor): Input tensor of shape [batch_size, in_channels, H, W]
+
+        Returns:
+            torch.Tensor: Output tensor of the same shape as the input tensor
+        """
         out = self.Pool(self.output_size)(x).view(x.size(0), -1)
         out = self.FC1(out)
         out = self.relu(out)
         out = self.FC2(out)
         out = self.sigmoid(out)
 
         dims = list(x.size())
@@ -242,63 +311,82 @@
         "num_layers": 1,
         "stride": 1,
     },
 ]
 
 
 def checkPatchDimensions(patch_size, numlay):
-    if isinstance(patch_size, int):
-        patch_size_to_check = np.array(patch_size)
-    else:
-        patch_size_to_check = patch_size
-    # for 2D, don't check divisibility of last dimension
+    """
+    Check if patch dimensions are divisible by 2^numlay.
+
+    Args:
+        patch_size (tuple or int): Tuple of integers or a single integer representing the patch size.
+        numlay (int): Number of layers.
+
+    Returns:
+        int: The largest number of layers that are divisible by 2^numlay.
+    """
+    patch_size_to_check = np.atleast_1d(patch_size)  # Convert to array if not already
     if patch_size_to_check[-1] == 1:
         patch_size_to_check = patch_size_to_check[:-1]
 
-    if all([x >= 2**numlay and x % 2**numlay == 0 for x in patch_size_to_check]):
+    if all(patch_size_to_check >= 2**numlay) and all(
+        patch_size_to_check % 2**numlay == 0
+    ):
         return numlay
     else:
         base2 = np.array(
-            [getBase2(x) for x in patch_size_to_check]
+            [np.log2(x).astype(int) for x in patch_size_to_check]
         )  # get largest possible number of layers for each dim
         return int(np.min(base2))
 
 
-def getBase2(num):
-    base = 0
-    while num % 2 == 0:
-        num = num / 2
-        base = base + 1
-    return base
+def num_channels(default_chan, width_factor, divisor):
+    """
+    Compute the number of channels closest to default_chan * width_factor that is divisible by divisor.
 
+    Args:
+        default_chan (int): Default number of channels.
+        width_factor (float): Width factor.
+        divisor (int): Divisor.
 
-def num_channels(default_chan, width_factor, divisor):
-    # find the number of channels closest to default * width such that it's divisible by divisor
+    Returns:
+        int: The number of channels closest to default_chan * width_factor that is divisible by divisor.
+    """
     default_chan *= width_factor
     new_out = int(default_chan + divisor / 2) // divisor * divisor
     new_out = max(new_out, divisor)
 
     if new_out < 0.9 * default_chan:
         new_out += divisor
 
     return int(new_out)
 
 
 def num_layers(default_lay, depth_factor):
-    # find the number of layers closest to default * depth
+    """
+    Compute the number of layers closest to default_lay * depth_factor.
+
+    Args:
+        default_lay (int): Default number of layers.
+        depth_factor (float): Depth factor.
+
+    Returns:
+        int: The number of layers closest to default_lay * depth_factor.
+    """
     return int(math.ceil(default_lay * depth_factor))
 
 
 class EfficientNet(ModelBase):
     """
-    Initializer function for the Resnet model
+    EfficientNet model with customizable scaling of depth and width.
 
     Args:
-        configuration (dict): A dictionary of configuration parameters for the model.
-        parameters (dict) - overall parameters dictionary
+        parameters (dict): A dictionary of configuration parameters for the model.
+        scale_params (dict) - A dictionary defining scaling of depth and width for the model.
     """
 
     def __init__(
         self,
         parameters: dict,
         scale_params,  # how to scale depth and width
     ):
@@ -404,20 +492,35 @@
                     m.weight.data.fill_(1)
                 if m.bias is not None:
                     m.bias.data.zero_()
             elif isinstance(m, nn.Linear):
                 nn.init.constant_(m.bias, 0)
 
     def forward(self, x):
+        """
+        Applies the model's layers to the input tensor and produces an output tensor.
+
+        Args:
+            x (torch.Tensor): Input tensor to the model.
+
+        Returns:
+            torch.Tensor: Output tensor produced by the model.
+        """
+        # Pass the input tensor through the feature extraction layers
         features = self.features(x)
+
+        # Apply adaptive average pooling to the output tensor from the previous step
         out = self.AdaptiveAvgPool(self.output_size)(features).view(
             features.size(0), -1
         )
+
+        # Pass the tensor through the classifier layers
         out = self.classifier(out)
 
+        # Apply the final convolution layer if not None
         if not self.final_convolution_layer is None:
             if self.final_convolution_layer == F.softmax:
                 out = self.final_convolution_layer(out, dim=1)
             else:
                 out = self.final_convolution_layer(out)
 
         return out
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/fcn.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/fcn.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import torch.nn.functional as F
 import torch
 from GANDLF.models.seg_modules.DownsamplingModule import DownsamplingModule
 from GANDLF.models.seg_modules.EncodingModule import EncodingModule
 from GANDLF.models.seg_modules.FCNUpsamplingModule import FCNUpsamplingModule
-from GANDLF.models.seg_modules.in_conv import in_conv
+from GANDLF.models.seg_modules.InitialConv import InitialConv
 from .modelBase import ModelBase
 
 
 class fcn(ModelBase):
     """
     This is the standard FCN (Fully Convolutional Network) architecture :
     https://arxiv.org/abs/1411.4038 . The Downsampling, Encoding, Decoding modules are defined in
@@ -24,15 +24,15 @@
     """
 
     def __init__(
         self,
         parameters: dict,
     ):
         super(fcn, self).__init__(parameters)
-        self.ins = in_conv(
+        self.ins = InitialConv(
             input_channels=self.n_channels,
             output_channels=self.base_filters,
             conv=self.Conv,
             dropout=self.Dropout,
             norm=self.Norm,
         )
         self.ds_0 = DownsamplingModule(
@@ -129,24 +129,19 @@
             stride=1,
             padding=0,
             bias=True,
         )
 
     def forward(self, x):
         """
-        Parameters
-        ----------
-        x : Tensor
-            Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
-
-        Returns
-        -------
-        x : Tensor
-            Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
+        Args:
+            x (Tensor): Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
 
+        Returns:
+            x (Tensor): Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
         """
         x1 = self.ins(x)
         x2 = self.ds_0(x1)
         x2 = self.en_1(x2)
         x3 = self.ds_1(x2)
         x3 = self.en_2(x3)
         x4 = self.ds_2(x3)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/imagenet_unet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,59 @@
 # -*- coding: utf-8 -*-
 # adapted from https://github.com/qubvel/segmentation_models.pytorch
 from typing import Optional, Union, List
 import torch
+import torch.nn as nn
 
 from segmentation_models_pytorch.base import (
     SegmentationHead,
     ClassificationHead,
 )
 from segmentation_models_pytorch.encoders import get_encoder
 from segmentation_models_pytorch.decoders.unet.decoder import UnetDecoder
 from segmentation_models_pytorch.base import initialization as init
 
 from .modelBase import ModelBase
 
 
 class SegmentationModel(torch.nn.Module):
     """
-    This has been adapted from its original implementation in
-    https://github.com/qubvel/segmentation_models.pytorch/blob/master/segmentation_models_pytorch/base/model.py
+    This class defines a segmentation model. It takes an input tensor and sequentially passes it through the model's
+    encoder, decoder and heads.
 
+    Methods:
+        initialize:
+            Initializes the model's classification or segmentation head
+
+        forward:
+            Sequentially passes the input tensor through the model's encoder, decoder, and heads and returns either the
+            segmentation masks or the class labels.
     """
 
     def initialize(self):
+        """
+        This function initializes the model's classification or segmentation head.
+        """
         if self.classification_head is None:
             init.initialize_decoder(self.decoder)
             init.initialize_head(self.segmentation_head)
         else:
             init.initialize_head(self.classification_head)
 
     def forward(self, x):
-        """Sequentially pass `x` trough model`s encoder, decoder and heads"""
+        """
+        This function sequentially passes the input tensor through the model's encoder, decoder, and heads and returns
+        either the segmentation masks or the class labels.
+
+        Args:
+            x (torch.Tensor): Input tensor
+
+        Returns:
+            torch.Tensor: Segmentation masks or class labels
+        """
         features = self.encoder(x)
 
         if self.classification_head is None:
             decoder_output = self.decoder(*features)
             masks = self.segmentation_head(decoder_output)
             return masks
         else:
@@ -60,53 +80,41 @@
     #     return x
 
 
 class Unet(SegmentationModel):
     """
     This has been adapted from its original implementation in
     https://github.com/qubvel/segmentation_models.pytorch/blob/master/segmentation_models_pytorch/decoders/unet/model.py
-
     Unet_ is a fully convolution neural network for image semantic segmentation. Consist of *encoder*
     and *decoder* parts connected with *skip connections*. Encoder extract features of different spatial
     resolution (skip connections) which are used by decoder to define accurate segmentation mask. Use *concatenation*
     for fusing decoder blocks with skip connections.
 
     Args:
-        encoder_name: Name of the classification model that will be used as an encoder (a.k.a backbone)
-            to extract features of different spatial resolution
-        encoder_depth: A number of stages used in encoder in range [3, 5]. Each stage generate features
-            two times smaller in spatial dimensions than previous one (e.g. for depth 0 we will have features
-            with shapes [(N, C, H, W),], for depth 1 - [(N, C, H, W), (N, C, H // 2, W // 2)] and so on).
-            Default is 5
-        encoder_weights: One of **None** (random initialization), **"imagenet"** (pre-training on ImageNet) and
-            other pretrained weights (see table with available weights for each encoder_name)
-        decoder_channels: List of integers which specify **in_channels** parameter for convolutions used in decoder.
-            Length of the list should be the same as **encoder_depth**
-        decoder_use_batchnorm: If **True**, BatchNorm2d layer between Conv2D and Activation layers
-            is used. If **"inplace"** InplaceABN will be used, allows to decrease memory consumption.
-            Available options are **True, False, "inplace"**
-        decoder_attention_type: Attention module used in decoder of the model. Available options are **None** and **scse**.
-            SCSE paper - https://arxiv.org/abs/1808.08127
-        in_channels: A number of input channels for the model, default is 3 (RGB images)
-        classes: A number of classes for output mask (or you can think as a number of channels of output mask)
-        activation: An activation function to apply after the final convolution layer.
-            Available options are **"sigmoid"**, **"softmax"**, **"logsoftmax"**, **"tanh"**, **"identity"**, **callable** and **None**.
-            Default is **None**
-        aux_params: Dictionary with parameters of the auxiliary output (classification head). Auxiliary output is build
-            on top of encoder if **aux_params** is not **None** (default). Supported params:
-                - classes (int): A number of classes
-                - pooling (str): One of "max", "avg". Default is "avg"
-                - dropout (float): Dropout factor in [0, 1)
-                - activation (str): An activation function to apply "sigmoid"/"softmax" (could be **None** to return logits)
+        encoder_name (str): Name of the classification model to be used as an encoder (a.k.a backbone) to extract features of different spatial resolution.
+        encoder_depth (int): A number of stages used in encoder in range [3, 5]. Each stage generates features two times smaller in spatial dimensions than the previous one. Default is 5.
+        encoder_weights (str or None): One of "None" (random initialization), "imagenet" (pre-training on ImageNet) and other pretrained weights (see table with available weights for each encoder_name).
+        decoder_channels (list of ints): List of integers specifying in_channels parameter for convolutions used in decoder. Length of the list should be the same as encoder_depth.
+        decoder_use_batchnorm (bool or str): If True, BatchNorm2d layer between Conv2D and Activation layers is used. If "inplace", InplaceABN will be used, allowing to decrease memory consumption. Available options are True, False, "inplace".
+        decoder_attention_type (str or None): Attention module used in the decoder of the model. Available options are None and "scse". SCSE paper - https://arxiv.org/abs/1808.08127.
+        in_channels (int): A number of input channels for the model. Default is 3 (RGB images).
+        classes (int): A number of classes for output mask (or you can think as a number of channels of output mask).
+        activation (str, callable, or None): An activation function to apply after the final convolution layer. Available options are "sigmoid", "softmax", "logsoftmax", "tanh", "identity", callable, and None. Default is None.
+        aux_params (dict or None): Dictionary with parameters of the auxiliary output (classification head). Auxiliary output is built on top of the encoder if aux_params is not None (default). Supported params:
+            - classes (int): A number of classes.
+            - pooling (str): One of "max", "avg". Default is "avg".
+            - dropout (float): Dropout factor in [0, 1).
+            - activation (str): An activation function to apply "sigmoid"/"softmax" (could be None to return logits).
 
     Returns:
-        ``torch.nn.Module``: Unet
+        model (torch.nn.Module): A UNet model for image semantic segmentation.
 
-    .. _Unet:
-        https://arxiv.org/abs/1505.04597
+    Reference:
+    Ronneberger, O., Fischer, P., & Brox, T. (2015). U-Net: Convolutional Networks for Biomedical Image Segmentation.
+    arXiv preprint arXiv:1505.04597.
 
     """
 
     def __init__(
         self,
         encoder_name: str = "resnet34",
         encoder_depth: int = 5,
@@ -117,24 +125,42 @@
         in_channels: int = 3,
         classes: int = 1,
         activation: Optional[Union[str, callable]] = None,
         aux_params: Optional[dict] = None,
     ):
         super().__init__()
 
+        def _get_fixed_encoder_channels(name, in_channels):
+            if "mit_" in name:
+                # MixVision Transformers only support 3-channel inputs
+                return 3
+            else:
+                return in_channels
+
         self.encoder = get_encoder(
             encoder_name,
-            in_channels=in_channels,
+            in_channels=_get_fixed_encoder_channels(encoder_name, in_channels),
             depth=encoder_depth,
             weights=encoder_weights,
         )
+        out_channels = self.encoder.out_channels
+        if "mit_" in encoder_name:
+            # MixVision Transformers only support 3-channel inputs
+            print(
+                "WARNING: MixVision Transformers only support 3 channels, adding an extra Conv layer for compatibility."
+            )
+            self.pre_encoder = nn.Conv2d(in_channels, 3, kernel_size=1, stride=1)
+            modules = []
+            modules.append(self.pre_encoder)
+            modules.append(self.encoder)
+            self.encoder = nn.Sequential(*modules)
 
         if aux_params is None:
             self.decoder = UnetDecoder(
-                encoder_channels=self.encoder.out_channels,
+                encoder_channels=out_channels,
                 decoder_channels=decoder_channels,
                 n_blocks=encoder_depth,
                 use_batchnorm=decoder_use_batchnorm,
                 center=True if encoder_name.startswith("vgg") else False,
                 attention_type=decoder_attention_type,
             )
             self.segmentation_head = SegmentationHead(
@@ -142,15 +168,15 @@
                 out_channels=classes,
                 activation=activation,
                 kernel_size=3,
             )
             self.classification_head = None
         else:
             self.classification_head = ClassificationHead(
-                in_channels=self.encoder.out_channels[-1], **aux_params
+                in_channels=out_channels[-1], **aux_params
             )
             self.segmentation_head = None
 
         self.name = "u-{}".format(encoder_name)
         self.initialize()
 
 
@@ -195,16 +221,22 @@
             )
             classifier_head_parameters["pooling"] = parameters["model"].get(
                 "pooling", "avg"
             )
         else:
             classifier_head_parameters = None
 
+        default_encoder_name = parameters["model"].get("encoder_name", "resnet34")
+        if "mit_" in default_encoder_name:
+            assert (
+                self.n_dimensions == 2
+            ), "MixVision Transformers only support 2D inputs"
+
         self.model = Unet(
-            encoder_name=parameters["model"].get("encoder_name", "resnet34"),
+            encoder_name=default_encoder_name,
             encoder_weights=parameters["model"]["encoder_weights"],
             in_channels=self.n_channels,
             classes=self.n_classes,
             activation=parameters["model"]["final_layer"],
             decoder_use_batchnorm=decoder_use_batchnorm,
             decoder_attention_type=parameters["model"].get(
                 "decoder_attention_type", None
@@ -216,12 +248,21 @@
             aux_params=classifier_head_parameters,
         )
 
         if self.n_dimensions == 3:
             self.model = self.converter(self.model).model
 
     def forward(self, x):
+        """
+        Forward pass of the model.
+
+        Args:
+            x (torch.Tensor): Input tensor.
+
+        Returns:
+            torch.Tensor: Output tensor.
+        """
         return self.model(x)
 
 
 def imagenet_unet_wrapper(parameters):
     return ImageNet_UNet(parameters)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/light_unet.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/light_unet.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Implementation of UNet
 """
 
 from GANDLF.models.seg_modules.DownsamplingModule import DownsamplingModule
 from GANDLF.models.seg_modules.EncodingModule import EncodingModule
 from GANDLF.models.seg_modules.DecodingModule import DecodingModule
 from GANDLF.models.seg_modules.UpsamplingModule import UpsamplingModule
-from GANDLF.models.seg_modules.in_conv import in_conv
+from GANDLF.models.seg_modules.InitialConv import InitialConv
 from GANDLF.models.seg_modules.out_conv import out_conv
 from .modelBase import ModelBase
 from GANDLF.utils.generic import checkPatchDivisibility
 
 
 class light_unet(ModelBase):
     """
@@ -29,15 +29,15 @@
         self.network_kwargs = {"res": False}
 
         assert checkPatchDivisibility(parameters["patch_size"]) == True, (
             "The patch size is not divisible by 16, which is required for "
             + parameters["model"]["architecture"]
         )
 
-        self.ins = in_conv(
+        self.ins = InitialConv(
             input_channels=self.n_channels,
             output_channels=self.base_filters,
             conv=self.Conv,
             dropout=self.Dropout,
             norm=self.Norm,
         )
         self.ds_0 = DownsamplingModule(
@@ -156,23 +156,19 @@
             norm=self.Norm,
             final_convolution_layer=self.final_convolution_layer,
             sigmoid_input_multiplier=self.sigmoid_input_multiplier,
         )
 
     def forward(self, x):
         """
-        Parameters
-        ----------
-        x : Tensor
-            Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
-
-        Returns
-        -------
-        x : Tensor
-            Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
+        Args:
+            x (torch.Tensor): A 5D tensor of shape [batch_size, channels, x_dims, y_dims, z_dims].
+
+        Returns:
+            torch.Tensor: A 5D tensor of shape [batch_size, n_classes, x_dims, y_dims, z_dims], representing the output of the model for image segmentation.
 
         """
         x1 = self.ins(x)
         x2 = self.ds_0(x1)
         x2 = self.en_1(x2)
         x3 = self.ds_1(x2)
         x3 = self.en_2(x3)
@@ -186,14 +182,15 @@
         x = self.us_2(x)
         x = self.de_2(x, x3)
         x = self.us_1(x)
         x = self.de_1(x, x2)
         x = self.us_0(x)
         x = self.de_0(x, x1)
         x = self.out(x)
+
         return x
 
 
 class light_resunet(light_unet):
     """
     This is the LIGHT U-Net architecture with residual connections.
     """
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/light_unet_multilayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from torch.nn import ModuleList
 
 from GANDLF.models.seg_modules.DownsamplingModule import DownsamplingModule
 from GANDLF.models.seg_modules.EncodingModule import EncodingModule
 from GANDLF.models.seg_modules.DecodingModule import DecodingModule
 from GANDLF.models.seg_modules.UpsamplingModule import UpsamplingModule
-from GANDLF.models.seg_modules.in_conv import in_conv
+from GANDLF.models.seg_modules.InitialConv import InitialConv
 from GANDLF.models.seg_modules.out_conv import out_conv
 from .modelBase import ModelBase
 
 
 class light_unet_multilayer(ModelBase):
     """
     This is the LIGHT U-Net architecture.
@@ -26,15 +26,15 @@
         self.network_kwargs = {"res": residualConnections}
         super(light_unet_multilayer, self).__init__(parameters)
 
         parameters["model"]["depth"] = parameters["model"].get("depth", 4)
 
         self.depth = self.model_depth_check(parameters)
 
-        self.ins = in_conv(
+        self.ins = InitialConv(
             input_channels=self.n_channels,
             output_channels=self.base_filters,
             conv=self.Conv,
             dropout=self.Dropout,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
         )
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/modelBase.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,48 @@
-import torch
 import torch.nn as nn
+import torch.nn.functional as F
 
 
-class DecodingModule(nn.Module):
+class IncUpsamplingModule(nn.Module):
     def __init__(
         self,
         input_channels,
         output_channels,
-        conv=nn.Conv2d,
-        conv_kwargs=None,
-        norm=nn.BatchNorm2d,
-        norm_kwargs=None,
-        act=nn.LeakyReLU,
-        act_kwargs=None,
-        network_kwargs=None,
+        ConvTranspose,
+        Dropout,
+        InstanceNorm,
+        dropout_p=0.3,
+        leakiness=1e-2,
+        conv_bias=True,
+        inst_norm_affine=True,
+        res=False,
+        lrelu_inplace=True,
     ):
         nn.Module.__init__(self)
-        if conv_kwargs is None:
-            conv_kwargs = {"kernel_size": 3, "stride": 1, "padding": 1, "bias": True}
-        if norm_kwargs is None:
-            norm_kwargs = {
-                "eps": 1e-5,
-                "affine": True,
-                "momentum": 0.1,
-                "track_running_stats": True,
-            }
-        if act_kwargs is None:
-            act_kwargs = {"negative_slope": 1e-2, "inplace": True}
-        if network_kwargs is None:
-            network_kwargs = {"res": False}
-
-        self.residual = network_kwargs["res"]
-
-        self.conv0 = conv(input_channels, output_channels, **conv_kwargs)
-        self.conv1 = conv(output_channels, output_channels, **conv_kwargs)
-        self.conv2 = conv(output_channels, output_channels, **conv_kwargs)
-
-        self.in_0 = norm(input_channels, **norm_kwargs)
-        self.in_1 = norm(output_channels, **norm_kwargs)
-        self.in_2 = norm(output_channels, **norm_kwargs)
-
-        self.act = act(**act_kwargs)
-
-    def forward(self, x1, x2):
-        x = torch.cat([x1, x2], dim=1)
-        x = self.conv0(self.act(self.in_0(x)))
-
-        if self.residual:
-            skip = x
-
-        x = self.conv1(self.act(self.in_1(x)))
-
-        x = self.conv2(self.act(self.in_2(x)))
-
-        if self.residual:
-            x = x + skip
-
+        self.input_channels = input_channels
+        self.output_channels = output_channels
+        self.dropout_p = dropout_p
+        self.leakiness = leakiness
+        self.conv_bias = conv_bias
+        self.inst_norm_affine = inst_norm_affine
+        self.residual = res
+        self.lrelu_inplace = lrelu_inplace
+        self.inst_norm = InstanceNorm(
+            output_channels, affine=self.inst_norm_affine, track_running_stats=True
+        )
+        self.up = ConvTranspose(
+            input_channels,
+            output_channels,
+            kernel_size=1,
+            stride=2,
+            padding=0,
+            output_padding=1,
+            bias=self.conv_bias,
+        )
+
+    def forward(self, x):
+        x = F.leaky_relu(
+            self.inst_norm(self.up(x)),
+            negative_slope=self.leakiness,
+            inplace=self.lrelu_inplace,
+        )
         return x
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/transunet.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/unet_multilayer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,176 @@
 # -*- coding: utf-8 -*-
 """
-Implementation of TransUNet
+Implementation of UNet
 """
+from torch.nn import ModuleList
 
 from GANDLF.models.seg_modules.DownsamplingModule import DownsamplingModule
 from GANDLF.models.seg_modules.EncodingModule import EncodingModule
-from GANDLF.models.seg_modules.in_conv import in_conv
+from GANDLF.models.seg_modules.DecodingModule import DecodingModule
+from GANDLF.models.seg_modules.UpsamplingModule import UpsamplingModule
+from GANDLF.models.seg_modules.InitialConv import InitialConv
 from GANDLF.models.seg_modules.out_conv import out_conv
 from .modelBase import ModelBase
-import torch
-import torch.nn as nn
-from torch.nn import ModuleList
-from .unetr import _Transformer
-
-
-class _DecoderCUP(nn.Sequential):
-    def __init__(self, in_feats, out_feats, Norm, Conv, Upsample):
-        super().__init__()
-
-        self.conv = Conv(
-            in_channels=in_feats,
-            out_channels=out_feats,
-            kernel_size=3,
-            stride=1,
-            padding=1,
-            bias=False,
-        )
-
-        self.norm = Norm(out_feats)
-        self.relu = nn.ReLU(inplace=True)
-        self.upsample = Upsample
-
-    def forward(self, x1, x2):
-        if x2 is not None:
-            x1 = torch.cat([x1, x2], dim=1)
-        x = self.conv(x1)
-        x = self.norm(x)
-        x = self.relu(x)
-        x = self.upsample(x)
-
-        return x
 
 
-class transunet(ModelBase):
+class unet_multilayer(ModelBase):
     """
-    This is the TransUNet architecture : https://doi.org/10.48550/arXiv.2102.04306. The 'residualConnections' flag controls residual connections, the
+    This is the standard U-Net architecture : https://arxiv.org/pdf/1606.06650.pdf. The 'residualConnections' flag controls residual connections, the
     Downsampling, Encoding, Decoding modules are defined in the seg_modules file. These smaller modules are basically defined by 2 parameters, the input
     channels (filters) and the output channels (filters), and some other hyperparameters, which remain constant all the modules. For more details on the
     smaller modules please have a look at the seg_modules file.
     """
 
     def __init__(
         self,
         parameters: dict,
+        residualConnections=False,
     ):
-        super(transunet, self).__init__(parameters)
+        """
+        Parameters
+        ----------
+        parameters (dict): A dictionary containing the model parameters.
+        residualConnections (bool, optional): A flag to control residual connections in the model, by default False.
+        """
 
-        # initialize defaults if not found
-        parameters["model"]["depth"] = parameters["model"].get("depth", 4)
-        parameters["model"]["num_heads"] = parameters["model"].get("num_heads", 12)
-        parameters["model"]["embed_dim"] = parameters["model"].get("embed_dim", 768)
+        self.network_kwargs = {"res": residualConnections}
+        super(unet_multilayer, self).__init__(parameters)
 
+        # Set the depth of the model based on the input parameters
+        # If the depth is not set, then set it to 4
+        parameters["model"]["depth"] = parameters["model"].get("depth", 4)
         self.depth = self.model_depth_check(parameters)
 
-        if self.n_dimensions == 2:
-            self.img_size = parameters["patch_size"][0:2]
-            self.upsample = nn.Upsample(
-                scale_factor=2, mode="bilinear", align_corners=True
-            )
-        elif self.n_dimensions == 3:
-            self.img_size = parameters["patch_size"]
-            self.upsample = nn.Upsample(
-                scale_factor=2, mode="trilinear", align_corners=True
-            )
-
-        self.num_layers = 3 * self.depth  # number of transformer layers
-        self.out_layers = [self.num_layers - 1]
-
-        self.num_heads = parameters["model"]["num_heads"]
-        self.embed_size = parameters["model"]["embed_dim"]
-
-        assert (
-            self.embed_size % self.num_heads == 0
-        ), "The embedding dimension must be divisible by the number of self-attention heads"
-
-        self.patch_dim = [i // 2 ** (self.depth) for i in self.img_size]
-
-        self.ins = in_conv(
+        # Create the initial convolution layer
+        self.ins = InitialConv(
             input_channels=self.n_channels,
             output_channels=self.base_filters,
             conv=self.Conv,
             dropout=self.Dropout,
             norm=self.Norm,
+            network_kwargs=self.network_kwargs,
         )
 
+        # Create lists of downsampling, encoding, decoding and upsampling modules
         self.ds = ModuleList([])
         self.en = ModuleList([])
+        self.us = ModuleList([])
         self.de = ModuleList([])
 
+        # Create the required number of downsampling, encoding, decoding and upsampling modules
         for i_lay in range(0, self.depth):
             self.ds.append(
                 DownsamplingModule(
                     input_channels=self.base_filters * 2 ** (i_lay),
                     output_channels=self.base_filters * 2 ** (i_lay + 1),
                     conv=self.Conv,
                     norm=self.Norm,
                 )
             )
 
+            self.us.append(
+                UpsamplingModule(
+                    input_channels=self.base_filters * 2 ** (i_lay + 1),
+                    output_channels=self.base_filters * 2 ** (i_lay),
+                    conv=self.Conv,
+                    interpolation_mode=self.linear_interpolation_mode,
+                )
+            )
+
             self.de.append(
-                _DecoderCUP(
-                    in_feats=2 * self.base_filters * 2 ** (i_lay + 1),
-                    out_feats=self.base_filters * 2 ** (i_lay),
-                    Conv=self.Conv,
-                    Norm=self.Norm,
-                    Upsample=self.upsample,
+                DecodingModule(
+                    input_channels=self.base_filters * 2 ** (i_lay + 1),
+                    output_channels=self.base_filters * 2 ** (i_lay),
+                    conv=self.Conv,
+                    norm=self.Norm,
+                    network_kwargs=self.network_kwargs,
                 )
             )
 
             self.en.append(
                 EncodingModule(
                     input_channels=self.base_filters * 2 ** (i_lay + 1),
                     output_channels=self.base_filters * 2 ** (i_lay + 1),
                     conv=self.Conv,
                     dropout=self.Dropout,
                     norm=self.Norm,
+                    network_kwargs=self.network_kwargs,
                 )
             )
 
-        self.transformer = _Transformer(
-            img_size=[i // 2 ** (self.depth) for i in self.img_size],
-            patch_size=1,
-            in_feats=self.base_filters * 2**self.depth,
-            embed_size=self.embed_size,
-            num_heads=self.num_heads,
-            mlp_dim=2048,
-            num_layers=self.num_layers,
-            out_layers=self.out_layers,
-            Conv=self.Conv,
-            Norm=self.Norm,
-        )
-
-        self.transCUP = _DecoderCUP(
-            in_feats=self.embed_size,
-            out_feats=self.base_filters * 2 ** (self.depth - 1),
-            Conv=self.Conv,
-            Norm=self.Norm,
-            Upsample=self.upsample,
-        )
-
-        # TODO: conv 3x3 --> ReLU --> outconv
+        # Create the final convolution layer
         self.out = out_conv(
             input_channels=self.base_filters,
             output_channels=self.n_classes,
             conv=self.Conv,
             norm=self.Norm,
+            network_kwargs=self.network_kwargs,
             final_convolution_layer=self.final_convolution_layer,
             sigmoid_input_multiplier=self.sigmoid_input_multiplier,
         )
 
+        # Check if converter_type is passed in model, generally referring to ACS
+        if "converter_type" in parameters["model"]:
+            self.ins = self.converter(self.ins).model
+            self.out = self.converter(self.out).model
+            for i_lay in range(0, self.depth):
+                self.ds[i_lay] = self.converter(self.ds[i_lay]).model
+                self.us[i_lay] = self.converter(self.us[i_lay]).model
+                self.de[i_lay] = self.converter(self.de[i_lay]).model
+                self.en[i_lay] = self.converter(self.en[i_lay]).model
+
     def forward(self, x):
         """
-        Parameters
-        ----------
-        x : Tensor
-            Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
+        Forward pass of the UNet model.
+
+        Args:
+            x (Tensor): Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
 
-        Returns
-        -------
-        x : Tensor
-            Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
+        Returns:
+            x (Tensor): Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
 
         """
+        # Store intermediate feature maps
+
         y = []
         y.append(self.ins(x))
 
         # [downsample --> encode] x num layers
         for i in range(0, self.depth):
             temp = self.ds[i](y[i])
             y.append(self.en[i](temp))
 
-        x = self.transformer(y[-1])[-1]
-        x = x.transpose(-1, -2).view(-1, self.embed_size, *self.patch_dim)
-        x = self.transCUP(x, None)
+        # Get the feature map at the last (deepest) layer
+        x = y[-1]
 
         # [upsample --> encode] x num layers
-        for i in range(self.depth - 1, 0, -1):
-            x = self.de[i - 1](x, y[i])
+        for i in range(self.depth - 1, -1, -1):
+            # Upsample the feature map to match the size of the corresponding feature map in the encoder
+            x = self.us[i](x)
+
+            # Concatenate with the corresponding feature map from the encoder
+            x = self.de[i](x, y[i])
 
+        # Get the final output
         x = self.out(x)
+
         return x
+
+
+class resunet_multilayer(unet_multilayer):
+    """
+    This is the standard U-Net architecture with residual connections : https://arxiv.org/pdf/1606.06650.pdf.
+    The 'residualConnections' flag controls residual connections, the
+    Downsampling, Encoding, Decoding modules are defined in the seg_modules file. These smaller modules are basically defined by 2 parameters, the input
+    channels (filters) and the output channels (filters), and some other hyperparameters, which remain constant all the modules. For more details on the
+    smaller modules please have a look at the seg_modules file.
+    """
+
+    def __init__(self, parameters: dict):
+        """
+        Parameters
+        ----------
+        parameters (dict): A dictionary containing the model parameters.
+
+        """
+        super(resunet_multilayer, self).__init__(parameters, residualConnections=True)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/uinc.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/uinc.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,23 +207,19 @@
             self.Dropout,
             self.InstanceNorm,
         )
 
     def forward(self, x):
         """
 
-        Parameters
-        ----------
-        x : TYPE
-            DESCRIPTION.
+        Args:
+            x (torch.Tensor): Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
 
-        Returns
-        -------
-        x6 : TYPE
-            DESCRIPTION.
+        Returns:
+            x6 (torch.Tensor): Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
 
         """
         x = self.conv0_1x1(x)
         x1 = self.rn_0(x)
         x2 = self.ri_0(x1)
         x3 = self.ds_0(x2)
         x3 = self.ri_1(x3)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/models/unet.py` & `GANDLF-0.0.16.dev20230413/GANDLF/models/deep_unet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # -*- coding: utf-8 -*-
 """
-Implementation of UNet
+Implementation of UNet with deep supervision and residual connections
 """
-from .modelBase import ModelBase
+
 from GANDLF.models.seg_modules.DownsamplingModule import DownsamplingModule
 from GANDLF.models.seg_modules.EncodingModule import EncodingModule
 from GANDLF.models.seg_modules.DecodingModule import DecodingModule
 from GANDLF.models.seg_modules.UpsamplingModule import UpsamplingModule
-from GANDLF.models.seg_modules.in_conv import in_conv
+from GANDLF.models.seg_modules.InitialConv import InitialConv
 from GANDLF.models.seg_modules.out_conv import out_conv
+from .modelBase import ModelBase
 from GANDLF.utils.generic import checkPatchDivisibility
 
 
-class unet(ModelBase):
+class deep_unet(ModelBase):
     """
     This is the standard U-Net architecture : https://arxiv.org/pdf/1606.06650.pdf. The 'residualConnections' flag controls residual connections, the
     Downsampling, Encoding, Decoding modules are defined in the seg_modules file. These smaller modules are basically defined by 2 parameters, the input
     channels (filters) and the output channels (filters), and some other hyperparameters, which remain constant all the modules. For more details on the
     smaller modules please have a look at the seg_modules file.
     """
 
     def __init__(
         self,
         parameters: dict,
         residualConnections=False,
     ):
         self.network_kwargs = {"res": residualConnections}
-        super(unet, self).__init__(parameters)
+        super(deep_unet, self).__init__(parameters)
 
         assert checkPatchDivisibility(parameters["patch_size"]) == True, (
             "The patch size is not divisible by 16, which is required for "
             + parameters["model"]["architecture"]
         )
 
-        self.ins = in_conv(
+        # Define layers of the UNet model
+        self.ins = InitialConv(
             input_channels=self.n_channels,
             output_channels=self.base_filters,
             conv=self.Conv,
             dropout=self.Dropout,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
         )
@@ -140,87 +142,114 @@
             input_channels=self.base_filters * 2,
             output_channels=self.base_filters,
             conv=self.Conv,
             interpolation_mode=self.linear_interpolation_mode,
         )
         self.de_0 = DecodingModule(
             input_channels=self.base_filters * 2,
-            output_channels=self.base_filters * 2,
+            output_channels=self.base_filters,
+            conv=self.Conv,
+            norm=self.Norm,
+            network_kwargs=self.network_kwargs,
+        )
+        self.out_3 = out_conv(
+            input_channels=self.base_filters * 8,
+            output_channels=self.n_classes,
             conv=self.Conv,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
+            final_convolution_layer=self.final_convolution_layer,
+            sigmoid_input_multiplier=self.sigmoid_input_multiplier,
         )
-        self.out = out_conv(
+        self.out_2 = out_conv(
+            input_channels=self.base_filters * 4,
+            output_channels=self.n_classes,
+            conv=self.Conv,
+            norm=self.Norm,
+            network_kwargs=self.network_kwargs,
+            final_convolution_layer=self.final_convolution_layer,
+            sigmoid_input_multiplier=self.sigmoid_input_multiplier,
+        )
+        self.out_1 = out_conv(
             input_channels=self.base_filters * 2,
             output_channels=self.n_classes,
             conv=self.Conv,
             norm=self.Norm,
             network_kwargs=self.network_kwargs,
             final_convolution_layer=self.final_convolution_layer,
             sigmoid_input_multiplier=self.sigmoid_input_multiplier,
         )
-
-        if "converter_type" in parameters["model"]:
-            self.ins = self.converter(self.ins).model
-            self.ds_0 = self.converter(self.ds_0).model
-            self.en_1 = self.converter(self.en_1).model
-            self.ds_1 = self.converter(self.ds_1).model
-            self.en_2 = self.converter(self.en_2).model
-            self.ds_2 = self.converter(self.ds_2).model
-            self.en_3 = self.converter(self.en_3).model
-            self.ds_3 = self.converter(self.ds_3).model
-            self.en_4 = self.converter(self.en_4).model
-            self.us_3 = self.converter(self.us_3).model
-            self.de_3 = self.converter(self.de_3).model
-            self.us_2 = self.converter(self.us_2).model
-            self.de_2 = self.converter(self.de_2).model
-            self.us_1 = self.converter(self.us_1).model
-            self.de_1 = self.converter(self.de_1).model
-            self.us_0 = self.converter(self.us_0).model
-            self.de_0 = self.converter(self.de_0).model
-            self.out = self.converter(self.out).model
+        self.out_0 = out_conv(
+            input_channels=self.base_filters,
+            output_channels=self.n_classes,
+            conv=self.Conv,
+            norm=self.Norm,
+            network_kwargs=self.network_kwargs,
+            final_convolution_layer=self.final_convolution_layer,
+            sigmoid_input_multiplier=self.sigmoid_input_multiplier,
+        )
 
     def forward(self, x):
         """
-        Parameters
-        ----------
-        x : Tensor
-            Should be a 5D Tensor as [batch_size, channels, x_dims, y_dims, z_dims].
-
-        Returns
-        -------
-        x : Tensor
-            Returns a 5D Output Tensor as [batch_size, n_classes, x_dims, y_dims, z_dims].
+        Forward pass of the U-Net model.
 
+        Args:
+            x (Tensor): Input Tensor with shape [batch_size, channels, x_dims, y_dims, z_dims].
+
+        Returns:
+            (list): List of output Tensors with shape [batch_size, n_classes, x_dims, y_dims, z_dims].
+                    The length of the list corresponds to the number of layers in the decoder path.
         """
-        x1 = self.ins(x)
+        # Encoding path
+        x1 = self.ins(x)  # First convolution layer
+
+        # Downsample and apply convolution
         x2 = self.ds_0(x1)
         x2 = self.en_1(x2)
+
+        # Downsample and apply convolution
         x3 = self.ds_1(x2)
         x3 = self.en_2(x3)
+
+        # Downsample and apply convolution
         x4 = self.ds_2(x3)
         x4 = self.en_3(x4)
+
+        # Downsample and apply convolution
         x5 = self.ds_3(x4)
         x5 = self.en_4(x5)
 
+        # Decoding path
+        # Upsample, concatenate with x4, and apply convolution
         x = self.us_3(x5)
-        x = self.de_3(x, x4)
-        x = self.us_2(x)
-        x = self.de_2(x, x3)
-        x = self.us_1(x)
-        x = self.de_1(x, x2)
-        x = self.us_0(x)
-        x = self.de_0(x, x1)
-        x = self.out(x)
-        return x
+        xl4 = self.de_3(x, x4)
+        out_3 = self.out_3(xl4)  # Output tensor level 3
+
+        # Upsample, concatenate with x3, and apply convolution
+        x = self.us_2(xl4)
+        xl3 = self.de_2(x, x3)
+        out_2 = self.out_2(xl3)  # Output tensor level 2
+
+        # Upsample, concatenate with x2, and apply convolution
+        x = self.us_1(xl3)
+        xl2 = self.de_1(x, x2)
+        out_1 = self.out_1(xl2)  # Output tensor level 1
+
+        # Upsample, concatenate with x2, and apply convolution
+        x = self.us_0(xl2)
+        xl1 = self.de_0(x, x1)
+        out_0 = self.out_0(xl1)  # Output tensor level 0
+
+        # Return the 4 output tensors as a list
+        return [out_0, out_1, out_2, out_3]
 
 
-class resunet(unet):
+class deep_resunet(deep_unet):
     """
     This is the standard U-Net architecture with residual connections : https://arxiv.org/pdf/1606.06650.pdf.
     The 'residualConnections' flag controls residual connections The Downsampling, Encoding, Decoding modules are defined in the seg_modules file.
     These smaller modules are basically defined by 2 parameters, the input channels (filters) and the output channels (filters),
     and some other hyperparameters, which remain constant all the modules. For more details on the smaller modules please have a look at the seg_modules file.
     """
 
     def __init__(self, parameters: dict):
-        super(resunet, self).__init__(parameters, residualConnections=True)
+        super(deep_resunet, self).__init__(parameters, residualConnections=True)
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.16.dev20230413/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/parseConfig.py` & `GANDLF-0.0.16.dev20230413/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.16.dev20230413/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/training_manager.py` & `GANDLF-0.0.16.dev20230413/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/__init__.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/generic.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/handle_collisions.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         df (pandas.DataFrame): The input dataframe.
         headers (dict): The parsed headers.
         output_path (str): The output directory.
     """
 
     # Find the subjectID header
     subject_id_column_name = headers.get("subjectIDHeader", None)
-    assert subject_id_column_name is not None, "No subject ID column found in the headers."
+    assert (
+        subject_id_column_name is not None
+    ), "No subject ID column found in the headers."
 
     # Create a dictionary to store the count of each subjectid
     subjectid_counts = {}
 
     # Create a list to store the colliding subjectids
     collisions = []
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/imaging.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/modelbase.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/modelio.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/modelio.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,19 @@
             print("WARNING: Cannot export to ONNX model.")
             return
 
         # https://github.com/mlcommons/GaNDLF/issues/605
         openvino_present = False
         try:
             import openvino
+
             openvino_present = True
         except ImportError:
             print("WARNING: OpenVINO is not present.")
-        
+
         if openvino_present:
             try:
                 if model_dimension == 2:
                     subprocess.call(
                         [
                             "mo",
                             "--input_model",
@@ -115,15 +116,18 @@
                     subprocess.call(
                         [
                             "mo",
                             "--input_model",
                             "{0}".format(onnx_path),
                             "--input_shape",
                             "[1,{0},{1},{2},{3}]".format(
-                                num_channel, input_shape[0], input_shape[1], input_shape[2]
+                                num_channel,
+                                input_shape[0],
+                                input_shape[1],
+                                input_shape[2],
                             ),
                             "--data_type",
                             "{0}".format(ov_output_data_type),
                             "--output_dir",
                             "{0}".format(ov_output_dir),
                         ],
                     )
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/tensor.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF/utils/write_parse.py` & `GANDLF-0.0.16.dev20230413/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.16.dev20230413/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230412
+Version: 0.0.16.dev20230413
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230412 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230413 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230412/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.16.dev20230413/GANDLF.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -114,22 +114,22 @@
 GANDLF/models/seg_modules/EncodingModule.py
 GANDLF/models/seg_modules/FCNUpsamplingModule.py
 GANDLF/models/seg_modules/IncConv.py
 GANDLF/models/seg_modules/IncDownsamplingModule.py
 GANDLF/models/seg_modules/IncDropout.py
 GANDLF/models/seg_modules/IncUpsamplingModule.py
 GANDLF/models/seg_modules/InceptionModule.py
+GANDLF/models/seg_modules/InitialConv.py
 GANDLF/models/seg_modules/Interpolate.py
 GANDLF/models/seg_modules/ResNetModule.py
 GANDLF/models/seg_modules/UpsamplingModule.py
 GANDLF/models/seg_modules/__init__.py
 GANDLF/models/seg_modules/add_conv_block.py
 GANDLF/models/seg_modules/add_downsample_conv_block.py
 GANDLF/models/seg_modules/average_pool.py
-GANDLF/models/seg_modules/in_conv.py
 GANDLF/models/seg_modules/out_conv.py
 GANDLF/optimizers/__init__.py
 GANDLF/optimizers/wrap_torch.py
 GANDLF/schedulers/__init__.py
 GANDLF/schedulers/wrap_torch.py
 GANDLF/utils/__init__.py
 GANDLF/utils/generic.py
```

### Comparing `GANDLF-0.0.16.dev20230412/HISTORY.md` & `GANDLF-0.0.16.dev20230413/HISTORY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/LICENSE` & `GANDLF-0.0.16.dev20230413/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/PKG-INFO` & `GANDLF-0.0.16.dev20230413/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230412
+Version: 0.0.16.dev20230413
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230412 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230413 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230412/README.md` & `GANDLF-0.0.16.dev20230413/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/SECURITY.md` & `GANDLF-0.0.16.dev20230413/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_anonymizer` & `GANDLF-0.0.16.dev20230413/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_collectStats` & `GANDLF-0.0.16.dev20230413/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_configGenerator` & `GANDLF-0.0.16.dev20230413/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_constructCSV` & `GANDLF-0.0.16.dev20230413/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_deploy` & `GANDLF-0.0.16.dev20230413/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_optimizeModel` & `GANDLF-0.0.16.dev20230413/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_patchMiner` & `GANDLF-0.0.16.dev20230413/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_preprocess` & `GANDLF-0.0.16.dev20230413/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_recoverConfig` & `GANDLF-0.0.16.dev20230413/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_run` & `GANDLF-0.0.16.dev20230413/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/gandlf_verifyInstall` & `GANDLF-0.0.16.dev20230413/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230412/setup.py` & `GANDLF-0.0.16.dev20230413/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     "opencv-python",
     "torchmetrics==0.5.1",  # newer versions have changed api for f1 invocation
     "OpenPatchMiner==0.1.8",
     "zarr==2.10.3",
     "pydicom",
     "onnx",
     "torchinfo==1.7.0",
-    "segmentation-models-pytorch==0.3.0",
+    "segmentation-models-pytorch==0.3.2",
     "ACSConv==0.1.1",
     "docker",
     "dicom-anonymizer",
     "twine",
     "zarr",
     "keyring",
 ]
```

