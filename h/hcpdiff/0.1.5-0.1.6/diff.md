# Comparing `tmp/hcpdiff-0.1.5.tar.gz` & `tmp/hcpdiff-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.1.5.tar", last modified: Wed Apr 12 09:55:12 2023, max compression
+gzip compressed data, was "hcpdiff-0.1.6.tar", last modified: Thu Apr 13 13:48:22 2023, max compression
```

## Comparing `hcpdiff-0.1.5.tar` & `hcpdiff-0.1.6.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.950890 hcpdiff-0.1.5/
--rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4856 2023-04-12 09:55:12.950890 hcpdiff-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4119 2023-04-12 09:50:49.000000 hcpdiff-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.899201 hcpdiff-0.1.5/cfgs/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.902195 hcpdiff-0.1.5/cfgs/infer/
--rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.1.5/cfgs/infer/change_vae.yaml
--rw-rw-rw-   0        0        0      651 2023-04-11 09:59:00.000000 hcpdiff-0.1.5/cfgs/infer/euler_a.yaml
--rw-rw-rw-   0        0        0     1413 2023-04-11 09:59:00.000000 hcpdiff-0.1.5/cfgs/infer/v1.yaml
--rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.1.5/cfgs/te_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.904192 hcpdiff-0.1.5/cfgs/train/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.911378 hcpdiff-0.1.5/cfgs/train/examples/
--rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/CustomDiffusion.yaml
--rw-rw-rw-   0        0        0     2680 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/DreamArtist++.yaml
--rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.1.5/cfgs/train/examples/DreamArtist.yaml
--rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/DreamBooth.yaml
--rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/TextualInversion.yaml
--rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/fine-tuning.yaml
--rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/locon.yaml
--rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/examples/lora_conventional.yaml
--rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/cfgs/train/train_base.yaml
--rw-rw-rw-   0        0        0      987 2023-04-11 08:41:31.000000 hcpdiff-0.1.5/cfgs/train/tuning_base.yaml
--rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.1.5/cfgs/unet_struct.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.915376 hcpdiff-0.1.5/hcpdiff/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.922376 hcpdiff-0.1.5/hcpdiff/data/
--rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/data/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/data/bucket.py
--rw-rw-rw-   0        0        0     5678 2023-04-12 06:39:19.000000 hcpdiff-0.1.5/hcpdiff/data/pair_dataset.py
--rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.929570 hcpdiff-0.1.5/hcpdiff/models/
--rw-rw-rw-   0        0        0      290 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/models/__init__.py
--rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/models/cfg_context.py
--rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/layers.py
--rw-rw-rw-   0        0        0     7732 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/lora.py
--rw-rw-rw-   0        0        0     7065 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/lora_layers.py
--rw-rw-rw-   0        0        0     4678 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/plugin.py
--rw-rw-rw-   0        0        0     3582 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/text_emb_ex.py
--rw-rw-rw-   0        0        0     5507 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/textencoder_ex.py
--rw-rw-rw-   0        0        0     2360 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/models/tokenizer_ex.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.935569 hcpdiff-0.1.5/hcpdiff/tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.1.5/hcpdiff/tools/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.1.5/hcpdiff/tools/convert_caption_txt2json.py
--rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/tools/create_embedding.py
--rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/tools/gen_from_ptlist.py
--rw-rw-rw-   0        0        0      654 2023-04-12 07:55:01.000000 hcpdiff-0.1.5/hcpdiff/tools/init_proj.py
--rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/tools/merge_model_part.py
--rw-rw-rw-   0        0        0     7233 2023-04-12 09:50:49.000000 hcpdiff-0.1.5/hcpdiff/tools/sd2diffusers.py
--rw-rw-rw-   0        0        0    23465 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/train_ac.py
--rw-rw-rw-   0        0        0     1827 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/train_ac_single.py
--rw-rw-rw-   0        0        0     9171 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/train_colo.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.941884 hcpdiff-0.1.5/hcpdiff/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.1.5/hcpdiff/utils/caption_tools.py
--rw-rw-rw-   0        0        0     7789 2023-04-11 12:47:28.000000 hcpdiff-0.1.5/hcpdiff/utils/cfg_net_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.944887 hcpdiff-0.1.5/hcpdiff/utils/ckpt_manager/
--rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/ckpt_manager/__init__.py
--rw-rw-rw-   0        0        0     2390 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
--rw-rw-rw-   0        0        0     1833 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
--rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/colo_utils.py
--rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/ema.py
--rw-rw-rw-   0        0        0      448 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/emb_utils.py
--rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/img_size_tool.py
--rw-rw-rw-   0        0        0     6623 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/utils/utils.py
--rw-rw-rw-   0        0        0     4215 2023-04-11 12:30:15.000000 hcpdiff-0.1.5/hcpdiff/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.919367 hcpdiff-0.1.5/hcpdiff.egg-info/
--rw-rw-rw-   0        0        0     4856 2023-04-12 09:55:12.000000 hcpdiff-0.1.5/hcpdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1935 2023-04-12 09:55:12.000000 hcpdiff-0.1.5/hcpdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:55:12.000000 hcpdiff-0.1.5/hcpdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-12 09:55:12.000000 hcpdiff-0.1.5/hcpdiff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      225 2023-04-12 09:55:12.000000 hcpdiff-0.1.5/hcpdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 09:55:12.000000 hcpdiff-0.1.5/hcpdiff.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 09:55:12.949890 hcpdiff-0.1.5/prompt_tuning_template/
--rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.1.5/prompt_tuning_template/caption.txt
--rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.1.5/prompt_tuning_template/name.txt
--rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.1.5/prompt_tuning_template/name_2pt_caption.txt
--rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.1.5/prompt_tuning_template/name_caption.txt
--rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.1.5/prompt_tuning_template/object.txt
--rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.1.5/prompt_tuning_template/style.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 09:55:12.950890 hcpdiff-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1833 2023-04-12 09:55:07.000000 hcpdiff-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.736085 hcpdiff-0.1.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-11 12:44:40.000000 hcpdiff-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4856 2023-04-13 13:48:22.735091 hcpdiff-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4119 2023-04-12 09:50:49.000000 hcpdiff-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.611278 hcpdiff-0.1.6/cfgs/
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.616777 hcpdiff-0.1.6/cfgs/infer/
+-rw-rw-rw-   0        0        0      179 2023-04-11 09:59:00.000000 hcpdiff-0.1.6/cfgs/infer/change_vae.yaml
+-rw-rw-rw-   0        0        0      672 2023-04-12 10:04:24.000000 hcpdiff-0.1.6/cfgs/infer/euler_a.yaml
+-rw-rw-rw-   0        0        0     1441 2023-04-12 10:04:24.000000 hcpdiff-0.1.6/cfgs/infer/v1.yaml
+-rw-rw-rw-   0        0        0     9971 2023-03-22 01:36:55.000000 hcpdiff-0.1.6/cfgs/te_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.621591 hcpdiff-0.1.6/cfgs/train/
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.634567 hcpdiff-0.1.6/cfgs/train/examples/
+-rw-rw-rw-   0        0        0     1846 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/CustomDiffusion.yaml
+-rw-rw-rw-   0        0        0     2807 2023-04-13 13:47:11.000000 hcpdiff-0.1.6/cfgs/train/examples/DreamArtist++.yaml
+-rw-rw-rw-   0        0        0     1334 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/cfgs/train/examples/DreamArtist.yaml
+-rw-rw-rw-   0        0        0     1644 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/DreamBooth.yaml
+-rw-rw-rw-   0        0        0     1124 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/TextualInversion.yaml
+-rw-rw-rw-   0        0        0     1178 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/fine-tuning.yaml
+-rw-rw-rw-   0        0        0     1397 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/locon.yaml
+-rw-rw-rw-   0        0        0     1228 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/examples/lora_conventional.yaml
+-rw-rw-rw-   0        0        0     2904 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/cfgs/train/train_base.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-11 08:41:31.000000 hcpdiff-0.1.6/cfgs/train/tuning_base.yaml
+-rw-rw-rw-   0        0        0    46121 2023-03-22 01:36:55.000000 hcpdiff-0.1.6/cfgs/unet_struct.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.643674 hcpdiff-0.1.6/hcpdiff/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.662458 hcpdiff-0.1.6/hcpdiff/data/
+-rw-rw-rw-   0        0        0      138 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/data/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/data/bucket.py
+-rw-rw-rw-   0        0        0     5678 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/hcpdiff/data/pair_dataset.py
+-rw-rw-rw-   0        0        0     1686 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.681221 hcpdiff-0.1.6/hcpdiff/models/
+-rw-rw-rw-   0        0        0      290 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/models/__init__.py
+-rw-rw-rw-   0        0        0     1422 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/models/cfg_context.py
+-rw-rw-rw-   0        0        0     3068 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/layers.py
+-rw-rw-rw-   0        0        0     7732 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/lora.py
+-rw-rw-rw-   0        0        0     7067 2023-04-13 07:55:06.000000 hcpdiff-0.1.6/hcpdiff/models/lora_layers.py
+-rw-rw-rw-   0        0        0     5721 2023-04-13 07:55:06.000000 hcpdiff-0.1.6/hcpdiff/models/plugin.py
+-rw-rw-rw-   0        0        0     3582 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/text_emb_ex.py
+-rw-rw-rw-   0        0        0     5507 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/textencoder_ex.py
+-rw-rw-rw-   0        0        0     2360 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/models/tokenizer_ex.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.694428 hcpdiff-0.1.6/hcpdiff/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/hcpdiff/tools/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-12 08:25:47.000000 hcpdiff-0.1.6/hcpdiff/tools/convert_caption_txt2json.py
+-rw-rw-rw-   0        0        0     1981 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/tools/create_embedding.py
+-rw-rw-rw-   0        0        0     1718 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/tools/gen_from_ptlist.py
+-rw-rw-rw-   0        0        0      654 2023-04-12 07:55:01.000000 hcpdiff-0.1.6/hcpdiff/tools/init_proj.py
+-rw-rw-rw-   0        0        0     4585 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/tools/merge_model_part.py
+-rw-rw-rw-   0        0        0     7233 2023-04-12 09:50:49.000000 hcpdiff-0.1.6/hcpdiff/tools/sd2diffusers.py
+-rw-rw-rw-   0        0        0    23465 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/train_ac.py
+-rw-rw-rw-   0        0        0     1827 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/train_ac_single.py
+-rw-rw-rw-   0        0        0     9171 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/train_colo.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.712161 hcpdiff-0.1.6/hcpdiff/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-04-12 06:39:19.000000 hcpdiff-0.1.6/hcpdiff/utils/caption_tools.py
+-rw-rw-rw-   0        0        0     7789 2023-04-11 12:47:28.000000 hcpdiff-0.1.6/hcpdiff/utils/cfg_net_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.720183 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/
+-rw-rw-rw-   0        0        0       82 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/__init__.py
+-rw-rw-rw-   0        0        0     2390 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_pkl.py
+-rw-rw-rw-   0        0        0     1833 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
+-rw-rw-rw-   0        0        0      860 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/colo_utils.py
+-rw-rw-rw-   0        0        0     3065 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/ema.py
+-rw-rw-rw-   0        0        0      448 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/emb_utils.py
+-rw-rw-rw-   0        0        0     8680 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/img_size_tool.py
+-rw-rw-rw-   0        0        0     6623 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/utils/utils.py
+-rw-rw-rw-   0        0        0     4215 2023-04-11 12:30:15.000000 hcpdiff-0.1.6/hcpdiff/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.655783 hcpdiff-0.1.6/hcpdiff.egg-info/
+-rw-rw-rw-   0        0        0     4856 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1961 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      225 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 13:48:22.000000 hcpdiff-0.1.6/hcpdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.733097 hcpdiff-0.1.6/prompt_tuning_template/
+-rw-rw-rw-   0        0        0       14 2023-04-03 03:15:56.000000 hcpdiff-0.1.6/prompt_tuning_template/caption.txt
+-rw-rw-rw-   0        0        0       14 2023-02-21 02:34:54.000000 hcpdiff-0.1.6/prompt_tuning_template/name.txt
+-rw-rw-rw-   0        0        0       55 2023-02-21 02:36:10.000000 hcpdiff-0.1.6/prompt_tuning_template/name_2pt_caption.txt
+-rw-rw-rw-   0        0        0       25 2023-03-22 03:52:13.000000 hcpdiff-0.1.6/prompt_tuning_template/name_caption.txt
+-rw-rw-rw-   0        0        0      915 2023-04-02 01:48:02.000000 hcpdiff-0.1.6/prompt_tuning_template/object.txt
+-rw-rw-rw-   0        0        0      890 2023-04-11 08:41:31.000000 hcpdiff-0.1.6/prompt_tuning_template/style.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 13:48:22.736085 hcpdiff-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1833 2023-04-13 13:48:19.000000 hcpdiff-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 13:48:22.734085 hcpdiff-0.1.6/test/
+-rw-rw-rw-   0        0        0      592 2023-04-13 07:54:04.000000 hcpdiff-0.1.6/test/test_plugin_param.py
```

### Comparing `hcpdiff-0.1.5/LICENSE` & `hcpdiff-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/PKG-INFO` & `hcpdiff-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.1.5
+Version: 0.1.6
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.1.5/README.md` & `hcpdiff-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/infer/v1.yaml` & `hcpdiff-0.1.6/cfgs/infer/v1.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -22,30 +22,30 @@
   exp_dir: '2023-04-03-10-10-36'
   alpha: 0.8
 
   group1:
     type: 'unet'
     base_model_alpha: 1.0 # base model weight to merge with lora or part
     lora:
