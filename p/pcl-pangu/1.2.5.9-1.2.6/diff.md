# Comparing `tmp/pcl_pangu-1.2.5.9.tar.gz` & `tmp/pcl_pangu-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcl_pangu-1.2.5.9.tar", last modified: Wed Apr 12 09:19:44 2023, max compression
+gzip compressed data, was "pcl_pangu-1.2.6.tar", last modified: Thu Apr 13 11:26:34 2023, max compression
```

## Comparing `pcl_pangu-1.2.5.9.tar` & `pcl_pangu-1.2.6.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7675 2023-04-06 01:29:53.000000 pcl_pangu-1.2.5.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/
--rw-r--r--   0 root         (0) root         (0)      208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/context/
--rw-r--r--   0 root         (0) root         (0)      263 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/context/check_context.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-30 08:59:08.000000 pcl_pangu-1.2.5.9/pcl_pangu/context/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/dataset/
--rw-r--r--   0 root         (0) root         (0)      151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14926 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/pre_process_chinese.py
--rw-r--r--   0 root         (0) root         (0)     5255 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/preprocess_data_pangu.py
--rw-r--r--   0 root         (0) root         (0)     3754 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2bin.py
--rw-r--r--   0 root         (0) root         (0)     7133 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2mindrecord.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/
--rw-r--r--   0 root         (0) root         (0)      130 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/
--rw-r--r--   0 root         (0) root         (0)      259 2023-03-30 09:00:28.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7356 2023-03-30 09:05:32.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/alpha.py
--rw-r--r--   0 root         (0) root         (0)     7659 2023-04-03 04:58:33.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/config_alpha.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/
--rw-r--r--   0 root         (0) root         (0)      210 2023-04-03 01:24:00.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-03-30 10:24:57.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/config_evolution.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-03-30 10:26:27.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/evolution.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/launcher_torch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/
--rw-r--r--   0 root         (0) root         (0)      203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7213 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/config_mPangu.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/mPangu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15353 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py
--rw-r--r--   0 root         (0) root         (0)    17636 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/generate.py
--rw-r--r--   0 root         (0) root         (0)    64752 2023-04-12 09:14:56.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py
--rw-r--r--   0 root         (0) root         (0)     6406 2023-04-12 09:14:56.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py
--rw-r--r--   0 root         (0) root         (0)    12303 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py
--rw-r--r--   0 root         (0) root         (0)     9209 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py
--rw-r--r--   0 root         (0) root         (0)    68987 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py
--rw-r--r--   0 root         (0) root         (0)    36469 2023-04-03 06:24:29.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py
--rw-r--r--   0 root         (0) root         (0)    26625 2023-04-12 09:18:43.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.910656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/
--rw-r--r--   0 root         (0) root         (0)     2220 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md
--rw-r--r--   0 root         (0) root         (0)    14695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8683 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README-en.md
--rw-r--r--   0 root         (0) root         (0)     8335 2023-04-06 01:31:51.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README.md
--rw-r--r--   0 root         (0) root         (0)    31808 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23215 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py
--rw-r--r--   0 root         (0) root         (0)    11011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/
--rw-r--r--   0 root         (0) root         (0)      288 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/Makefile
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9841 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py
--rw-r--r--   0 root         (0) root         (0)    18923 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py
--rw-r--r--   0 root         (0) root         (0)    13647 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py
--rw-r--r--   0 root         (0) root         (0)    25244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp
--rw-r--r--   0 root         (0) root         (0)     5695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py
--rw-r--r--   0 root         (0) root         (0)    19128 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py
--rw-r--r--   0 root         (0) root         (0)     7721 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/
--rw-r--r--   0 root         (0) root         (0)      971 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32911 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py
--rw-r--r--   0 root         (0) root         (0)     8331 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py
--rw-r--r--   0 root         (0) root         (0)    10504 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 root         (0) root         (0)    19953 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 root         (0) root         (0)     2959 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 root         (0) root         (0)     7538 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py
--rw-r--r--   0 root         (0) root         (0)     4182 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py
--rw-r--r--   0 root         (0) root         (0)     5054 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/
--rw-r--r--   0 root         (0) root         (0)      936 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11546 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py
--rw-r--r--   0 root         (0) root         (0)     8364 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py
--rw-r--r--   0 root         (0) root         (0)     4283 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py
--rw-r--r--   0 root         (0) root         (0)     5151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py
--rw-r--r--   0 root         (0) root         (0)    27501 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py
--rw-r--r--   0 root         (0) root         (0)     4752 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py
--rw-r--r--   0 root         (0) root         (0)     8874 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py
--rw-r--r--   0 root         (0) root         (0)    36536 2023-03-30 03:27:44.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/
--rw-r--r--   0 root         (0) root         (0)     2144 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py
--rw-r--r--   0 root         (0) root         (0)     5025 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py
--rw-r--r--   0 root         (0) root         (0)     5733 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py
--rw-r--r--   0 root         (0) root         (0)    16415 2023-03-30 03:21:36.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py
--rw-r--r--   0 root         (0) root         (0)     4444 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py
--rw-r--r--   0 root         (0) root         (0)    13208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py
--rw-r--r--   0 root         (0) root         (0)    16248 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13952 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py
--rw-r--r--   0 root         (0) root         (0)    13780 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py
--rw-r--r--   0 root         (0) root         (0)     6864 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    21991 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py
--rw-r--r--   0 root         (0) root         (0)    23337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py
--rw-r--r--   0 root         (0) root         (0)     3960 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py
--rw-r--r--   0 root         (0) root         (0)     3681 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     3106 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/setup.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.914656 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/
--rw-r--r--   0 root         (0) root         (0)    16425 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py
--rw-r--r--   0 root         (0) root         (0)    10948 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py
--rw-r--r--   0 root         (0) root         (0)    10812 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py
--rw-r--r--   0 root         (0) root         (0)    11619 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py
--rw-r--r--   0 root         (0) root         (0)     7896 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py
--rw-r--r--   0 root         (0) root         (0)     9474 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15563 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1354 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/merge_pytorch_model.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/ms_2_numpy.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/numpy_2_pt.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/model_converter/split_pytorch_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/online/
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/
--rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3229 2023-04-06 09:12:13.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/infer.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-04-06 10:11:00.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_alpha_dto.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-04-06 10:10:09.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_evolution_dto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/
--rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1166 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/modelinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-04-04 01:24:04.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/conver_pt_onnx.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-03-30 09:53:40.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/
--rw-r--r--   0 root         (0) root         (0)     2125 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/config.py
--rw-r--r--   0 root         (0) root         (0)     9588 2023-04-03 13:33:22.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-04-03 13:53:20.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py
--rw-r--r--   0 root         (0) root         (0)     5040 2023-03-30 09:23:46.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/sample.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/utils.py
--rw-r--r--   0 root         (0) root         (0)     7867 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/
--rw-r--r--   0 root         (0) root         (0)      246 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.918655 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/
--rw-r--r--   0 root         (0) root         (0)   879697 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model
--rw-r--r--   0 root         (0) root         (0)   717452 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1991068 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt
--rw-r--r--   0 root         (0) root         (0)  2423393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1
--rw-r--r--   0 root         (0) root         (0)    14949 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-03-09 08:17:18.000000 pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/tokenization_jieba.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8394 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-12 09:19:44.000000 pcl_pangu-1.2.5.9/pcl_pangu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 09:19:44.922655 pcl_pangu-1.2.5.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1955 2023-04-12 09:19:21.000000 pcl_pangu-1.2.5.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.113314 pcl_pangu-1.2.6/
+-rw-r--r--   0 root         (0) root         (0)      287 2023-04-13 11:26:34.113314 pcl_pangu-1.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7675 2023-04-06 01:29:53.000000 pcl_pangu-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/context/
+-rw-r--r--   0 root         (0) root         (0)      263 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/context/check_context.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-03-30 08:59:08.000000 pcl_pangu-1.2.6/pcl_pangu/context/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/dataset/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14926 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/dataset/pre_process_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/dataset/preprocess_data_pangu.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/dataset/txt2bin.py
+-rw-r--r--   0 root         (0) root         (0)     7133 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/dataset/txt2mindrecord.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/alpha/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-04-12 09:58:15.000000 pcl_pangu-1.2.6/pcl_pangu/model/alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11490 2023-04-13 11:21:55.000000 pcl_pangu-1.2.6/pcl_pangu/model/alpha/alpha.py
+-rw-r--r--   0 root         (0) root         (0)     7659 2023-04-03 04:58:33.000000 pcl_pangu-1.2.6/pcl_pangu/model/alpha/config_alpha.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/evolution/
+-rw-r--r--   0 root         (0) root         (0)      210 2023-04-03 01:24:00.000000 pcl_pangu-1.2.6/pcl_pangu/model/evolution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-03-30 10:24:57.000000 pcl_pangu-1.2.6/pcl_pangu/model/evolution/config_evolution.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-03-30 10:26:27.000000 pcl_pangu-1.2.6/pcl_pangu/model/evolution/evolution.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/launcher_torch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/mPangu/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/mPangu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7213 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/mPangu/config_mPangu.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2023-04-13 11:23:13.000000 pcl_pangu-1.2.6/pcl_pangu/model/mPangu/mPangu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15353 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    17636 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/generate.py
+-rw-r--r--   0 root         (0) root         (0)    65013 2023-04-13 06:43:09.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py
+-rw-r--r--   0 root         (0) root         (0)     6491 2023-04-13 03:43:35.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py
+-rw-r--r--   0 root         (0) root         (0)     9209 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py
+-rw-r--r--   0 root         (0) root         (0)    68987 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py
+-rw-r--r--   0 root         (0) root         (0)    36469 2023-04-03 06:24:29.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py
+-rw-r--r--   0 root         (0) root         (0)    23369 2023-04-13 07:19:59.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.101315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-06 01:31:51.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-06 01:31:51.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md
+-rw-r--r--   0 root         (0) root         (0)    14695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8683 2023-04-06 01:31:51.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/README-en.md
+-rw-r--r--   0 root         (0) root         (0)     8335 2023-04-06 01:31:51.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/README.md
+-rw-r--r--   0 root         (0) root         (0)    31808 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23215 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py
+-rw-r--r--   0 root         (0) root         (0)    11011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/
+-rw-r--r--   0 root         (0) root         (0)      288 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/Makefile
+-rw-r--r--   0 root         (0) root         (0)       31 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    18923 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13647 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    25244 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    19128 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     7721 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/
+-rw-r--r--   0 root         (0) root         (0)      971 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32911 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py
+-rw-r--r--   0 root         (0) root         (0)     8331 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 root         (0) root         (0)    19953 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)     7538 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4182 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     5054 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/
+-rw-r--r--   0 root         (0) root         (0)      936 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11546 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py
+-rw-r--r--   0 root         (0) root         (0)     8364 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py
+-rw-r--r--   0 root         (0) root         (0)     4283 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py
+-rw-r--r--   0 root         (0) root         (0)     5151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py
+-rw-r--r--   0 root         (0) root         (0)    27501 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4752 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)     8874 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py
+-rw-r--r--   0 root         (0) root         (0)    36536 2023-03-30 03:27:44.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     4134 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py
+-rw-r--r--   0 root         (0) root         (0)     5025 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py
+-rw-r--r--   0 root         (0) root         (0)    16415 2023-03-30 03:21:36.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py
+-rw-r--r--   0 root         (0) root         (0)    13208 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py
+-rw-r--r--   0 root         (0) root         (0)    16248 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13952 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py
+-rw-r--r--   0 root         (0) root         (0)    13780 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py
+-rw-r--r--   0 root         (0) root         (0)     6864 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    21991 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23337 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py
+-rw-r--r--   0 root         (0) root         (0)       36 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.105315 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/
+-rw-r--r--   0 root         (0) root         (0)    16425 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py
+-rw-r--r--   0 root         (0) root         (0)    10812 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py
+-rw-r--r--   0 root         (0) root         (0)    11619 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     7896 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py
+-rw-r--r--   0 root         (0) root         (0)     9474 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/model_converter/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model_converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15563 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model_converter/merge_pytorch_model.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model_converter/ms_2_numpy.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model_converter/numpy_2_pt.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/model_converter/split_pytorch_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/online/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/online/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/online/infer/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/online/infer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-04-06 09:12:13.000000 pcl_pangu-1.2.6/pcl_pangu/online/infer/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-04-06 10:11:00.000000 pcl_pangu-1.2.6/pcl_pangu/online/infer/pangu_alpha_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-04-06 10:10:09.000000 pcl_pangu-1.2.6/pcl_pangu/online/infer/pangu_evolution_dto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/online/modelinfo/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/online/modelinfo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/online/modelinfo/modelinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-04-04 01:24:04.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/conver_pt_onnx.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-03-30 09:53:40.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/config.py
+-rw-r--r--   0 root         (0) root         (0)     9588 2023-04-03 13:33:22.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/model.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-04-03 13:53:20.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2023-03-30 09:23:46.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/sample.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7867 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/onnx_inference/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/tokenizer/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.109314 pcl_pangu-1.2.6/pcl_pangu/tokenizer/bpe_4w_pcl/
+-rw-r--r--   0 root         (0) root         (0)   879697 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model
+-rw-r--r--   0 root         (0) root         (0)   717452 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.113314 pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1991068 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt
+-rw-r--r--   0 root         (0) root         (0)  2423393 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1
+-rw-r--r--   0 root         (0) root         (0)    14949 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-03-09 08:17:18.000000 pcl_pangu-1.2.6/pcl_pangu/tokenizer/tokenization_jieba.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:26:34.113314 pcl_pangu-1.2.6/pcl_pangu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      287 2023-04-13 11:26:33.000000 pcl_pangu-1.2.6/pcl_pangu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8394 2023-04-13 11:26:33.000000 pcl_pangu-1.2.6/pcl_pangu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 11:26:33.000000 pcl_pangu-1.2.6/pcl_pangu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-13 11:26:33.000000 pcl_pangu-1.2.6/pcl_pangu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 11:26:33.000000 pcl_pangu-1.2.6/pcl_pangu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 11:26:34.113314 pcl_pangu-1.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-04-13 11:22:03.000000 pcl_pangu-1.2.6/setup.py
```

### Comparing `pcl_pangu-1.2.5.9/README.md` & `pcl_pangu-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/dataset/pre_process_chinese.py` & `pcl_pangu-1.2.6/pcl_pangu/dataset/pre_process_chinese.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/dataset/preprocess_data_pangu.py` & `pcl_pangu-1.2.6/pcl_pangu/dataset/preprocess_data_pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2bin.py` & `pcl_pangu-1.2.6/pcl_pangu/dataset/txt2bin.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/dataset/txt2mindrecord.py` & `pcl_pangu-1.2.6/pcl_pangu/dataset/txt2mindrecord.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/alpha.py` & `pcl_pangu-1.2.6/pcl_pangu/model/evolution/evolution.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,103 +2,88 @@
 # -*- coding: utf-8 -*-
 
 # @Date: 2022/7/20
 # @Author: 2022 PCL
 import os
 import sys
 from loguru import logger
