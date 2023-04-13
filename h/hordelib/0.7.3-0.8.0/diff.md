# Comparing `tmp/hordelib-0.7.3.tar.gz` & `tmp/hordelib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.7.3.tar", last modified: Wed Apr 12 18:17:59 2023, max compression
+gzip compressed data, was "hordelib-0.8.0.tar", last modified: Thu Apr 13 10:58:02 2023, max compression
```

## Comparing `hordelib-0.7.3.tar` & `hordelib-0.8.0.tar`

### file list

```diff
@@ -1,865 +1,883 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.476575 hordelib-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 18:17:44.000000 hordelib-0.7.3/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 18:17:44.000000 hordelib-0.7.3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.376575 hordelib-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.388575 hordelib-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 18:17:44.000000 hordelib-0.7.3/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-12 18:17:44.000000 hordelib-0.7.3/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-12 18:17:44.000000 hordelib-0.7.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-12 18:17:44.000000 hordelib-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    19969 2023-04-12 18:17:49.000000 hordelib-0.7.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-12 18:17:44.000000 hordelib-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 18:17:44.000000 hordelib-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    49875 2023-04-12 18:17:59.476575 hordelib-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-12 18:17:44.000000 hordelib-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-12 18:17:44.000000 hordelib-0.7.3/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.388575 hordelib-0.7.3/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.392575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.396575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.400575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.400575 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38675 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.400575 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.400575 hordelib-0.7.3/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.400575 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.400575 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.404575 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.404575 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.404575 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.376575 hordelib-0.7.3/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.408575 hordelib-0.7.3/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.412575 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.412575 hordelib-0.7.3/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   480383 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.412575 hordelib-0.7.3/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-12 18:17:51.000000 hordelib-0.7.3/hordelib/_comfyui/web/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 18:17:59.000000 hordelib-0.7.3/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.412575 hordelib-0.7.3/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.412575 hordelib-0.7.3/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/clip/interrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.416575 hordelib-0.7.3/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.416575 hordelib-0.7.3/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24866 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/model_manager/torch_hijack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.416575 hordelib-0.7.3/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.416575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.420575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.380575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.424575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.428575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.428575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.380575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.428575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.428575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.432575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.432575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.432575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.432575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.432575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.436575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.436575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.436575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.436575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.440575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.444575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.444575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.444575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.448575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.448575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.448575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.448575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.448575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.448575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.384575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.452575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.456575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.460575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.464575 hordelib-0.7.3/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.468575 hordelib-0.7.3/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.468575 hordelib-0.7.3/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 18:17:44.000000 hordelib-0.7.3/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.388575 hordelib-0.7.3/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49875 2023-04-12 18:17:59.000000 hordelib-0.7.3/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    48684 2023-04-12 18:17:59.000000 hordelib-0.7.3/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:17:59.000000 hordelib-0.7.3/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 18:17:59.000000 hordelib-0.7.3/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 18:17:59.000000 hordelib-0.7.3/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.472575 hordelib-0.7.3/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-12 18:17:44.000000 hordelib-0.7.3/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-12 18:17:51.000000 hordelib-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 18:17:44.000000 hordelib-0.7.3/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 18:17:51.000000 hordelib-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:17:59.476575 hordelib-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.476575 hordelib-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:17:59.476575 hordelib-0.7.3/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/run_upscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 18:17:44.000000 hordelib-0.7.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 18:17:44.000000 hordelib-0.7.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.257927 hordelib-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-13 10:57:43.000000 hordelib-0.8.0/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 10:57:43.000000 hordelib-0.8.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:01.997920 hordelib-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.021921 hordelib-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 10:57:43.000000 hordelib-0.8.0/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-13 10:57:43.000000 hordelib-0.8.0/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-13 10:57:43.000000 hordelib-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-13 10:57:43.000000 hordelib-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-04-13 10:57:49.000000 hordelib-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 10:57:43.000000 hordelib-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 10:57:43.000000 hordelib-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    49875 2023-04-13 10:58:02.257927 hordelib-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-04-13 10:57:43.000000 hordelib-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-13 10:57:43.000000 hordelib-0.8.0/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.021921 hordelib-0.8.0/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.025921 hordelib-0.8.0/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.029921 hordelib-0.8.0/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.029921 hordelib-0.8.0/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.029921 hordelib-0.8.0/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.029921 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.033921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.037921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.037921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.037921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.037921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.037921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.041921 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.045922 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38675 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.049922 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.049922 hordelib-0.8.0/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.049922 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.049922 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.053922 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.057922 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.057922 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.057922 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.005921 hordelib-0.8.0/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.061922 hordelib-0.8.0/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.065922 hordelib-0.8.0/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.069922 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.069922 hordelib-0.8.0/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   480383 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.069922 hordelib-0.8.0/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-04-13 10:57:52.000000 hordelib-0.8.0/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-13 10:57:53.000000 hordelib-0.8.0/hordelib/_comfyui/web/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 10:58:01.000000 hordelib-0.8.0/hordelib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.069922 hordelib-0.8.0/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.069922 hordelib-0.8.0/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.073922 hordelib-0.8.0/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.073922 hordelib-0.8.0/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.077922 hordelib-0.8.0/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.081923 hordelib-0.8.0/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24866 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/model_manager/torch_hijack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.085923 hordelib-0.8.0/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.089923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.089923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.089923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.089923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.089923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.089923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.093923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.093923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.097923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.097923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.097923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.101923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.101923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.105923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.105923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.105923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.105923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.109923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.109923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.109923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.009921 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.109923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.113923 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.121924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.125924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.009921 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.125924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.125924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.129924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.129924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.137924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.137924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.137924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.137924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.141924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.141924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.141924 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.153925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.157925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.161925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.165925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.169925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.169925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.173925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.173925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.173925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.177925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.013921 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.177925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.177925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.177925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.177925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.181925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.181925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.185925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.185925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.185925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.193925 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.201926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.205926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.205926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.205926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.209926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.209926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.213926 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.213926 hordelib-0.8.0/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.213926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.213926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.213926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.217926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.217926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.221926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.221926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.225926 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.225926 hordelib-0.8.0/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.229926 hordelib-0.8.0/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/run_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/shared_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.233927 hordelib-0.8.0/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.233927 hordelib-0.8.0/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41379 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 10:57:43.000000 hordelib-0.8.0/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.025921 hordelib-0.8.0/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49875 2023-04-13 10:58:01.000000 hordelib-0.8.0/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49188 2023-04-13 10:58:01.000000 hordelib-0.8.0/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:58:01.000000 hordelib-0.8.0/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-13 10:58:01.000000 hordelib-0.8.0/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 10:58:01.000000 hordelib-0.8.0/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.241927 hordelib-0.8.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-13 10:57:43.000000 hordelib-0.8.0/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-13 10:57:53.000000 hordelib-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:57:43.000000 hordelib-0.8.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-13 10:57:53.000000 hordelib-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:58:02.261927 hordelib-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.257927 hordelib-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/make_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:58:02.257927 hordelib-0.8.0/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/run_upscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-13 10:57:43.000000 hordelib-0.8.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-13 10:57:43.000000 hordelib-0.8.0/tox.ini
```

### Comparing `hordelib-0.7.3/.changelog` & `hordelib-0.8.0/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/.github/workflows/maintests.yml` & `hordelib-0.8.0/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/.github/workflows/prtests.yml` & `hordelib-0.8.0/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/.github/workflows/release.yml` & `hordelib-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/.gitignore` & `hordelib-0.8.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -133,25 +133,28 @@
 
 # Cython debug symbols
 cython_debug/
 
 # Local
 test-image.png
 hordelib/ComfyUI
