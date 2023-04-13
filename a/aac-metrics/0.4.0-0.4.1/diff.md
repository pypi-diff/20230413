# Comparing `tmp/aac-metrics-0.4.0.tar.gz` & `tmp/aac-metrics-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aac-metrics-0.4.0.tar", last modified: Thu Apr 13 14:04:55 2023, max compression
+gzip compressed data, was "aac-metrics-0.4.1.tar", last modified: Thu Apr 13 14:21:04 2023, max compression
```

## Comparing `aac-metrics-0.4.0.tar` & `aac-metrics-0.4.1.tar`

### file list

```diff
@@ -1,108 +1,102 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.738138 aac-metrics-0.4.0/.github/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.742138 aac-metrics-0.4.0/.github/workflows/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1891 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/.github/workflows/python-package-pip.yaml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.0/LICENCE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      135 2022-10-31 09:45:25.000000 aac-metrics-0.4.0/MANIFEST.in
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11098 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/README.md
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/examples/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/examples/example_1.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2022-09-30 12:10:31.000000 aac-metrics-0.4.0/examples/example_2.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/install_spice.sh
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1954 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.738138 aac-metrics-0.4.0/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.742138 aac-metrics-0.4.0/src/aac_metrics/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/src/aac_metrics/__main__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/src/aac_metrics/classes/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2023-03-16 14:40:20.000000 aac-metrics-0.4.0/src/aac_metrics/classes/base.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2528 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/classes/fluency_error.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/fluerr.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2286 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/classes/sbert.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/sbert_sim.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4222 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider_err.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider_fl.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7654 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7466 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/evaluate.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/src/aac_metrics/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9592 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9590 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15053 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/functional/fluency_error.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/fluerr.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/mult_cands.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3949 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/functional/sbert.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/sbert_sim.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5128 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider_err.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider_fl.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/src/aac_metrics/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/src/aac_metrics/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/src/aac_metrics/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2973 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/utils/checks.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.0/src/aac_metrics/utils/collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.0/src/aac_metrics/utils/imports.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7678 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/utils/tokenization.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.750138 aac-metrics-0.4.0/src/aac_metrics.egg-info/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4284 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/tests/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/eval_metrics.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_bleu_tchmet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4279 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_compare_cet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3906 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_compare_fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_pickable.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1024 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.598118 aac-metrics-0.4.1/.github/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/.github/workflows/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1891 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/.github/workflows/python-package-pip.yaml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.1/LICENCE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      135 2022-10-31 09:45:25.000000 aac-metrics-0.4.1/MANIFEST.in
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11098 2023-04-13 14:18:42.000000 aac-metrics-0.4.1/README.md
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/examples/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/examples/example_1.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2022-09-30 12:10:31.000000 aac-metrics-0.4.1/examples/example_2.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/install_spice.sh
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1954 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.598118 aac-metrics-0.4.1/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/src/aac_metrics/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-04-13 14:18:42.000000 aac-metrics-0.4.1/src/aac_metrics/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/src/aac_metrics/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/src/aac_metrics/classes/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2023-03-16 14:40:20.000000 aac-metrics-0.4.1/src/aac_metrics/classes/base.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/classes/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/classes/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7654 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7466 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/evaluate.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/src/aac_metrics/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9592 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9590 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/mult_cands.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.1/src/aac_metrics/functional/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/src/aac_metrics/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/src/aac_metrics/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.1/src/aac_metrics/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2973 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/utils/checks.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.1/src/aac_metrics/utils/collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.1/src/aac_metrics/utils/imports.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7678 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/src/aac_metrics/utils/tokenization.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/src/aac_metrics.egg-info/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4051 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-04-13 14:21:04.000000 aac-metrics-0.4.1/src/aac_metrics.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.610118 aac-metrics-0.4.1/tests/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.602118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:21:04.606118 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.1/tests/caption-evaluation-tools/eval_metrics.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_bleu_tchmet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4279 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_compare_cet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3906 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_compare_fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_pickable.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1024 2023-04-13 14:01:18.000000 aac-metrics-0.4.1/tests/test_utils.py
```

### Comparing `aac-metrics-0.4.0/.github/workflows/python-package-pip.yaml` & `aac-metrics-0.4.1/.github/workflows/python-package-pip.yaml`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/LICENCE` & `aac-metrics-0.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/PKG-INFO` & `aac-metrics-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.4.0
+Version: 0.4.1
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/
 Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
 Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
@@ -239,15 +239,15 @@
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
     month = {4},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.0},
+    version = {0.4.1},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.0 Summary: Metrics for
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.1 Summary: Metrics for
 evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
 email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
 repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
 https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
@@ -139,9 +139,9 @@
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
 license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.0}, year = {2023}, } ``` ##
+github.com/Labbeti/aac-metrics/}, version = {0.4.1}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.0/README.md` & `aac-metrics-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
     month = {4},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.0},