-from ..launcher_torch import launch
 
 from pcl_pangu.context import check_context
-from .config_alpha import DISTRUBUTED_CONFIG, model_config_gpu, model_config_npu
+from pcl_pangu.model.launcher_torch import launch
+from pcl_pangu.model.evolution.config_evolution import DISTRUBUTED_CONFIG, model_config_gpu
 
 
 def train(config):
-    print('---------------------------- train config ----------------------------')
-    print("> Base Model: [alpha]")
+    print('----------------------------- training config -----------------------------')
+    print("> Base Model: [evolution]")
     print("> Model Size: [{}]".format(config.model))
     print("> data_path: {}".format(config.data_path))
     print("> global batch_size: {}".format(config.batch_size))
     print("> save to path: {}".format(config.save))
-    print('--------------------------- end of config ----------------------------')
+    print('------------------------------ end of config -----------------------------')
 
     if check_context()=='pytorch':
-        assert isinstance(config, model_config_gpu)
         script_args = config._get_training_script_args()
-        py_script = '/panguAlpha_pytorch/pretrain_gpt2.py'
+        py_script = '/panguAlpha_pytorch/pretrain_evolution.py'
         run_pt(script_args, py_script)
-    elif check_context()=='mindspore':
-        assert isinstance(config, model_config_npu)
-        config_dict = config._cover_modelarts_training_args()
-        run_ms_train(config_dict)
-
 