-      - path: 'exps/${....exp_dir}/ckpts/unet-600.ckpt'
+      - path: 'exps/${....exp_dir}/ckpts/unet-600.safetensors'
         alpha: ${....alpha}
         layers: 'all'
         mask: [0.5, 1]
-      - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.ckpt'
+      - path: 'exps/${....exp_dir}/ckpts/unet-neg-600.safetensors'
         alpha: 0.65
         layers: 'all'
         mask: [0, 0.5]
     part: null
 
   group2:
     type: 'TE'
     base_model_alpha: 1.0 # base model weight to infer with lora or part
     lora:
-      - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.ckpt'
+      - path: 'exps/${....exp_dir}/ckpts/text_encoder-600.safetensors'
         alpha: ${....alpha}
         layers: 'all'
         mask: [0.5, 1]
-      - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.ckpt'
+      - path: 'exps/${....exp_dir}/ckpts/text_encoder-neg-600.safetensors'
         alpha: 0.65
         layers: 'all'
         mask: [0, 0.5]
     part: null
```

### Comparing `hcpdiff-0.1.5/cfgs/te_struct.txt` & `hcpdiff-0.1.6/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/DreamArtist++.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 lora_unet:
   - lr: 1e-4
     rank: 0.01875
     type: p
     layers:
       - 're:.*\.attn.?$'