+hordelib/_comfyui
 ComfyUI
 model.ckpt
 coverage.lcov
 images/pip*.png
 images/test.png
 images/hor*.png
 images/hor*.webp
 images/pip*.webp
 images/test.webp
 images/run_*
 comfy-prompt*.json
 images/index.html
+hordelib/_comfyui
 _version.py
+_comfyui
 
 .vscode
 *.ckpt
 *.pth
 .gitignore
```

### Comparing `hordelib-0.7.3/CHANGELOG.md` & `hordelib-0.8.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 ## hordelib Changelog
 
+## [v0.8.0](https://github.com/jug-dev/hordelib/compare/v0.7.3...v0.8.0)
+
+13 April 2023
+
+- feat: Clip Rankings [`#117`](https://github.com/jug-dev/hordelib/pull/117) (Divided by Zer0)
+- feat: Blip [`#116`](https://github.com/jug-dev/hordelib/pull/116) (Divided by Zer0)
+- fix: make library thread safe [`b7274b4`](https://github.com/jug-dev/hordelib/commit/b7274b4dc1170480513fbd7eb34a4e6a0cd3aaf4)  (Jug)
+- fix: remove thread mutex for now [`1a901b8`](https://github.com/jug-dev/hordelib/commit/1a901b8d8274f84663dd2933224d375105120a1b)  (Jug)
+- build: fix build_helper for local use [`6ec5f38`](https://github.com/jug-dev/hordelib/commit/6ec5f38279eca2643fbfdf0ff9cc1ab7031b6bb3)  (Jug)
+
 ## [v0.7.3](https://github.com/jug-dev/hordelib/compare/v0.7.2...v0.7.3)
 
 12 April 2023
 
 - build: more production build fixes. [`0ca0367`](https://github.com/jug-dev/hordelib/commit/0ca0367e98ec88f9b30428f797101e333902a0f9)  (Jug)
 
 ## [v0.7.2](https://github.com/jug-dev/hordelib/compare/v0.7.1...v0.7.2)
```

### Comparing `hordelib-0.7.3/LICENSE` & `hordelib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/PKG-INFO` & `hordelib-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.7.3
+Version: 0.8.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -698,15 +698,15 @@
 
 The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
 If being installed from pypi, use a requirements file of the form:
 ```
---extra-index-url https://download.pytorch.org/whl/cu117
+--extra-index-url https://download.pytorch.org/whl/cu118
 hordelib
 
 ...your other dependencies...
 ```
 
 ## Usage
```

### Comparing `hordelib-0.7.3/README.md` & `hordelib-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
 If being installed from pypi, use a requirements file of the form:
 ```
---extra-index-url https://download.pytorch.org/whl/cu117
+--extra-index-url https://download.pytorch.org/whl/cu118
 hordelib
 
 ...your other dependencies...
 ```
 
 ## Usage
```

### Comparing `hordelib-0.7.3/build_helper.py` & `hordelib-0.8.0/build_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # build_helper.py
 # This is just a build helper script to build the pypi package.
 import os
 import shutil
 import subprocess
+import argparse
 
 from hordelib import install_comfy
 from hordelib.consts import COMFYUI_VERSION
 
 
 def run(command):
     result = subprocess.run(command, shell=True, text=True)
@@ -48,20 +49,58 @@
             newfile.append(f"#{line}")
         else:
             newfile.append(line)
     with open("pyproject.toml", "w") as outfile:
         outfile.writelines(newfile)
 
 
-def static_package_comfyui():
-    installer = install_comfy.Installer()
-    installer.install(COMFYUI_VERSION)
-
-    if not os.path.exists("ComfyUI"):
-        raise Exception("ComfyUI not found")
-    shutil.copytree("ComfyUI", "hordelib/_comfyui")
+def static_package_comfyui(unpatch=False):
+    if unpatch:
+        if os.path.exists("hordelib/_version.py"):
+            os.remove("hordelib/_version.py")
+
+        if os.path.exists("hordelib/_comfyui"):
+            try:
+                shutil.rmtree("hordelib/_comfyui")
+            except PermissionError:
+                print("Can't delete `hordelib/_comfyUI/` please delete it manually and try again")
+                exit(1)
+
+    else:
+        installer = install_comfy.Installer()
+        installer.install(COMFYUI_VERSION)
+
+        if not os.path.exists("ComfyUI"):
+            raise Exception("ComfyUI not found")
+        shutil.copytree("ComfyUI", "hordelib/_comfyui")
+
+
+def unpatch():
+    static_package_comfyui(True)
+    patch_requirements(True)
+    patch_toml(True)
 
 
-if __name__ == "__main__":
+def patch():
     static_package_comfyui()
     patch_requirements()
     patch_toml()
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--fix", action="store_true", help="Cleanup after the build")
+    args = parser.parse_args()
+    undo = args.fix
+
+    if os.path.exists("hordelib/_comfyui"):
+        # cleanup before the new build
+        unpatch()
+
+    if not args.fix:
+        static_package_comfyui()
+        patch_requirements()
+        patch_toml()
+    else:
+        static_package_comfyui(True)
+        patch_requirements(True)
+        patch_toml(True)
```

### Comparing `hordelib-0.7.3/hordelib/_comfyui/LICENSE` & `hordelib-0.8.0/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/README.md` & `hordelib-0.8.0/hordelib/_comfyui/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/model_management.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/model_management.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/samplers.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/samplers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_clip.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-0.8.0/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy/utils.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-0.8.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-0.8.0/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-0.8.0/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/execution.py` & `hordelib-0.8.0/hordelib/_comfyui/execution.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-0.8.0/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/folder_paths.py` & `hordelib-0.8.0/hordelib/_comfyui/folder_paths.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/input/example.png` & `hordelib-0.8.0/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/main.py` & `hordelib-0.8.0/hordelib/_comfyui/main.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-0.8.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/nodes.py` & `hordelib-0.8.0/hordelib/_comfyui/nodes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-0.8.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-0.8.0/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/server.py` & `hordelib-0.8.0/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-0.8.0/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/index.html` & `hordelib-0.8.0/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-0.8.0/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-0.8.0/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/scripts/api.js` & `hordelib-0.8.0/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/scripts/app.js` & `hordelib-0.8.0/hordelib/_comfyui/web/scripts/app.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-0.8.0/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-0.8.0/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-0.8.0/hordelib/_comfyui/web/scripts/ui.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-0.8.0/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/_comfyui/web/style.css` & `hordelib-0.8.0/hordelib/_comfyui/web/style.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/cache/cache.py` & `hordelib-0.8.0/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/clip/bulk.py` & `hordelib-0.8.0/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/clip/coca.py` & `hordelib-0.8.0/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/clip/image.py` & `hordelib-0.8.0/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/clip/interrogate.py` & `hordelib-0.8.0/hordelib/clip/interrogate.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from hordelib.clip.text import TextEmbed
 
 
 class Interrogator:
     def __init__(self, model_info):
         """
         :param model: Loaded model from ModelManager
-        For each data list in model["data_lists"], check if all items are cached.
+        For each data list in model["ranking_lists"], check if all items are cached.
         If not, embed all items and save to cache.
         If yes, load all text embeds from cache.
         """
         self.model_info = model_info
         self.cache = Cache(
             self.model_info["cache_name"],
             cache_parentname="embeds",
@@ -214,30 +214,30 @@
         :param text_array: List of text to compare to image, or dict of lists of text to compare to image
         :param top_count: Number of top results to return
         :return:
             * If similarity is True, returns dict of {text: similarity}
             * If rank is True, returns list of tuples of (text, similarity)
             See rank() for more details
             See similarity() for more details
-        If text_array is None, uses default text_array from model["data_lists"]
+        If text_array is None, uses default text_array from model["ranking_lists"]
         """
         if image is None and filename is None:
             logger.error("Either image or filename must be set")
             return
         if image is not None and filename is not None:
             logger.error("Only one of image or filename must be set")
             return
         if os.path.isdir(f"{directory}/{filename}"):
             logger.error("Filename must be a file, not a directory")
             return
         if not similarity and not rank:
             logger.error("Must specify similarity or rank")
             return
         if text_array is None:
-            text_array = self.model_info["data_lists"]
+            text_array = self.model_info["ranking_lists"]
         if isinstance(text_array, list):
             text_array = {"default": text_array}
         elif isinstance(text_array, dict):
             pass
         image_embed = ImageEmbed(self.model_info, self.cache_image)
         image_hash = image_embed(image, filename, directory)
         image_embed_array = np.load(f"{self.cache_image.cache_dir}/{image_hash}.npy")
```

### Comparing `hordelib-0.7.3/hordelib/clip/text.py` & `hordelib-0.8.0/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/comfy_horde.py` & `hordelib-0.8.0/hordelib/comfy_horde.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import contextlib
 import copy
 import glob
 import json
 import os
 import re
 import typing
-from io import BytesIO
 from pprint import pformat
 
 from loguru import logger
-from PIL import Image
 
 from hordelib.utils.ioredirect import OutputCollector
 
 # Do not change the order of these imports
 # isort: off
 import execution
 import comfy.sd
@@ -32,43 +30,36 @@
     output_clip: bool = True,
     embeddings_path: str | None = None,
 ) -> dict[str, typing.Any]:  # XXX # FIXME 'any'
     # XXX Needs docstring
     # XXX # TODO One day this signature should be generic, and not comfy specific
     # XXX # This can remain a comfy call, but the rest of the code should be able
     # XXX # to pretend it isn't
-
     # Redirect IO
-    stdio = OutputCollector()
-    with contextlib.redirect_stdout(stdio):
-        (modelPatcher, clipModel, vae, clipVisionModel) = comfy.sd.load_checkpoint_guess_config(
-            ckpt_path=ckpt_path,
-            output_vae=output_vae,
-            output_clip=output_clip,
-            embedding_directory=embeddings_path,
-        )
-    stdio.replay()
+    (modelPatcher, clipModel, vae, clipVisionModel) = comfy.sd.load_checkpoint_guess_config(
+        ckpt_path=ckpt_path,
+        output_vae=output_vae,
+        output_clip=output_clip,
+        embedding_directory=embeddings_path,
+    )
 
     return {
         "model": modelPatcher,
         "clip": clipModel,
         "vae": vae,
         "clipVisionModel": clipVisionModel,
     }
 
 
 def horde_load_controlnet(  # XXX Needs docstring
     controlnet_path: str,
     target_model,
 ) -> comfy.sd.ControlNet | comfy.sd.T2IAdapter | None:
     # Redirect IO
-    stdio = OutputCollector()
-    with contextlib.redirect_stdout(stdio):
-        controlnet = comfy.sd.load_controlnet(ckpt_path=controlnet_path, model=target_model)
-    stdio.replay()
+    controlnet = comfy.sd.load_controlnet(ckpt_path=controlnet_path, model=target_model)
     return controlnet
 
 
 class Comfy_Horde:
     """Handles horde-specific behavior against ComfyUI."""
 
     # We save pipelines from the ComfyUI GUI. This is very convenient as it
@@ -274,15 +265,14 @@
     def run_pipeline(self, pipeline_name: str, params: dict) -> dict | None:
         # Sanity
         if pipeline_name not in self.pipelines:
             logger.error(f"Unknown inference pipeline: {pipeline_name}")
             return None
 
         logger.info(f"Running pipeline {pipeline_name}")
-        logger.debug(f"Ug oh  {pipeline_name}")
 
         # Grab a copy of the pipeline
         pipeline = copy.copy(self.pipelines[pipeline_name])
 
         # Inject our model manager if required
         from hordelib.shared_model_manager import SharedModelManager
 
@@ -320,34 +310,27 @@
                 )
 
         # Set the pipeline parameters
         self._set(pipeline, **params)
 
         # Create our prompt executive
         inference = execution.PromptExecutor(self)
-        stdio = OutputCollector()
-        with contextlib.redirect_stdout(stdio):
-            # Load our custom nodes
-            self._load_custom_nodes()
-        stdio.replay()
+        # Load our custom nodes
+        self._load_custom_nodes()
 
         # This is useful for dumping the entire pipeline to the terminal when
         # developing and debugging new pipelines. A badly structured pipeline
         # file just results in a cryptic error from comfy
         pretty_pipeline = pformat(pipeline)
         if False:  # This isn't here Tazlin :)
             logger.error(pretty_pipeline)
 
         # The client_id parameter here is just so we receive comfy callbacks for debugging.
         # We pretend we are a web client and want async callbacks.
-        stdio = OutputCollector()
-        with contextlib.redirect_stdout(stdio):
-            with contextlib.redirect_stderr(stdio):
-                inference.execute(pipeline, extra_data={"client_id": 1})
-        stdio.replay()
+        inference.execute(pipeline, extra_data={"client_id": 1})
 
         return inference.outputs
 
     # Run a pipeline that returns an image in pixel space
     def run_image_pipeline(self, pipeline_name: str, params: dict) -> list[dict] | None:
         # From the horde point of view, let us assume the output we are interested in
         # is always in a HordeImageOutput node named "output_image". This is an array of
```

### Comparing `hordelib-0.7.3/hordelib/config_path.py` & `hordelib-0.8.0/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/consts.py` & `hordelib-0.8.0/hordelib/consts.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/horde.py` & `hordelib-0.8.0/hordelib/horde.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         # "<unused>": "BinaryPreprocessor",
         # "<unused>": "ColorPreprocessor",
         # "<unused>": "PiDiNetPreprocessor",
     }
 
     SOURCE_IMAGE_PROCESSING_OPTIONS = ["img2img", "inpainting", "outpainting"]
 
+    def __init__(self):
+        pass
+
     def _parameter_remap(self, payload: dict[str, str | None]) -> dict[str, str | None]:
         params = {}
         # Extract from the payload things we understand
         for key, value in payload.items():
             newkey = HordeLib.BASIC_INFERENCE_PARAMS.get(key, None)
             if newkey:
                 params[newkey] = value
```

### Comparing `hordelib-0.7.3/hordelib/initialisation.py` & `hordelib-0.8.0/hordelib/initialisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 
 def initialise(
     model_managers_to_load: dict[MODEL_CATEGORY_NAMES, bool] = DEFAULT_MODEL_MANAGERS,
     setup_logging=True,
 ):
     # Setup logging if requested
-    if setup_logging:
-        HordeLog.initialise()
+    HordeLog.initialise(setup_logging)
 
     logger.level("DEBUG")  # XXX # FIXME
 
     # If developer mode, don't permit some things
     if not RELEASE_VERSION and " " in get_hordelib_path():
         # Our runtime patching can't handle this
         raise Exception(
```

### Comparing `hordelib-0.7.3/hordelib/install_comfy.patch` & `hordelib-0.8.0/hordelib/install_comfy.patch`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/install_comfy.py` & `hordelib-0.8.0/hordelib/install_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/aitemplate.json` & `hordelib-0.8.0/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/blip.json` & `hordelib-0.8.0/hordelib/model_database/blip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/clip.json` & `hordelib-0.8.0/hordelib/model_database/clip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/controlnet.json` & `hordelib-0.8.0/hordelib/model_database/controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/db.json` & `hordelib-0.8.0/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/db_dep.json` & `hordelib-0.8.0/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/db_embeds.json` & `hordelib-0.8.0/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/diffusers.json` & `hordelib-0.8.0/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/esrgan.json` & `hordelib-0.8.0/hordelib/model_database/esrgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/gfpgan.json` & `hordelib-0.8.0/hordelib/model_database/gfpgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/safety_checker.json` & `hordelib-0.8.0/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_database/stable_diffusion.json` & `hordelib-0.8.0/hordelib/model_database/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/base.py` & `hordelib-0.8.0/hordelib/model_manager/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/blip.py` & `hordelib-0.8.0/hordelib/model_manager/blip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import importlib.resources as importlib_resources
 import time
+from pathlib import Path
 
 import torch
 from loguru import logger
 
+from hordelib.config_path import get_hordelib_path
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
+from hordelib.utils.blip.blip import blip_decoder
 
 
 class BlipModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.blip],
             download_reference=download_reference,
@@ -43,15 +46,15 @@
             logger.info(
                 f"{model_name} downloaded",
                 status="Downloading",
             )  # logger.init_ok
         if model_name not in self.loaded_models:
             tic = time.time()
             logger.info(f"{model_name}", status="Loading")  # logger.init
-            self.loaded_models[model_name] = self.load_blip(  # XXX # FIXME
+            self.loaded_models[model_name] = self.modelToRam(
                 model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
                 blip_image_eval_size=blip_image_eval_size,
             )
             logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
@@ -67,34 +70,36 @@
         self,
         model_name,
         half_precision=True,
         gpu_id=0,
         cpu_only=False,
         blip_image_eval_size=512,
     ):
-        raise NotImplementedError("BLIP is not currently implemented!")
-        # if not self.cuda_available:
-        #     cpu_only = True
-        # vit = "base" if model_name == "BLIP" else "large"
-        # model_path = self.get_model_files(model_name)[0]["path"]
-        # model_path = f"{self.modelFolderPath}/{model_path}"
-        # if cpu_only:
-        #     device = torch.device("cpu")
-        #     half_precision = False
-        # else:
-        #     device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
-        # logger.info(f"Loading model {model_name} on {device}")
-        # logger.info(f"Model path: {model_path}")
-        # with importlib_resources.as_file(self.pkg / "med_config.json") as med_config:
-        #     logger.info(f"Med config path: {med_config}")
-        #     model = blip_decoder(
-        #         # XXX # FIXME
-        #         pretrained=model_path,
-        #         med_config=med_config,
-        #         image_size=blip_image_eval_size,
-        #         vit=vit,
-        #     )
-        # model = model.eval()
-        # model.to(device)
-        # if half_precision:
-        #     model = model.half()
-        # return {"model": model, "device": device, "half_precision": half_precision}
+        if not self.cuda_available:
+            cpu_only = True
+        vit = "base" if model_name == "BLIP" else "large"
+        model_path = self.get_model_files(model_name)[0]["path"]
+        model_path = f"{self.modelFolderPath}/{model_path}"
+        if cpu_only:
+            device = torch.device("cpu")
+            half_precision = False
+        else:
+            device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
+        logger.info(f"Loading model {model_name} on {device}")
+        logger.info(f"Model path: {model_path}")
+        med_path = Path(get_hordelib_path()).joinpath(
+            "model_database/",
+            "med_config.json",
+        )
+        with importlib_resources.as_file(med_path.resolve()) as med_config:
+            logger.info(f"Med config path: {med_config}")
+            model = blip_decoder(
+                pretrained=model_path,
+                med_config=med_config,
+                image_size=blip_image_eval_size,
+                vit=vit,
+            )
+        model = model.eval()
+        model.to(device)
+        if half_precision:
+            model = model.half()
+        return {"model": model, "device": device, "half_precision": half_precision}
```

### Comparing `hordelib-0.7.3/hordelib/model_manager/clip.py` & `hordelib-0.8.0/hordelib/model_manager/clip.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import time
+from pathlib import Path
 
 import clip
 import open_clip
 import torch
 from loguru import logger
 
+from hordelib.config_path import get_hordelib_path
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
 
 class ClipModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.clip],
             download_reference=download_reference,
         )
 
-    def load_data_lists(self):
-        # data_lists = {}
-        # data_lists["artist"] = load_list(self.pkg / "artists.txt")
-        # data_lists["flavors"] = load_list(self.pkg / "flavors.txt")
-        # data_lists["medium"] = load_list(self.pkg / "mediums.txt")
-        # data_lists["movement"] = load_list(self.pkg / "movements.txt")
-        # data_lists["trending"] = load_list(self.pkg / "sites.txt")
-        # data_lists["techniques"] = load_list(self.pkg / "techniques.txt")
-        # data_lists["tags"] = load_list(self.pkg / "tags.txt")
-        # return data_list
-        return {}
+    def load_ranking_lists(self):
+        ranking_lists = {}
+        ranking_lists_path = Path(get_hordelib_path()).joinpath(
+            "clip/",
+            "ranking_lists/",
+        )
+        for file in ranking_lists_path.glob("*.txt"):
+            ranking_lists[file.stem] = load_list(file)
+        return ranking_lists
 
     def load_coca(self, model_name, half_precision=True, gpu_id=0, cpu_only=False):
         model_path = self.get_model_files(model_name)[0]["path"]
         model_path = f"{self.modelFolderPath}/{model_path}"
         if cpu_only:
             device = torch.device("cpu")
             half_precision = False
@@ -68,20 +68,20 @@
             device=device,
             precision="fp16" if half_precision else "fp32",
         )
         model = model.eval()
         model.to(device)
         if half_precision:
             model = model.half()
-        data_lists = self.load_data_lists()
+        ranking_lists = self.load_ranking_lists()
         return {
             "model": model,
             "device": device,
             "preprocess": preprocess,
-            "data_lists": data_lists,
+            "ranking_lists": ranking_lists,
             "half_precision": half_precision,
             "cache_name": model_name.replace("/", "_"),
         }
 
     def load_clip(self, model_name, half_precision=True, gpu_id=0, cpu_only=False):
         if cpu_only:
             device = torch.device("cpu")
@@ -92,20 +92,20 @@
             model_name,
             device=device,
             download_root=self.modelFolderPath,
         )
         model = model.eval()
         if half_precision:
             model = model.half()
-        data_lists = self.load_data_lists()
+        ranking_lists = self.load_ranking_lists()
         return {
             "model": model,
             "device": device,
             "preprocess": preprocess,
-            "data_lists": data_lists,
+            "ranking_lists": ranking_lists,
             "half_precision": half_precision,
             "cache_name": model_name.replace("/", "_"),
         }
 
     def modelToRam(
         self,
         model_name: str,
@@ -160,7 +160,13 @@
         logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
         toc = time.time()
         logger.info(
             f"Loading {model_name}: Took {toc-tic} seconds",
             status="Success",
         )  # logger.init_ok
         return loaded_model_info
+
+
+def load_list(filename):
+    with open(filename, "r", encoding="utf-8", errors="replace") as f:
+        items = [line.strip() for line in f.readlines()]
+        return items
```

### Comparing `hordelib-0.7.3/hordelib/model_manager/codeformer.py` & `hordelib-0.8.0/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/compvis.py` & `hordelib-0.8.0/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/controlnet.py` & `hordelib-0.8.0/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/diffusers.py` & `hordelib-0.8.0/hordelib/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/esrgan.py` & `hordelib-0.8.0/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/gfpgan.py` & `hordelib-0.8.0/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/hyper.py` & `hordelib-0.8.0/hordelib/model_manager/hyper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/safety_checker.py` & `hordelib-0.8.0/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/model_manager/torch_hijack.py` & `hordelib-0.8.0/hordelib/model_manager/torch_hijack.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/install.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-0.8.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/__init__.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-0.8.0/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.8.0/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-0.8.0/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/node_image_loader.py` & `hordelib-0.8.0/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/node_image_output.py` & `hordelib-0.8.0/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/node_model_loader.py` & `hordelib-0.8.0/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.8.0/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-0.8.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.8.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/run_comfyui.py` & `hordelib-0.8.0/hordelib/run_comfyui.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/safety_checker.py` & `hordelib-0.8.0/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/shared_model_manager.py` & `hordelib-0.8.0/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/utils/cast.py` & `hordelib-0.8.0/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/utils/ioredirect.py` & `hordelib-0.8.0/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/hordelib/utils/logger.py` & `hordelib-0.8.0/hordelib/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         else:
             cls.setup_compatibility()
 
     @classmethod
     def setup_compatibility(cls):
         logger.__class__.generation = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.prompt = partialmethod(logger.__class__.log, "INFO")
-        logger.__class__.init = partialmethod(logger.__class__.log, "INIT")
+        logger.__class__.init = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.init_ok = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.init_warn = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.init_err = partialmethod(logger.__class__.log, "ERROR")
         logger.__class__.message = partialmethod(logger.__class__.log, "INFO")
         logger.__class__.stats = partialmethod(logger.__class__.log, "DEBUG")
 
     @classmethod
```

### Comparing `hordelib-0.7.3/hordelib.egg-info/PKG-INFO` & `hordelib-0.8.0/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.7.3
+Version: 0.8.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -698,15 +698,15 @@
 
 The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
 If being installed from pypi, use a requirements file of the form:
 ```
---extra-index-url https://download.pytorch.org/whl/cu117
+--extra-index-url https://download.pytorch.org/whl/cu118
 hordelib
 
 ...your other dependencies...
 ```
 
 ## Usage
```

### Comparing `hordelib-0.7.3/hordelib.egg-info/SOURCES.txt` & `hordelib-0.8.0/hordelib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -204,33 +204,43 @@
 hordelib/_comfyui/web/lib/litegraph.css
 hordelib/_comfyui/web/scripts/api.js
 hordelib/_comfyui/web/scripts/app.js
 hordelib/_comfyui/web/scripts/defaultGraph.js
 hordelib/_comfyui/web/scripts/pnginfo.js
 hordelib/_comfyui/web/scripts/ui.js
 hordelib/_comfyui/web/scripts/widgets.js
+hordelib/blip/__init__.py
+hordelib/blip/caption.py
 hordelib/cache/__init__.py
 hordelib/cache/cache.py
 hordelib/clip/__init__.py
 hordelib/clip/bulk.py
 hordelib/clip/coca.py
 hordelib/clip/image.py
 hordelib/clip/interrogate.py
 hordelib/clip/text.py
+hordelib/clip/ranking_lists/artists.txt
+hordelib/clip/ranking_lists/flavors.txt
+hordelib/clip/ranking_lists/mediums.txt
+hordelib/clip/ranking_lists/movements.txt
+hordelib/clip/ranking_lists/sites.txt
+hordelib/clip/ranking_lists/tags.txt
+hordelib/clip/ranking_lists/techniques.txt
 hordelib/model_database/aitemplate.json
 hordelib/model_database/blip.json
 hordelib/model_database/clip.json
 hordelib/model_database/codeformer.json
 hordelib/model_database/controlnet.json
 hordelib/model_database/db.json
 hordelib/model_database/db_dep.json
 hordelib/model_database/db_embeds.json
 hordelib/model_database/diffusers.json
 hordelib/model_database/esrgan.json
 hordelib/model_database/gfpgan.json
+hordelib/model_database/med_config.json
 hordelib/model_database/safety_checker.json
 hordelib/model_database/stable_diffusion.json
 hordelib/model_manager/__init__.py
 hordelib/model_manager/base.py
 hordelib/model_manager/blip.py
 hordelib/model_manager/clip.py
 hordelib/model_manager/codeformer.py
@@ -680,14 +690,18 @@
 hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
 hordelib/pipelines/pipeline_stable_diffusion_paint.json
 hordelib/utils/__init__.py
 hordelib/utils/cast.py
 hordelib/utils/ioredirect.py
 hordelib/utils/logger.py
 hordelib/utils/switch.py
+hordelib/utils/blip/__init__.py
+hordelib/utils/blip/blip.py
+hordelib/utils/blip/med.py
+hordelib/utils/blip/vit.py
 images/test_annotator.jpg
 images/test_db0.jpg
 images/test_facefix.png
 images/test_inpaint.png
 images/test_inpaint_alpha.png
 images/test_inpaint_mask.png
 images/test_inpaint_original.png
@@ -702,14 +716,15 @@
 tests/run_img2img_inpaint.py
 tests/run_img2img_inpaint_mask.py
 tests/run_img2img_outpaint.py
 tests/run_inpainting.py
 tests/run_txt2img.py
 tests/run_txt2img_hires.py
 tests/run_upscale.py
+tests/test_blip.py
 tests/test_clip.py
 tests/test_comfy.py
 tests/test_horde_controlnet_annotator.py
 tests/test_horde_inference.py
 tests/test_horde_inference_controlnet.py
 tests/test_horde_inference_img2img.py
 tests/test_horde_inference_painting.py
```

### Comparing `hordelib-0.7.3/images/test_annotator.jpg` & `hordelib-0.8.0/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_db0.jpg` & `hordelib-0.8.0/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_facefix.png` & `hordelib-0.8.0/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_inpaint.png` & `hordelib-0.8.0/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_inpaint_alpha.png` & `hordelib-0.8.0/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_inpaint_mask.png` & `hordelib-0.8.0/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_inpaint_original.png` & `hordelib-0.8.0/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/images/test_outpaint.png` & `hordelib-0.8.0/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/pyproject.toml` & `hordelib-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/requirements.txt` & `hordelib-0.8.0/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -32,7 +32,8 @@
 scikit-image
 prettytable==3.6.0
 svglib
 reportlab
 addict
 yapf
 mediapipe==0.9.1.0
+fairscale
```

### Comparing `hordelib-0.7.3/tests/make_index.py` & `hordelib-0.8.0/tests/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/model_managers/test_comvis.py` & `hordelib-0.8.0/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/model_managers/test_diffusers.py` & `hordelib-0.8.0/tests/model_managers/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/model_managers/test_safety_checker.py` & `hordelib-0.8.0/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_controlnet.py` & `hordelib-0.8.0/tests/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_controlnet_annotator.py` & `hordelib-0.8.0/tests/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_facefix.py` & `hordelib-0.8.0/tests/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_img2img.py` & `hordelib-0.8.0/tests/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_img2img_hires.py` & `hordelib-0.8.0/tests/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_img2img_inpaint.py` & `hordelib-0.8.0/tests/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_img2img_inpaint_mask.py` & `hordelib-0.8.0/tests/run_img2img_inpaint_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_img2img_outpaint.py` & `hordelib-0.8.0/tests/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_inpainting.py` & `hordelib-0.8.0/tests/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_txt2img.py` & `hordelib-0.8.0/tests/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_txt2img_hires.py` & `hordelib-0.8.0/tests/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/run_upscale.py` & `hordelib-0.8.0/tests/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_clip.py` & `hordelib-0.8.0/tests/test_clip.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,47 +3,59 @@
 from PIL import Image
 
 from hordelib.clip.interrogate import Interrogator
 from hordelib.horde import HordeLib
 from hordelib.shared_model_manager import SharedModelManager
 
 
-class TestHordePostProcessing:
-    @pytest.fixture(autouse=True)
+class TestHordeClip:
+    @pytest.fixture(autouse=True, scope="class")
     def setup_and_teardown(self):
-        self.horde = HordeLib()
+        TestHordeClip.horde = HordeLib()
 
-        self.default_model_manager_args = {
+        TestHordeClip.default_model_manager_args = {
             # aitemplate
             # "blip": True,
             "clip": True,
             # "codeformer": True,
             # "compvis": True,
             # "controlnet": True,
             # "diffusers": True,
             # "esrgan": True,
             # "gfpgan": True,
             # "safety_checker": True,
         }
-        self.image = Image.open("images/test_db0.jpg")
+        TestHordeClip.image = Image.open("images/test_db0.jpg")
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         SharedModelManager.manager.load("ViT-L/14")
         yield
-        del self.horde
+        del TestHordeClip.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
     def test_clip_similarities(self):
-        assert SharedModelManager.manager.clip.is_model_loaded("ViT-L/14") is True
+        assert SharedModelManager.manager.is_model_loaded("ViT-L/14") is True
         word_list = ["outlaw", "explosion", "underwater"]
         model_info = SharedModelManager.manager.loaded_models["ViT-L/14"]
         interrogator = Interrogator(model_info)
         similarity_result = interrogator(
             image=self.image,
             text_array=word_list,
             similarity=True,
         )
         assert "default" in similarity_result
         assert similarity_result["default"]["outlaw"] > 0.15
         assert similarity_result["default"]["explosion"] > 0.15
         assert similarity_result["default"]["underwater"] < 0.15
+
+    def test_clip_rankings(self):
+        assert SharedModelManager.manager.is_model_loaded("ViT-L/14") is True
+        model_info = SharedModelManager.manager.loaded_models["ViT-L/14"]
+        interrogator = Interrogator(model_info)
+        ranking_result = interrogator(
+            image=self.image,
+            rank=True,
+        )
+        assert type(ranking_result) is dict
+        assert "artists" in ranking_result
+        assert "mediums" in ranking_result
```

### Comparing `hordelib-0.7.3/tests/test_comfy.py` & `hordelib-0.8.0/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_horde_controlnet_annotator.py` & `hordelib-0.8.0/tests/test_horde_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_horde_inference.py` & `hordelib-0.8.0/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_horde_inference_controlnet.py` & `hordelib-0.8.0/tests/test_horde_inference_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_horde_inference_img2img.py` & `hordelib-0.8.0/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_horde_inference_painting.py` & `hordelib-0.8.0/tests/test_horde_inference_painting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_horde_pp.py` & `hordelib-0.8.0/tests/test_horde_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_inference.py` & `hordelib-0.8.0/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_safety_checker.py` & `hordelib-0.8.0/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tests/test_shared_model_manager.py` & `hordelib-0.8.0/tests/test_shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.7.3/tox.ini` & `hordelib-0.8.0/tox.ini`

 * *Files identical despite different names*