+    else:
+        print("ERROR: wrong backend.")
+        return 1
 
 def fine_tune(config):
-    print('-------------------------- finetune config ---------------------------')
-    print("> Base Model: [alpha]")
+    print('--------------------------- finetune config -----------------------------')
+    print("> Base Model: [evolution]")
     print("> Model Size: [{}]".format(config.model))
     print("> data_path: {}".format(config.data_path))
     print("> global batch_size: {}".format(config.batch_size))
     print("> save to path: {}".format(config.save))
-    print('--------------------------- end of config ----------------------------')
+    print('---------------------------- end of config -------------------------------')
 
     if check_context()=='pytorch':
-        from .config_alpha import DEFAULT_CONFIG
-        DEFAULT_CONFIG['finetune'] = True
         script_args = config._get_training_script_args()
-        py_script = '/panguAlpha_pytorch/pretrain_gpt2.py'
+        py_script = '/panguAlpha_pytorch/pretrain_evolution.py'
         run_pt(script_args, py_script)
-    elif check_context()=='mindspore':
-        assert isinstance(config, model_config_npu)
-        config_dict = config._cover_modelarts_training_args()
-        run_ms_train(config_dict)
 
+    else:
+        print("ERROR: wrong backend.")
+        return 1
 
-def inference(config,top_k=1,top_p=0.9,input=None,input_file=None,
-              generate_max_tokens=128, output_file=None,oneCardInference=True):
+def inference(config,top_k=1,top_p=0.9,input=None,input_file=None,output_file=None,
+              generate_max_tokens=128,oneCardInference=True):
 
     backend_context = check_context()
 