-      - 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
+      #- 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
   - lr: 4e-5 # Low negative unet lr prevents image collapse
     rank: 0.01875
     type: n
     layers:
       - 're:.*\.attn.?$'
-      - 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
+      #- 're:.*\.ff\.net\.0$' # Increases fitness, but potentially reduces controllability
   #  - lr: 1e-4
   #    rank: 0.01875
   #    type: p
   #    layers:
   #      - 're:.*\.resnets$' # Increases fitness, but potentially reduces controllability and change style
   #  - lr: 4e-5
   #    rank: 0.01875
@@ -53,14 +53,20 @@
   cfg_scale: '3.0'
 
   scheduler:
     name: 'constant_with_warmup'
     num_warmup_steps: 50
     num_training_steps: 1000
 
+  scheduler_pt:
+    name: 'one_cycle'
+    num_warmup_steps: 200
+    num_training_steps: 1000
+    scheduler_kwargs: {}
+
 model:
   pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
   tokenizer_repeats: 1
   ema_unet: 0
   ema_text_encoder: 0
 
 data:
```

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/DreamArtist.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/DreamBooth.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/DreamBooth.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/TextualInversion.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/fine-tuning.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/fine-tuning.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/locon.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/locon.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/examples/lora_conventional.yaml` & `hcpdiff-0.1.6/cfgs/train/examples/lora_conventional.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/train_base.yaml` & `hcpdiff-0.1.6/cfgs/train/train_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/train/tuning_base.yaml` & `hcpdiff-0.1.6/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/cfgs/unet_struct.txt` & `hcpdiff-0.1.6/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/data/bucket.py` & `hcpdiff-0.1.6/hcpdiff/data/bucket.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.1.6/hcpdiff/data/pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/data/utils.py` & `hcpdiff-0.1.6/hcpdiff/data/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/models/cfg_context.py` & `hcpdiff-0.1.6/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/models/layers.py` & `hcpdiff-0.1.6/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/models/lora.py` & `hcpdiff-0.1.6/hcpdiff/models/lora.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/models/lora_layers.py` & `hcpdiff-0.1.6/hcpdiff/models/lora_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.host = host
         self.rank = rank
         self.dropout = nn.Dropout(dropout)
         self.host_type = None
         self.bias = bias
 
         if isinstance(self.rank, float):
-            self.rank = max(round(host.out_features * self.rank), 1)
+            self.rank = max(round(host().out_features * self.rank), 1)
 
         self.build_layers()
 
     def build_layers(self):
         pass
 
     def feed_sdv(self, U, V, weight):
```