+    version = {0.4.1},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -123,9 +123,9 @@
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
 license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.0}, year = {2023}, } ``` ##
+github.com/Labbeti/aac-metrics/}, version = {0.4.1}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.0/examples/example_1.csv` & `aac-metrics-0.4.1/examples/example_1.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/examples/example_2.csv` & `aac-metrics-0.4.1/examples/example_2.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/install_spice.sh` & `aac-metrics-0.4.1/install_spice.sh`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/pyproject.toml` & `aac-metrics-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/__init__.py` & `aac-metrics-0.4.1/src/aac_metrics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __name__ = "aac-metrics"
 __author__ = "Etienne Labbé (Labbeti)"
 __author_email__ = "labbeti.pub@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "Etienne Labbé (Labbeti)"
 __status__ = "Development"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 from .classes.base import AACMetric
 from .classes.bleu import BLEU
 from .classes.cider_d import CIDErD
 from .classes.evaluate import AACEvaluate, _get_metric_factory_classes
 from .classes.fense import FENSE
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/__main__.py` & `aac-metrics-0.4.1/src/aac_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/__init__.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/base.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/base.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/bleu.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/cider_d.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/cider_d.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/evaluate.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/fense.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/fluency_error.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/fluerr.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 from typing import Union
 
 import torch
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
-from aac_metrics.functional.fluency_error import (
-    fluency_error,
+from aac_metrics.functional.fluerr import (
+    fluerr,
     _load_echecker_and_tokenizer,
     ERROR_NAMES,
 )
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
-class FluencyError(AACMetric):
-    """Return fluency error detected by a pre-trained BERT model.
+class FluErr(AACMetric):
+    """Return fluency error rate detected by a pre-trained BERT model.
 
     - Paper: https://arxiv.org/abs/2110.04684
     - Original implementation: https://github.com/blmoistawinde/fense
 
-    For more information, see :func:`~aac_metrics.functional.fluency_error.fluency_error`.
+    For more information, see :func:`~aac_metrics.functional.fluerr.fluerr`.
     """
 
     full_state_update = False
     higher_is_better = False
     is_differentiable = False
 
     min_value = -1.0
@@ -40,48 +40,51 @@
         self,
         return_all_scores: bool = True,
         echecker: str = "echecker_clotho_audiocaps_base",
         error_threshold: float = 0.9,
         device: Union[str, torch.device, None] = "auto",
         batch_size: int = 32,
         reset_state: bool = True,
+        return_probs: bool = True,
         verbose: int = 0,
     ) -> None:
         echecker, echecker_tokenizer = _load_echecker_and_tokenizer(echecker, None, device, reset_state, verbose)  # type: ignore
 
         super().__init__()
         self._return_all_scores = return_all_scores
         self._echecker = echecker
         self._echecker_tokenizer = echecker_tokenizer
         self._error_threshold = error_threshold
         self._device = device
         self._batch_size = batch_size
         self._reset_state = reset_state
+        self._return_probs = return_probs
         self._verbose = verbose
 
         self._candidates = []
 
     def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
-        return fluency_error(
+        return fluerr(
             self._candidates,
             self._return_all_scores,
             self._echecker,
             self._echecker_tokenizer,
             self._error_threshold,
             self._device,
             self._batch_size,
             self._reset_state,
+            self._return_probs,
             self._verbose,
         )
 
     def extra_repr(self) -> str:
         return f"device={self._device}, batch_size={self._batch_size}"
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("fluency_error",) + tuple(f"fluerr.{name}_prob" for name in ERROR_NAMES)
+        return ("fluerr",) + tuple(f"fluerr.{name}_prob" for name in ERROR_NAMES)
 
     def reset(self) -> None:
         self._candidates = []
         return super().reset()
 
     def update(
         self,
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/fluerr.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/sbert_sim.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,93 +3,85 @@
 
 import logging
 
 from typing import Union
 
 import torch
 
+from sentence_transformers import SentenceTransformer
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
-from aac_metrics.functional.fluerr import (
-    fluerr,
-    _load_echecker_and_tokenizer,
-    ERROR_NAMES,
-)
+from aac_metrics.functional.sbert_sim import sbert_sim, _load_sbert
 
 
 pylog = logging.getLogger(__name__)
 
 
-class FluErr(AACMetric):
-    """Return fluency error rate detected by a pre-trained BERT model.
+class SBERTSim(AACMetric):
+    """Cosine-similarity of the Sentence-BERT embeddings.
 
-    - Paper: https://arxiv.org/abs/2110.04684
+    - Paper: https://arxiv.org/abs/1908.10084
     - Original implementation: https://github.com/blmoistawinde/fense
 
-    For more information, see :func:`~aac_metrics.functional.fluerr.fluerr`.
+    For more information, see :func:`~aac_metrics.functional.sbert.sbert`.
     """
 
     full_state_update = False
-    higher_is_better = False
+    higher_is_better = True
     is_differentiable = False
 
     min_value = -1.0
     max_value = 1.0
 
     def __init__(
         self,
         return_all_scores: bool = True,
-        echecker: str = "echecker_clotho_audiocaps_base",
-        error_threshold: float = 0.9,
+        sbert_model: Union[str, SentenceTransformer] = "paraphrase-TinyBERT-L6-v2",
         device: Union[str, torch.device, None] = "auto",
         batch_size: int = 32,
         reset_state: bool = True,
-        return_probs: bool = True,
         verbose: int = 0,
     ) -> None:
-        echecker, echecker_tokenizer = _load_echecker_and_tokenizer(echecker, None, device, reset_state, verbose)  # type: ignore
+        sbert_model = _load_sbert(sbert_model, device, reset_state)
 
         super().__init__()
         self._return_all_scores = return_all_scores
-        self._echecker = echecker
-        self._echecker_tokenizer = echecker_tokenizer
-        self._error_threshold = error_threshold
+        self._sbert_model = sbert_model
         self._device = device
         self._batch_size = batch_size
         self._reset_state = reset_state
-        self._return_probs = return_probs
         self._verbose = verbose
 
         self._candidates = []
+        self._mult_references = []
 
     def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
-        return fluerr(
+        return sbert_sim(
             self._candidates,
+            self._mult_references,
             self._return_all_scores,
-            self._echecker,
-            self._echecker_tokenizer,
-            self._error_threshold,
+            self._sbert_model,
             self._device,
             self._batch_size,
             self._reset_state,
-            self._return_probs,
             self._verbose,
         )
 
     def extra_repr(self) -> str:
         return f"device={self._device}, batch_size={self._batch_size}"
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("fluerr",) + tuple(f"fluerr.{name}_prob" for name in ERROR_NAMES)
+        return ("sbert.sim",)
 
     def reset(self) -> None:
         self._candidates = []
+        self._mult_references = []
         return super().reset()
 
     def update(
         self,
         candidates: list[str],
-        *args,
-        **kwargs,
+        mult_references: list[list[str]],
     ) -> None:
         self._candidates += candidates
+        self._mult_references += mult_references
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/meteor.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/rouge_l.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/sbert.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/spice.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,84 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 
-from typing import Union
-
-import torch
+from typing import Iterable, Optional, Union
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
-from aac_metrics.functional.sbert import sbert, _load_sbert
+from aac_metrics.functional.spice import spice
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
-class SBERT(AACMetric):
-    """Cosine-similarity of the Sentence-BERT embeddings.
+class SPICE(AACMetric):
+    """Semantic Propositional Image Caption Evaluation class.
 
-    - Paper: https://arxiv.org/abs/1908.10084
-    - Original implementation: https://github.com/blmoistawinde/fense
+    - Paper: https://arxiv.org/pdf/1607.08822.pdf
 
-    For more information, see :func:`~aac_metrics.functional.sbert.sbert`.
+    For more information, see :func:`~aac_metrics.functional.spice.spice`.
     """
 
     full_state_update = False
     higher_is_better = True
     is_differentiable = False
 
-    min_value = -1.0
+    min_value = 0.0
     max_value = 1.0
 
     def __init__(
         self,
         return_all_scores: bool = True,
-        sbert_model: str = "paraphrase-TinyBERT-L6-v2",
-        device: Union[str, torch.device, None] = "auto",
-        batch_size: int = 32,
-        reset_state: bool = True,
+        cache_path: str = "$HOME/.cache",
+        java_path: str = "java",
+        tmp_path: str = "/tmp",
+        n_threads: Optional[int] = None,
+        java_max_memory: str = "8G",
+        timeout: Union[None, int, Iterable[int]] = None,
+        separate_cache_dir: bool = True,
         verbose: int = 0,
     ) -> None:
-        sbert_model = _load_sbert(sbert_model, device, reset_state, verbose)  # type: ignore
-
         super().__init__()
         self._return_all_scores = return_all_scores
-        self._sbert_model = sbert_model
-        self._device = device
-        self._batch_size = batch_size
-        self._reset_state = reset_state
+        self._cache_path = cache_path
+        self._java_path = java_path
+        self._tmp_path = tmp_path
+        self._n_threads = n_threads
+        self._java_max_memory = java_max_memory
+        self._timeout = timeout
+        self._separate_cache_dir = separate_cache_dir
         self._verbose = verbose
 
         self._candidates = []
         self._mult_references = []
 
     def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
-        return sbert(
+        return spice(
             self._candidates,
             self._mult_references,
             self._return_all_scores,
-            self._sbert_model,
-            self._device,
-            self._batch_size,
-            self._reset_state,
+            self._cache_path,
+            self._java_path,
+            self._tmp_path,
+            self._n_threads,
+            self._java_max_memory,
+            self._timeout,
+            self._separate_cache_dir,
             self._verbose,
         )
 
     def extra_repr(self) -> str:
-        return f"device={self._device}, batch_size={self._batch_size}"
+        return f"java_max_memory={self._java_max_memory}"
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("sbert.sim",)
+        return ("spice",)
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
 
     def update(
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/spice.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/spider.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,81 +4,90 @@
 import logging
 
 from typing import Iterable, Optional, Union
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
-from aac_metrics.functional.spice import spice
+from aac_metrics.functional.spider import spider
 
 
 pylog = logging.getLogger(__name__)
 
 
-class SPICE(AACMetric):
-    """Semantic Propositional Image Caption Evaluation class.
+class SPIDEr(AACMetric):
+    """SPIDEr class.
 
-    - Paper: https://arxiv.org/pdf/1607.08822.pdf
+    - Paper: https://arxiv.org/pdf/1612.00370.pdf
 
-    For more information, see :func:`~aac_metrics.functional.spice.spice`.
+    For more information, see :func:`~aac_metrics.functional.spider.spider`.
     """
 
     full_state_update = False
     higher_is_better = True
     is_differentiable = False
 
     min_value = 0.0
-    max_value = 1.0
+    max_value = 5.5
 
     def __init__(
         self,
         return_all_scores: bool = True,
+        # CIDErD args
+        n: int = 4,
+        sigma: float = 6.0,
+        # SPICE args
         cache_path: str = "$HOME/.cache",
         java_path: str = "java",
         tmp_path: str = "/tmp",
         n_threads: Optional[int] = None,
         java_max_memory: str = "8G",
         timeout: Union[None, int, Iterable[int]] = None,
-        separate_cache_dir: bool = True,
         verbose: int = 0,
     ) -> None:
         super().__init__()
         self._return_all_scores = return_all_scores
+        self._n = n
+        self._sigma = sigma
         self._cache_path = cache_path
         self._java_path = java_path
         self._tmp_path = tmp_path
         self._n_threads = n_threads
         self._java_max_memory = java_max_memory
         self._timeout = timeout
-        self._separate_cache_dir = separate_cache_dir
         self._verbose = verbose
 
         self._candidates = []
         self._mult_references = []
 
     def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
-        return spice(
+        return spider(
             self._candidates,
             self._mult_references,
             self._return_all_scores,
-            self._cache_path,
-            self._java_path,
-            self._tmp_path,
-            self._n_threads,
-            self._java_max_memory,
-            self._timeout,
-            self._separate_cache_dir,
-            self._verbose,
+            # CIDEr args
+            n=self._n,
+            sigma=self._sigma,
+            # SPICE args
+            cache_path=self._cache_path,
+            java_path=self._java_path,
+            tmp_path=self._tmp_path,
+            n_threads=self._n_threads,
+            java_max_memory=self._java_max_memory,
+            timeout=self._timeout,
+            verbose=self._verbose,
         )
 
     def extra_repr(self) -> str:
-        return f"java_max_memory={self._java_max_memory}"
+        return (
+            f"n={self._n}, sigma={self._sigma}, java_max_memory={self._java_max_memory}"
+        )
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("spice",)
+        return ("cider_d", "spice", "spider")
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
 
     def update(
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/spider.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/spider_max.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,74 +4,75 @@
 import logging
 
 from typing import Iterable, Optional, Union
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
-from aac_metrics.functional.spider import spider
+from aac_metrics.functional.spider_max import spider_max
 
 
 pylog = logging.getLogger(__name__)
 
 
-class SPIDEr(AACMetric):
-    """SPIDEr class.
+class SPIDErMax(AACMetric):
+    """SPIDEr-max class.
 
-    - Paper: https://arxiv.org/pdf/1612.00370.pdf
+    - Paper: https://hal.archives-ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf
 
     For more information, see :func:`~aac_metrics.functional.spider.spider`.
     """
 
     full_state_update = False
     higher_is_better = True
     is_differentiable = False
 
     min_value = 0.0
     max_value = 5.5
 
     def __init__(
         self,
         return_all_scores: bool = True,
-        # CIDErD args
+        return_all_cands_scores: bool = False,
+        # CIDEr args
         n: int = 4,
         sigma: float = 6.0,
         # SPICE args
         cache_path: str = "$HOME/.cache",
         java_path: str = "java",
         tmp_path: str = "/tmp",
         n_threads: Optional[int] = None,
         java_max_memory: str = "8G",
         timeout: Union[None, int, Iterable[int]] = None,
         verbose: int = 0,
     ) -> None:
         super().__init__()
         self._return_all_scores = return_all_scores
+        self._return_all_cands_scores = return_all_cands_scores
         self._n = n
         self._sigma = sigma
         self._cache_path = cache_path
         self._java_path = java_path
         self._tmp_path = tmp_path
         self._n_threads = n_threads
         self._java_max_memory = java_max_memory
         self._timeout = timeout
         self._verbose = verbose
 
-        self._candidates = []
+        self._mult_candidates = []
         self._mult_references = []
 
     def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
-        return spider(
-            self._candidates,
+        return spider_max(
+            self._mult_candidates,
             self._mult_references,
             self._return_all_scores,
-            # CIDEr args
+            self._return_all_cands_scores,
             n=self._n,
             sigma=self._sigma,
-            # SPICE args
             cache_path=self._cache_path,
             java_path=self._java_path,
             tmp_path=self._tmp_path,
             n_threads=self._n_threads,
             java_max_memory=self._java_max_memory,
             timeout=self._timeout,
             verbose=self._verbose,
@@ -79,21 +80,21 @@
 
     def extra_repr(self) -> str:
         return (
             f"n={self._n}, sigma={self._sigma}, java_max_memory={self._java_max_memory}"
         )
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("cider_d", "spice", "spider")
+        return ("spider_max",)
 
     def reset(self) -> None:
-        self._candidates = []
+        self._mult_candidates = []
         self._mult_references = []
         return super().reset()
 
     def update(
         self,
-        candidates: list[str],
+        mult_candidates: list[list[str]],
         mult_references: list[list[str]],
     ) -> None:
-        self._candidates += candidates
+        self._mult_candidates += mult_candidates
         self._mult_references += mult_references
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/classes/spider_err.py` & `aac-metrics-0.4.1/src/aac_metrics/classes/spider_fl.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 
 import torch
 
 from torch import Tensor
 from transformers.models.auto.tokenization_auto import AutoTokenizer
 
 from aac_metrics.classes.base import AACMetric
-from aac_metrics.functional.fluency_error import (
+from aac_metrics.functional.fluerr import (
     BERTFlatClassifier,
     _load_echecker_and_tokenizer,
 )
-from aac_metrics.functional.spider_err import spider_err
+from aac_metrics.functional.spider_fl import spider_fl
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
-class SPIDErErr(AACMetric):
-    """SPIDErErr class.
+class SPIDErFL(AACMetric):
+    """SPIDErFL class.
 
-    For more information, see :func:`~aac_metrics.functional.spider_err.spider_err`.
+    For more information, see :func:`~aac_metrics.functional.spider_fl.spider_fl`.
     """
 
     full_state_update = False
     higher_is_better = True
     is_differentiable = False
 
     min_value = 0.0
     max_value = 5.5
 
     def __init__(
         self,
         return_all_scores: bool = True,
-        # CIDEr args
+        # CIDErD args
         n: int = 4,
         sigma: float = 6.0,
         # SPICE args
         cache_path: str = "$HOME/.cache",
         java_path: str = "java",
         tmp_path: str = "/tmp",
         n_threads: Optional[int] = None,
@@ -50,14 +50,15 @@
         # FluencyError args
         echecker: Union[str, BERTFlatClassifier] = "echecker_clotho_audiocaps_base",
         echecker_tokenizer: Optional[AutoTokenizer] = None,
         error_threshold: float = 0.9,
         device: Union[str, torch.device, None] = "auto",
         batch_size: int = 32,
         reset_state: bool = True,
+        return_probs: bool = True,
         # Other args
         penalty: float = 0.9,
         verbose: int = 0,
     ) -> None:
         echecker, echecker_tokenizer = _load_echecker_and_tokenizer(
             echecker, echecker_tokenizer, device, reset_state, verbose
         )
@@ -74,22 +75,23 @@
         self._timeout = timeout
         self._echecker = echecker
         self._echecker_tokenizer = echecker_tokenizer
         self._error_threshold = error_threshold
         self._device = device
         self._batch_size = batch_size
         self._reset_state = reset_state
+        self._return_probs = return_probs
         self._penalty = penalty
         self._verbose = verbose
 
         self._candidates = []
         self._mult_references = []
 
     def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
-        return spider_err(
+        return spider_fl(
             self._candidates,
             self._mult_references,
             self._return_all_scores,
             # CIDEr args
             n=self._n,
             sigma=self._sigma,
             # SPICE args
@@ -102,14 +104,15 @@
             # FluencyError args
             echecker=self._echecker,
             echecker_tokenizer=self._echecker_tokenizer,
             error_threshold=self._error_threshold,
             device=self._device,
             batch_size=self._batch_size,
             reset_state=self._reset_state,
+            return_probs=self._return_probs,
             # Other args
             penalty=self._penalty,
             verbose=self._verbose,
         )
 
     def extra_repr(self) -> str:
         hparams = {
@@ -119,15 +122,15 @@
             "device": self._device,
             "batch_size": self._batch_size,
         }
         extra = ", ".join(f"{k}={v}" for k, v in hparams.items())
         return extra
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("cider_d", "spice", "spider", "spider_err", "fluency_error")
+        return ("cider_d", "spice", "spider", "spider_fl", "fluerr")
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
 
     def update(
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/download.py` & `aac-metrics-0.4.1/src/aac_metrics/download.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/evaluate.py` & `aac-metrics-0.4.1/src/aac_metrics/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/__init__.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/bleu.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/cider_d.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/cider_d.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/evaluate.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/evaluate.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/fense.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/fluency_error.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/fluerr.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,20 +37,20 @@
         "https://github.com/blmoistawinde/fense/releases/download/V0.1/echecker_clotho_audiocaps_base.ckpt",
         "1a719f090af70614bbdb9f9437530b7e133c48cfa4a58d964de0d47fc974a2fa",
     ),
     "echecker_clotho_audiocaps_tiny": (
         "https://github.com/blmoistawinde/fense/releases/download/V0.1/echecker_clotho_audiocaps_tiny.ckpt",
         "90ed0ac5033ec497ec66d4f68588053813e085671136dae312097c96c504f673",
     ),
-    "none": (None, None),
 }
 
 RemoteFileMetadata = namedtuple("RemoteFileMetadata", ["filename", "url", "checksum"])
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
+
 
 ERROR_NAMES = (
     "add_tail",
     "repeat_event",
     "repeat_adv",
     "remove_conj",
     "remove_verb",
@@ -88,23 +88,24 @@
         outputs = self.encoder(input_ids, attention_mask, token_type_ids)
         x = outputs.last_hidden_state[:, 0, :]
         x = self.dropout(x)
         logits = self.clf(x)
         return logits
 
 
-def fluency_error(
+def fluerr(
     candidates: list[str],
     return_all_scores: bool = True,
     echecker: Union[str, BERTFlatClassifier] = "echecker_clotho_audiocaps_base",
     echecker_tokenizer: Optional[AutoTokenizer] = None,
     error_threshold: float = 0.9,
     device: Union[str, torch.device, None] = "auto",
     batch_size: int = 32,
     reset_state: bool = True,
+    return_probs: bool = True,
     verbose: int = 0,
 ) -> Union[Tensor, tuple[dict[str, Tensor], dict[str, Tensor]]]:
     """Return fluency error detected by a pre-trained BERT model.
 
     - Paper: https://arxiv.org/abs/2110.04684
     - Original implementation: https://github.com/blmoistawinde/fense
 
@@ -116,53 +117,65 @@
     :param echecker: The echecker model used to detect fluency errors.
         Can be "echecker_clotho_audiocaps_base", "echecker_clotho_audiocaps_tiny", "none" or None.
         defaults to "echecker_clotho_audiocaps_base".
     :param echecker_tokenizer: The tokenizer of the echecker model.
         If None and echecker is not None, this value will be inferred with `echecker.model_type`.
         defaults to None.
     :param error_threshold: The threshold used to detect fluency errors for echecker model. defaults to 0.9.
-    :param device: The PyTorch device used to run FENSE models. If "auto", it will use cuda if available. defaults to "cpu".
+    :param device: The PyTorch device used to run FENSE models. If "auto", it will use cuda if available. defaults to "auto".
     :param batch_size: The batch size of the echecker models. defaults to 32.
+    :param reset_state: If True, reset the state of the PyTorch global generator after the pre-trained model are built. defaults to True.
+    :param return_probs: If True, return each individual error probability given by the fluency detector model. defaults to True.
     :param verbose: The verbose level. defaults to 0.
     :returns: A tuple of globals and locals scores or a scalar tensor with the main global score.
     """
 
     # Init models
     echecker, echecker_tokenizer = _load_echecker_and_tokenizer(
         echecker, echecker_tokenizer, device, reset_state, verbose
     )
 
     # Compute and apply fluency error detection penalty
-    sents_probs_dic = __detect_error_sents(
+    probs_outs_sents = __detect_error_sents(
         echecker,
         echecker_tokenizer,  # type: ignore
         candidates,
         batch_size,
         device,
     )
-    fluency_errors = (sents_probs_dic["error"] > error_threshold).astype(float)
-    sents_probs_dic = {f"fluerr.{k}_prob": v for k, v in sents_probs_dic.items()}
-
-    sents_probs_dic = {k: torch.from_numpy(v) for k, v in sents_probs_dic.items()}
-    corpus_probs_dic = {k: v.mean() for k, v in sents_probs_dic.items()}
+    fluerr_scores = (probs_outs_sents["error"] > error_threshold).astype(float)
 
-    fluency_errors = torch.from_numpy(fluency_errors)
-    fluency_error = fluency_errors.mean()
+    fluerr_scores = torch.from_numpy(fluerr_scores)
+    fluerr_score = fluerr_scores.mean()
 
     if return_all_scores:
-        sents_scores = {
-            "fluency_error": fluency_errors,
-        } | sents_probs_dic
-        corpus_scores = {
-            "fluency_error": fluency_error,
-        } | corpus_probs_dic
+        fluerr_outs_corpus = {
+            "fluerr": fluerr_score,
+        }
+        fluerr_outs_sents = {
+            "fluerr": fluerr_scores,
+        }
+
+        if return_probs:
+            probs_outs_sents = {
+                f"fluerr.{k}_prob": v for k, v in probs_outs_sents.items()
+            }
+            probs_outs_sents = {
+                k: torch.from_numpy(v) for k, v in probs_outs_sents.items()
+            }
+            probs_outs_corpus = {k: v.mean() for k, v in probs_outs_sents.items()}
+
+            fluerr_outs_corpus = probs_outs_corpus | fluerr_outs_corpus
+            fluerr_outs_sents = probs_outs_sents | fluerr_outs_sents
+
+        fluerr_outs = fluerr_outs_corpus, fluerr_outs_sents
 
-        return corpus_scores, sents_scores
+        return fluerr_outs
     else:
-        return fluency_error
+        return fluerr_score
 
 
 # - Private functions
 def _load_echecker_and_tokenizer(
     echecker: Union[str, BERTFlatClassifier] = "echecker_clotho_audiocaps_base",
     echecker_tokenizer: Optional[AutoTokenizer] = None,
     device: Union[str, torch.device, None] = "auto",
@@ -392,15 +405,15 @@
     url, checksum = PRETRAIN_ECHECKERS_DICT[echecker_model]
     remote = RemoteFileMetadata(
         filename=f"{echecker_model}.ckpt", url=url, checksum=checksum
     )
     file_path = __check_download_resource(remote, use_proxy, proxies)
 
     if verbose >= 2:
-        logger.debug(f"Loading echecker model from '{file_path}'.")
+        pylog.debug(f"Loading echecker model from '{file_path}'.")
 
     model_states = torch.load(file_path)
     echecker = BERTFlatClassifier(
         model_type=model_states["model_type"],
         num_classes=model_states["num_classes"],
     )
     echecker.load_state_dict(model_states["state_dict"])
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/meteor.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/mult_cands.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/mult_cands.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/rouge_l.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/sbert.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/sbert_sim.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from sentence_transformers import SentenceTransformer
 from torch import Tensor
 
 
 pylog = logging.getLogger(__name__)
 
 
-def sbert(
+def sbert_sim(
     candidates: list[str],
     mult_references: list[list[str]],
     return_all_scores: bool = True,
     sbert_model: Union[str, SentenceTransformer] = "paraphrase-TinyBERT-L6-v2",
     device: Union[str, torch.device, None] = "auto",
     batch_size: int = 32,
     reset_state: bool = True,
@@ -36,16 +36,17 @@
 
     :param candidates: The list of sentences to evaluate.
     :param mult_references: The list of list of sentences used as target.
     :param return_all_scores: If True, returns a tuple containing the globals and locals scores.
         Otherwise returns a scalar tensor containing the main global score.
         defaults to True.
     :param sbert_model: The sentence BERT model used to extract sentence embeddings for cosine-similarity. defaults to "paraphrase-TinyBERT-L6-v2".
-    :param device: The PyTorch device used to run FENSE models. If "auto", it will use cuda if available. defaults to "cpu".
+    :param device: The PyTorch device used to run FENSE models. If "auto", it will use cuda if available. defaults to "auto".
     :param batch_size: The batch size of the sBERT models. defaults to 32.
+    :param reset_state: If True, reset the state of the PyTorch global generator after the pre-trained model are built. defaults to True.
     :param verbose: The verbose level. defaults to 0.
     :returns: A tuple of globals and locals scores or a scalar tensor with the main global score.
     """
     # Init models
     sbert_model = _load_sbert(sbert_model, device, reset_state)
 
     # Encode sents
@@ -54,37 +55,37 @@
         rng_ids.append(rng_ids[-1] + len(refs))
     flat_references = [ref for refs in mult_references for ref in refs]
 
     cands_embs = _encode_sents_sbert(sbert_model, candidates, batch_size, verbose)
     mrefs_embs = _encode_sents_sbert(sbert_model, flat_references, batch_size, verbose)
 
     # Compute sBERT similarities
-    sbert_cos_sims = [
+    sbert_sim_scores = [
         (cands_embs[i] @ mrefs_embs[rng_ids[i] : rng_ids[i + 1]].T).mean().item()
         for i in range(len(cands_embs))
     ]
-    sbert_cos_sims = np.array(sbert_cos_sims)
+    sbert_sim_scores = np.array(sbert_sim_scores)
 
     # Aggregate and return
-    sbert_cos_sim = sbert_cos_sims.mean()
+    sbert_sim_score = sbert_sim_scores.mean()
 
-    sbert_cos_sim = torch.as_tensor(sbert_cos_sim)
-    sbert_cos_sims = torch.from_numpy(sbert_cos_sims)
+    sbert_sim_score = torch.as_tensor(sbert_sim_score)
+    sbert_sim_scores = torch.from_numpy(sbert_sim_scores)
 
     if return_all_scores:
-        sents_scores = {
-            "sbert.sim": sbert_cos_sims,
+        sbert_sim_outs_corpus = {
+            "sbert_sim": sbert_sim_score,
         }
-        corpus_scores = {
-            "sbert.sim": sbert_cos_sim,
+        sbert_sim_outs_sents = {
+            "sbert_sim": sbert_sim_scores,
         }
 
-        return corpus_scores, sents_scores
+        return sbert_sim_outs_corpus, sbert_sim_outs_sents
     else:
-        return sbert_cos_sim
+        return sbert_sim_score
 
 
 def _load_sbert(
     sbert_model: Union[str, SentenceTransformer] = "paraphrase-TinyBERT-L6-v2",
     device: Union[str, torch.device, None] = "auto",
     reset_state: bool = True,
 ) -> SentenceTransformer:
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/spice.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/spider.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/spider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/spider_err.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/spider_fl.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 from typing import Callable, Iterable, Optional, Union
 
 import torch
 
 from torch import Tensor
 from transformers.models.auto.tokenization_auto import AutoTokenizer
 
-from aac_metrics.functional.fluency_error import (
-    fluency_error,
+from aac_metrics.functional.fluerr import (
+    fluerr,
     _load_echecker_and_tokenizer,
     BERTFlatClassifier,
 )
 from aac_metrics.functional.spider import spider
 
 
 pylog = logging.getLogger(__name__)
 
 
-def spider_err(
+def spider_fl(
     candidates: list[str],
     mult_references: list[list[str]],
     return_all_scores: bool = True,
-    # CIDEr args
+    # CIDErD args
     n: int = 4,
     sigma: float = 6.0,
     tokenizer: Callable[[str], list[str]] = str.split,
     return_tfidf: bool = False,
     # SPICE args
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
@@ -44,20 +44,23 @@
     # FluencyError args
     echecker: Union[str, BERTFlatClassifier] = "echecker_clotho_audiocaps_base",
     echecker_tokenizer: Optional[AutoTokenizer] = None,
     error_threshold: float = 0.9,
     device: Union[str, torch.device, None] = "auto",
     batch_size: int = 32,
     reset_state: bool = True,
+    return_probs: bool = True,
     # Other args
     penalty: float = 0.9,
     verbose: int = 0,
 ) -> Union[Tensor, tuple[dict[str, Tensor], dict[str, Tensor]]]:
     """Combinaison of SPIDEr with Fluency Error detector.
 
+    Based on https://github.com/felixgontier/dcase-2023-baseline/blob/main/metrics.py#L48.
+
     :param candidates: The list of sentences to evaluate.
     :param mult_references: The list of list of sentences used as target.
     :param return_all_scores: If True, returns a tuple containing the globals and locals scores.
         Otherwise returns a scalar tensor containing the main global score.
         defaults to True.
     :param n: Maximal number of n-grams taken into account. defaults to 4.
     :param sigma: Standard deviation parameter used for gaussian penalty. defaults to 6.0.
@@ -74,46 +77,57 @@
     :param echecker: The echecker model used to detect fluency errors.
         Can be "echecker_clotho_audiocaps_base", "echecker_clotho_audiocaps_tiny", "none" or None.
         defaults to "echecker_clotho_audiocaps_base".
     :param echecker_tokenizer: The tokenizer of the echecker model.
         If None and echecker is not None, this value will be inferred with `echecker.model_type`.
         defaults to None.
     :param error_threshold: The threshold used to detect fluency errors for echecker model. defaults to 0.9.
-    :param device: The PyTorch device used to run FENSE models. If "auto", it will use cuda if available. defaults to "cpu".
+    :param device: The PyTorch device used to run FENSE models. If "auto", it will use cuda if available. defaults to "auto".
     :param batch_size: The batch size of the sBERT and echecker models. defaults to 32.
+    :param reset_state: If True, reset the state of the PyTorch global generator after the pre-trained model are built. defaults to True.
+    :param return_probs: If True, return each individual error probability given by the fluency detector model. defaults to True.
     :param penalty: The penalty coefficient applied. Higher value means to lower the cos-sim scores when an error is detected. defaults to 0.9.
     :param verbose: The verbose level. defaults to 0.
     :returns: A tuple of globals and locals scores or a scalar tensor with the main global score.
     """
 
     # Init models
     echecker, echecker_tokenizer = _load_echecker_and_tokenizer(
         echecker, echecker_tokenizer, device, reset_state, verbose
     )
 
-    spider_corpus_scores, spider_sents_scores = spider(candidates, mult_references, True, n, sigma, tokenizer, return_tfidf, cache_path, java_path, tmp_path, n_threads, java_max_memory, timeout, verbose)  # type: ignore
-    spider_corpus_scores: dict[str, Tensor]
-    spider_sents_scores: dict[str, Tensor]
-
-    fluerr_corpus_scores, fluerr_sents_scores = fluency_error(candidates, True, echecker, echecker_tokenizer, error_threshold, device, batch_size, verbose)  # type: ignore
-    fluerr_corpus_scores: dict[str, Tensor]
-    fluerr_sents_scores: dict[str, Tensor]
-
-    spider_scores = spider_sents_scores["spider"]
-    fluency_errors = fluerr_sents_scores["fluency_error"]
-    spider_err_scores = spider_scores * (1.0 - penalty * fluency_errors)
-    spider_err_score = spider_err_scores.mean()
+    spider_outs: tuple = spider(candidates, mult_references, True, n, sigma, tokenizer, return_tfidf, cache_path, java_path, tmp_path, n_threads, java_max_memory, timeout, verbose)  # type: ignore
+    fluerr_outs: tuple = fluerr(candidates, True, echecker, echecker_tokenizer, error_threshold, device, batch_size, reset_state, return_probs, verbose)  # type: ignore
+    spider_fl_outs = _spider_fl_from_outputs(spider_outs, fluerr_outs, penalty)
 
     if return_all_scores:
-        corpus_scores = (
-            spider_corpus_scores
-            | fluerr_corpus_scores
-            | {"spider_err": spider_err_score}
-        )
-        sents_scores = (
-            spider_corpus_scores
-            | fluerr_sents_scores
-            | {"spider_err": spider_err_scores}
-        )
-        return corpus_scores, sents_scores
+        return spider_fl_outs
     else:
-        return spider_err_score
+        return spider_fl_outs[0]["spider_fl"]
+
+
+def _spider_fl_from_outputs(
+    spider_outs: tuple[dict[str, Tensor], dict[str, Tensor]],
+    fluerr_outs: tuple[dict[str, Tensor], dict[str, Tensor]],
+    penalty: float = 0.9,
+) -> tuple[dict[str, Tensor], dict[str, Tensor]]:
+    """Combines SPIDEr and FluErr outputs.
+
+    Based on https://github.com/felixgontier/dcase-2023-baseline/blob/main/metrics.py#L48
+    """
+    spider_outs_corpus, spider_outs_sents = spider_outs
+    fluerr_outs_corpus, fluerr_outs_sents = fluerr_outs
+
+    spider_scores = spider_outs_sents["spider"]
+    fluerr_scores = fluerr_outs_sents["fluerr"]
+    spider_fl_scores = spider_scores * (1.0 - penalty * fluerr_scores)
+    spider_fl_score = spider_fl_scores.mean()
+
+    spider_fl_outs_corpus = (
+        spider_outs_corpus | fluerr_outs_corpus | {"spider_fl": spider_fl_score}
+    )
+    spider_fl_outs_sents = (
+        spider_outs_sents | fluerr_outs_sents | {"spider_fl": spider_fl_scores}
+    )
+    spider_fl_outs = spider_fl_outs_corpus, spider_fl_outs_sents
+
+    return spider_fl_outs
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics/functional/spider_max.py` & `aac-metrics-0.4.1/src/aac_metrics/functional/spider_max.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/info.py` & `aac-metrics-0.4.1/src/aac_metrics/info.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/utils/checks.py` & `aac-metrics-0.4.1/src/aac_metrics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/utils/collections.py` & `aac-metrics-0.4.1/src/aac_metrics/utils/collections.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics/utils/tokenization.py` & `aac-metrics-0.4.1/src/aac_metrics/utils/tokenization.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/src/aac_metrics.egg-info/PKG-INFO` & `aac-metrics-0.4.1/src/aac_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.4.0
+Version: 0.4.1
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/
 Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
 Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
@@ -239,15 +239,15 @@
 @software{
     Labbe_aac-metrics_2023,
     author = {Labbé, Etienne},
     license = {MIT},
     month = {4},
     title = {{aac-metrics}},
     url = {https://github.com/Labbeti/aac-metrics/},
-    version = {0.4.0},
+    version = {0.4.1},
     year = {2023},
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.0 Summary: Metrics for
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.1 Summary: Metrics for
 evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
 email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
 pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
 Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
 repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
 https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
@@ -139,9 +139,9 @@
 ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
 France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
 metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
 ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
 HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
 below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
 license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
-github.com/Labbeti/aac-metrics/}, version = {0.4.0}, year = {2023}, } ``` ##
+github.com/Labbeti/aac-metrics/}, version = {0.4.1}, year = {2023}, } ``` ##
 Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.4.0/src/aac_metrics.egg-info/SOURCES.txt` & `aac-metrics-0.4.1/src/aac_metrics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -61,40 +61,34 @@
 src/aac_metrics.egg-info/top_level.txt
 src/aac_metrics/classes/__init__.py
 src/aac_metrics/classes/base.py
 src/aac_metrics/classes/bleu.py
 src/aac_metrics/classes/cider_d.py
 src/aac_metrics/classes/evaluate.py
 src/aac_metrics/classes/fense.py
-src/aac_metrics/classes/fluency_error.py
 src/aac_metrics/classes/fluerr.py
 src/aac_metrics/classes/meteor.py
 src/aac_metrics/classes/rouge_l.py
-src/aac_metrics/classes/sbert.py
 src/aac_metrics/classes/sbert_sim.py
 src/aac_metrics/classes/spice.py
 src/aac_metrics/classes/spider.py
-src/aac_metrics/classes/spider_err.py
 src/aac_metrics/classes/spider_fl.py
 src/aac_metrics/classes/spider_max.py
 src/aac_metrics/functional/__init__.py
 src/aac_metrics/functional/bleu.py
 src/aac_metrics/functional/cider_d.py
 src/aac_metrics/functional/evaluate.py
 src/aac_metrics/functional/fense.py
-src/aac_metrics/functional/fluency_error.py
 src/aac_metrics/functional/fluerr.py
 src/aac_metrics/functional/meteor.py
 src/aac_metrics/functional/mult_cands.py
 src/aac_metrics/functional/rouge_l.py
-src/aac_metrics/functional/sbert.py
 src/aac_metrics/functional/sbert_sim.py
 src/aac_metrics/functional/spice.py
 src/aac_metrics/functional/spider.py
-src/aac_metrics/functional/spider_err.py
 src/aac_metrics/functional/spider_fl.py
 src/aac_metrics/functional/spider_max.py
 src/aac_metrics/utils/__init__.py
 src/aac_metrics/utils/checks.py
 src/aac_metrics/utils/collections.py
 src/aac_metrics/utils/imports.py
 src/aac_metrics/utils/tokenization.py
```

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/caption-evaluation-tools/eval_metrics.py` & `aac-metrics-0.4.1/tests/caption-evaluation-tools/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/test_bleu_tchmet.py` & `aac-metrics-0.4.1/tests/test_bleu_tchmet.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/test_compare_cet.py` & `aac-metrics-0.4.1/tests/test_compare_cet.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/test_compare_fense.py` & `aac-metrics-0.4.1/tests/test_compare_fense.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/test_pickable.py` & `aac-metrics-0.4.1/tests/test_pickable.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.4.0/tests/test_utils.py` & `aac-metrics-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