-    assert generate_max_tokens > 0 and generate_max_tokens <= 800, "> generate_max_tokens always in (0, 800]"
+    assert generate_max_tokens > 0 and generate_max_tokens<=800, "> generate_max_tokens always in (0, 800]"
     print('--------------------------- inference config --------------------------')
-    print("> Base Model: [alpha]")
+    print("> Base Model: [evolution]")
     print("> Model Size: [{}]".format(config.model))
     print("> global batch_size: {}".format(config.batch_size))
     print("> generate_max_tokens length: {}".format(generate_max_tokens))
     print('---------------------------- end of config ----------------------------')
 
-    if backend_context == 'pytorch':
-        from .config_alpha import DEFAULT_CONFIG
+    if backend_context=='pytorch':
+        from .config_evolution import DEFAULT_CONFIG
         DEFAULT_CONFIG['finetune'] = True
         config.batch_size = 1
         script_args = config._get_training_script_args(oneCardInference=oneCardInference)
-        py_script = '/panguAlpha_pytorch/tools/generate_samples_Pangu.py'
+        py_script = '/panguAlpha_pytorch/tools/generate_samples_epangu.py'
         script_args.append('--top-k={}'.format(top_k))
         script_args.append('--top-p={}'.format(top_p))
         if input is not None:
             script_args.append('--sample-input={}'.format(input.encode('utf-8').hex()))
         if input_file is not None:
             script_args.append('--sample-input-file={}'.format(input_file))
         if output_file is not None:
             script_args.append('--sample-output-file={}'.format(output_file))
         if generate_max_tokens is not None:
             script_args.append('--generate_max_tokens={}'.format(generate_max_tokens))