### Comparing `hcpdiff-0.1.5/hcpdiff/models/plugin.py` & `hcpdiff-0.1.6/hcpdiff/models/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,42 @@
 
     def layer_hook(self, host, fea_in:Tuple[torch.Tensor], fea_out:torch.Tensor):
         return self(fea_in, fea_out)
 
     def remove(self):
         self.hook_handle.remove()
 
+class SinglePluginParameter(BasePluginBlock):
+    def __init__(self, layer:nn.Module, hook_target='weight'):
+        super().__init__()
+        self.host = weakref.ref(layer)
+        self.backup = getattr(layer, hook_target)
+        self.target = hook_target
+        self.handle_pre = layer.register_forward_pre_hook(self.pre_hook)
+        self.handle_post = layer.register_forward_hook(self.post_hook)
+
+    def forward(self, host_param: nn.Parameter):
+        return host_param
+
+    def pre_hook(self, host, fea_in:torch.Tensor):
+        host.weight_restored = False
+        host_param = getattr(host, self.target)
+        delattr(host, self.target)
+        setattr(host, self.target, self(host_param))
+        return fea_in
+
+    def post_hook(self, host, fea_int, fea_out):
+        if not getattr(host, 'weight_restored', False):
+            setattr(host, self.target, self.backup)
+            host.weight_restored = True
+
+    def remove(self):
+        self.handle_pre.remove()
+        self.handle_post.remove()
+
 class PluginBlock(BasePluginBlock):
     def __init__(self, from_layer:nn.Module, to_layer:nn.Module, pre_hook_to=False):
         super().__init__()
         self.host_from = weakref.ref(from_layer)
         self.host_to = weakref.ref(to_layer)
         #self.pre_hook_to = pre_hook_to