-        run_pt(script_args, py_script)
 
-    elif backend_context == 'mindspore':
-        assert isinstance(config, model_config_npu)
-        config_dict = config._cover_modelarts_training_args(oneCardInference=oneCardInference)
-        config_dict['top_k'] = top_k
-        config_dict['top_p'] = top_p
-        config_dict['input'] = input
-        config_dict['input_file'] = input_file
-        config_dict['output_file'] = output_file
-        config_dict['generate_max_tokens'] = generate_max_tokens
-        run_ms_inference(config_dict)
+        script_args.append('--isEvolution=True')
+        run_pt(script_args, py_script)
 
     elif 'onnx-' in backend_context:
         from pcl_pangu.onnx_inference.infer import onnx_generate
         from pcl_pangu.tokenizer.tokenization_jieba import get_tokenizer
 
         num_threads = 2
         past_path = None
@@ -108,58 +93,51 @@
                 past_path = os.path.join(config.load, filename)
             if filename.endswith('.onnx'):
                 model_path = os.path.join(config.load, filename)
 
         tokenizer = get_tokenizer()
         if input is not None:
             raw_text = input
-            output_samples = onnx_generate(raw_text, model_path, tokenizer, past_path,
-                                           topk=top_k, top_p=top_p, threads=num_threads,
+            output_samples = onnx_generate(raw_text,model_path,tokenizer,past_path,
+                                           topk=top_k,top_p=top_p,threads=num_threads,
                                            max_len=generate_max_tokens, backend=backend_context)
 
             print('Input is:', raw_text)
             print('Output is:', output_samples[len(raw_text):], flush=True)
             print()
 
         if input_file is not None:
             raw_texts = open(input_file, 'r').read().split('\n\n')
             write_output = print
             if output_file is not None:
                 output_file = open(output_file, 'w')
                 write_output = lambda x: output_file.write(x + '\n')
             for raw_text in raw_texts:
-                output_samples = onnx_generate(raw_text, model_path, tokenizer, past_path,
-                                               topk=top_k, top_p=top_p, threads=num_threads,
+                output_samples = onnx_generate(raw_text,model_path,tokenizer,past_path,
+                                               topk=top_k,top_p=top_p,threads=num_threads,
                                                max_len=generate_max_tokens, backend=backend_context)
                 write_output('Input is: ' + raw_text)
                 write_output('Output is: ' + output_samples[len(raw_text):])
                 write_output()
 
+    else:
+        print("ERROR: wrong backend.")
+        return 1
+
+
 def run_pt(script_args, py_script, **kwargs):
     current_dir = os.path.dirname(os.path.dirname(__file__))
-    sys.path.append(current_dir+'/panguAlpha_pytorch')
+    sys.path.append(current_dir + '/panguAlpha_pytorch')
+
     py_script = current_dir + py_script
     logger.info("> Running {} with args: {}".format(py_script, script_args))
+
     launch(training_script=py_script,
            training_script_args=script_args,
            **DISTRUBUTED_CONFIG,
            **kwargs)
+    return 0
 
 
-def run_ms_train(config_dict):
-    current_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.path.pardir))
-    sys.path.append(current_dir + '/panguAlpha_mindspore')
-    from train_alpha_ms13 import opt, setup_args, main, alpha_add_args
-    new_opt = setup_args(opt, config_dict)
-    new_opt = alpha_add_args(new_opt)
-    main(new_opt)
-
-def run_ms_inference(config_dict):
-    current_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.path.pardir))
-    sys.path.append(current_dir + '/panguAlpha_mindspore')
-    from inference_alpha_ms13 import opt, setup_args, main
-    new_opt = setup_args(opt, config_dict)
-    main(new_opt)
-
 if __name__ == '__main__':
     config = model_config_gpu()
-    run_pt(config)
+    inference(config)
```

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/alpha/config_alpha.py` & `pcl_pangu-1.2.6/pcl_pangu/model/alpha/config_alpha.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/evolution/config_evolution.py` & `pcl_pangu-1.2.6/pcl_pangu/model/evolution/config_evolution.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/launcher_torch.py` & `pcl_pangu-1.2.6/pcl_pangu/model/launcher_torch.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/mPangu/config_mPangu.py` & `pcl_pangu-1.2.6/pcl_pangu/model/mPangu/config_mPangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/inference_alpha_ms13.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/generate.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/generate.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -667,14 +667,15 @@
             # Position embedding
             if config.load_ckpt_path:
                 # Loading the embedding table from the ckpt path:
                 embedding_path = os.path.join(config.load_ckpt_path, 'position_embedding.npy')
                 if os.path.exists(embedding_path):
                     p_table = np.load(embedding_path)
                     position_table_param = Tensor(p_table, mstype.float32)
+                    print("###### loading Position embedding Table successed! ######")
                 else:
                     raise ValueError(f"{embedding_path} file not exits, "
                                      f"please check whether position_embedding file exit.")
             else:
                 position_table_param = TruncatedNormal(0.02)
             # Position embedding
             self.position_embedding = nn.Embedding(
@@ -957,14 +958,15 @@
             # self-attention layers, a new attention layer will be attached to the output of the model
             if config.load_ckpt_path:
                 # Loading the embedding table from the ckpt path:
                 embedding_path = os.path.join(config.load_ckpt_path, 'top_query_embedding.npy')
                 if os.path.exists(embedding_path):
                     top_query_table = np.load(embedding_path)
                     top_query_table_param = Tensor(top_query_table, mstype.float32)
+                    print("###### loading Toq_query embedding Table successed! ######")
                 else:
                     raise ValueError(
                         f"{embedding_path} file not exits, please check whether top_query_embedding file exist.")
             else:
                 top_query_table_param = TruncatedNormal(0.02)
             self.top_query_embedding_table = Parameter(initializer(top_query_table_param,
                                                                    [config.seq_length, config.embedding_size]),
@@ -1076,14 +1078,15 @@
             if config.load_ckpt_path:
                 # Loading the embedding table from the ckpt path:
                 embedding_path = os.path.join(config.load_ckpt_path, 'word_embedding.npy')
                 if os.path.exists(embedding_path):
                     e_table = np.load(embedding_path)
                     e_table = Tensor(e_table, mstype.float32)
                     self.embedding_table = Parameter(e_table, name="embedding_table", parallel_optimizer=False)
+                    print("###### loading Word embedding Table successed! ######")
                 else:
                     raise ValueError(f"{embedding_path} file not exits, "
                                      f"please check whether word_embedding file exist.")
             else:
                 self.embedding_table = Parameter(initializer(Normal(0.02), [self.vocab_size, self.embedding_size]),
                                                  name="embedding_table", parallel_optimizer=False)
```

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                  num_layers=12,
                  num_heads=12,
                  expand_ratio=4,
                  post_layernorm_residual=False,
                  dropout_rate=0.1,
                  compute_dtype=mstype.float16,
                  use_past=False,
+                 self_layernorm=True,
                  word_emb_dp=True,
                  stage_num=16,
                  eod_reset=True,
                  micro_size=32,
                  load_ckpt_path='/cache/ckpt_file',
                  use_top_query_attention=False,
                  param_init_type=mstype.float32):
@@ -55,14 +56,15 @@
         self.post_layernorm_residual = post_layernorm_residual
         self.dropout_rate = dropout_rate
         self.compute_dtype = compute_dtype
         # Whether use incremental inference
         self.use_past = use_past
         self.dp = data_parallel_num
         self.mp = model_parallel_num
+        self.self_layernorm = self_layernorm
         self.stage_num = stage_num
         self.micro_size = micro_size
         self.word_emb_dp = word_emb_dp
         self.eod_reset = eod_reset
         self.use_top_query_attention = use_top_query_attention
         self.param_init_type = param_init_type
         # Used for loading embedding tables