```

### Comparing `hcpdiff-0.1.5/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.1.6/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.1.6/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.1.6/hcpdiff/models/tokenizer_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.1.6/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.1.6/hcpdiff/tools/create_embedding.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.1.6/hcpdiff/tools/gen_from_ptlist.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/tools/init_proj.py` & `hcpdiff-0.1.6/hcpdiff/tools/init_proj.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/tools/merge_model_part.py` & `hcpdiff-0.1.6/hcpdiff/tools/merge_model_part.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.1.6/hcpdiff/tools/sd2diffusers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/train_ac.py` & `hcpdiff-0.1.6/hcpdiff/train_ac.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/train_ac_single.py` & `hcpdiff-0.1.6/hcpdiff/train_ac_single.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/train_colo.py` & `hcpdiff-0.1.6/hcpdiff/train_colo.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.1.6/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.1.6/hcpdiff/utils/cfg_net_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_pkl.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.1.6/hcpdiff/utils/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.1.6/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/ema.py` & `hcpdiff-0.1.6/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.1.6/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/utils/utils.py` & `hcpdiff-0.1.6/hcpdiff/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff/visualizer.py` & `hcpdiff-0.1.6/hcpdiff/visualizer.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.1.6/hcpdiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.1.5
+Version: 0.1.6
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hcpdiff-0.1.5/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.1.6/hcpdiff.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -59,8 +59,9 @@
 hcpdiff/utils/ckpt_manager/ckpt_pkl.py
 hcpdiff/utils/ckpt_manager/ckpt_safetensor.py
 prompt_tuning_template/caption.txt
 prompt_tuning_template/name.txt
 prompt_tuning_template/name_2pt_caption.txt
 prompt_tuning_template/name_caption.txt
 prompt_tuning_template/object.txt
-prompt_tuning_template/style.txt
+prompt_tuning_template/style.txt
+test/test_plugin_param.py
```

### Comparing `hcpdiff-0.1.5/prompt_tuning_template/object.txt` & `hcpdiff-0.1.6/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/prompt_tuning_template/style.txt` & `hcpdiff-0.1.6/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.1.5/setup.py` & `hcpdiff-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.1.5",
+    version="0.1.6",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