```

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/pangu_alpha_wrapcell.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/preprocess.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/serialization.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/tokenization_jieba.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/src/utils_pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_mindspore/train_alpha_ms13.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 from mindspore.parallel._cost_model_context import _set_multi_subgraphs
 from mindspore.nn.wrap.cell_wrapper import PipelineCell, _VirtualDatasetCell
 from mindspore.train.callback import ModelCheckpoint, CheckpointConfig
 from mindspore.train.serialization import load_checkpoint, load_param_into_net
 
 from src.dataset import create_dataset
 from src.pangu_alpha import PanguAlpha, PanguAlphaWithLoss, CrossEntropyLoss
+
+# from src.pangu_alpha_raw import PanguAlphaModel as PanguAlpha
+# from src.pangu_alpha_raw import PanGuAlphaWithLoss as PanguAlphaWithLoss
+# from src.pangu_alpha_raw import CrossEntropyLoss
+
 from src.pangu_alpha_wrapcell import PanguAlphaTrainOneStepWithLossScaleCell
 from src.pangu_alpha_config import PANGUALPHAConfig, set_parse
 from src.utils_pangu import LearningRate, get_args, FP32StateAdamWeightDecay
 from src.utils_pangu import download_data, get_openi_tar, ckpt_tar_openi, ckpt_copy_tar_new, get_ckpt_file_list
 from src.utils_pangu import StrategySaveCallback, CheckpointSaveCallback
 
 try:
@@ -132,16 +137,16 @@
         elif args_param.model == '13B':
             args_param.ckpt_name_prefix = args_param.base_model_type + '-13B'
         else:
             raise ImportError
         save_ckptfile_name = args_param.ckpt_name_prefix + '_' + str(rank_id)
         if not os.path.exists(save_dir_rank):
             os.makedirs(save_dir_rank, exist_ok=True)
-        print(">>> save_checkpoint_steps: {}, train_url: {}, save_name: {}>>>".format(args_param.save_checkpoint_steps,
-                                                                        args_param.train_url, save_ckptfile_name))
+        print(">>> save_checkpoint_steps: {}, train_url: {}, save_dir: {}, save_name: {}>>>".format(args_param.save_checkpoint_steps,
+                                                                        args_param.train_url, save_dir_rank, save_ckptfile_name))
         ckpoint_cb = ModelCheckpoint(prefix=save_ckptfile_name,
                                      directory=save_dir_rank,
                                      config=ckpt_config)
 
         # # need to compress mp_parellel_model to OneCKPT!!!! Disable OBS SYNC during Training!
         # ckpt_save_obs_cb = CheckpointSaveCallback(local_ckpt_dir=save_dir_rank,
         #                                           local_rank=rank_id,
@@ -440,88 +445,14 @@
     # 初始化，从头学习
     else:
         model._init(train_dataset=ds, sink_size=2)
     print("===== training {} epochs of dataset!!! ======".format(args_opt.train_iters / float(actual_epoch_num)))
     print("=====[{}/{}]: train_iters / actual_1epoch_iters: ".format(args_opt.train_iters, actual_epoch_num), flush=True)
     model.train(args_opt.train_iters, ds, callbacks=callback, sink_size=callback_size, dataset_sink_mode=True)
 
-    if args_opt.incremental_training:
-        # do merge
-        save_dir_rank = os.path.join(args_opt.save_checkpoint_path, f"rank_{rank_id}")
-        save_dir_strategy = os.path.join(args_opt.save_checkpoint_path, "strategy")
-        strategy = ms.build_searched_strategy("/cache/strategy.ckpt")
-        mp = args_opt.op_level_model_parallel_num
-        # load mp slice modelWeight
-
-        if rank_id % 8 == 0:
-            maxStepNumber = find_local_ckpt_maxStepNumber(save_dir_rank)
-
-            sliced_parameters = []
-            for i in range(mp):
-
-                save_dir_rank = os.path.join(args_opt.save_checkpoint_path, f"rank_{rank_id}")
-                os.system("ls {}".format(save_dir_rank))
-                save_ckptfile_name = args_opt.ckpt_name_prefix + '_' + str(rank_id)
-                # model_prefix = os.path.join(save_dir_rank, "alpha-2B6_{}-{}_2.ckpt".format(i, maxStepNumber))
-                model_prefix = os.path.join(save_dir_rank, "{}-{}_2.ckpt".format(save_ckptfile_name, maxStepNumber))
-
-                param_dict = ms.load_checkpoint(model_prefix)
-                adam_names = [item for item in param_dict.keys() if 'adam' in item]
-                for item in adam_names:
-                    param_dict.pop(item)
-                param_dict.pop("scale_sense")
-                param_dict.pop("global_step")
-                param_dict.pop("current_iterator_step")
-                param_dict.pop("last_overflow_iterator_step")
-                param_dict.pop("epoch_num")
-                param_dict.pop("step_num")
-
-                sliced_parameters.append(param_dict)
-
-            merged_parameter = {}
-            for key in sliced_parameters[0].keys():
-                this_merged_list = [sliced_parameters[0].get(key), sliced_parameters[1].get(key)]
-                this_merged_parameter = ms.merge_sliced_parameter(this_merged_list, strategy)
-                merged_parameter[key] = this_merged_parameter
-
-            ops_cast = ops.Cast()
-
-            param_list_fp32 = []
-            param_list_fp16 = []
-            for (key, value) in merged_parameter.items():
-                each_param_fp32 = {}
-                each_param_fp32["name"] = key
-                each_param_fp16 = {}
-                each_param_fp16["name"] = key
-                if isinstance(value.data, ms.Tensor):
-                    param_data = value.data
-                    param_data_fp16 = ops_cast(value.data, ms.float16)
-                else:
-                    param_data = ms.Tensor(value.data)
-                    param_data_fp16 = ops_cast(ms.Tensor(value.data), ms.float16)
-
-                # each_param_fp32["data"] = param_data
-                # param_list_fp32.append(each_param_fp32)
-
-                each_param_fp16["data"] = param_data_fp16
-                param_list_fp16.append(each_param_fp16)
-
-            ms.save_checkpoint(param_list_fp16, "alpha-2B6-{}_2-fp16.ckpt".format(maxStepNumber))
-            try:
-                mox.file.copy("alpha-2B6-{}_2-fp16.ckpt".format(maxStepNumber),
-                              os.path.join(args_opt.train_url, "alpha-2B6-fp16.ckpt"))
-            except:
-                pass
-            f = open("merge.txt", 'w')
-            f.close()
-        while not os.path.exists("merge.txt"):
-            time.sleep(1)
-
-        print('>>> merge mp={} model-slices to: {} >>>\n'.format(args_opt.op_level_model_parallel_num, args_opt.train_url))
-
 def find_local_ckpt_maxStepNumber(save_dir_rank):
     tmp_items = os.listdir(save_dir_rank)
     steps_numbers = []
     for item in tmp_items:
         if item.endswith('.ckpt') and 'alpha-2B6' in item:
             step_number = int(item.split('_2.ckpt')[0].split('-')[-1])
             steps_numbers.append(step_number)
```

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference-en.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/3-minus-inference.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/LICENSE` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/LICENSE`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README-en.md` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/README-en.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README.md` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/README.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/README_mgt.md`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/arguments.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/checkpointing.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/gpt2_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/helpers.cpp`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/ict_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/realm_index.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/data/samplers.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/fp16util.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/fused_kernels/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/global_vars.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/indexer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/initialize.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/learning_rates.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/memory.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/alpha_enhanced_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/bert_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/classification.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/distributed.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_bias_gelu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/language_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/mpu_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/realm_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/transformer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/model/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/module.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/data.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/grads.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/random.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/package_info.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/text_generation_utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/bert_tokenization.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/gpt2_tokenization.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenization_jieba.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/training.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/megatron/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/mergeMpCkpt.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_bert.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_evolution.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_gpt2.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/pretrain_ict.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/setup.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/setup.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/testLayerNorm.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/change_MspCkpt_ToMgt.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/create_doc_index.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_Pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/generate_samples_epangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/linter.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/merge_mp_partitions.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/preprocess_data_pangu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/splitMergedCkpt_v0.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model/panguAlpha_pytorch/tools/split_full_model_into_mp_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py` & `pcl_pangu-1.2.6/pcl_pangu/model_converter/_numpy_ckpt_2_pytorch.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/merge_pytorch_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model_converter/merge_pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/ms_2_numpy.py` & `pcl_pangu-1.2.6/pcl_pangu/model_converter/ms_2_numpy.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/numpy_2_pt.py` & `pcl_pangu-1.2.6/pcl_pangu/model_converter/numpy_2_pt.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/model_converter/split_pytorch_model.py` & `pcl_pangu-1.2.6/pcl_pangu/model_converter/split_pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/online/infer/infer.py` & `pcl_pangu-1.2.6/pcl_pangu/online/infer/infer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_alpha_dto.py` & `pcl_pangu-1.2.6/pcl_pangu/online/infer/pangu_alpha_dto.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/online/infer/pangu_evolution_dto.py` & `pcl_pangu-1.2.6/pcl_pangu/online/infer/pangu_evolution_dto.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/online/modelinfo/modelinfo.py` & `pcl_pangu-1.2.6/pcl_pangu/online/modelinfo/modelinfo.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/conver_pt_onnx.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/conver_pt_onnx.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/infer.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/infer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/config.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/config.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/model.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/model_onnx_gpu.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/sample.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/sample.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/pangu/utils.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/pangu/utils.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/onnx_inference/test.py` & `pcl_pangu-1.2.6/pcl_pangu/onnx_inference/test.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model` & `pcl_pangu-1.2.6/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.model`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab` & `pcl_pangu-1.2.6/pcl_pangu/tokenizer/bpe_4w_pcl/vocab.vocab`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt` & `pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/data_dict.128k.txt`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1` & `pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/spm.128k.model.1`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/spm_13w/tokenizer.py` & `pcl_pangu-1.2.6/pcl_pangu/tokenizer/spm_13w/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu/tokenizer/tokenization_jieba.py` & `pcl_pangu-1.2.6/pcl_pangu/tokenizer/tokenization_jieba.py`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/pcl_pangu.egg-info/SOURCES.txt` & `pcl_pangu-1.2.6/pcl_pangu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcl_pangu-1.2.5.9/setup.py` & `pcl_pangu-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  'loguru>=0.3.0']
 
 extras_require = \
 {':python_version < "3.7"': ['dataclasses==0.6']}
 
 setup_kwargs = {
     'name': 'pcl_pangu',
-    'version': '1.2.5.9',
+    'version': '1.2.6',
     'description': 'pcl_pangu',
     'long_description': '# pcl_pangu ',
     'author': '2022 PCL',
     'author_email': 'pcl.openi@pcl.ac.cn',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://openi.pcl.ac.cn/PCL-Platform.Intelligence/pcl_pangu',
```

