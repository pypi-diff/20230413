# Comparing `tmp/aac-metrics-0.3.0.tar.gz` & `tmp/aac-metrics-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aac-metrics-0.3.0.tar", last modified: Mon Feb 27 13:08:46 2023, max compression
+gzip compressed data, was "aac-metrics-0.4.0.tar", last modified: Thu Apr 13 14:04:55 2023, max compression
```

## Comparing `aac-metrics-0.3.0.tar` & `aac-metrics-0.4.0.tar`

### file list

```diff
@@ -1,98 +1,108 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:46.001663 aac-metrics-0.3.0/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.989663 aac-metrics-0.3.0/.github/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/.github/workflows/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2213 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/.github/workflows/python-package-pip.yaml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.3.0/LICENCE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      135 2022-10-31 09:45:25.000000 aac-metrics-0.3.0/MANIFEST.in
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    13725 2023-02-27 13:08:46.001663 aac-metrics-0.3.0/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12895 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/README.md
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/examples/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2022-09-28 09:41:46.000000 aac-metrics-0.3.0/examples/example_1.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2022-09-30 12:10:31.000000 aac-metrics-0.3.0/examples/example_2.csv
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/install_spice.sh
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1410 2023-02-27 13:08:46.005663 aac-metrics-0.3.0/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.3.0/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.989663 aac-metrics-0.3.0/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/src/aac_metrics/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1527 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.3.0/src/aac_metrics/__main__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:46.001663 aac-metrics-0.3.0/src/aac_metrics/classes/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      568 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/src/aac_metrics/classes/base.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5784 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3012 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2528 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/fluency_error.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2286 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/sbert.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2439 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4222 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/spider_err.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2841 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/classes/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7226 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7172 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/src/aac_metrics/evaluate.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:46.001663 aac-metrics-0.3.0/src/aac_metrics/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      578 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9219 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9593 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7924 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/evaluate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4852 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/fense.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15053 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/fluency_error.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5509 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/meteor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4105 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/mult_cands.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5359 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/rouge_l.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3949 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/sbert.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8194 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/spice.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4199 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/spider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5128 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/spider_err.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/functional/spider_max.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.3.0/src/aac_metrics/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:46.001663 aac-metrics-0.3.0/src/aac_metrics/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.3.0/src/aac_metrics/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2015 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/src/aac_metrics/utils/checks.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/src/aac_metrics/utils/collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/src/aac_metrics/utils/imports.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7687 2023-02-27 13:03:46.000000 aac-metrics-0.3.0/src/aac_metrics/utils/tokenization.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:46.001663 aac-metrics-0.3.0/src/aac_metrics.egg-info/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    13725 2023-02-27 13:08:45.000000 aac-metrics-0.3.0/src/aac_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3931 2023-02-27 13:08:45.000000 aac-metrics-0.3.0/src/aac_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-02-27 13:08:45.000000 aac-metrics-0.3.0/src/aac_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-02-27 13:08:45.000000 aac-metrics-0.3.0/src/aac_metrics.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-02-27 13:08:45.000000 aac-metrics-0.3.0/src/aac_metrics.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-02-27 13:08:45.000000 aac-metrics-0.3.0/src/aac_metrics.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/tests/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/tests/caption-evaluation-tools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2022-09-30 09:32:10.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2022-09-30 09:32:10.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.993663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2022-09-30 09:32:10.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-02-27 13:08:45.997663 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocotools/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2022-11-10 14:20:27.000000 aac-metrics-0.3.0/tests/caption-evaluation-tools/eval_metrics.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1039 2022-12-14 13:14:25.000000 aac-metrics-0.3.0/tests/test_bleu_tchmet.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      557 2022-10-31 09:45:25.000000 aac-metrics-0.3.0/tests/test_pickable.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.738138 aac-metrics-0.4.0/.github/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.742138 aac-metrics-0.4.0/.github/workflows/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1891 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/.github/workflows/python-package-pip.yaml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1080 2022-11-28 15:41:53.000000 aac-metrics-0.4.0/LICENCE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      135 2022-10-31 09:45:25.000000 aac-metrics-0.4.0/MANIFEST.in
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11098 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/README.md
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/examples/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   125595 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/examples/example_1.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   378908 2022-09-30 12:10:31.000000 aac-metrics-0.4.0/examples/example_2.csv
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1530 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/install_spice.sh
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1954 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.738138 aac-metrics-0.4.0/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.742138 aac-metrics-0.4.0/src/aac_metrics/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1537 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      519 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/src/aac_metrics/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/src/aac_metrics/classes/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      607 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1480 2023-03-16 14:40:20.000000 aac-metrics-0.4.0/src/aac_metrics/classes/base.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2192 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2151 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6399 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3106 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2528 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/classes/fluency_error.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2593 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2145 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/classes/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2286 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/classes/sbert.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2357 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2438 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2663 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4222 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider_err.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4322 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2840 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/classes/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7654 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7466 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/evaluate.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/src/aac_metrics/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      631 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9592 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9590 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/cider_d.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9909 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/evaluate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5660 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15053 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/functional/fluency_error.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15574 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/fluerr.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5546 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/meteor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4087 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/mult_cands.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5376 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/rouge_l.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3949 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/functional/sbert.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4148 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/sbert_sim.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8738 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spice.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4047 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5128 2023-04-13 13:59:45.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider_err.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5879 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider_fl.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3219 2023-02-27 13:03:46.000000 aac-metrics-0.4.0/src/aac_metrics/functional/spider_max.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      889 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/src/aac_metrics/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/src/aac_metrics/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2022-09-28 09:41:46.000000 aac-metrics-0.4.0/src/aac_metrics/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2973 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/utils/checks.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      688 2022-12-14 13:14:25.000000 aac-metrics-0.4.0/src/aac_metrics/utils/collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      466 2022-12-14 13:14:25.000000 aac-metrics-0.4.0/src/aac_metrics/utils/imports.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7678 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/src/aac_metrics/utils/tokenization.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.750138 aac-metrics-0.4.0/src/aac_metrics.egg-info/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12236 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4284 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      170 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       12 2023-04-13 14:04:55.000000 aac-metrics-0.4.0/src/aac_metrics.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.754138 aac-metrics-0.4.0/tests/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       47 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1565 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9066 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1989 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7994 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3879 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3356 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       23 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3920 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3217 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3168 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-04-13 14:04:55.746138 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       21 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15731 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10312 2023-03-13 13:47:09.000000 aac-metrics-0.4.0/tests/caption-evaluation-tools/eval_metrics.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1059 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_bleu_tchmet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4279 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_compare_cet.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3906 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_compare_fense.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      583 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_pickable.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1024 2023-04-13 14:01:18.000000 aac-metrics-0.4.0/tests/test_utils.py
```

### Comparing `aac-metrics-0.3.0/.github/workflows/python-package-pip.yaml` & `aac-metrics-0.4.0/.github/workflows/python-package-pip.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -6,78 +6,74 @@
   push:
     branches: [ main, dev ]
   pull_request:
     branches: [ main, dev ]
 
 jobs:
   build:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+        python-version: ["3.9"]
+        java-version: ["11"]
 
     steps:
     # --- INSTALLATIONS ---
-    - name: Checkout repository and submodules
+
+    - name: Checkout repository
       uses: actions/checkout@v2
       with:
         submodules: recursive
 
-    - name: Set up Python 3.9
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
-        python-version: 3.9
-
-    - name: Set up Java 11
+        python-version: ${{ matrix.python-version }}
+        cache: 'pip'
+  
+    - name: Set up Java ${{ matrix.java-version }}
       uses: actions/setup-java@v2
       with:
         distribution: 'temurin'
-        java-version: '11'
-
-    - name: Load cache of pip dependencies
-      uses: actions/cache@master
-      id: cache_requirements
-      with:
-        path: ${{ env.pythonLocation }}/lib/python3.9/site-packages/*
-        key: ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}
-        restore-keys: |
-          ${{ runner.os }}-pip-
-          ${{ runner.os }}-
+        java-version: ${{ matrix.java-version }}
+        java-package: jre
 
-    - name: Install pip dev dependencies + package if needed
-      if: steps.cache_requirements.outputs.cache-hit != 'true'
+    - name: Install package
       run: |
-        python -m pip install --upgrade pip
         python -m pip install -e .[dev]
-
-    - name: Install package if needed
-      if: steps.cache_requirements.outputs.cache-hit == 'true'
-      run: |
-        python -m pip install -e . --no-dependencies
   
-    - name: Load cache of external code
+    - name: Load cache of external code and data
       uses: actions/cache@master
       id: cache_external
       with:
-        path: /home/runner/.cache/aac-metrics-/*
+        path: /home/runner/.cache/aac-metrics/*
         key: ${{ runner.os }}-${{ hashFiles('install_spice.sh') }}
         restore-keys: |
           ${{ runner.os }}-
 
     # --- TESTS ---
     - name: Lint with flake8
       run: |
         python -m flake8 --config .flake8 --exit-zero --show-source --statistics src
 
     - name: Check format with Black
       run: |
         python -m black --check --diff src
+
+    - name: Print install info
+      run: |
+        aac-metrics-info
+
+    - name: Print Java version
+      run: |
+        java --version
   
     - name: Install external code if needed
       if: steps.cache_external.outputs.cache-hit != 'true'
       run: |
         aac-metrics-download
-      
-    - name: Print install info
-      run: |
-        aac-metrics-info
   
     - name: Test with pytest
       run: |
         python -m pytest -v
```

### Comparing `aac-metrics-0.3.0/LICENCE` & `aac-metrics-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/PKG-INFO` & `aac-metrics-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.3.0
+Version: 0.4.0
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
-Home-page: https://github.com/Labbeti/aac-metrics
-Author: Etienne Labbé (Labbeti)
-Author-email: labbeti.pub@gmail.com
-License: MIT
-Project-URL: Documentation, https://aac-metrics.readthedocs.io/
-Project-URL: Source, https://github.com/Labbeti/aac-metrics
-Project-URL: PyPI, https://pypi.org/project/aac-metrics/
+Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
+Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
+Project-URL: homepage, https://pypi.org/project/aac-metrics/
+Project-URL: documentation, https://aac-metrics.readthedocs.io/
+Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
+Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
+Keywords: audio,metrics,text,captioning,audio-captioning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
@@ -44,52 +47,60 @@
     - BLEU [[1]](#bleu)
     - ROUGE-L [[2]](#rouge-l)
     - METEOR [[3]](#meteor)
     - CIDEr-D [[4]](#cider)
     - SPICE [[5]](#spice)
     - SPIDEr [[6]](#spider)
     - SPIDEr-max [[7]](#spider-max)
-    - SBERT [[8]](#fense)
-    - FluencyError [[8]](#fense)
+    - SBERT-sim [[8]](#fense)
+    - Fluency Error [[8]](#fense)
     - FENSE [[8]](#fense)
-    - SPIDErErr
+    - SPIDEr-FL [[9]](#spider-fl)
 
 ## Installation
 Install the pip package:
 ```bash
 pip install aac-metrics
 ```
 
-Download the external code and models needed for METEOR, SPICE, PTBTokenizer and FENSE:
+Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and SPIDEr-FL:
 ```bash
 aac-metrics-download
 ```
 
 Notes:
 - The external code for SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`.
 - The weights of the FENSE fluency error detector and the the SBERT model are respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and `$HOME/.cache/torch/sentence_transformers`.
 
 ## Usage
-### Evaluate default AAC metrics
-The full evaluation process to compute AAC metrics can be done with `aac_metrics.aac_evaluate` function.
+### Evaluate default metrics
+The full evaluation pipeline to compute AAC metrics can be done with `aac_metrics.evaluate` function.
 
 ```python
-from aac_metrics import aac_evaluate
+from aac_metrics import evaluate
 
 candidates: list[str] = ["a man is speaking"]
 mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
 
-corpus_scores, _ = aac_evaluate(candidates, mult_references)
+corpus_scores, _ = evaluate(candidates, mult_references)
 print(corpus_scores)
-# dict containing the score of each aac metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d", "spice", "spider"
+# dict containing the score of each metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d", "spice", "spider"
 # {"bleu_1": tensor(0.7), "bleu_2": ..., ...}
 ```
+### Evaluate DCASE2023 metrics
+To compute metrics for the DCASE2023 challenge, just set the argument `metrics="dcase2023"` in `evaluate` function call.
+
+```python
+corpus_scores, _ = evaluate(candidates, mult_references, metrics="dcase2023")
+print(corpus_scores)
+# dict containing the score of each metric: "meteor", "cider_d", "spice", "spider", "spider_fl", "fluerr"
+```
 
 ### Evaluate a specific metric
-Evaluate a specific metric can be done using the `aac_metrics.functional.<metric_name>.<metric_name>` function or the `aac_metrics.classes.<metric_name>.<metric_name>` class. Unlike `aac_evaluate`, the tokenization with PTBTokenizer is not done with these functions, but you can do it manually with `preprocess_mono_sents` and `preprocess_mult_sents` functions.
+Evaluate a specific metric can be done using the `aac_metrics.functional.<metric_name>.<metric_name>` function or the `aac_metrics.classes.<metric_name>.<metric_name>` class. Unlike `evaluate`, the tokenization with PTBTokenizer is not done with these functions, but you can do it manually with `preprocess_mono_sents` and `preprocess_mult_sents` functions.
 
 ```python
 from aac_metrics.functional import cider_d
 from aac_metrics.utils.tokenization import preprocess_mono_sents, preprocess_mult_sents
 
 candidates: list[str] = ["a man is speaking"]
 mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
@@ -103,132 +114,65 @@
 print(sents_scores)
 # {"cider_d": tensor([0.9, ...])}
 ```
 
 Each metrics also exists as a python class version, like `aac_metrics.classes.cider_d.CIDErD`.
 
 ## Metrics
-### Default AAC metrics
+### Legacy metrics
 | Metric | Python Class | Origin | Range | Short description |
 |:---|:---|:---|:---|:---|
 | BLEU [[1]](#bleu) | `BLEU` | machine translation | [0, 1] | Precision of n-grams |
 | ROUGE-L [[2]](#rouge-l) | `ROUGEL` | machine translation | [0, 1] | FScore of the longest common subsequence |
 | METEOR [[3]](#meteor) | `METEOR` | machine translation | [0, 1] | Cosine-similarity of frequencies with synonyms matching |
 | CIDEr-D [[4]](#cider) | `CIDErD` | image captioning | [0, 10] | Cosine-similarity of TF-IDF computed on n-grams |
 | SPICE [[5]](#spice) | `SPICE` | image captioning | [0, 1] | FScore of semantic graph |
 | SPIDEr [[6]](#spider) | `SPIDEr` | image captioning | [0, 5.5] | Mean of CIDEr-D and SPICE |
 
-### Other metrics
+### AAC-specific metrics
 | Metric name | Python Class | Origin | Range | Short description |
 |:---|:---|:---|:---|:---|
 | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning | [0, 5.5] | Max of SPIDEr scores for multiples candidates |
-| SBERT [[7]](#spider-max) | `SBERT` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-BERT embeddings** |
-| FluencyError [[7]](#spider-max) | `FluencyError` | audio captioning | [0, 1] | Use pretrained model to detect fluency errors in sentences |
-| FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] | Combines `SBERT` and `FluencyError` |
-| SPIDErErr | `SPIDErErr` | audio captioning | [0, 5.5] | Combines `SPIDEr` and `FluencyError` |
-
-## SPIDEr-max metric
-SPIDEr-max [[7]](#spider-max)  is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model.
-
-### SPIDEr-max: why ?
-The SPIDEr metric used in audio captioning is highly sensitive to the frequencies of the words used.
-
-Here is 2 examples with the 5 candidates generated by the beam search algorithm, their corresponding SPIDEr scores and the associated references:
-
-<div align="center">
-
-| Beam search candidates | SPIDEr |
-|:---|:---:|
-| heavy rain is falling on a roof | 0.562 |
-| heavy rain is falling on **a tin roof** | **0.930** |
-| a heavy rain is falling on a roof | 0.594 |
-| a heavy rain is falling on the ground | 0.335 |
-| a heavy rain is falling on the roof | 0.594 |
-
-| References |
-|:---|
-| heavy rain falls loudly onto a structure with a thin roof |
-| heavy rainfall falling onto a thin structure with a thin roof |
-| it is raining hard and the rain hits **a tin roof** |
-| rain that is pouring down very hard outside |
-| the hard rain is noisy as it hits **a tin roof** |
-
-_(Candidates and references for the Clotho development-testing file named "rain.wav")_
-
-| Beam search candidates | SPIDEr |
-|:---|:---:|
-| a woman speaks and a sheep bleats | 0.190 |
-| a woman **speaks and a goat bleats** | **1.259** |
-| a man speaks and a sheep bleats | 0.344 |
-| an adult male speaks and a sheep bleats | 0.231 |
-| an adult male is speaking and a sheep bleats | 0.189 |
-
-| References |
-|:---|
-| a man speaking and laughing followed by a goat bleat |
-| a man is speaking in high tone while a goat is bleating one time |
-| a man speaks followed by a goat bleat |
-| a person **speaks and a goat bleats** |
-| a man is talking and snickering followed by a goat bleating |
-
-_(Candidates and references for an AudioCaps testing file with the id "jid4t-FzUn0")_
-</div>
-
-Even with very similar candidates, the SPIDEr scores varies drastically. To adress this issue, we proposed a SPIDEr-max metric which take the maximum value of several candidates for the same audio. SPIDEr-max demonstrate that SPIDEr can exceed state-of-the-art scores on AudioCaps and Clotho and even human scores on AudioCaps [[7]](#spider-max).
-
-### SPIDEr-max: usage
-This usage is very similar to other captioning metrics, with the main difference of take a multiple candidates list as input.
-
-```python
-from aac_metrics.functional import spider_max
-from aac_metrics.utils.tokenization import preprocess_mult_sents
-
-mult_candidates: list[list[str]] = [["a man is speaking", "maybe someone speaking"]]
-mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
-
-mult_candidates = preprocess_mult_sents(mult_candidates)
-mult_references = preprocess_mult_sents(mult_references)
-
-corpus_scores, sents_scores = spider_max(mult_candidates, mult_references)
-print(corpus_scores)
-# {"spider": tensor(0.1), ...}
-print(sents_scores)
-# {"spider": tensor([0.9, ...]), ...}
-```
+| SBERT-sim [[8]](#spider-max) | `SBERTSim` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-BERT embeddings** |
+| Fluency Error [[8]](#spider-max) | `FluErr` | audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in sentences |
+| FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] | Combines SBERT-sim and Fluency Error |
+| SPIDEr-FL [[9]](#spider-fl) | `SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
 
 ## Requirements
 ### Python packages
 
 The pip requirements are automatically installed when using `pip install` on this repository.
 ```
 torch >= 1.10.1
 numpy >= 1.21.2
 pyyaml >= 6.0
 tqdm >= 4.64.0
 sentence-transformers>=2.2.2
 ```
 
 ### External requirements
-- `java` >= 1.8 is required to compute METEOR, SPICE and use the PTBTokenizer.
+- `java` **>= 1.8 and <= 1.11** is required to compute METEOR, SPICE and use the PTBTokenizer.
 Most of these functions can specify a java executable path with `java_path` argument.
 
 - `unzip` command to extract SPICE zipped files.
 
-
 ## Additional notes
 ### CIDEr or CIDEr-D ?
 The CIDEr metric differs from CIDEr-D because it applies a stemmer to each word before computing the n-grams of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 
 ### Does metrics work on multi-GPU ?
 No. Most of these metrics use numpy or external java programs to run, which prevents multi-GPU testing for now.
 
 ### Is torchmetrics needed for this package ?
 No. But if torchmetrics is installed, all metrics classes will inherit from the base class `torchmetrics.Metric`.
 It is because most of the metrics does not use PyTorch tensors to compute scores and numpy and strings cannot be added to states of `torchmetrics.Metric`.
 
+## SPIDEr-max metric
+SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model. For more detail, please see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/stable/spider_max.html).
+
 ## References
 #### BLEU
 [1] K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, “BLEU: a
 method for automatic evaluation of machine translation,” in Proceed-
 ings of the 40th Annual Meeting on Association for Computational
 Linguistics - ACL ’02. Philadelphia, Pennsylvania: Association
 for Computational Linguistics, 2001, p. 311. [Online]. Available:
@@ -263,18 +207,21 @@
 national Conference on Computer Vision (ICCV), pp. 873–881, Oct. 2017,
 arXiv: 1612.00370. [Online]. Available: http://arxiv.org/abs/1612.00370
 
 #### SPIDEr-max
 [7] E. Labbé, T. Pellegrini, and J. Pinquier, “Is my automatic audio captioning system so bad? spider-max: a metric to consider several caption candidates,” Nov. 2022. [Online]. Available: https://hal.archives-ouvertes.fr/hal-03810396
 
 #### FENSE
-[8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/2110.04684 
+[8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/2110.04684
+
+#### SPIDEr-FL
+[9] DCASE website task6a description: https://dcase.community/challenge2023/task-automated-audio-captioning#evaluation
 
 ## Citation
-If you use **SPIDEr-max**, you can cite the following paper using BibTex:
+If you use **SPIDEr-max**, you can cite the following paper using BibTex :
 ```
 @inproceedings{labbe:hal-03810396,
     TITLE = {{Is my automatic audio captioning system so bad? spider-max: a metric to consider several caption candidates}},
     AUTHOR = {Labb{\'e}, Etienne and Pellegrini, Thomas and Pinquier, Julien},
     URL = {https://hal.archives-ouvertes.fr/hal-03810396},
     BOOKTITLE = {{Workshop DCASE}},
     ADDRESS = {Nancy, France},
@@ -283,10 +230,24 @@
     KEYWORDS = {audio captioning ; evaluation metric ; beam search ; multiple candidates},
     PDF = {https://hal.archives-ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf},
     HAL_ID = {hal-03810396},
     HAL_VERSION = {v1},
 }
 ```
 
+If you use this software, please consider cite it as below :
+```
+@software{
+    Labbe_aac-metrics_2023,
+    author = {Labbé, Etienne},
+    license = {MIT},
+    month = {4},
+    title = {{aac-metrics}},
+    url = {https://github.com/Labbeti/aac-metrics/},
+    version = {0.4.0},
+    year = {2023},
+}
+```
+
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,167 +1,147 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.3.0 Summary: Metrics for
-evaluating Automated Audio Captioning systems, designed for PyTorch. Home-page:
-https://github.com/Labbeti/aac-metrics Author: Etienne LabbÃ© (Labbeti) Author-
-email: labbeti.pub@gmail.com License: MIT Project-URL: Documentation, https://
-aac-metrics.readthedocs.io/ Project-URL: Source, https://github.com/Labbeti/
-aac-metrics Project-URL: PyPI, https://pypi.org/project/aac-metrics/
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.9 Description-
-Content-Type: text/markdown Provides-Extra: dev License-File: LICENCE
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.0 Summary: Metrics for
+evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
+email: "Etienne LabbÃ© (Labbeti)"
+pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
+pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
+Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
+repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
+https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
+audio,metrics,text,captioning,audio-captioning Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.9 Description-Content-Type: text/markdown
+Provides-Extra: dev License-File: LICENCE
 # Audio Captioning metrics (aac-metrics) [Python] [PyTorch] [Code_style:_black]
      [Build] [Documentation_Status] Metrics for evaluating Automated Audio
                    Captioning systems, designed for PyTorch.
 ## Why using this package? - **Easy installation and download** - **Same
 results than [caption-evaluation-tools](https://github.com/audio-captioning/
 caption-evaluation-tools) and [fense](https://github.com/blmoistawinde/fense)
 repositories** - **Provides the following metrics:** - BLEU [[1]](#bleu) -
 ROUGE-L [[2]](#rouge-l) - METEOR [[3]](#meteor) - CIDEr-D [[4]](#cider) - SPICE
-[[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT [
-[8]](#fense) - FluencyError [[8]](#fense) - FENSE [[8]](#fense) - SPIDErErr ##
-Installation Install the pip package: ```bash pip install aac-metrics ```
-Download the external code and models needed for METEOR, SPICE, PTBTokenizer
-and FENSE: ```bash aac-metrics-download ``` Notes: - The external code for
+[[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT-
+sim [[8]](#fense) - Fluency Error [[8]](#fense) - FENSE [[8]](#fense) - SPIDEr-
+FL [[9]](#spider-fl) ## Installation Install the pip package: ```bash pip
+install aac-metrics ``` Download the external code and models needed for
+METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and
+SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
 SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`. - The
 weights of the FENSE fluency error detector and the the SBERT model are
 respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and
-`$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default AAC
-metrics The full evaluation process to compute AAC metrics can be done with
-`aac_metrics.aac_evaluate` function. ```python from aac_metrics import
-aac_evaluate candidates: list[str] = ["a man is speaking"] mult_references:
-list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking
-while a bird is chirping in the background"]] corpus_scores, _ = aac_evaluate
-(candidates, mult_references) print(corpus_scores) # dict containing the score
-of each aac metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l",
-"meteor", "cider_d", "spice", "spider" # {"bleu_1": tensor(0.7), "bleu_2": ...,
-...} ``` ### Evaluate a specific metric Evaluate a specific metric can be done
-using the `aac_metrics.functional..` function or the `aac_metrics.classes..`
-class. Unlike `aac_evaluate`, the tokenization with PTBTokenizer is not done
-with these functions, but you can do it manually with `preprocess_mono_sents`
-and `preprocess_mult_sents` functions. ```python from aac_metrics.functional
-import cider_d from aac_metrics.utils.tokenization import
-preprocess_mono_sents, preprocess_mult_sents candidates: list[str] = ["a man is
-speaking"] mult_references: list[list[str]] = [["a man speaks.", "someone
-speaks.", "a man is speaking while a bird is chirping in the background"]]
-candidates = preprocess_mono_sents(candidates) mult_references =
-preprocess_mult_sents(mult_references) corpus_scores, sents_scores = cider_d
-(candidates, mult_references) print(corpus_scores) # {"cider_d": tensor(0.1)}
-print(sents_scores) # {"cider_d": tensor([0.9, ...])} ``` Each metrics also
-exists as a python class version, like `aac_metrics.classes.cider_d.CIDErD`. ##
-Metrics ### Default AAC metrics | Metric | Python Class | Origin | Range |
-Short description | |:---|:---|:---|:---|:---| | BLEU [[1]](#bleu) | `BLEU` |
-machine translation | [0, 1] | Precision of n-grams | | ROUGE-L [[2]](#rouge-l)
-| `ROUGEL` | machine translation | [0, 1] | FScore of the longest common
+`$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default
+metrics The full evaluation pipeline to compute AAC metrics can be done with
+`aac_metrics.evaluate` function. ```python from aac_metrics import evaluate
+candidates: list[str] = ["a man is speaking"] mult_references: list[list[str]]
+= [["a man speaks.", "someone speaks.", "a man is speaking while a bird is
+chirping in the background"]] corpus_scores, _ = evaluate(candidates,
+mult_references) print(corpus_scores) # dict containing the score of each
+metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d",
+"spice", "spider" # {"bleu_1": tensor(0.7), "bleu_2": ..., ...} ``` ###
+Evaluate DCASE2023 metrics To compute metrics for the DCASE2023 challenge, just
+set the argument `metrics="dcase2023"` in `evaluate` function call. ```python
+corpus_scores, _ = evaluate(candidates, mult_references, metrics="dcase2023")
+print(corpus_scores) # dict containing the score of each metric: "meteor",
+"cider_d", "spice", "spider", "spider_fl", "fluerr" ``` ### Evaluate a specific
+metric Evaluate a specific metric can be done using the
+`aac_metrics.functional..` function or the `aac_metrics.classes..` class.
+Unlike `evaluate`, the tokenization with PTBTokenizer is not done with these
+functions, but you can do it manually with `preprocess_mono_sents` and
+`preprocess_mult_sents` functions. ```python from aac_metrics.functional import
+cider_d from aac_metrics.utils.tokenization import preprocess_mono_sents,
+preprocess_mult_sents candidates: list[str] = ["a man is speaking"]
+mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man
+is speaking while a bird is chirping in the background"]] candidates =
+preprocess_mono_sents(candidates) mult_references = preprocess_mult_sents
+(mult_references) corpus_scores, sents_scores = cider_d(candidates,
+mult_references) print(corpus_scores) # {"cider_d": tensor(0.1)} print
+(sents_scores) # {"cider_d": tensor([0.9, ...])} ``` Each metrics also exists
+as a python class version, like `aac_metrics.classes.cider_d.CIDErD`. ##
+Metrics ### Legacy metrics | Metric | Python Class | Origin | Range | Short
+description | |:---|:---|:---|:---|:---| | BLEU [[1]](#bleu) | `BLEU` | machine
+translation | [0, 1] | Precision of n-grams | | ROUGE-L [[2]](#rouge-l) |
+`ROUGEL` | machine translation | [0, 1] | FScore of the longest common
 subsequence | | METEOR [[3]](#meteor) | `METEOR` | machine translation | [0, 1]
 | Cosine-similarity of frequencies with synonyms matching | | CIDEr-D [[4]]
 (#cider) | `CIDErD` | image captioning | [0, 10] | Cosine-similarity of TF-IDF
 computed on n-grams | | SPICE [[5]](#spice) | `SPICE` | image captioning | [0,
 1] | FScore of semantic graph | | SPIDEr [[6]](#spider) | `SPIDEr` | image
-captioning | [0, 5.5] | Mean of CIDEr-D and SPICE | ### Other metrics | Metric
-name | Python Class | Origin | Range | Short description | |:---|:---|:---|:---
-|:---| | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning | [0,
-5.5] | Max of SPIDEr scores for multiples candidates | | SBERT [[7]](#spider-
-max) | `SBERT` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-
-BERT embeddings** | | FluencyError [[7]](#spider-max) | `FluencyError` | audio
-captioning | [0, 1] | Use pretrained model to detect fluency errors in
+captioning | [0, 5.5] | Mean of CIDEr-D and SPICE | ### AAC-specific metrics |
+Metric name | Python Class | Origin | Range | Short description | |:---|:---|:-
+--|:---|:---| | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning
+| [0, 5.5] | Max of SPIDEr scores for multiples candidates | | SBERT-sim [[8]]
+(#spider-max) | `SBERTSim` | audio captioning | [-1, 1] | Cosine-similarity of
+**Sentence-BERT embeddings** | | Fluency Error [[8]](#spider-max) | `FluErr` |
+audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in
 sentences | | FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] |
-Combines `SBERT` and `FluencyError` | | SPIDErErr | `SPIDErErr` | audio
-captioning | [0, 5.5] | Combines `SPIDEr` and `FluencyError` | ## SPIDEr-max
-metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes
-into account multiple candidates for the same audio. It computes the maximum of
-the SPIDEr scores for each candidate to balance the high sensitivity to the
-frequency of the words generated by the model. ### SPIDEr-max: why ? The SPIDEr
-metric used in audio captioning is highly sensitive to the frequencies of the
-words used. Here is 2 examples with the 5 candidates generated by the beam
-search algorithm, their corresponding SPIDEr scores and the associated
-references:
- | Beam search candidates | SPIDEr | |:---|:---:| | heavy rain is falling on a
-  roof | 0.562 | | heavy rain is falling on **a tin roof** | **0.930** | | a
-  heavy rain is falling on a roof | 0.594 | | a heavy rain is falling on the
-ground | 0.335 | | a heavy rain is falling on the roof | 0.594 | | References |
- |:---| | heavy rain falls loudly onto a structure with a thin roof | | heavy
-rainfall falling onto a thin structure with a thin roof | | it is raining hard
-   and the rain hits **a tin roof** | | rain that is pouring down very hard
-outside | | the hard rain is noisy as it hits **a tin roof** | _(Candidates and
- references for the Clotho development-testing file named "rain.wav")_ | Beam
-search candidates | SPIDEr | |:---|:---:| | a woman speaks and a sheep bleats |
-0.190 | | a woman **speaks and a goat bleats** | **1.259** | | a man speaks and
-a sheep bleats | 0.344 | | an adult male speaks and a sheep bleats | 0.231 | |
-an adult male is speaking and a sheep bleats | 0.189 | | References | |:---| |
- a man speaking and laughing followed by a goat bleat | | a man is speaking in
-high tone while a goat is bleating one time | | a man speaks followed by a goat
-   bleat | | a person **speaks and a goat bleats** | | a man is talking and
-  snickering followed by a goat bleating | _(Candidates and references for an
-              AudioCaps testing file with the id "jid4t-FzUn0")_
-Even with very similar candidates, the SPIDEr scores varies drastically. To
-adress this issue, we proposed a SPIDEr-max metric which take the maximum value
-of several candidates for the same audio. SPIDEr-max demonstrate that SPIDEr
-can exceed state-of-the-art scores on AudioCaps and Clotho and even human
-scores on AudioCaps [[7]](#spider-max). ### SPIDEr-max: usage This usage is
-very similar to other captioning metrics, with the main difference of take a
-multiple candidates list as input. ```python from aac_metrics.functional import
-spider_max from aac_metrics.utils.tokenization import preprocess_mult_sents
-mult_candidates: list[list[str]] = [["a man is speaking", "maybe someone
-speaking"]] mult_references: list[list[str]] = [["a man speaks.", "someone
-speaks.", "a man is speaking while a bird is chirping in the background"]]
-mult_candidates = preprocess_mult_sents(mult_candidates) mult_references =
-preprocess_mult_sents(mult_references) corpus_scores, sents_scores = spider_max
-(mult_candidates, mult_references) print(corpus_scores) # {"spider": tensor
-(0.1), ...} print(sents_scores) # {"spider": tensor([0.9, ...]), ...} ``` ##
-Requirements ### Python packages The pip requirements are automatically
+Combines SBERT-sim and Fluency Error | | SPIDEr-FL [[9]](#spider-fl) |
+`SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
+## Requirements ### Python packages The pip requirements are automatically
 installed when using `pip install` on this repository. ``` torch >= 1.10.1
 numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers>=2.2.2 ```
-### External requirements - `java` >= 1.8 is required to compute METEOR, SPICE
-and use the PTBTokenizer. Most of these functions can specify a java executable
-path with `java_path` argument. - `unzip` command to extract SPICE zipped
-files. ## Additional notes ### CIDEr or CIDEr-D ? The CIDEr metric differs from
-CIDEr-D because it applies a stemmer to each word before computing the n-grams
-of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in
-[caption-evaluation-tools](https://github.com/audio-captioning/caption-
-evaluation-tools), but some papers called it "CIDEr". ### Does metrics work on
-multi-GPU ? No. Most of these metrics use numpy or external java programs to
-run, which prevents multi-GPU testing for now. ### Is torchmetrics needed for
-this package ? No. But if torchmetrics is installed, all metrics classes will
-inherit from the base class `torchmetrics.Metric`. It is because most of the
-metrics does not use PyTorch tensors to compute scores and numpy and strings
-cannot be added to states of `torchmetrics.Metric`. ## References #### BLEU [1]
-K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, âBLEU: a method for automatic
-evaluation of machine translation,â in Proceed- ings of the 40th Annual
-Meeting on Association for Computational Linguistics - ACL â02. Philadelphia,
-Pennsylvania: Association for Computational Linguistics, 2001, p. 311.
-[Online]. Available: http://portal.acm.org/citation.cfm?doid=1073083.1073135
-#### ROUGE-L [2] C.-Y. Lin, âROUGE: A package for automatic evaluation of
-summaries,â in Text Summarization Branches Out. Barcelona, Spain: Association
-for Computational Linguistics, Jul. 2004, pp. 74â81. [Online]. Available:
-https://aclanthology.org/W04-1013 #### METEOR [3] M. Denkowski and A. Lavie,
-âMeteor Universal: Language Specific Translation Evaluation for Any Target
-Language,â in Proceedings of the Ninth Workshop on Statistical Machine
-Translation. Baltimore, Maryland, USA: Association for Computational
-Linguistics, 2014, pp. 376â380. [Online]. Available: http://aclweb.org/
-anthology/W14-3348 #### CIDEr [4] R. Vedantam, C. L. Zitnick, and D. Parikh,
-âCIDEr: Consensus-based Image Description Evaluation,â arXiv:1411.5726
-[cs], Jun. 2015, arXiv: 1411.5726. [Online]. Available: http://arxiv.org/abs/
-1411.5726 #### SPICE [5] P. Anderson, B. Fernando, M. Johnson, and S. Gould,
-âSPICE: Semantic Propositional Image Caption Evaluation,â arXiv:1607.08822
-[cs], Jul. 2016, arXiv: 1607.08822. [Online]. Available: http://arxiv.org/abs/
-1607.08822 #### SPIDEr [6] S. Liu, Z. Zhu, N. Ye, S. Guadarrama, and K. Murphy,
-âImproved Image Captioning via Policy Gradient optimization of SPIDEr,â
-2017 IEEE Inter- national Conference on Computer Vision (ICCV), pp. 873â881,
-Oct. 2017, arXiv: 1612.00370. [Online]. Available: http://arxiv.org/abs/
-1612.00370 #### SPIDEr-max [7] E. LabbÃ©, T. Pellegrini, and J. Pinquier, âIs
-my automatic audio captioning system so bad? spider-max: a metric to consider
-several caption candidates,â Nov. 2022. [Online]. Available: https://
-hal.archives-ouvertes.fr/hal-03810396 #### FENSE [8] Z. Zhou, Z. Zhang, X. Xu,
-Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image
-Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/
-2110.04684 ## Citation If you use **SPIDEr-max**, you can cite the following
-paper using BibTex: ``` @inproceedings{labbe:hal-03810396, TITLE = {{Is my
-automatic audio captioning system so bad? spider-max: a metric to consider
-several caption candidates}}, AUTHOR = {Labb{\'e}, Etienne and Pellegrini,
-Thomas and Pinquier, Julien}, URL = {https://hal.archives-ouvertes.fr/hal-
-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy, France}, YEAR =
-{2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation metric ; beam
-search ; multiple candidates}, PDF = {https://hal.archives-ouvertes.fr/hal-
-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396}, HAL_VERSION =
-{v1}, } ``` ## Contact Maintainer: - Etienne LabbÃ© "Labbeti":
-labbeti.pub@gmail.com
+### External requirements - `java` **>= 1.8 and <= 1.11** is required to
+compute METEOR, SPICE and use the PTBTokenizer. Most of these functions can
+specify a java executable path with `java_path` argument. - `unzip` command to
+extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
+CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
+before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
+reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
+audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
+### Does metrics work on multi-GPU ? No. Most of these metrics use numpy or
+external java programs to run, which prevents multi-GPU testing for now. ### Is
+torchmetrics needed for this package ? No. But if torchmetrics is installed,
+all metrics classes will inherit from the base class `torchmetrics.Metric`. It
+is because most of the metrics does not use PyTorch tensors to compute scores
+and numpy and strings cannot be added to states of `torchmetrics.Metric`. ##
+SPIDEr-max metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr
+that takes into account multiple candidates for the same audio. It computes the
+maximum of the SPIDEr scores for each candidate to balance the high sensitivity
+to the frequency of the words generated by the model. For more detail, please
+see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/
+stable/spider_max.html). ## References #### BLEU [1] K. Papineni, S. Roukos, T.
+Ward, and W.-J. Zhu, âBLEU: a method for automatic evaluation of machine
+translation,â in Proceed- ings of the 40th Annual Meeting on Association for
+Computational Linguistics - ACL â02. Philadelphia, Pennsylvania: Association
+for Computational Linguistics, 2001, p. 311. [Online]. Available: http://
+portal.acm.org/citation.cfm?doid=1073083.1073135 #### ROUGE-L [2] C.-Y. Lin,
+âROUGE: A package for automatic evaluation of summaries,â in Text
+Summarization Branches Out. Barcelona, Spain: Association for Computational
+Linguistics, Jul. 2004, pp. 74â81. [Online]. Available: https://
+aclanthology.org/W04-1013 #### METEOR [3] M. Denkowski and A. Lavie, âMeteor
+Universal: Language Specific Translation Evaluation for Any Target Language,â
+in Proceedings of the Ninth Workshop on Statistical Machine Translation.
+Baltimore, Maryland, USA: Association for Computational Linguistics, 2014, pp.
+376â380. [Online]. Available: http://aclweb.org/anthology/W14-3348 #### CIDEr
+[4] R. Vedantam, C. L. Zitnick, and D. Parikh, âCIDEr: Consensus-based Image
+Description Evaluation,â arXiv:1411.5726 [cs], Jun. 2015, arXiv: 1411.5726.
+[Online]. Available: http://arxiv.org/abs/1411.5726 #### SPICE [5] P. Anderson,
+B. Fernando, M. Johnson, and S. Gould, âSPICE: Semantic Propositional Image
+Caption Evaluation,â arXiv:1607.08822 [cs], Jul. 2016, arXiv: 1607.08822.
+[Online]. Available: http://arxiv.org/abs/1607.08822 #### SPIDEr [6] S. Liu, Z.
+Zhu, N. Ye, S. Guadarrama, and K. Murphy, âImproved Image Captioning via
+Policy Gradient optimization of SPIDEr,â 2017 IEEE Inter- national Conference
+on Computer Vision (ICCV), pp. 873â881, Oct. 2017, arXiv: 1612.00370.
+[Online]. Available: http://arxiv.org/abs/1612.00370 #### SPIDEr-max [7] E.
+LabbÃ©, T. Pellegrini, and J. Pinquier, âIs my automatic audio captioning
+system so bad? spider-max: a metric to consider several caption candidates,â
+Nov. 2022. [Online]. Available: https://hal.archives-ouvertes.fr/hal-03810396
+#### FENSE [8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can
+Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online].
+Available: http://arxiv.org/abs/2110.04684 #### SPIDEr-FL [9] DCASE website
+task6a description: https://dcase.community/challenge2023/task-automated-audio-
+captioning#evaluation ## Citation If you use **SPIDEr-max**, you can cite the
+following paper using BibTex : ``` @inproceedings{labbe:hal-03810396, TITLE = {
+{Is my automatic audio captioning system so bad? spider-max: a metric to
+consider several caption candidates}}, AUTHOR = {Labb{\'e}, Etienne and
+Pellegrini, Thomas and Pinquier, Julien}, URL = {https://hal.archives-
+ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
+France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
+metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
+ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
+HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
+below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
+license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
+github.com/Labbeti/aac-metrics/}, version = {0.4.0}, year = {2023}, } ``` ##
+Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.3.0/README.md` & `aac-metrics-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -23,52 +23,60 @@
     - BLEU [[1]](#bleu)
     - ROUGE-L [[2]](#rouge-l)
     - METEOR [[3]](#meteor)
     - CIDEr-D [[4]](#cider)
     - SPICE [[5]](#spice)
     - SPIDEr [[6]](#spider)
     - SPIDEr-max [[7]](#spider-max)
-    - SBERT [[8]](#fense)
-    - FluencyError [[8]](#fense)
+    - SBERT-sim [[8]](#fense)
+    - Fluency Error [[8]](#fense)
     - FENSE [[8]](#fense)
-    - SPIDErErr
+    - SPIDEr-FL [[9]](#spider-fl)
 
 ## Installation
 Install the pip package:
 ```bash
 pip install aac-metrics
 ```
 
-Download the external code and models needed for METEOR, SPICE, PTBTokenizer and FENSE:
+Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and SPIDEr-FL:
 ```bash
 aac-metrics-download
 ```
 
 Notes:
 - The external code for SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`.
 - The weights of the FENSE fluency error detector and the the SBERT model are respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and `$HOME/.cache/torch/sentence_transformers`.
 
 ## Usage
-### Evaluate default AAC metrics
-The full evaluation process to compute AAC metrics can be done with `aac_metrics.aac_evaluate` function.
+### Evaluate default metrics
+The full evaluation pipeline to compute AAC metrics can be done with `aac_metrics.evaluate` function.
 
 ```python
-from aac_metrics import aac_evaluate
+from aac_metrics import evaluate
 
 candidates: list[str] = ["a man is speaking"]
 mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
 
-corpus_scores, _ = aac_evaluate(candidates, mult_references)
+corpus_scores, _ = evaluate(candidates, mult_references)
 print(corpus_scores)
-# dict containing the score of each aac metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d", "spice", "spider"
+# dict containing the score of each metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d", "spice", "spider"
 # {"bleu_1": tensor(0.7), "bleu_2": ..., ...}
 ```
+### Evaluate DCASE2023 metrics
+To compute metrics for the DCASE2023 challenge, just set the argument `metrics="dcase2023"` in `evaluate` function call.
+
+```python
+corpus_scores, _ = evaluate(candidates, mult_references, metrics="dcase2023")
+print(corpus_scores)
+# dict containing the score of each metric: "meteor", "cider_d", "spice", "spider", "spider_fl", "fluerr"
+```
 
 ### Evaluate a specific metric
-Evaluate a specific metric can be done using the `aac_metrics.functional.<metric_name>.<metric_name>` function or the `aac_metrics.classes.<metric_name>.<metric_name>` class. Unlike `aac_evaluate`, the tokenization with PTBTokenizer is not done with these functions, but you can do it manually with `preprocess_mono_sents` and `preprocess_mult_sents` functions.
+Evaluate a specific metric can be done using the `aac_metrics.functional.<metric_name>.<metric_name>` function or the `aac_metrics.classes.<metric_name>.<metric_name>` class. Unlike `evaluate`, the tokenization with PTBTokenizer is not done with these functions, but you can do it manually with `preprocess_mono_sents` and `preprocess_mult_sents` functions.
 
 ```python
 from aac_metrics.functional import cider_d
 from aac_metrics.utils.tokenization import preprocess_mono_sents, preprocess_mult_sents
 
 candidates: list[str] = ["a man is speaking"]
 mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
@@ -82,132 +90,65 @@
 print(sents_scores)
 # {"cider_d": tensor([0.9, ...])}
 ```
 
 Each metrics also exists as a python class version, like `aac_metrics.classes.cider_d.CIDErD`.
 
 ## Metrics
-### Default AAC metrics
+### Legacy metrics
 | Metric | Python Class | Origin | Range | Short description |
 |:---|:---|:---|:---|:---|
 | BLEU [[1]](#bleu) | `BLEU` | machine translation | [0, 1] | Precision of n-grams |
 | ROUGE-L [[2]](#rouge-l) | `ROUGEL` | machine translation | [0, 1] | FScore of the longest common subsequence |
 | METEOR [[3]](#meteor) | `METEOR` | machine translation | [0, 1] | Cosine-similarity of frequencies with synonyms matching |
 | CIDEr-D [[4]](#cider) | `CIDErD` | image captioning | [0, 10] | Cosine-similarity of TF-IDF computed on n-grams |
 | SPICE [[5]](#spice) | `SPICE` | image captioning | [0, 1] | FScore of semantic graph |
 | SPIDEr [[6]](#spider) | `SPIDEr` | image captioning | [0, 5.5] | Mean of CIDEr-D and SPICE |
 
-### Other metrics
+### AAC-specific metrics
 | Metric name | Python Class | Origin | Range | Short description |
 |:---|:---|:---|:---|:---|
 | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning | [0, 5.5] | Max of SPIDEr scores for multiples candidates |
-| SBERT [[7]](#spider-max) | `SBERT` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-BERT embeddings** |
-| FluencyError [[7]](#spider-max) | `FluencyError` | audio captioning | [0, 1] | Use pretrained model to detect fluency errors in sentences |
-| FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] | Combines `SBERT` and `FluencyError` |
-| SPIDErErr | `SPIDErErr` | audio captioning | [0, 5.5] | Combines `SPIDEr` and `FluencyError` |
-
-## SPIDEr-max metric
-SPIDEr-max [[7]](#spider-max)  is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model.
-
-### SPIDEr-max: why ?
-The SPIDEr metric used in audio captioning is highly sensitive to the frequencies of the words used.
-
-Here is 2 examples with the 5 candidates generated by the beam search algorithm, their corresponding SPIDEr scores and the associated references:
-
-<div align="center">
-
-| Beam search candidates | SPIDEr |
-|:---|:---:|
-| heavy rain is falling on a roof | 0.562 |
-| heavy rain is falling on **a tin roof** | **0.930** |
-| a heavy rain is falling on a roof | 0.594 |
-| a heavy rain is falling on the ground | 0.335 |
-| a heavy rain is falling on the roof | 0.594 |
-
-| References |
-|:---|
-| heavy rain falls loudly onto a structure with a thin roof |
-| heavy rainfall falling onto a thin structure with a thin roof |
-| it is raining hard and the rain hits **a tin roof** |
-| rain that is pouring down very hard outside |
-| the hard rain is noisy as it hits **a tin roof** |
-
-_(Candidates and references for the Clotho development-testing file named "rain.wav")_
-
-| Beam search candidates | SPIDEr |
-|:---|:---:|
-| a woman speaks and a sheep bleats | 0.190 |
-| a woman **speaks and a goat bleats** | **1.259** |
-| a man speaks and a sheep bleats | 0.344 |
-| an adult male speaks and a sheep bleats | 0.231 |
-| an adult male is speaking and a sheep bleats | 0.189 |
-
-| References |
-|:---|
-| a man speaking and laughing followed by a goat bleat |
-| a man is speaking in high tone while a goat is bleating one time |
-| a man speaks followed by a goat bleat |
-| a person **speaks and a goat bleats** |
-| a man is talking and snickering followed by a goat bleating |
-
-_(Candidates and references for an AudioCaps testing file with the id "jid4t-FzUn0")_
-</div>
-
-Even with very similar candidates, the SPIDEr scores varies drastically. To adress this issue, we proposed a SPIDEr-max metric which take the maximum value of several candidates for the same audio. SPIDEr-max demonstrate that SPIDEr can exceed state-of-the-art scores on AudioCaps and Clotho and even human scores on AudioCaps [[7]](#spider-max).
-
-### SPIDEr-max: usage
-This usage is very similar to other captioning metrics, with the main difference of take a multiple candidates list as input.
-
-```python
-from aac_metrics.functional import spider_max
-from aac_metrics.utils.tokenization import preprocess_mult_sents
-
-mult_candidates: list[list[str]] = [["a man is speaking", "maybe someone speaking"]]
-mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
-
-mult_candidates = preprocess_mult_sents(mult_candidates)
-mult_references = preprocess_mult_sents(mult_references)
-
-corpus_scores, sents_scores = spider_max(mult_candidates, mult_references)
-print(corpus_scores)
-# {"spider": tensor(0.1), ...}
-print(sents_scores)
-# {"spider": tensor([0.9, ...]), ...}
-```
+| SBERT-sim [[8]](#spider-max) | `SBERTSim` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-BERT embeddings** |
+| Fluency Error [[8]](#spider-max) | `FluErr` | audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in sentences |
+| FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] | Combines SBERT-sim and Fluency Error |
+| SPIDEr-FL [[9]](#spider-fl) | `SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
 
 ## Requirements
 ### Python packages
 
 The pip requirements are automatically installed when using `pip install` on this repository.
 ```
 torch >= 1.10.1
 numpy >= 1.21.2
 pyyaml >= 6.0
 tqdm >= 4.64.0
 sentence-transformers>=2.2.2
 ```
 
 ### External requirements
-- `java` >= 1.8 is required to compute METEOR, SPICE and use the PTBTokenizer.
+- `java` **>= 1.8 and <= 1.11** is required to compute METEOR, SPICE and use the PTBTokenizer.
 Most of these functions can specify a java executable path with `java_path` argument.
 
 - `unzip` command to extract SPICE zipped files.
 
-
 ## Additional notes
 ### CIDEr or CIDEr-D ?
 The CIDEr metric differs from CIDEr-D because it applies a stemmer to each word before computing the n-grams of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 
 ### Does metrics work on multi-GPU ?
 No. Most of these metrics use numpy or external java programs to run, which prevents multi-GPU testing for now.
 
 ### Is torchmetrics needed for this package ?
 No. But if torchmetrics is installed, all metrics classes will inherit from the base class `torchmetrics.Metric`.
 It is because most of the metrics does not use PyTorch tensors to compute scores and numpy and strings cannot be added to states of `torchmetrics.Metric`.
 
+## SPIDEr-max metric
+SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model. For more detail, please see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/stable/spider_max.html).
+
 ## References
 #### BLEU
 [1] K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, “BLEU: a
 method for automatic evaluation of machine translation,” in Proceed-
 ings of the 40th Annual Meeting on Association for Computational
 Linguistics - ACL ’02. Philadelphia, Pennsylvania: Association
 for Computational Linguistics, 2001, p. 311. [Online]. Available:
@@ -242,18 +183,21 @@
 national Conference on Computer Vision (ICCV), pp. 873–881, Oct. 2017,
 arXiv: 1612.00370. [Online]. Available: http://arxiv.org/abs/1612.00370
 
 #### SPIDEr-max
 [7] E. Labbé, T. Pellegrini, and J. Pinquier, “Is my automatic audio captioning system so bad? spider-max: a metric to consider several caption candidates,” Nov. 2022. [Online]. Available: https://hal.archives-ouvertes.fr/hal-03810396
 
 #### FENSE
-[8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/2110.04684 
+[8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/2110.04684
+
+#### SPIDEr-FL
+[9] DCASE website task6a description: https://dcase.community/challenge2023/task-automated-audio-captioning#evaluation
 
 ## Citation
-If you use **SPIDEr-max**, you can cite the following paper using BibTex:
+If you use **SPIDEr-max**, you can cite the following paper using BibTex :
 ```
 @inproceedings{labbe:hal-03810396,
     TITLE = {{Is my automatic audio captioning system so bad? spider-max: a metric to consider several caption candidates}},
     AUTHOR = {Labb{\'e}, Etienne and Pellegrini, Thomas and Pinquier, Julien},
     URL = {https://hal.archives-ouvertes.fr/hal-03810396},
     BOOKTITLE = {{Workshop DCASE}},
     ADDRESS = {Nancy, France},
@@ -262,10 +206,24 @@
     KEYWORDS = {audio captioning ; evaluation metric ; beam search ; multiple candidates},
     PDF = {https://hal.archives-ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf},
     HAL_ID = {hal-03810396},
     HAL_VERSION = {v1},
 }
 ```
 
+If you use this software, please consider cite it as below :
+```
+@software{
+    Labbe_aac-metrics_2023,
+    author = {Labbé, Etienne},
+    license = {MIT},
+    month = {4},
+    title = {{aac-metrics}},
+    url = {https://github.com/Labbeti/aac-metrics/},
+    version = {0.4.0},
+    year = {2023},
+}
+```
+
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -2,155 +2,130 @@
      [Build] [Documentation_Status] Metrics for evaluating Automated Audio
                    Captioning systems, designed for PyTorch.
 ## Why using this package? - **Easy installation and download** - **Same
 results than [caption-evaluation-tools](https://github.com/audio-captioning/
 caption-evaluation-tools) and [fense](https://github.com/blmoistawinde/fense)
 repositories** - **Provides the following metrics:** - BLEU [[1]](#bleu) -
 ROUGE-L [[2]](#rouge-l) - METEOR [[3]](#meteor) - CIDEr-D [[4]](#cider) - SPICE
-[[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT [
-[8]](#fense) - FluencyError [[8]](#fense) - FENSE [[8]](#fense) - SPIDErErr ##
-Installation Install the pip package: ```bash pip install aac-metrics ```
-Download the external code and models needed for METEOR, SPICE, PTBTokenizer
-and FENSE: ```bash aac-metrics-download ``` Notes: - The external code for
+[[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT-
+sim [[8]](#fense) - Fluency Error [[8]](#fense) - FENSE [[8]](#fense) - SPIDEr-
+FL [[9]](#spider-fl) ## Installation Install the pip package: ```bash pip
+install aac-metrics ``` Download the external code and models needed for
+METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and
+SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
 SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`. - The
 weights of the FENSE fluency error detector and the the SBERT model are
 respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and
-`$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default AAC
-metrics The full evaluation process to compute AAC metrics can be done with
-`aac_metrics.aac_evaluate` function. ```python from aac_metrics import
-aac_evaluate candidates: list[str] = ["a man is speaking"] mult_references:
-list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking
-while a bird is chirping in the background"]] corpus_scores, _ = aac_evaluate
-(candidates, mult_references) print(corpus_scores) # dict containing the score
-of each aac metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l",
-"meteor", "cider_d", "spice", "spider" # {"bleu_1": tensor(0.7), "bleu_2": ...,
-...} ``` ### Evaluate a specific metric Evaluate a specific metric can be done
-using the `aac_metrics.functional..` function or the `aac_metrics.classes..`
-class. Unlike `aac_evaluate`, the tokenization with PTBTokenizer is not done
-with these functions, but you can do it manually with `preprocess_mono_sents`
-and `preprocess_mult_sents` functions. ```python from aac_metrics.functional
-import cider_d from aac_metrics.utils.tokenization import
-preprocess_mono_sents, preprocess_mult_sents candidates: list[str] = ["a man is
-speaking"] mult_references: list[list[str]] = [["a man speaks.", "someone
-speaks.", "a man is speaking while a bird is chirping in the background"]]
-candidates = preprocess_mono_sents(candidates) mult_references =
-preprocess_mult_sents(mult_references) corpus_scores, sents_scores = cider_d
-(candidates, mult_references) print(corpus_scores) # {"cider_d": tensor(0.1)}
-print(sents_scores) # {"cider_d": tensor([0.9, ...])} ``` Each metrics also
-exists as a python class version, like `aac_metrics.classes.cider_d.CIDErD`. ##
-Metrics ### Default AAC metrics | Metric | Python Class | Origin | Range |
-Short description | |:---|:---|:---|:---|:---| | BLEU [[1]](#bleu) | `BLEU` |
-machine translation | [0, 1] | Precision of n-grams | | ROUGE-L [[2]](#rouge-l)
-| `ROUGEL` | machine translation | [0, 1] | FScore of the longest common
+`$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default
+metrics The full evaluation pipeline to compute AAC metrics can be done with
+`aac_metrics.evaluate` function. ```python from aac_metrics import evaluate
+candidates: list[str] = ["a man is speaking"] mult_references: list[list[str]]
+= [["a man speaks.", "someone speaks.", "a man is speaking while a bird is
+chirping in the background"]] corpus_scores, _ = evaluate(candidates,
+mult_references) print(corpus_scores) # dict containing the score of each
+metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d",
+"spice", "spider" # {"bleu_1": tensor(0.7), "bleu_2": ..., ...} ``` ###
+Evaluate DCASE2023 metrics To compute metrics for the DCASE2023 challenge, just
+set the argument `metrics="dcase2023"` in `evaluate` function call. ```python
+corpus_scores, _ = evaluate(candidates, mult_references, metrics="dcase2023")
+print(corpus_scores) # dict containing the score of each metric: "meteor",
+"cider_d", "spice", "spider", "spider_fl", "fluerr" ``` ### Evaluate a specific
+metric Evaluate a specific metric can be done using the
+`aac_metrics.functional..` function or the `aac_metrics.classes..` class.
+Unlike `evaluate`, the tokenization with PTBTokenizer is not done with these
+functions, but you can do it manually with `preprocess_mono_sents` and
+`preprocess_mult_sents` functions. ```python from aac_metrics.functional import
+cider_d from aac_metrics.utils.tokenization import preprocess_mono_sents,
+preprocess_mult_sents candidates: list[str] = ["a man is speaking"]
+mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man
+is speaking while a bird is chirping in the background"]] candidates =
+preprocess_mono_sents(candidates) mult_references = preprocess_mult_sents
+(mult_references) corpus_scores, sents_scores = cider_d(candidates,
+mult_references) print(corpus_scores) # {"cider_d": tensor(0.1)} print
+(sents_scores) # {"cider_d": tensor([0.9, ...])} ``` Each metrics also exists
+as a python class version, like `aac_metrics.classes.cider_d.CIDErD`. ##
+Metrics ### Legacy metrics | Metric | Python Class | Origin | Range | Short
+description | |:---|:---|:---|:---|:---| | BLEU [[1]](#bleu) | `BLEU` | machine
+translation | [0, 1] | Precision of n-grams | | ROUGE-L [[2]](#rouge-l) |
+`ROUGEL` | machine translation | [0, 1] | FScore of the longest common
 subsequence | | METEOR [[3]](#meteor) | `METEOR` | machine translation | [0, 1]
 | Cosine-similarity of frequencies with synonyms matching | | CIDEr-D [[4]]
 (#cider) | `CIDErD` | image captioning | [0, 10] | Cosine-similarity of TF-IDF
 computed on n-grams | | SPICE [[5]](#spice) | `SPICE` | image captioning | [0,
 1] | FScore of semantic graph | | SPIDEr [[6]](#spider) | `SPIDEr` | image
-captioning | [0, 5.5] | Mean of CIDEr-D and SPICE | ### Other metrics | Metric
-name | Python Class | Origin | Range | Short description | |:---|:---|:---|:---
-|:---| | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning | [0,
-5.5] | Max of SPIDEr scores for multiples candidates | | SBERT [[7]](#spider-
-max) | `SBERT` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-
-BERT embeddings** | | FluencyError [[7]](#spider-max) | `FluencyError` | audio
-captioning | [0, 1] | Use pretrained model to detect fluency errors in
+captioning | [0, 5.5] | Mean of CIDEr-D and SPICE | ### AAC-specific metrics |
+Metric name | Python Class | Origin | Range | Short description | |:---|:---|:-
+--|:---|:---| | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning
+| [0, 5.5] | Max of SPIDEr scores for multiples candidates | | SBERT-sim [[8]]
+(#spider-max) | `SBERTSim` | audio captioning | [-1, 1] | Cosine-similarity of
+**Sentence-BERT embeddings** | | Fluency Error [[8]](#spider-max) | `FluErr` |
+audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in
 sentences | | FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] |
-Combines `SBERT` and `FluencyError` | | SPIDErErr | `SPIDErErr` | audio
-captioning | [0, 5.5] | Combines `SPIDEr` and `FluencyError` | ## SPIDEr-max
-metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes
-into account multiple candidates for the same audio. It computes the maximum of
-the SPIDEr scores for each candidate to balance the high sensitivity to the
-frequency of the words generated by the model. ### SPIDEr-max: why ? The SPIDEr
-metric used in audio captioning is highly sensitive to the frequencies of the
-words used. Here is 2 examples with the 5 candidates generated by the beam
-search algorithm, their corresponding SPIDEr scores and the associated
-references:
- | Beam search candidates | SPIDEr | |:---|:---:| | heavy rain is falling on a
-  roof | 0.562 | | heavy rain is falling on **a tin roof** | **0.930** | | a
-  heavy rain is falling on a roof | 0.594 | | a heavy rain is falling on the
-ground | 0.335 | | a heavy rain is falling on the roof | 0.594 | | References |
- |:---| | heavy rain falls loudly onto a structure with a thin roof | | heavy
-rainfall falling onto a thin structure with a thin roof | | it is raining hard
-   and the rain hits **a tin roof** | | rain that is pouring down very hard
-outside | | the hard rain is noisy as it hits **a tin roof** | _(Candidates and
- references for the Clotho development-testing file named "rain.wav")_ | Beam
-search candidates | SPIDEr | |:---|:---:| | a woman speaks and a sheep bleats |
-0.190 | | a woman **speaks and a goat bleats** | **1.259** | | a man speaks and
-a sheep bleats | 0.344 | | an adult male speaks and a sheep bleats | 0.231 | |
-an adult male is speaking and a sheep bleats | 0.189 | | References | |:---| |
- a man speaking and laughing followed by a goat bleat | | a man is speaking in
-high tone while a goat is bleating one time | | a man speaks followed by a goat
-   bleat | | a person **speaks and a goat bleats** | | a man is talking and
-  snickering followed by a goat bleating | _(Candidates and references for an
-              AudioCaps testing file with the id "jid4t-FzUn0")_
-Even with very similar candidates, the SPIDEr scores varies drastically. To
-adress this issue, we proposed a SPIDEr-max metric which take the maximum value
-of several candidates for the same audio. SPIDEr-max demonstrate that SPIDEr
-can exceed state-of-the-art scores on AudioCaps and Clotho and even human
-scores on AudioCaps [[7]](#spider-max). ### SPIDEr-max: usage This usage is
-very similar to other captioning metrics, with the main difference of take a
-multiple candidates list as input. ```python from aac_metrics.functional import
-spider_max from aac_metrics.utils.tokenization import preprocess_mult_sents
-mult_candidates: list[list[str]] = [["a man is speaking", "maybe someone
-speaking"]] mult_references: list[list[str]] = [["a man speaks.", "someone
-speaks.", "a man is speaking while a bird is chirping in the background"]]
-mult_candidates = preprocess_mult_sents(mult_candidates) mult_references =
-preprocess_mult_sents(mult_references) corpus_scores, sents_scores = spider_max
-(mult_candidates, mult_references) print(corpus_scores) # {"spider": tensor
-(0.1), ...} print(sents_scores) # {"spider": tensor([0.9, ...]), ...} ``` ##
-Requirements ### Python packages The pip requirements are automatically
+Combines SBERT-sim and Fluency Error | | SPIDEr-FL [[9]](#spider-fl) |
+`SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
+## Requirements ### Python packages The pip requirements are automatically
 installed when using `pip install` on this repository. ``` torch >= 1.10.1
 numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers>=2.2.2 ```
-### External requirements - `java` >= 1.8 is required to compute METEOR, SPICE
-and use the PTBTokenizer. Most of these functions can specify a java executable
-path with `java_path` argument. - `unzip` command to extract SPICE zipped
-files. ## Additional notes ### CIDEr or CIDEr-D ? The CIDEr metric differs from
-CIDEr-D because it applies a stemmer to each word before computing the n-grams
-of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in
-[caption-evaluation-tools](https://github.com/audio-captioning/caption-
-evaluation-tools), but some papers called it "CIDEr". ### Does metrics work on
-multi-GPU ? No. Most of these metrics use numpy or external java programs to
-run, which prevents multi-GPU testing for now. ### Is torchmetrics needed for
-this package ? No. But if torchmetrics is installed, all metrics classes will
-inherit from the base class `torchmetrics.Metric`. It is because most of the
-metrics does not use PyTorch tensors to compute scores and numpy and strings
-cannot be added to states of `torchmetrics.Metric`. ## References #### BLEU [1]
-K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, âBLEU: a method for automatic
-evaluation of machine translation,â in Proceed- ings of the 40th Annual
-Meeting on Association for Computational Linguistics - ACL â02. Philadelphia,
-Pennsylvania: Association for Computational Linguistics, 2001, p. 311.
-[Online]. Available: http://portal.acm.org/citation.cfm?doid=1073083.1073135
-#### ROUGE-L [2] C.-Y. Lin, âROUGE: A package for automatic evaluation of
-summaries,â in Text Summarization Branches Out. Barcelona, Spain: Association
-for Computational Linguistics, Jul. 2004, pp. 74â81. [Online]. Available:
-https://aclanthology.org/W04-1013 #### METEOR [3] M. Denkowski and A. Lavie,
-âMeteor Universal: Language Specific Translation Evaluation for Any Target
-Language,â in Proceedings of the Ninth Workshop on Statistical Machine
-Translation. Baltimore, Maryland, USA: Association for Computational
-Linguistics, 2014, pp. 376â380. [Online]. Available: http://aclweb.org/
-anthology/W14-3348 #### CIDEr [4] R. Vedantam, C. L. Zitnick, and D. Parikh,
-âCIDEr: Consensus-based Image Description Evaluation,â arXiv:1411.5726
-[cs], Jun. 2015, arXiv: 1411.5726. [Online]. Available: http://arxiv.org/abs/
-1411.5726 #### SPICE [5] P. Anderson, B. Fernando, M. Johnson, and S. Gould,
-âSPICE: Semantic Propositional Image Caption Evaluation,â arXiv:1607.08822
-[cs], Jul. 2016, arXiv: 1607.08822. [Online]. Available: http://arxiv.org/abs/
-1607.08822 #### SPIDEr [6] S. Liu, Z. Zhu, N. Ye, S. Guadarrama, and K. Murphy,
-âImproved Image Captioning via Policy Gradient optimization of SPIDEr,â
-2017 IEEE Inter- national Conference on Computer Vision (ICCV), pp. 873â881,
-Oct. 2017, arXiv: 1612.00370. [Online]. Available: http://arxiv.org/abs/
-1612.00370 #### SPIDEr-max [7] E. LabbÃ©, T. Pellegrini, and J. Pinquier, âIs
-my automatic audio captioning system so bad? spider-max: a metric to consider
-several caption candidates,â Nov. 2022. [Online]. Available: https://
-hal.archives-ouvertes.fr/hal-03810396 #### FENSE [8] Z. Zhou, Z. Zhang, X. Xu,
-Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image
-Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/
-2110.04684 ## Citation If you use **SPIDEr-max**, you can cite the following
-paper using BibTex: ``` @inproceedings{labbe:hal-03810396, TITLE = {{Is my
-automatic audio captioning system so bad? spider-max: a metric to consider
-several caption candidates}}, AUTHOR = {Labb{\'e}, Etienne and Pellegrini,
-Thomas and Pinquier, Julien}, URL = {https://hal.archives-ouvertes.fr/hal-
-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy, France}, YEAR =
-{2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation metric ; beam
-search ; multiple candidates}, PDF = {https://hal.archives-ouvertes.fr/hal-
-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396}, HAL_VERSION =
-{v1}, } ``` ## Contact Maintainer: - Etienne LabbÃ© "Labbeti":
-labbeti.pub@gmail.com
+### External requirements - `java` **>= 1.8 and <= 1.11** is required to
+compute METEOR, SPICE and use the PTBTokenizer. Most of these functions can
+specify a java executable path with `java_path` argument. - `unzip` command to
+extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
+CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
+before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
+reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
+audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
+### Does metrics work on multi-GPU ? No. Most of these metrics use numpy or
+external java programs to run, which prevents multi-GPU testing for now. ### Is
+torchmetrics needed for this package ? No. But if torchmetrics is installed,
+all metrics classes will inherit from the base class `torchmetrics.Metric`. It
+is because most of the metrics does not use PyTorch tensors to compute scores
+and numpy and strings cannot be added to states of `torchmetrics.Metric`. ##
+SPIDEr-max metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr
+that takes into account multiple candidates for the same audio. It computes the
+maximum of the SPIDEr scores for each candidate to balance the high sensitivity
+to the frequency of the words generated by the model. For more detail, please
+see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/
+stable/spider_max.html). ## References #### BLEU [1] K. Papineni, S. Roukos, T.
+Ward, and W.-J. Zhu, âBLEU: a method for automatic evaluation of machine
+translation,â in Proceed- ings of the 40th Annual Meeting on Association for
+Computational Linguistics - ACL â02. Philadelphia, Pennsylvania: Association
+for Computational Linguistics, 2001, p. 311. [Online]. Available: http://
+portal.acm.org/citation.cfm?doid=1073083.1073135 #### ROUGE-L [2] C.-Y. Lin,
+âROUGE: A package for automatic evaluation of summaries,â in Text
+Summarization Branches Out. Barcelona, Spain: Association for Computational
+Linguistics, Jul. 2004, pp. 74â81. [Online]. Available: https://
+aclanthology.org/W04-1013 #### METEOR [3] M. Denkowski and A. Lavie, âMeteor
+Universal: Language Specific Translation Evaluation for Any Target Language,â
+in Proceedings of the Ninth Workshop on Statistical Machine Translation.
+Baltimore, Maryland, USA: Association for Computational Linguistics, 2014, pp.
+376â380. [Online]. Available: http://aclweb.org/anthology/W14-3348 #### CIDEr
+[4] R. Vedantam, C. L. Zitnick, and D. Parikh, âCIDEr: Consensus-based Image
+Description Evaluation,â arXiv:1411.5726 [cs], Jun. 2015, arXiv: 1411.5726.
+[Online]. Available: http://arxiv.org/abs/1411.5726 #### SPICE [5] P. Anderson,
+B. Fernando, M. Johnson, and S. Gould, âSPICE: Semantic Propositional Image
+Caption Evaluation,â arXiv:1607.08822 [cs], Jul. 2016, arXiv: 1607.08822.
+[Online]. Available: http://arxiv.org/abs/1607.08822 #### SPIDEr [6] S. Liu, Z.
+Zhu, N. Ye, S. Guadarrama, and K. Murphy, âImproved Image Captioning via
+Policy Gradient optimization of SPIDEr,â 2017 IEEE Inter- national Conference
+on Computer Vision (ICCV), pp. 873â881, Oct. 2017, arXiv: 1612.00370.
+[Online]. Available: http://arxiv.org/abs/1612.00370 #### SPIDEr-max [7] E.
+LabbÃ©, T. Pellegrini, and J. Pinquier, âIs my automatic audio captioning
+system so bad? spider-max: a metric to consider several caption candidates,â
+Nov. 2022. [Online]. Available: https://hal.archives-ouvertes.fr/hal-03810396
+#### FENSE [8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can
+Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online].
+Available: http://arxiv.org/abs/2110.04684 #### SPIDEr-FL [9] DCASE website
+task6a description: https://dcase.community/challenge2023/task-automated-audio-
+captioning#evaluation ## Citation If you use **SPIDEr-max**, you can cite the
+following paper using BibTex : ``` @inproceedings{labbe:hal-03810396, TITLE = {
+{Is my automatic audio captioning system so bad? spider-max: a metric to
+consider several caption candidates}}, AUTHOR = {Labb{\'e}, Etienne and
+Pellegrini, Thomas and Pinquier, Julien}, URL = {https://hal.archives-
+ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
+France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
+metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
+ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
+HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
+below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
+license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
+github.com/Labbeti/aac-metrics/}, version = {0.4.0}, year = {2023}, } ``` ##
+Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.3.0/examples/example_1.csv` & `aac-metrics-0.4.0/examples/example_1.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/examples/example_2.csv` & `aac-metrics-0.4.0/examples/example_2.csv`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/install_spice.sh` & `aac-metrics-0.4.0/install_spice.sh`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/__init__.py` & `aac-metrics-0.4.0/src/aac_metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,53 +6,53 @@
 
 __name__ = "aac-metrics"
 __author__ = "Etienne Labbé (Labbeti)"
 __author_email__ = "labbeti.pub@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "Etienne Labbé (Labbeti)"
 __status__ = "Development"
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 
 from .classes.base import AACMetric
 from .classes.bleu import BLEU
 from .classes.cider_d import CIDErD
-from .classes.evaluate import AACEvaluate, _get_metrics_classes_factory
+from .classes.evaluate import AACEvaluate, _get_metric_factory_classes
 from .classes.fense import FENSE
 from .classes.meteor import METEOR
 from .classes.rouge_l import ROUGEL
 from .classes.spice import SPICE
 from .classes.spider import SPIDEr
-from .functional.evaluate import aac_evaluate, evaluate
+from .functional.evaluate import dcase2023_evaluate, evaluate
 
 
 __all__ = [
     "BLEU",
     "CIDErD",
     "AACEvaluate",
     "FENSE",
     "METEOR",
     "ROUGEL",
     "SPICE",
     "SPIDEr",
-    "aac_evaluate",
+    "dcase2023_evaluate",
     "evaluate",
 ]
 
 
 def load_metric(name: str, **kwargs) -> AACMetric:
     """Load a metric class by name.
 
     :param name: The name of the metric.
         Must be one of ("bleu_1", "bleu_2", "bleu_3", "bleu_4", "meteor", "rouge_l", "cider_d", "spice", "spider", "fense").
     :param **kwargs: The keyword optional arguments passed to the metric.
     :returns: The Metric object built.
     """
     name = name.lower().strip()
 
-    factory = _get_metrics_classes_factory(**kwargs)
+    factory = _get_metric_factory_classes(**kwargs)
     if name in factory:
         return factory[name]()
     else:
         raise ValueError(
             f"Invalid argument {name=}. (expected one of {tuple(factory.keys())})"
         )
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/__main__.py` & `aac-metrics-0.4.0/src/aac_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/__init__.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .bleu import BLEU
-from .cider_d import CIDErD
-from .evaluate import Evaluate, AACEvaluate
-from .fense import FENSE
-from .fluency_error import FluencyError
-from .meteor import METEOR
-from .rouge_l import ROUGEL
-from .sbert import SBERT
-from .spice import SPICE
-from .spider import SPIDEr
-from .spider_max import SPIDErMax
+from .bleu import bleu
+from .cider_d import cider_d
+from .evaluate import dcase2023_evaluate, evaluate
+from .fense import fense
+from .fluerr import fluerr
+from .meteor import meteor
+from .rouge_l import rouge_l
+from .sbert_sim import sbert_sim
+from .spice import spice
+from .spider import spider
+from .spider_fl import spider_fl
+from .spider_max import spider_max
 
 
 __all__ = [
-    "BLEU",
-    "CIDErD",
-    "AACEvaluate",
-    "Evaluate",
-    "FENSE",
-    "FluencyError",
-    "METEOR",
-    "ROUGEL",
-    "SBERT",
-    "SPICE",
-    "SPIDEr",
-    "SPIDErMax",
+    "bleu",
+    "cider_d",
+    "dcase2023_evaluate",
+    "evaluate",
+    "fense",
+    "fluerr",
+    "meteor",
+    "rouge_l",
+    "sbert_sim",
+    "spice",
+    "spider",
+    "spider_fl",
+    "spider_max",
 ]
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/base.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/base.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/bleu.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/cider_d.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/cider_d.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/evaluate.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 
 import torch
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
 from aac_metrics.classes.bleu import BLEU
+from aac_metrics.classes.cider_d import CIDErD
 from aac_metrics.classes.fense import FENSE
-from aac_metrics.classes.fluency_error import FluencyError
+from aac_metrics.classes.fluerr import FluErr
 from aac_metrics.classes.meteor import METEOR
 from aac_metrics.classes.rouge_l import ROUGEL
-from aac_metrics.classes.sbert import SBERT
+from aac_metrics.classes.sbert_sim import SBERTSim
+from aac_metrics.classes.spice import SPICE
 from aac_metrics.classes.spider import SPIDEr
+from aac_metrics.classes.spider_fl import SPIDErFL
 from aac_metrics.functional.evaluate import METRICS_SETS, evaluate
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 class Evaluate(AACMetric, list[AACMetric]):
     """Evaluate candidates with multiple references with custom metrics.
 
     For more information, see :func:`~aac_metrics.functional.evaluate.evaluate`.
     """
@@ -32,53 +35,53 @@
     full_state_update = False
     higher_is_better = None
     is_differentiable = False
 
     def __init__(
         self,
         preprocess: bool = True,
+        metrics: Union[str, Iterable[str], Iterable[AACMetric]] = "aac",
         cache_path: str = "$HOME/.cache",
         java_path: str = "java",
         tmp_path: str = "/tmp",
         device: Union[str, torch.device, None] = "auto",
         verbose: int = 0,
-        metrics: Union[str, Iterable[AACMetric]] = "aac",
     ) -> None:
-        if isinstance(metrics, str):
-            metrics = _get_metrics_classes_list(
-                metrics,
-                True,
-                cache_path,
-                java_path,
-                tmp_path,
-                device,
-                verbose,
-            )
+        metrics = _instantiate_metrics_classes(
+            metrics,
+            cache_path,
+            java_path,
+            tmp_path,
+            device,
+            verbose,
+        )
 
         AACMetric.__init__(self)
         list.__init__(self, metrics)
         self._preprocess = preprocess
         self._cache_path = cache_path
         self._java_path = java_path
         self._tmp_path = tmp_path
+        self._device = device
         self._verbose = verbose
 
         self._candidates = []
         self._mult_references = []
 
     def compute(self) -> tuple[dict[str, Tensor], dict[str, Tensor]]:
         return evaluate(
             self._candidates,
             self._mult_references,
             self._preprocess,
             self,
-            cache_path=self._cache_path,
-            java_path=self._java_path,
-            tmp_path=self._tmp_path,
-            verbose=self._verbose,
+            self._cache_path,
+            self._java_path,
+            self._tmp_path,
+            self._device,
+            self._verbose,
         )
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
 
@@ -103,56 +106,57 @@
         cache_path: str = "$HOME/.cache",
         java_path: str = "java",
         tmp_path: str = "/tmp",
         verbose: int = 0,
     ) -> None:
         super().__init__(
             preprocess,
+            "aac",
             cache_path,
             java_path,
             tmp_path,
-            "cpu",
+            "auto",
             verbose,
-            "aac",
         )
 
 
-def _get_metrics_classes_list(
-    metric_set_name: str,
-    return_all_scores: bool = True,
+def _instantiate_metrics_classes(
+    metrics: Union[str, Iterable[str], Iterable[AACMetric]] = "aac",
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
     tmp_path: str = "/tmp",
     device: Union[str, torch.device, None] = "auto",
     verbose: int = 0,
 ) -> list[AACMetric]:
-    metrics_factory = _get_metrics_classes_factory(
-        return_all_scores,
+    if isinstance(metrics, str) and metrics in METRICS_SETS:
+        metrics = METRICS_SETS[metrics]
+
+    if isinstance(metrics, str):
+        metrics = [metrics]
+    else:
+        metrics = list(metrics)  # type: ignore
+
+    metric_factory = _get_metric_factory_classes(
+        True,
         cache_path,
         java_path,
         tmp_path,
         device,
         verbose,
     )
 
-    if metric_set_name in METRICS_SETS:
-        metrics = [
-            factory()
-            for metric_name, factory in metrics_factory.items()
-            if metric_name in METRICS_SETS[metric_set_name]
-        ]
-    else:
-        raise ValueError(
-            f"Invalid argument {metric_set_name=}. (expected one of {tuple(METRICS_SETS.keys())})"
-        )
-
-    return metrics
+    metrics_inst: list[AACMetric] = []
+    for metric in metrics:
+        if isinstance(metric, str):
+            metric = metric_factory[metric]()
+        metrics_inst.append(metric)
+    return metrics_inst
 
 
-def _get_metrics_classes_factory(
+def _get_metric_factory_classes(
     return_all_scores: bool = True,
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
     tmp_path: str = "/tmp",
     device: Union[str, torch.device, None] = "auto",
     verbose: int = 0,
 ) -> dict[str, Callable[[], AACMetric]]:
@@ -178,31 +182,48 @@
             cache_path=cache_path,
             java_path=java_path,
             verbose=verbose,
         ),
         "rouge_l": lambda: ROUGEL(
             return_all_scores=return_all_scores,
         ),
-        # Note: cider_d and spice and computed inside spider metric
+        "cider_d": lambda: CIDErD(
+            return_all_scores=return_all_scores,
+        ),
+        "spice": lambda: SPICE(
+            return_all_scores=return_all_scores,
+            cache_path=cache_path,
+            java_path=java_path,
+            tmp_path=tmp_path,
+            verbose=verbose,
+        ),
         "spider": lambda: SPIDEr(
             return_all_scores=return_all_scores,
             cache_path=cache_path,
             java_path=java_path,
             tmp_path=tmp_path,
             verbose=verbose,
         ),
-        "fense": lambda: FENSE(
+        "sbert": lambda: SBERTSim(
             return_all_scores=return_all_scores,
             device=device,
             verbose=verbose,
         ),
-        "sbert": lambda: SBERT(
+        "fluerr": lambda: FluErr(
             return_all_scores=return_all_scores,
             device=device,
             verbose=verbose,
         ),
-        "fluency_error": lambda: FluencyError(
+        "fense": lambda: FENSE(
             return_all_scores=return_all_scores,
             device=device,
             verbose=verbose,
         ),
+        "spider_fl": lambda: SPIDErFL(
+            return_all_scores=return_all_scores,
+            cache_path=cache_path,
+            java_path=java_path,
+            tmp_path=tmp_path,
+            device=device,
+            verbose=verbose,
+        ),
     }
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/fense.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/fense.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 import torch
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
 from aac_metrics.functional.fense import fense, _load_models_and_tokenizer
-from aac_metrics.functional.fluency_error import ERROR_NAMES
+from aac_metrics.functional.fluerr import ERROR_NAMES
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 class FENSE(AACMetric):
     """Fluency ENhanced Sentence-bert Evaluation (FENSE)
 
     - Paper: https://arxiv.org/abs/2110.04684
     - Original implementation: https://github.com/blmoistawinde/fense
@@ -38,28 +38,30 @@
         return_all_scores: bool = True,
         sbert_model: str = "paraphrase-TinyBERT-L6-v2",
         echecker: str = "echecker_clotho_audiocaps_base",
         error_threshold: float = 0.9,
         device: Union[str, torch.device, None] = "auto",
         batch_size: int = 32,
         reset_state: bool = True,
+        return_probs: bool = True,
         penalty: float = 0.9,
         verbose: int = 0,
     ) -> None:
         sbert_model, echecker, echecker_tokenizer = _load_models_and_tokenizer(sbert_model, echecker, None, device, reset_state, verbose)  # type: ignore
 
         super().__init__()
         self._return_all_scores = return_all_scores
         self._sbert_model = sbert_model
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
@@ -70,23 +72,24 @@
             self._sbert_model,
             self._echecker,
             self._echecker_tokenizer,
             self._error_threshold,
             self._device,
             self._batch_size,
             self._reset_state,
+            self._return_probs,
             self._penalty,
             self._verbose,
         )
 
     def extra_repr(self) -> str:
         return f"error_threshold={self._error_threshold}, penalty={self._penalty}, device={self._device}, batch_size={self._batch_size}"
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("sbert.sim", "fluency_error", "fense") + tuple(
+        return ("sbert.sim", "fluerr", "fense") + tuple(
             f"fluerr.{name}_prob" for name in ERROR_NAMES
         )
 
     def reset(self) -> None:
         self._candidates = []
         self._mult_references = []
         return super().reset()
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/fluency_error.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/fluency_error.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/meteor.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/rouge_l.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/rouge_l.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/sbert.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/sbert.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/spice.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/spice.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
 from aac_metrics.functional.spice import spice
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 class SPICE(AACMetric):
     """Semantic Propositional Image Caption Evaluation class.
 
     - Paper: https://arxiv.org/pdf/1607.08822.pdf
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/spider.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
 from aac_metrics.functional.spider import spider
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 class SPIDEr(AACMetric):
     """SPIDEr class.
 
     - Paper: https://arxiv.org/pdf/1612.00370.pdf
 
@@ -28,15 +28,15 @@
 
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
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/spider_err.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/spider_err.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/classes/spider_max.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/spider_max.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from torch import Tensor
 
 from aac_metrics.classes.base import AACMetric
 from aac_metrics.functional.spider_max import spider_max
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 class SPIDErMax(AACMetric):
     """SPIDEr-max class.
 
     - Paper: https://hal.archives-ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/download.py` & `aac-metrics-0.4.0/src/aac_metrics/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from aac_metrics.classes.fense import FENSE
 from aac_metrics.functional.meteor import FNAME_METEOR_JAR
 from aac_metrics.functional.spice import FNAME_SPICE_JAR, DNAME_SPICE_CACHE
 from aac_metrics.utils.tokenization import FNAME_STANFORD_CORENLP_3_4_1_JAR
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 JAR_URLS = {
     "meteor": {
         "url": "https://github.com/tylin/coco-caption/raw/master/pycocoevalcap/meteor/meteor-1.5.jar",
         "fname": "meteor-1.5.jar",
     },
@@ -51,14 +51,19 @@
     spice: bool = True,
     fense: bool = True,
     verbose: int = 0,
 ) -> None:
     """Download the code needed for SPICE, METEOR and PTB Tokenizer.
 
     :param cache_path: The path to the external code directory. defaults to "$HOME/.cache".
+    :param tmp_path: The path to a temporary directory. defaults to "/tmp".
+    :param ptb_tokenizer: If True, downloads the PTBTokenizer code in cache directory. defaults to True.
+    :param meteor: If True, downloads the METEOR code in cache directory. defaults to True.
+    :param spice: If True, downloads the SPICE code in cache directory. defaults to True.
+    :param fense: If True, downloads the FENSE models. defaults to True.
     :param verbose: The verbose level. defaults to 0.
     """
     cache_path = osp.expandvars(cache_path)
     tmp_path = osp.expandvars(tmp_path)
 
     os.makedirs(cache_path, exist_ok=True)
     os.makedirs(tmp_path, exist_ok=True)
@@ -73,21 +78,21 @@
         name = "stanford_nlp"
         info = JAR_URLS[name]
         url = info["url"]
         fname = info["fname"]
         fpath = osp.join(stanford_nlp_dpath, fname)
         if not osp.isfile(fpath):
             if verbose >= 1:
-                logger.info(
+                pylog.info(
                     f"Downloading jar source for '{name}' in directory {stanford_nlp_dpath}."
                 )
             download_url_to_file(url, fpath, progress=verbose >= 1)
         else:
             if verbose >= 1:
-                logger.info(f"Stanford model file '{name}' is already downloaded.")
+                pylog.info(f"Stanford model file '{name}' is already downloaded.")
 
     if meteor:
         # Download JAR files for METEOR metric
         meteor_dpath = osp.join(cache_path, osp.dirname(FNAME_METEOR_JAR))
         os.makedirs(meteor_dpath, exist_ok=True)
 
         for name in ("meteor", "meteor_data"):
@@ -95,62 +100,62 @@
             url = info["url"]
             fname = info["fname"]
             subdir = osp.dirname(fname)
             fpath = osp.join(meteor_dpath, fname)
 
             if not osp.isfile(fpath):
                 if verbose >= 1:
-                    logger.info(
+                    pylog.info(
                         f"Downloading jar source for '{name}' in directory {meteor_dpath}."
                     )
                 if subdir not in ("", "."):
                     os.makedirs(osp.join(meteor_dpath, subdir), exist_ok=True)
 
                 download_url_to_file(
                     url,
                     fpath,
                     progress=verbose >= 1,
                 )
             else:
                 if verbose >= 1:
-                    logger.info(f"Meteor file '{name}' is already downloaded.")
+                    pylog.info(f"Meteor file '{name}' is already downloaded.")
 
     if spice:
         # Download JAR files for SPICE metric
         spice_jar_dpath = osp.join(cache_path, osp.dirname(FNAME_SPICE_JAR))
-        os.makedirs(spice_jar_dpath, exist_ok=True)
-
         spice_cache_path = osp.join(cache_path, DNAME_SPICE_CACHE)
+
+        os.makedirs(spice_jar_dpath, exist_ok=True)
         os.makedirs(spice_cache_path, exist_ok=True)
 
         script_path = osp.join(osp.dirname(__file__), "..", "..", "install_spice.sh")
         if not osp.isfile(script_path):
             raise FileNotFoundError(
                 f"Cannot find script '{osp.basename(script_path)}'."
             )
 
         if verbose >= 1:
-            logger.info(
+            pylog.info(
                 f"Downloading JAR sources for SPICE metric into '{spice_jar_dpath}'..."
             )
 
         command = ["bash", script_path, spice_jar_dpath]
         try:
             subprocess.check_call(
                 command,
                 stdout=None if verbose >= 2 else subprocess.DEVNULL,
                 stderr=None if verbose >= 2 else subprocess.DEVNULL,
             )
         except (CalledProcessError, PermissionError) as err:
-            logger.error(err)
+            pylog.error(err)
 
     if fense:
         # Download models files for FENSE metric
         if verbose >= 1:
-            logger.info("Downloading sBert and Bert error detector for FENSE metric...")
+            pylog.info("Downloading sBert and Bert error detector for FENSE metric...")
         _ = FENSE(device="cpu")
 
 
 def _get_main_download_args() -> Namespace:
     parser = ArgumentParser(
         description="Download models and external code to evaluate captions."
     )
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/evaluate.py` & `aac-metrics-0.4.0/src/aac_metrics/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import Iterable, Union
 
 import yaml
 
-from aac_metrics.functional.evaluate import aac_evaluate
+from aac_metrics.functional.evaluate import evaluate, METRICS_SETS
 from aac_metrics.utils.checks import check_metric_inputs, check_java_path
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 def load_csv_file(
     fpath: Union[str, Path],
     cands_columns: Union[str, Iterable[str]] = ("caption_predicted",),
     mrefs_columns: Union[str, Iterable[str]] = (
         "caption_1",
@@ -146,14 +146,21 @@
             "caption_4",
             "caption_5",
             "captions",
         ),
         help="The column names of the candidates in the CSV file. defaults to ('caption_1', 'caption_2', 'caption_3', 'caption_4', 'caption_5', 'captions').",
     )
     parser.add_argument(
+        "--metrics_set_name",
+        type=str,
+        default="default",
+        choices=tuple(METRICS_SETS.keys()),
+        help=f"The metrics set to compute. Can be one of {tuple(METRICS_SETS.keys())}. defaults to 'default'.",
+    )
+    parser.add_argument(
         "--cache_path",
         type=str,
         default="$HOME/.cache",
         help="Cache directory path. defaults to '$HOME/.cache'.",
     )
     parser.add_argument(
         "--java_path",
@@ -179,42 +186,43 @@
     handler.setFormatter(logging.Formatter(format_))
     pkg_logger = logging.getLogger("aac_metrics")
     pkg_logger.addHandler(handler)
 
     args = _get_main_evaluate_args()
 
     if not check_java_path(args.java_path):
-        raise RuntimeError(f"Invalid argument java_path={args.java_path}.")
+        raise RuntimeError(f"Invalid Java executable. ({args.java_path})")
 
     level = logging.INFO if args.verbose <= 1 else logging.DEBUG
     pkg_logger.setLevel(level)
 
     if args.verbose >= 1:
-        logger.info(f"Load file {args.input_file}...")
+        pylog.info(f"Load file {args.input_file}...")
 
     candidates, mult_references = load_csv_file(
         args.input_file, args.cand_columns, args.mrefs_columns
     )
     check_metric_inputs(candidates, mult_references)
 
     refs_lens = list(map(len, mult_references))
     if args.verbose >= 1:
-        logger.info(
+        pylog.info(
             f"Found {len(candidates)} candidates, {len(mult_references)} references and [{min(refs_lens)}, {max(refs_lens)}] references per candidate."
         )
 
-    corpus_scores, _sents_scores = aac_evaluate(
+    corpus_scores, _sents_scores = evaluate(
         candidates,
         mult_references,
         True,
+        args.metrics_set_name,
         args.cache_path,
         args.java_path,
         args.tmp_path,
         args.verbose,
     )
 
     corpus_scores = {k: v.item() for k, v in corpus_scores.items()}
-    logger.info(f"Global scores:\n{yaml.dump(corpus_scores, sort_keys=False)}")
+    pylog.info(f"Global scores:\n{yaml.dump(corpus_scores, sort_keys=False)}")
 
 
 if __name__ == "__main__":
     _main_evaluate()
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/__init__.py` & `aac-metrics-0.4.0/src/aac_metrics/classes/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .bleu import bleu
-from .cider_d import cider_d
-from .evaluate import aac_evaluate, evaluate
-from .fense import fense
-from .fluency_error import fluency_error
-from .meteor import meteor
-from .rouge_l import rouge_l
-from .sbert import sbert
-from .spice import spice
-from .spider import spider
-from .spider_max import spider_max
+from .bleu import BLEU
+from .cider_d import CIDErD
+from .evaluate import Evaluate, AACEvaluate
+from .fense import FENSE
+from .fluerr import FluErr
+from .meteor import METEOR
+from .rouge_l import ROUGEL
+from .sbert_sim import SBERTSim
+from .spice import SPICE
+from .spider import SPIDEr
+from .spider_fl import SPIDErFL
+from .spider_max import SPIDErMax
 
 
 __all__ = [
-    "bleu",
-    "cider_d",
-    "aac_evaluate",
-    "evaluate",
-    "fense",
-    "fluency_error",
-    "meteor",
-    "rouge_l",
-    "sbert",
-    "spice",
-    "spider",
-    "spider_max",
+    "BLEU",
+    "CIDErD",
+    "AACEvaluate",
+    "Evaluate",
+    "FENSE",
+    "FluErr",
+    "METEOR",
+    "ROUGEL",
+    "SBERTSim",
+    "SPICE",
+    "SPIDEr",
+    "SPIDErFL",
+    "SPIDErMax",
 ]
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/bleu.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/bleu.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     tokenizer: Callable[[str], list[str]] = str.split,
     return_1_to_n: bool = False,
 ) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
     """BiLingual Evaluation Understudy function.
 
     - Paper: https://www.aclweb.org/anthology/P02-1040.pdf
 
+    Note: this version of the BLEU metric applies a penalty formula that depends on the size of all candidates and the length of the references, which means that the average score of the candidates is not equal to the corpus score.
+
     :param candidates: The list of sentences to evaluate.
     :param mult_references: The list of list of sentences used as target.
     :param return_all_scores: If True, returns a tuple containing the globals and locals scores.
         Otherwise returns a scalar tensor containing the main global score.
         defaults to True.
     :param n: Maximal number of n-grams taken into account. defaults to 4.
     :param option: Corpus reference length mode. Can be "shortest", "average" or "closest". defaults to "closest".
@@ -93,44 +95,46 @@
     option: str = "closest",
     verbose: int = 0,
     return_1_to_n: bool = False,
 ) -> Union[Tensor, tuple[dict[str, Tensor], dict[str, Tensor]]]:
     if option not in BLEU_OPTIONS:
         raise ValueError(f"Invalid option {option=}. (expected one of {BLEU_OPTIONS})")
 
-    score_1_to_n, scores_1_to_n = __compute_bleu_score(
+    bleu_1_to_n_score, bleu_1_to_n_scores = __compute_bleu_score(
         cooked_cands,
         cooked_mrefs,
         n,
         option=option,
         verbose=verbose,
     )
 
     # Note: we use f64 because the original implem use numpy which uses f64 precision
     dtype = torch.float64
-    score_n = torch.as_tensor(score_1_to_n[-1], dtype=dtype)
-    scores_n = torch.as_tensor(scores_1_to_n[-1], dtype=dtype)
+    bleu_n_score = torch.as_tensor(bleu_1_to_n_score[-1], dtype=dtype)
+    bleu_n_scores = torch.as_tensor(bleu_1_to_n_scores[-1], dtype=dtype)
 
     if return_all_scores:
-        corpus_scores = {
-            f"bleu_{n}": score_n,
+        bleu_n_outs_corpus = {
+            f"bleu_{n}": bleu_n_score,
         }
-        sents_scores = {
-            f"bleu_{n}": scores_n,
+        bleu_n_outs_sents = {
+            f"bleu_{n}": bleu_n_scores,
         }
 
         if return_1_to_n:
-            score_1_to_n = torch.as_tensor(score_1_to_n, dtype=dtype)
-            scores_1_to_n = torch.as_tensor(scores_1_to_n, dtype=dtype)
-            corpus_scores[f"bleu_1_to_{n}"] = score_1_to_n
-            sents_scores[f"bleu_1_to_{n}"] = scores_1_to_n
+            bleu_1_to_n_score = torch.as_tensor(bleu_1_to_n_score, dtype=dtype)
+            bleu_1_to_n_scores = torch.as_tensor(bleu_1_to_n_scores, dtype=dtype)
+            bleu_n_outs_corpus[f"bleu_1_to_{n}"] = bleu_1_to_n_score
+            bleu_n_outs_sents[f"bleu_1_to_{n}"] = bleu_1_to_n_scores
+
+        bleu_n_outs = bleu_n_outs_corpus, bleu_n_outs_sents
 
-        return corpus_scores, sents_scores
+        return bleu_n_outs
     else:
-        return score_n
+        return bleu_n_score
 
 
 def __cook_sentence(
     s: str,
     n: int = 4,
     tokenizer: Callable[[str], list[str]] = str.split,
 ) -> tuple[int, Counter[tuple[str, ...]]]:
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/cider_d.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/cider_d.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,46 +86,47 @@
     scale: float,
 ) -> Union[Tensor, tuple[dict[str, Tensor], dict[str, Any]]]:
     if len(cooked_cands) <= 1:
         raise ValueError(
             f"CIDEr-D metric does not support less than 2 candidates with 2 references. (found {len(cooked_cands)} candidates, but expected > 1)"
         )
     # compute idf
-    document_frequency = __compute_doc_freq(cooked_mrefs)
+    doc_frequencies = __compute_doc_freq(cooked_mrefs)
     # sanity check: assert to check document frequency
-    assert len(cooked_cands) >= max(document_frequency.values()), "Sanity check failed."
+    assert len(cooked_cands) >= max(doc_frequencies.values()), "Sanity check failed."
 
     # compute log reference length
     log_n_refs = np.log(float(len(cooked_mrefs)))
     # compute cider score
     cider_d_scores, tfidf_lst = __compute_cider(
         cooked_cands,
         cooked_mrefs,
-        document_frequency,
+        doc_frequencies,
         log_n_refs,
         n,
         sigma,
         scale=scale,
     )
     cider_d_score = cider_d_scores.mean()
 
     cider_d_scores = torch.from_numpy(cider_d_scores)
     cider_d_score = torch.as_tensor(cider_d_score, dtype=torch.float64)
 
     if return_all_scores:
-        cider_d_global_outs = {
+        cider_d_outs_corpus = {
             "cider_d": cider_d_score,
         }
-        cider_d_local_outs = {
+        cider_d_outs_sents = {
             "cider_d": cider_d_scores,
         }
         if return_tfidf:
-            cider_d_local_outs["tfidf_lst"] = tfidf_lst  # type: ignore
+            cider_d_outs_sents["tfidf_lst"] = tfidf_lst  # type: ignore
+        cider_d_outs = cider_d_outs_corpus, cider_d_outs_sents
 
-        return cider_d_global_outs, cider_d_local_outs
+        return cider_d_outs
     else:
         return cider_d_score
 
 
 def __cook_sentence(
     sentence: str,
     n: int,
@@ -151,45 +152,45 @@
 def __compute_doc_freq(cooked_mrefs: list[list[Counter]]) -> Counter[tuple[str, ...]]:
     """
     Compute term frequency for reference data.
     This will be used to compute idf (inverse document frequency later)
     The term frequency is stored in the object
     :return: None
     """
-    document_frequency = Counter()
+    doc_frequencies = Counter()
     for refs in cooked_mrefs:
         all_refs_ngrams = set(ngram for ref in refs for ngram in ref.keys())
         for ngram in all_refs_ngrams:
-            document_frequency[ngram] += 1
+            doc_frequencies[ngram] += 1
 
-    return document_frequency
+    return doc_frequencies
 
 
 def __counter_to_vec(
     counters: dict[tuple, int],
     log_n_refs: float,
     n: int,
-    document_frequency: Union[Mapping[tuple, int], Callable[[tuple], int]],
+    doc_frequencies: Union[Mapping[tuple, int], Callable[[tuple], int]],
 ) -> tuple[list[defaultdict], np.ndarray, int]:
     """
     Function maps counts of ngram to vector of tfidf weights.
     The function returns vec, an array of dictionary that store mapping of n-gram and tf-idf weights.
     The n-th entry of array denotes length of n-grams.
     :param cnts:
     :return: tf-idf of n-grams (array of n dict[tuple, float]), norm (array of n floats) (norms for n-grams), length (int) (number of distinct n-grams from 1 to n)
     """
     vec = [defaultdict(float) for _ in range(n)]
     length = 0
     norm = np.zeros((n,))
 
     for (ngram, term_freq) in counters.items():
-        if isinstance(document_frequency, Mapping):
-            count = document_frequency[ngram]
+        if isinstance(doc_frequencies, Mapping):
+            count = doc_frequencies[ngram]
         else:
-            count = document_frequency(ngram)
+            count = doc_frequencies(ngram)
 
         # give ngram count 1 if it doesn't appear in reference corpus
         log_df = np.log(max(1.0, count))
 
         # ngram index
         cur_n = len(ngram) - 1
 
@@ -244,33 +245,33 @@
 
     return similarities
 
 
 def __compute_cider(
     cooked_cands: list[Counter],
     cooked_mrefs: list[list[Counter]],
-    document_frequency: Union[Counter[tuple], Callable[[tuple], int]],
+    doc_frequencies: Union[Counter[tuple], Callable[[tuple], int]],
     log_n_refs: float,
     n: int,
     sigma: float,
     scale: float,
 ) -> tuple[np.ndarray, list[tuple[list, list]]]:
 
     scores = np.empty((len(cooked_cands),))
     tfidf_lst = []
 
     for i, (cand, refs) in enumerate(zip(cooked_cands, cooked_mrefs)):
         # compute vector for test captions
-        vec, norm, length = __counter_to_vec(cand, log_n_refs, n, document_frequency)
+        vec, norm, length = __counter_to_vec(cand, log_n_refs, n, doc_frequencies)
         # compute vector for ref captions
         ngrams_scores = np.zeros((n,))
         vec_refs = []
         for ref in refs:
             vec_ref, norm_ref, length_ref = __counter_to_vec(
-                ref, log_n_refs, n, document_frequency
+                ref, log_n_refs, n, doc_frequencies
             )
             vec_refs.append(vec_ref)
             ngrams_scores += __similarity(
                 vec, vec_ref, norm, norm_ref, length, length_ref, n, sigma
             )
         # change by vrama91 - mean of ngram scores, instead of sum
         score_avg = np.mean(ngrams_scores)
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/evaluate.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,89 +8,99 @@
 from typing import Any, Callable, Iterable, Union
 
 import torch
 
 from torch import Tensor
 
 from aac_metrics.functional.bleu import bleu
+from aac_metrics.functional.cider_d import cider_d
 from aac_metrics.functional.fense import fense
-from aac_metrics.functional.fluency_error import fluency_error
+from aac_metrics.functional.fluerr import fluerr
 from aac_metrics.functional.meteor import meteor
 from aac_metrics.functional.rouge_l import rouge_l
-from aac_metrics.functional.sbert import sbert
+from aac_metrics.functional.sbert_sim import sbert_sim
+from aac_metrics.functional.spice import spice
 from aac_metrics.functional.spider import spider
+from aac_metrics.functional.spider_fl import spider_fl
 from aac_metrics.utils.tokenization import preprocess_mono_sents, preprocess_mult_sents
 
 
 pylog = logging.getLogger(__name__)
 
 
-METRICS_SETS = {
-    "aac": (
+METRICS_SETS: dict[str, tuple[str, ...]] = {
+    # Legacy metrics for AAC
+    "default": (
         "bleu_1",
         "bleu_2",
         "bleu_3",
         "bleu_4",
         "meteor",
         "rouge_l",
-        "cider_d",
-        "spice",
-        "spider",
+        "spider",  # includes cider_d, spice
     ),
+    # DCASE challenge task6a metrics for 2020, 2021 and 2022
+    "dcase2020": (
+        "bleu_1",
+        "bleu_2",
+        "bleu_3",
+        "bleu_4",
+        "meteor",
+        "rouge_l",
+        "spider",  # includes cider_d, spice
+    ),
+    # DCASE challenge task6a metrics for 2023
+    "dcase2023": (
+        "meteor",
+        "spider_fl",  # includes cider_d, spice, spider, fluerr
+    ),
+    # All metrics
     "all": (
         "bleu_1",
         "bleu_2",
         "bleu_3",
         "bleu_4",
         "meteor",
         "rouge_l",
-        "cider_d",
-        "spice",
-        "spider",
-        "fense",
+        "fense",  # includes sbert, fluerr
+        "spider_fl",  # includes cider_d, spice, spider, fluerr
     ),
 }
 
 
 def evaluate(
     candidates: list[str],
     mult_references: list[list[str]],
     preprocess: bool = True,
-    metrics: Union[str, Iterable[Callable[[list, list], tuple]]] = "all",
+    metrics: Union[
+        str, Iterable[str], Iterable[Callable[[list, list], tuple]]
+    ] = "default",
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
     tmp_path: str = "/tmp",
     device: Union[str, torch.device, None] = "auto",
     verbose: int = 0,
 ) -> tuple[dict[str, Tensor], dict[str, Tensor]]:
     """Evaluate candidates with multiple references with custom metrics.
 
     :param candidates: The list of sentences to evaluate.
     :param mult_references: The list of list of sentences used as target.
     :param preprocess: If True, the candidates and references will be passed as input to the PTB stanford tokenizer before computing metrics.defaults to True.
-    :param metrics: The name of the metric list or the explicit list of metrics to compute. defaults to "aac".
+    :param metrics: The name of the metric list or the explicit list of metrics to compute. defaults to "default".
     :param cache_path: The path to the external code directory. defaults to "$HOME/.cache".
     :param java_path: The path to the java executable. defaults to "java".
     :param tmp_path: Temporary directory path. defaults to "/tmp".
-    :param device: The PyTorch device used to run FENSE models. If None, it will try to detect use cuda if available. defaults to "cpu".
+    :param device: The PyTorch device used to run FENSE and SPIDErFL models.
+        If None, it will try to detect use cuda if available. defaults to "auto".
     :param verbose: The verbose level. defaults to 0.
     :returns: A tuple of globals and locals scores.
     """
-    if isinstance(metrics, str):
-        metrics = _get_metrics_functions_list(
-            metrics,
-            return_all_scores=True,
-            cache_path=cache_path,
-            java_path=java_path,
-            tmp_path=tmp_path,
-            device=device,
-            verbose=verbose,
-        )
-    else:
-        metrics = list(metrics)
+    metrics = _instantiate_metrics_functions(
+        metrics, cache_path, java_path, tmp_path, device, verbose
+    )
 
     if preprocess:
         candidates = preprocess_mono_sents(
             candidates,
             cache_path,
             java_path,
             tmp_path,
@@ -100,108 +110,129 @@
             mult_references,
             cache_path,
             java_path,
             tmp_path,
             verbose=verbose,
         )
 
-    corpus_scores = {}
-    sents_scores = {}
+    outs_corpus = {}
+    outs_sents = {}
 
     for i, metric in enumerate(metrics):
         if hasattr(metric, "__qualname__"):
             name = metric.__qualname__
         else:
             name = metric.__class__.__qualname__
 
         if verbose >= 1:
             pylog.info(f"[{i+1:2d}/{len(metrics):2d}] Computing {name} metric...")
-        start = time.perf_counter()
-
-        corpus_scores_i, sents_scores_i = metric(candidates, mult_references)
 
+        start = time.perf_counter()
+        outs_corpus_i, outs_sents_i = metric(candidates, mult_references)
         end = time.perf_counter()
+
         if verbose >= 1:
             pylog.info(
                 f"[{i+1:2d}/{len(metrics):2d}] Metric {name} computed in {end - start:.2f}s."
             )
 
-        corpus_scores |= corpus_scores_i
-        sents_scores |= sents_scores_i
+        if __debug__:
+            corpus_overlap = tuple(
+                set(outs_corpus_i.keys()).intersection(outs_corpus.keys())
+            )
+            sents_overlap = tuple(
+                set(outs_sents_i.keys()).intersection(outs_sents.keys())
+            )
+            if len(corpus_overlap) > 0 or len(sents_overlap) > 0:
+                pylog.warning(
+                    f"Found overlapping metric outputs names. (found {corpus_overlap=} and {sents_overlap=})"
+                )
 
-    return corpus_scores, sents_scores
+        outs_corpus |= outs_corpus_i
+        outs_sents |= outs_sents_i
 
+    return outs_corpus, outs_sents
 
-def aac_evaluate(
+
+def dcase2023_evaluate(
     candidates: list[str],
     mult_references: list[list[str]],
     preprocess: bool = True,
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
     tmp_path: str = "/tmp",
+    device: Union[str, torch.device, None] = "auto",
     verbose: int = 0,
 ) -> tuple[dict[str, Tensor], dict[str, Tensor]]:
     """Evaluate candidates with multiple references with all Audio Captioning metrics.
 
     :param candidates: The list of sentences to evaluate.
     :param mult_references: The list of list of sentences used as target.
     :param preprocess: If True, the candidates and references will be passed as input to the PTB stanford tokenizer before computing metrics.
         defaults to True.
     :param cache_path: The path to the external code directory. defaults to "$HOME/.cache".
     :param java_path: The path to the java executable. defaults to "java".
     :param tmp_path: Temporary directory path. defaults to "/tmp".
+    :param device: The PyTorch device used to run FENSE and SPIDErFL models.
+        If None, it will try to detect use cuda if available. defaults to "auto".
     :param verbose: The verbose level. defaults to 0.
     :returns: A tuple of globals and locals scores.
     """
     return evaluate(
         candidates,
         mult_references,
         preprocess,
-        "aac",
+        "dcase2023",
         cache_path,
         java_path,
         tmp_path,
-        "cpu",
+        device,
         verbose,
     )
 
 
-def _get_metrics_functions_list(
-    metric_set_name: str,
-    return_all_scores: bool = True,
+def _instantiate_metrics_functions(
+    metrics: Union[str, Iterable[str], Iterable[Callable[[list, list], tuple]]] = "all",
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
     tmp_path: str = "/tmp",
     device: Union[str, torch.device, None] = "auto",
     verbose: int = 0,
 ) -> list[Callable]:
-    metrics_factory = _get_metrics_functions_factory(
-        return_all_scores,
+    if isinstance(metrics, str) and metrics in METRICS_SETS:
+        metrics = METRICS_SETS[metrics]
+
+    if isinstance(metrics, str):
+        metrics = [metrics]
+    else:
+        metrics = list(metrics)  # type: ignore
+
+    if not all(isinstance(metric, (str, Callable)) for metric in metrics):
+        raise TypeError(
+            "Invalid argument type for metrics. (expected str, Iterable[str] or Iterable[Metric])"
+        )
+
+    metric_factory = _get_metric_factory_functions(
+        True,
         cache_path,
         java_path,
         tmp_path,
         device,
         verbose,
     )
 
-    if metric_set_name in METRICS_SETS:
-        metrics = [
-            factory
-            for metric_name, factory in metrics_factory.items()
-            if metric_name in METRICS_SETS[metric_set_name]
-        ]
-    else:
-        raise ValueError(
-            f"Invalid argument {metric_set_name=}. (expected one of {tuple(METRICS_SETS.keys())})"
-        )
-
-    return metrics
+    metrics_inst: list[Callable] = []
+    for metric in metrics:
+        if isinstance(metric, str):
+            metric = metric_factory[metric]
+        metrics_inst.append(metric)
+    return metrics_inst
 
 
-def _get_metrics_functions_factory(
+def _get_metric_factory_functions(
     return_all_scores: bool = True,
     cache_path: str = "$HOME/.cache",
     java_path: str = "java",
     tmp_path: str = "/tmp",
     device: Union[str, torch.device, None] = "auto",
     verbose: int = 0,
 ) -> dict[str, Callable[[list[str], list[list[str]]], Any]]:
@@ -233,35 +264,55 @@
             java_path=java_path,
             verbose=verbose,
         ),
         "rouge_l": partial(
             rouge_l,
             return_all_scores=return_all_scores,
         ),
-        # Note: cider_d and spice and computed inside spider metric
+        "cider_d": partial(
+            cider_d,
+            return_all_scores=return_all_scores,
+        ),
+        "spice": partial(
+            spice,
+            return_all_scores=return_all_scores,
+            cache_path=cache_path,
+            java_path=java_path,
+            tmp_path=tmp_path,
+            verbose=verbose,
+        ),
         "spider": partial(
             spider,
             return_all_scores=return_all_scores,
             cache_path=cache_path,
             java_path=java_path,
             tmp_path=tmp_path,
             verbose=verbose,
         ),
-        "fense": partial(
-            fense,
+        "sbert": partial(
+            sbert_sim,
             return_all_scores=return_all_scores,
             device=device,
             verbose=verbose,
         ),
-        "sbert": partial(
-            sbert,
+        "fluerr": partial(
+            fluerr,
+            return_all_scores=return_all_scores,
+            device=device,
+            verbose=verbose,
+        ),
+        "fense": partial(
+            fense,
             return_all_scores=return_all_scores,
             device=device,
             verbose=verbose,
         ),
-        "fluency_error": partial(
-            fluency_error,
+        "spider_fl": partial(
+            spider_fl,
             return_all_scores=return_all_scores,
+            cache_path=cache_path,
+            java_path=java_path,
+            tmp_path=tmp_path,
             device=device,
             verbose=verbose,
         ),
     }
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/fluency_error.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/fluency_error.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/meteor.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/meteor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch
 
 from torch import Tensor
 
 from aac_metrics.utils.checks import check_java_path
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 FNAME_METEOR_JAR = osp.join("aac-metrics", "meteor", "meteor-1.5.jar")
 SUPPORTED_LANGUAGES = ("en", "cz", "de", "es", "fr")
 
 
 def meteor(
@@ -59,16 +59,16 @@
 
     if __debug__:
         if not osp.isfile(meteor_jar_fpath):
             raise FileNotFoundError(
                 f"Cannot find JAR file '{meteor_jar_fpath}' for METEOR metric. Maybe run 'aac-metrics-download' or specify another 'cache_path' directory."
             )
         if not check_java_path(java_path):
-            raise ValueError(
-                f"Cannot find java executable with {java_path=} for compute METEOR metric score."
+            raise RuntimeError(
+                f"Invalid Java executable to compute METEOR score. ({java_path})"
             )
 
     if len(candidates) != len(mult_references):
         raise ValueError(
             f"Invalid number of candidates and references. (found {len(candidates)=} != {len(mult_references)=})"
         )
 
@@ -87,15 +87,15 @@
         "-stdio",
         "-l",
         language,
         "-norm",
     ]
 
     if verbose >= 2:
-        logger.debug(f"Start METEOR process with command '{' '.join(meteor_cmd)}'...")
+        pylog.debug(f"Start METEOR process with command '{' '.join(meteor_cmd)}'...")
 
     meteor_process = Popen(
         meteor_cmd,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
@@ -116,15 +116,15 @@
         assert meteor_process.stdout is not None, "INTERNAL METEOR process error"
         stat = meteor_process.stdout.readline().decode().strip()
         eval_line += " ||| {}".format(stat)
 
     # Eval encoded candidates and references
     assert meteor_process.stdin is not None, "INTERNAL METEOR process error"
     if verbose >= 3:
-        logger.debug(f"Write line {eval_line=}.")
+        pylog.debug(f"Write line {eval_line=}.")
     meteor_process.stdin.write("{}\n".format(eval_line).encode())
     meteor_process.stdin.flush()
 
     # Read scores
     assert meteor_process.stdout is not None, "INTERNAL METEOR process error"
     meteor_scores = []
     for _ in range(n_candidates):
@@ -137,21 +137,22 @@
     meteor_process.wait()
 
     dtype = torch.float64
     meteor_score = torch.as_tensor(meteor_score, dtype=dtype)
     meteor_scores = torch.as_tensor(meteor_scores, dtype=dtype)
 
     if return_all_scores:
-        corpus_scores = {
+        meteor_outs_corpus = {
             "meteor": meteor_score,
         }
-        sents_scores = {
+        meteor_outs_sents = {
             "meteor": meteor_scores,
         }
-        return corpus_scores, sents_scores
+        meteor_outs = meteor_outs_corpus, meteor_outs_sents
+        return meteor_outs
     else:
         return meteor_score
 
 
 def encore_cand_and_refs(candidate: str, references: list[str]) -> bytes:
     # SCORE ||| reference 1 words ||| ... ||| reference N words ||| candidate words
     candidate = candidate.replace("|||", "").replace("  ", " ")
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/mult_cands.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/mult_cands.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,39 +71,39 @@
         k: torch.stack([sents_scores_i[k] for sents_scores_i in all_sents_scores_lst])
         for k in keys
     }
     # all_sents_scores dict of tensor of shapes (n_cands_per_audio, n_items)
 
     if selection == "max":
         indexes = all_sents_scores[metric_out_name].argmax(dim=0).unsqueeze(dim=0)
-        sents_scores = {
+        outs_sents = {
             k: scores.gather(0, indexes).squeeze(dim=0)
             for k, scores in all_sents_scores.items()
         }
 
     elif selection == "min":
         indexes = all_sents_scores[metric_out_name].argmin(dim=0).unsqueeze(dim=0)
-        sents_scores = {
+        outs_sents = {
             k: scores.gather(0, indexes).squeeze(dim=0)
             for k, scores in all_sents_scores.items()
         }
 
     elif selection == "mean":
         selected_scores = all_sents_scores[metric_out_name].mean(dim=0)
-        sents_scores = {metric_out_name: selected_scores}
+        outs_sents = {metric_out_name: selected_scores}
 
     else:
         raise ValueError(
             f"Invalid argument {selection=}. (expected one of {SELECTIONS})"
         )
 
     if return_all_cands_scores:
-        sents_scores |= {
+        outs_sents |= {
             f"{k}_all": scores.transpose(0, 1) for k, scores in all_sents_scores.items()
         }
 
-    corpus_scores = {k: reduction(scores) for k, scores in sents_scores.items()}
+    outs_corpus = {k: reduction(scores) for k, scores in outs_sents.items()}
 
     if return_all_scores:
-        return corpus_scores, sents_scores
+        return outs_corpus, outs_sents
     else:
-        return corpus_scores[metric_out_name]
+        return outs_corpus[metric_out_name]
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/rouge_l.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/rouge_l.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import numpy as np
 import torch
 
 from torch import Tensor
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 def rouge_l(
     candidates: list[str],
     mult_references: list[list[str]],
     return_all_scores: bool = True,
     beta: float = 1.2,
@@ -64,32 +64,32 @@
         for cand, refs in zip(candidates, mult_references)
     ]
     prev_rouge_l_scores += new_rouge_l_scores
     return prev_rouge_l_scores
 
 
 def _rouge_l_compute(
-    rouge_l_scores: list[float],
+    rouge_l_scs: list[float],
     return_all_scores: bool,
 ) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
     # Note: use numpy to compute mean because np.mean and torch.mean can give very small differences
-    rouge_l_scores_np = np.array(rouge_l_scores)
+    rouge_l_scores_np = np.array(rouge_l_scs)
     rouge_l_score_np = rouge_l_scores_np.mean()
 
     rouge_l_score_pt = torch.as_tensor(rouge_l_score_np)
     rouge_l_scores_pt = torch.from_numpy(rouge_l_scores_np)
 
     if return_all_scores:
-        corpus_scores = {
+        rouge_l_outs_corpus = {
             "rouge_l": rouge_l_score_pt,
         }
-        sents_scores = {
+        rouge_l_outs_sents = {
             "rouge_l": rouge_l_scores_pt,
         }
-        return corpus_scores, sents_scores
+        return rouge_l_outs_corpus, rouge_l_outs_sents
     else:
         return rouge_l_score_pt
 
 
 def __calc_score(
     candidate: str,
     references: list[str],
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/sbert.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/sbert.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/spice.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/spice.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import torch
 
 from torch import Tensor
 
 from aac_metrics.utils.checks import check_java_path
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 DNAME_SPICE_CACHE = osp.join("aac-metrics", "spice", "cache")
 FNAME_SPICE_JAR = osp.join("aac-metrics", "spice", "spice-1.0.jar")
 
 
 def spice(
@@ -78,32 +78,32 @@
 
     if __debug__:
         if not osp.isfile(spice_fpath):
             raise FileNotFoundError(
                 f"Cannot find JAR file '{spice_fpath}' for SPICE metric. Maybe run 'aac-metrics-download' or specify another 'cache_path' directory."
             )
         if not check_java_path(java_path):
-            raise ValueError(
-                f"Cannot find java executable with {java_path=} for compute SPICE metric score."
+            raise RuntimeError(
+                f"Invalid Java executable to compute SPICE score. ({java_path})"
             )
 
     if len(candidates) != len(mult_references):
         raise ValueError(
             f"Invalid number of candidates and references. (found {len(candidates)=} != {len(mult_references)=})"
         )
 
     if separate_cache_dir:
         spice_cache = tempfile.mkdtemp(dir=tmp_path)
     else:
         spice_cache = osp.join(cache_path, DNAME_SPICE_CACHE)
     del cache_path
 
     if verbose >= 2:
-        logger.debug(f"Use cache directory {spice_cache}.")
-        logger.debug(f"Computing SPICE with JAR file {spice_fpath}...")
+        pylog.debug(f"Use cache directory {spice_cache}.")
+        pylog.debug(f"Computing SPICE with JAR file {spice_fpath}...")
 
     input_data = [
         {
             "image_id": i,
             "test": cand,
             "refs": refs,
         }
@@ -159,15 +159,15 @@
             out_file.name,
             "-subset",
         ]
         if n_threads is not None:
             spice_cmd += ["-threads", str(n_threads)]
 
         if verbose >= 2:
-            logger.debug(f"Run SPICE java code with: {' '.join(spice_cmd)}")
+            pylog.debug(f"Run SPICE java code with: {' '.join(spice_cmd)}")
 
         try:
             subprocess.check_call(
                 spice_cmd,
                 stdout=stdout,
                 stderr=stderr,
                 timeout=timeout_i,
@@ -175,15 +175,15 @@
             if stdout is not None:
                 stdout.close()
             if stderr is not None:
                 stderr.close()
             break
 
         except subprocess.TimeoutExpired as err:
-            logger.warning(
+            pylog.warning(
                 f"Timeout SPICE java program with {timeout_i=}s (nb timeouts done={i+1}/{len(timeout_lst)})."
             )
 
             if i < len(timeout_lst) - 1:
                 # Clear out files
                 open(out_file.name, "w").close()
                 if stdout is not None:
@@ -191,35 +191,50 @@
                 if stderr is not None:
                     stderr.close()
                 time.sleep(1.0)
             else:
                 raise err
 
         except (CalledProcessError, PermissionError) as err:
-            logger.error("Invalid SPICE call.")
-            logger.error(f"Full command: '{' '.join(spice_cmd)}'")
-            if stdout is not None and stderr is not None:
-                logger.error(
-                    f"For more information, see temp files '{stdout.name}' and '{stderr.name}'."
+            pylog.error("Invalid SPICE call.")
+            pylog.error(f"Full command: '{' '.join(spice_cmd)}'")
+            if (
+                stdout is not None
+                and stderr is not None
+                and osp.isfile(stdout.name)
+                and osp.isfile(stderr.name)
+            ):
+                stdout_crashlog = stdout.name.replace(
+                    "spice_stdout", "CRASH_spice_stdout"
+                )
+                stderr_crashlog = stderr.name.replace(
+                    "spice_stderr", "CRASH_spice_stderr"
+                )
+                shutil.copy(stdout.name, stdout_crashlog)
+                shutil.copy(stderr.name, stderr_crashlog)
+                pylog.error(
+                    f"For more information, see temp files '{stdout_crashlog}' and '{stderr_crashlog}'."
                 )
             else:
-                logger.info(
+                pylog.info(
                     f"Note: No temp file recorded. (found {stdout=} and {stderr=})"
                 )
             raise err
 
     if verbose >= 2:
-        logger.debug("SPICE java code finished.")
+        pylog.debug("SPICE java code finished.")
 
     # Read and process results
     with open(out_file.name, "r") as data_file:
         results = json.load(data_file)
     os.remove(in_file.name)
     os.remove(out_file.name)
-    shutil.rmtree(spice_cache)
+
+    if separate_cache_dir:
+        shutil.rmtree(spice_cache)
 
     imgId_to_scores = {}
     spice_scores = []
     for item in results:
         imgId_to_scores[item["image_id"]] = item["scores"]
         spice_scores.append(__float_convert(item["scores"]["All"]["f"]))
 
@@ -228,21 +243,21 @@
     spice_score = spice_scores.mean()
 
     dtype = torch.float64
     spice_scores = torch.from_numpy(spice_scores)
     spice_score = torch.as_tensor(spice_score, dtype=dtype)
 
     if return_all_scores:
-        corpus_scores = {
+        spice_outs_corpus = {
             "spice": spice_score,
         }
-        sents_scores = {
+        spice_outs_sents = {
             "spice": spice_scores,
         }
-        return corpus_scores, sents_scores
+        return spice_outs_corpus, spice_outs_sents
     else:
         return spice_score
 
 
 def __float_convert(obj: Any) -> float:
     try:
         return float(obj)
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/spider.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/spider.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from aac_metrics.functional.spice import spice
 
 
 def spider(
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
@@ -53,58 +53,60 @@
     """
 
     if len(candidates) != len(mult_references):
         raise ValueError(
             f"Number of candidates and mult_references are different (found {len(candidates)} != {len(mult_references)})."
         )
 
-    cider_d_out = cider_d(
+    cider_d_outs: tuple = cider_d(  # type: ignore
         candidates,
         mult_references,
-        return_all_scores,
+        True,
         n=n,
         sigma=sigma,
         tokenizer=tokenizer,
         return_tfidf=return_tfidf,
     )
-    spice_out = spice(
+    spice_outs: tuple = spice(  # type: ignore
         candidates,
         mult_references,
-        return_all_scores,
+        True,
         cache_path=cache_path,
         java_path=java_path,
         tmp_path=tmp_path,
         n_threads=n_threads,
         java_max_memory=java_max_memory,
         timeout=timeout,
         verbose=verbose,
     )
+    spider_outs = _spider_from_outputs(cider_d_outs, spice_outs)
 
     if return_all_scores:
-        assert isinstance(
-            cider_d_out, tuple
-        ), f"INTERNAL error type. ({type(cider_d_out)})"
-        assert isinstance(spice_out, tuple), f"INTERNAL error type. ({type(spice_out)})"
-        cider_d_global_scores, cider_d_sents_scores = cider_d_out
-        spice_global_scores, spice_sents_scores = spice_out
-
-        spider_global_scores = {
-            "cider_d": cider_d_global_scores["cider_d"],
-            "spice": spice_global_scores["spice"],
-            "spider": (cider_d_global_scores["cider_d"] + spice_global_scores["spice"])
-            / 2.0,
-        }
-        spider_sents_scores = {
-            "cider_d": cider_d_sents_scores["cider_d"],
-            "spice": spice_sents_scores["spice"],
-            "spider": (cider_d_sents_scores["cider_d"] + spice_sents_scores["spice"])
-            / 2.0,
-        }
-        return spider_global_scores, spider_sents_scores
+        return spider_outs
     else:
-        assert isinstance(
-            cider_d_out, Tensor
-        ), f"INTERNAL error type. ({type(cider_d_out)})"
-        assert isinstance(
-            spice_out, Tensor
-        ), f"INTERNAL error type. ({type(spice_out)})"
-        return (cider_d_out + spice_out) / 2.0
+        return spider_outs[0]["spider"]
+
+
+def _spider_from_outputs(
+    cider_d_outs: tuple[dict[str, Tensor], dict[str, Tensor]],
+    spice_outs: tuple[dict[str, Tensor], dict[str, Tensor]],
+) -> tuple[dict[str, Tensor], dict[str, Tensor]]:
+    """Combines CIDErD and SPICE outputs."""
+    cider_d_outs_corpus, cider_d_outs_sents = cider_d_outs
+    spice_outs_corpus, spice_outs_sents = spice_outs
+
+    spider_score = (cider_d_outs_corpus["cider_d"] + spice_outs_corpus["spice"]) / 2.0
+    spider_scores = (cider_d_outs_sents["cider_d"] + spice_outs_sents["spice"]) / 2.0
+
+    spider_outs_corpus = (
+        cider_d_outs_corpus | spice_outs_corpus | {"spider": spider_score}
+    )
+    spider_outs_sents = (
+        cider_d_outs_sents
+        | spice_outs_sents
+        | {
+            "spider": spider_scores,
+        }
+    )
+    spider_outs = spider_outs_corpus, spider_outs_sents
+
+    return spider_outs
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/spider_err.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/spider_err.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/functional/spider_max.py` & `aac-metrics-0.4.0/src/aac_metrics/functional/spider_max.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/info.py` & `aac-metrics-0.4.0/src/aac_metrics/info.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/utils/collections.py` & `aac-metrics-0.4.0/src/aac_metrics/utils/collections.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/src/aac_metrics/utils/tokenization.py` & `aac-metrics-0.4.0/src/aac_metrics/utils/tokenization.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from typing import Any, Hashable, Iterable, Optional
 
 from aac_metrics.utils.checks import check_java_path
 from aac_metrics.utils.collections import flat_list, unflat_list
 
 
-logger = logging.getLogger(__name__)
+pylog = logging.getLogger(__name__)
 
 
 # Path to the stanford corenlp jar
 FNAME_STANFORD_CORENLP_3_4_1_JAR = osp.join(
     "aac-metrics", "stanford_nlp", "stanford-corenlp-3.4.1.jar"
 )
 # Punctuations to be removed from the sentences
@@ -80,21 +80,21 @@
         if not osp.isdir(tmp_path):
             raise RuntimeError(f"Cannot find tmp directory at {tmp_path=}.")
         if not osp.isfile(stanford_fpath):
             raise FileNotFoundError(
                 f"Cannot find JAR file '{stanford_fpath}' for tokenization. Maybe run 'aac-metrics-download' or specify another 'cache_path' directory."
             )
         if not check_java_path(java_path):
-            raise ValueError(
-                f"Cannot find java executable with {java_path=} to tokenize sentences."
+            raise RuntimeError(
+                f"Invalid Java executable to tokenize sentences. ({java_path})"
             )
 
     start_time = time.perf_counter()
     if verbose >= 2:
-        logger.debug(
+        pylog.debug(
             f"Start executing {FNAME_STANFORD_CORENLP_3_4_1_JAR} JAR file for tokenization. ({len(sentences)=})"
         )
 
     cmd = [
         java_path,
         "-cp",
         stanford_fpath,
@@ -161,15 +161,15 @@
             w for w in line.rstrip().split(" ") if w not in punctuations
         ]
         outs[k] = tokenized_caption
     assert all(out is not None for out in outs)
 
     if verbose >= 2:
         duration = time.perf_counter() - start_time
-        logger.debug(f"Tokenization finished in {duration:.2f}s.")
+        pylog.debug(f"Tokenization finished in {duration:.2f}s.")
 
     return outs
 
 
 def preprocess_mono_sents(
     sentences: list[str],
     cache_path: str = "$HOME/.cache",
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics.egg-info/PKG-INFO` & `aac-metrics-0.4.0/src/aac_metrics.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: aac-metrics
-Version: 0.3.0
+Version: 0.4.0
 Summary: Metrics for evaluating Automated Audio Captioning systems, designed for PyTorch.
-Home-page: https://github.com/Labbeti/aac-metrics
-Author: Etienne Labbé (Labbeti)
-Author-email: labbeti.pub@gmail.com
-License: MIT
-Project-URL: Documentation, https://aac-metrics.readthedocs.io/
-Project-URL: Source, https://github.com/Labbeti/aac-metrics
-Project-URL: PyPI, https://pypi.org/project/aac-metrics/
+Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
+Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
+Project-URL: homepage, https://pypi.org/project/aac-metrics/
+Project-URL: documentation, https://aac-metrics.readthedocs.io/
+Project-URL: repository, https://github.com//Labbeti/aac-metrics.git
+Project-URL: changelog, https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md
+Keywords: audio,metrics,text,captioning,audio-captioning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
@@ -44,52 +47,60 @@
     - BLEU [[1]](#bleu)
     - ROUGE-L [[2]](#rouge-l)
     - METEOR [[3]](#meteor)
     - CIDEr-D [[4]](#cider)
     - SPICE [[5]](#spice)
     - SPIDEr [[6]](#spider)
     - SPIDEr-max [[7]](#spider-max)
-    - SBERT [[8]](#fense)
-    - FluencyError [[8]](#fense)
+    - SBERT-sim [[8]](#fense)
+    - Fluency Error [[8]](#fense)
     - FENSE [[8]](#fense)
-    - SPIDErErr
+    - SPIDEr-FL [[9]](#spider-fl)
 
 ## Installation
 Install the pip package:
 ```bash
 pip install aac-metrics
 ```
 
-Download the external code and models needed for METEOR, SPICE, PTBTokenizer and FENSE:
+Download the external code and models needed for METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and SPIDEr-FL:
 ```bash
 aac-metrics-download
 ```
 
 Notes:
 - The external code for SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`.
 - The weights of the FENSE fluency error detector and the the SBERT model are respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and `$HOME/.cache/torch/sentence_transformers`.
 
 ## Usage
-### Evaluate default AAC metrics
-The full evaluation process to compute AAC metrics can be done with `aac_metrics.aac_evaluate` function.
+### Evaluate default metrics
+The full evaluation pipeline to compute AAC metrics can be done with `aac_metrics.evaluate` function.
 
 ```python
-from aac_metrics import aac_evaluate
+from aac_metrics import evaluate
 
 candidates: list[str] = ["a man is speaking"]
 mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
 
-corpus_scores, _ = aac_evaluate(candidates, mult_references)
+corpus_scores, _ = evaluate(candidates, mult_references)
 print(corpus_scores)
-# dict containing the score of each aac metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d", "spice", "spider"
+# dict containing the score of each metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d", "spice", "spider"
 # {"bleu_1": tensor(0.7), "bleu_2": ..., ...}
 ```
+### Evaluate DCASE2023 metrics
+To compute metrics for the DCASE2023 challenge, just set the argument `metrics="dcase2023"` in `evaluate` function call.
+
+```python
+corpus_scores, _ = evaluate(candidates, mult_references, metrics="dcase2023")
+print(corpus_scores)
+# dict containing the score of each metric: "meteor", "cider_d", "spice", "spider", "spider_fl", "fluerr"
+```
 
 ### Evaluate a specific metric
-Evaluate a specific metric can be done using the `aac_metrics.functional.<metric_name>.<metric_name>` function or the `aac_metrics.classes.<metric_name>.<metric_name>` class. Unlike `aac_evaluate`, the tokenization with PTBTokenizer is not done with these functions, but you can do it manually with `preprocess_mono_sents` and `preprocess_mult_sents` functions.
+Evaluate a specific metric can be done using the `aac_metrics.functional.<metric_name>.<metric_name>` function or the `aac_metrics.classes.<metric_name>.<metric_name>` class. Unlike `evaluate`, the tokenization with PTBTokenizer is not done with these functions, but you can do it manually with `preprocess_mono_sents` and `preprocess_mult_sents` functions.
 
 ```python
 from aac_metrics.functional import cider_d
 from aac_metrics.utils.tokenization import preprocess_mono_sents, preprocess_mult_sents
 
 candidates: list[str] = ["a man is speaking"]
 mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
@@ -103,132 +114,65 @@
 print(sents_scores)
 # {"cider_d": tensor([0.9, ...])}
 ```
 
 Each metrics also exists as a python class version, like `aac_metrics.classes.cider_d.CIDErD`.
 
 ## Metrics
-### Default AAC metrics
+### Legacy metrics
 | Metric | Python Class | Origin | Range | Short description |
 |:---|:---|:---|:---|:---|
 | BLEU [[1]](#bleu) | `BLEU` | machine translation | [0, 1] | Precision of n-grams |
 | ROUGE-L [[2]](#rouge-l) | `ROUGEL` | machine translation | [0, 1] | FScore of the longest common subsequence |
 | METEOR [[3]](#meteor) | `METEOR` | machine translation | [0, 1] | Cosine-similarity of frequencies with synonyms matching |
 | CIDEr-D [[4]](#cider) | `CIDErD` | image captioning | [0, 10] | Cosine-similarity of TF-IDF computed on n-grams |
 | SPICE [[5]](#spice) | `SPICE` | image captioning | [0, 1] | FScore of semantic graph |
 | SPIDEr [[6]](#spider) | `SPIDEr` | image captioning | [0, 5.5] | Mean of CIDEr-D and SPICE |
 
-### Other metrics
+### AAC-specific metrics
 | Metric name | Python Class | Origin | Range | Short description |
 |:---|:---|:---|:---|:---|
 | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning | [0, 5.5] | Max of SPIDEr scores for multiples candidates |
-| SBERT [[7]](#spider-max) | `SBERT` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-BERT embeddings** |
-| FluencyError [[7]](#spider-max) | `FluencyError` | audio captioning | [0, 1] | Use pretrained model to detect fluency errors in sentences |
-| FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] | Combines `SBERT` and `FluencyError` |
-| SPIDErErr | `SPIDErErr` | audio captioning | [0, 5.5] | Combines `SPIDEr` and `FluencyError` |
-
-## SPIDEr-max metric
-SPIDEr-max [[7]](#spider-max)  is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model.
-
-### SPIDEr-max: why ?
-The SPIDEr metric used in audio captioning is highly sensitive to the frequencies of the words used.
-
-Here is 2 examples with the 5 candidates generated by the beam search algorithm, their corresponding SPIDEr scores and the associated references:
-
-<div align="center">
-
-| Beam search candidates | SPIDEr |
-|:---|:---:|
-| heavy rain is falling on a roof | 0.562 |
-| heavy rain is falling on **a tin roof** | **0.930** |
-| a heavy rain is falling on a roof | 0.594 |
-| a heavy rain is falling on the ground | 0.335 |
-| a heavy rain is falling on the roof | 0.594 |
-
-| References |
-|:---|
-| heavy rain falls loudly onto a structure with a thin roof |
-| heavy rainfall falling onto a thin structure with a thin roof |
-| it is raining hard and the rain hits **a tin roof** |
-| rain that is pouring down very hard outside |
-| the hard rain is noisy as it hits **a tin roof** |
-
-_(Candidates and references for the Clotho development-testing file named "rain.wav")_
-
-| Beam search candidates | SPIDEr |
-|:---|:---:|
-| a woman speaks and a sheep bleats | 0.190 |
-| a woman **speaks and a goat bleats** | **1.259** |
-| a man speaks and a sheep bleats | 0.344 |
-| an adult male speaks and a sheep bleats | 0.231 |
-| an adult male is speaking and a sheep bleats | 0.189 |
-
-| References |
-|:---|
-| a man speaking and laughing followed by a goat bleat |
-| a man is speaking in high tone while a goat is bleating one time |
-| a man speaks followed by a goat bleat |
-| a person **speaks and a goat bleats** |
-| a man is talking and snickering followed by a goat bleating |
-
-_(Candidates and references for an AudioCaps testing file with the id "jid4t-FzUn0")_
-</div>
-
-Even with very similar candidates, the SPIDEr scores varies drastically. To adress this issue, we proposed a SPIDEr-max metric which take the maximum value of several candidates for the same audio. SPIDEr-max demonstrate that SPIDEr can exceed state-of-the-art scores on AudioCaps and Clotho and even human scores on AudioCaps [[7]](#spider-max).
-
-### SPIDEr-max: usage
-This usage is very similar to other captioning metrics, with the main difference of take a multiple candidates list as input.
-
-```python
-from aac_metrics.functional import spider_max
-from aac_metrics.utils.tokenization import preprocess_mult_sents
-
-mult_candidates: list[list[str]] = [["a man is speaking", "maybe someone speaking"]]
-mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking while a bird is chirping in the background"]]
-
-mult_candidates = preprocess_mult_sents(mult_candidates)
-mult_references = preprocess_mult_sents(mult_references)
-
-corpus_scores, sents_scores = spider_max(mult_candidates, mult_references)
-print(corpus_scores)
-# {"spider": tensor(0.1), ...}
-print(sents_scores)
-# {"spider": tensor([0.9, ...]), ...}
-```
+| SBERT-sim [[8]](#spider-max) | `SBERTSim` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-BERT embeddings** |
+| Fluency Error [[8]](#spider-max) | `FluErr` | audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in sentences |
+| FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] | Combines SBERT-sim and Fluency Error |
+| SPIDEr-FL [[9]](#spider-fl) | `SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
 
 ## Requirements
 ### Python packages
 
 The pip requirements are automatically installed when using `pip install` on this repository.
 ```
 torch >= 1.10.1
 numpy >= 1.21.2
 pyyaml >= 6.0
 tqdm >= 4.64.0
 sentence-transformers>=2.2.2
 ```
 
 ### External requirements
-- `java` >= 1.8 is required to compute METEOR, SPICE and use the PTBTokenizer.
+- `java` **>= 1.8 and <= 1.11** is required to compute METEOR, SPICE and use the PTBTokenizer.
 Most of these functions can specify a java executable path with `java_path` argument.
 
 - `unzip` command to extract SPICE zipped files.
 
-
 ## Additional notes
 ### CIDEr or CIDEr-D ?
 The CIDEr metric differs from CIDEr-D because it applies a stemmer to each word before computing the n-grams of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
 
 ### Does metrics work on multi-GPU ?
 No. Most of these metrics use numpy or external java programs to run, which prevents multi-GPU testing for now.
 
 ### Is torchmetrics needed for this package ?
 No. But if torchmetrics is installed, all metrics classes will inherit from the base class `torchmetrics.Metric`.
 It is because most of the metrics does not use PyTorch tensors to compute scores and numpy and strings cannot be added to states of `torchmetrics.Metric`.
 
+## SPIDEr-max metric
+SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes into account multiple candidates for the same audio. It computes the maximum of the SPIDEr scores for each candidate to balance the high sensitivity to the frequency of the words generated by the model. For more detail, please see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/stable/spider_max.html).
+
 ## References
 #### BLEU
 [1] K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, “BLEU: a
 method for automatic evaluation of machine translation,” in Proceed-
 ings of the 40th Annual Meeting on Association for Computational
 Linguistics - ACL ’02. Philadelphia, Pennsylvania: Association
 for Computational Linguistics, 2001, p. 311. [Online]. Available:
@@ -263,18 +207,21 @@
 national Conference on Computer Vision (ICCV), pp. 873–881, Oct. 2017,
 arXiv: 1612.00370. [Online]. Available: http://arxiv.org/abs/1612.00370
 
 #### SPIDEr-max
 [7] E. Labbé, T. Pellegrini, and J. Pinquier, “Is my automatic audio captioning system so bad? spider-max: a metric to consider several caption candidates,” Nov. 2022. [Online]. Available: https://hal.archives-ouvertes.fr/hal-03810396
 
 #### FENSE
-[8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/2110.04684 
+[8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/2110.04684
+
+#### SPIDEr-FL
+[9] DCASE website task6a description: https://dcase.community/challenge2023/task-automated-audio-captioning#evaluation
 
 ## Citation
-If you use **SPIDEr-max**, you can cite the following paper using BibTex:
+If you use **SPIDEr-max**, you can cite the following paper using BibTex :
 ```
 @inproceedings{labbe:hal-03810396,
     TITLE = {{Is my automatic audio captioning system so bad? spider-max: a metric to consider several caption candidates}},
     AUTHOR = {Labb{\'e}, Etienne and Pellegrini, Thomas and Pinquier, Julien},
     URL = {https://hal.archives-ouvertes.fr/hal-03810396},
     BOOKTITLE = {{Workshop DCASE}},
     ADDRESS = {Nancy, France},
@@ -283,10 +230,24 @@
     KEYWORDS = {audio captioning ; evaluation metric ; beam search ; multiple candidates},
     PDF = {https://hal.archives-ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf},
     HAL_ID = {hal-03810396},
     HAL_VERSION = {v1},
 }
 ```
 
+If you use this software, please consider cite it as below :
+```
+@software{
+    Labbe_aac-metrics_2023,
+    author = {Labbé, Etienne},
+    license = {MIT},
+    month = {4},
+    title = {{aac-metrics}},
+    url = {https://github.com/Labbeti/aac-metrics/},
+    version = {0.4.0},
+    year = {2023},
+}
+```
+
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,167 +1,147 @@
-Metadata-Version: 2.1 Name: aac-metrics Version: 0.3.0 Summary: Metrics for
-evaluating Automated Audio Captioning systems, designed for PyTorch. Home-page:
-https://github.com/Labbeti/aac-metrics Author: Etienne LabbÃ© (Labbeti) Author-
-email: labbeti.pub@gmail.com License: MIT Project-URL: Documentation, https://
-aac-metrics.readthedocs.io/ Project-URL: Source, https://github.com/Labbeti/
-aac-metrics Project-URL: PyPI, https://pypi.org/project/aac-metrics/
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.9 Description-
-Content-Type: text/markdown Provides-Extra: dev License-File: LICENCE
+Metadata-Version: 2.1 Name: aac-metrics Version: 0.4.0 Summary: Metrics for
+evaluating Automated Audio Captioning systems, designed for PyTorch. Author-
+email: "Etienne LabbÃ© (Labbeti)"
+pub@gmail.com> Maintainer-email: "Etienne LabbÃ© (Labbeti)"
+pub@gmail.com> Project-URL: homepage, https://pypi.org/project/aac-metrics/
+Project-URL: documentation, https://aac-metrics.readthedocs.io/ Project-URL:
+repository, https://github.com//Labbeti/aac-metrics.git Project-URL: changelog,
+https://github.com/Labbeti/aac-metrics/blob/main/CHANGELOG.md Keywords:
+audio,metrics,text,captioning,audio-captioning Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.9 Description-Content-Type: text/markdown
+Provides-Extra: dev License-File: LICENCE
 # Audio Captioning metrics (aac-metrics) [Python] [PyTorch] [Code_style:_black]
      [Build] [Documentation_Status] Metrics for evaluating Automated Audio
                    Captioning systems, designed for PyTorch.
 ## Why using this package? - **Easy installation and download** - **Same
 results than [caption-evaluation-tools](https://github.com/audio-captioning/
 caption-evaluation-tools) and [fense](https://github.com/blmoistawinde/fense)
 repositories** - **Provides the following metrics:** - BLEU [[1]](#bleu) -
 ROUGE-L [[2]](#rouge-l) - METEOR [[3]](#meteor) - CIDEr-D [[4]](#cider) - SPICE
-[[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT [
-[8]](#fense) - FluencyError [[8]](#fense) - FENSE [[8]](#fense) - SPIDErErr ##
-Installation Install the pip package: ```bash pip install aac-metrics ```
-Download the external code and models needed for METEOR, SPICE, PTBTokenizer
-and FENSE: ```bash aac-metrics-download ``` Notes: - The external code for
+[[5]](#spice) - SPIDEr [[6]](#spider) - SPIDEr-max [[7]](#spider-max) - SBERT-
+sim [[8]](#fense) - Fluency Error [[8]](#fense) - FENSE [[8]](#fense) - SPIDEr-
+FL [[9]](#spider-fl) ## Installation Install the pip package: ```bash pip
+install aac-metrics ``` Download the external code and models needed for
+METEOR, SPICE, SPIDEr, SPIDEr-max, PTBTokenizer, SBERT, FluencyError, FENSE and
+SPIDEr-FL: ```bash aac-metrics-download ``` Notes: - The external code for
 SPICE, METEOR and PTBTokenizer is stored in `$HOME/.cache/aac-metrics`. - The
 weights of the FENSE fluency error detector and the the SBERT model are
 respectively stored by default in `$HOME/.cache/torch/hub/fense_data` and
-`$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default AAC
-metrics The full evaluation process to compute AAC metrics can be done with
-`aac_metrics.aac_evaluate` function. ```python from aac_metrics import
-aac_evaluate candidates: list[str] = ["a man is speaking"] mult_references:
-list[list[str]] = [["a man speaks.", "someone speaks.", "a man is speaking
-while a bird is chirping in the background"]] corpus_scores, _ = aac_evaluate
-(candidates, mult_references) print(corpus_scores) # dict containing the score
-of each aac metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l",
-"meteor", "cider_d", "spice", "spider" # {"bleu_1": tensor(0.7), "bleu_2": ...,
-...} ``` ### Evaluate a specific metric Evaluate a specific metric can be done
-using the `aac_metrics.functional..` function or the `aac_metrics.classes..`
-class. Unlike `aac_evaluate`, the tokenization with PTBTokenizer is not done
-with these functions, but you can do it manually with `preprocess_mono_sents`
-and `preprocess_mult_sents` functions. ```python from aac_metrics.functional
-import cider_d from aac_metrics.utils.tokenization import
-preprocess_mono_sents, preprocess_mult_sents candidates: list[str] = ["a man is
-speaking"] mult_references: list[list[str]] = [["a man speaks.", "someone
-speaks.", "a man is speaking while a bird is chirping in the background"]]
-candidates = preprocess_mono_sents(candidates) mult_references =
-preprocess_mult_sents(mult_references) corpus_scores, sents_scores = cider_d
-(candidates, mult_references) print(corpus_scores) # {"cider_d": tensor(0.1)}
-print(sents_scores) # {"cider_d": tensor([0.9, ...])} ``` Each metrics also
-exists as a python class version, like `aac_metrics.classes.cider_d.CIDErD`. ##
-Metrics ### Default AAC metrics | Metric | Python Class | Origin | Range |
-Short description | |:---|:---|:---|:---|:---| | BLEU [[1]](#bleu) | `BLEU` |
-machine translation | [0, 1] | Precision of n-grams | | ROUGE-L [[2]](#rouge-l)
-| `ROUGEL` | machine translation | [0, 1] | FScore of the longest common
+`$HOME/.cache/torch/sentence_transformers`. ## Usage ### Evaluate default
+metrics The full evaluation pipeline to compute AAC metrics can be done with
+`aac_metrics.evaluate` function. ```python from aac_metrics import evaluate
+candidates: list[str] = ["a man is speaking"] mult_references: list[list[str]]
+= [["a man speaks.", "someone speaks.", "a man is speaking while a bird is
+chirping in the background"]] corpus_scores, _ = evaluate(candidates,
+mult_references) print(corpus_scores) # dict containing the score of each
+metric: "bleu_1", "bleu_2", "bleu_3", "bleu_4", "rouge_l", "meteor", "cider_d",
+"spice", "spider" # {"bleu_1": tensor(0.7), "bleu_2": ..., ...} ``` ###
+Evaluate DCASE2023 metrics To compute metrics for the DCASE2023 challenge, just
+set the argument `metrics="dcase2023"` in `evaluate` function call. ```python
+corpus_scores, _ = evaluate(candidates, mult_references, metrics="dcase2023")
+print(corpus_scores) # dict containing the score of each metric: "meteor",
+"cider_d", "spice", "spider", "spider_fl", "fluerr" ``` ### Evaluate a specific
+metric Evaluate a specific metric can be done using the
+`aac_metrics.functional..` function or the `aac_metrics.classes..` class.
+Unlike `evaluate`, the tokenization with PTBTokenizer is not done with these
+functions, but you can do it manually with `preprocess_mono_sents` and
+`preprocess_mult_sents` functions. ```python from aac_metrics.functional import
+cider_d from aac_metrics.utils.tokenization import preprocess_mono_sents,
+preprocess_mult_sents candidates: list[str] = ["a man is speaking"]
+mult_references: list[list[str]] = [["a man speaks.", "someone speaks.", "a man
+is speaking while a bird is chirping in the background"]] candidates =
+preprocess_mono_sents(candidates) mult_references = preprocess_mult_sents
+(mult_references) corpus_scores, sents_scores = cider_d(candidates,
+mult_references) print(corpus_scores) # {"cider_d": tensor(0.1)} print
+(sents_scores) # {"cider_d": tensor([0.9, ...])} ``` Each metrics also exists
+as a python class version, like `aac_metrics.classes.cider_d.CIDErD`. ##
+Metrics ### Legacy metrics | Metric | Python Class | Origin | Range | Short
+description | |:---|:---|:---|:---|:---| | BLEU [[1]](#bleu) | `BLEU` | machine
+translation | [0, 1] | Precision of n-grams | | ROUGE-L [[2]](#rouge-l) |
+`ROUGEL` | machine translation | [0, 1] | FScore of the longest common
 subsequence | | METEOR [[3]](#meteor) | `METEOR` | machine translation | [0, 1]
 | Cosine-similarity of frequencies with synonyms matching | | CIDEr-D [[4]]
 (#cider) | `CIDErD` | image captioning | [0, 10] | Cosine-similarity of TF-IDF
 computed on n-grams | | SPICE [[5]](#spice) | `SPICE` | image captioning | [0,
 1] | FScore of semantic graph | | SPIDEr [[6]](#spider) | `SPIDEr` | image
-captioning | [0, 5.5] | Mean of CIDEr-D and SPICE | ### Other metrics | Metric
-name | Python Class | Origin | Range | Short description | |:---|:---|:---|:---
-|:---| | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning | [0,
-5.5] | Max of SPIDEr scores for multiples candidates | | SBERT [[7]](#spider-
-max) | `SBERT` | audio captioning | [-1, 1] | Cosine-similarity of **Sentence-
-BERT embeddings** | | FluencyError [[7]](#spider-max) | `FluencyError` | audio
-captioning | [0, 1] | Use pretrained model to detect fluency errors in
+captioning | [0, 5.5] | Mean of CIDEr-D and SPICE | ### AAC-specific metrics |
+Metric name | Python Class | Origin | Range | Short description | |:---|:---|:-
+--|:---|:---| | SPIDEr-max [[7]](#spider-max) | `SPIDErMax` | audio captioning
+| [0, 5.5] | Max of SPIDEr scores for multiples candidates | | SBERT-sim [[8]]
+(#spider-max) | `SBERTSim` | audio captioning | [-1, 1] | Cosine-similarity of
+**Sentence-BERT embeddings** | | Fluency Error [[8]](#spider-max) | `FluErr` |
+audio captioning | [0, 1] | Use a pretrained model to detect fluency errors in
 sentences | | FENSE [[8]](#fense) | `FENSE` | audio captioning | [-1, 1] |
-Combines `SBERT` and `FluencyError` | | SPIDErErr | `SPIDErErr` | audio
-captioning | [0, 5.5] | Combines `SPIDEr` and `FluencyError` | ## SPIDEr-max
-metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr that takes
-into account multiple candidates for the same audio. It computes the maximum of
-the SPIDEr scores for each candidate to balance the high sensitivity to the
-frequency of the words generated by the model. ### SPIDEr-max: why ? The SPIDEr
-metric used in audio captioning is highly sensitive to the frequencies of the
-words used. Here is 2 examples with the 5 candidates generated by the beam
-search algorithm, their corresponding SPIDEr scores and the associated
-references:
- | Beam search candidates | SPIDEr | |:---|:---:| | heavy rain is falling on a
-  roof | 0.562 | | heavy rain is falling on **a tin roof** | **0.930** | | a
-  heavy rain is falling on a roof | 0.594 | | a heavy rain is falling on the
-ground | 0.335 | | a heavy rain is falling on the roof | 0.594 | | References |
- |:---| | heavy rain falls loudly onto a structure with a thin roof | | heavy
-rainfall falling onto a thin structure with a thin roof | | it is raining hard
-   and the rain hits **a tin roof** | | rain that is pouring down very hard
-outside | | the hard rain is noisy as it hits **a tin roof** | _(Candidates and
- references for the Clotho development-testing file named "rain.wav")_ | Beam
-search candidates | SPIDEr | |:---|:---:| | a woman speaks and a sheep bleats |
-0.190 | | a woman **speaks and a goat bleats** | **1.259** | | a man speaks and
-a sheep bleats | 0.344 | | an adult male speaks and a sheep bleats | 0.231 | |
-an adult male is speaking and a sheep bleats | 0.189 | | References | |:---| |
- a man speaking and laughing followed by a goat bleat | | a man is speaking in
-high tone while a goat is bleating one time | | a man speaks followed by a goat
-   bleat | | a person **speaks and a goat bleats** | | a man is talking and
-  snickering followed by a goat bleating | _(Candidates and references for an
-              AudioCaps testing file with the id "jid4t-FzUn0")_
-Even with very similar candidates, the SPIDEr scores varies drastically. To
-adress this issue, we proposed a SPIDEr-max metric which take the maximum value
-of several candidates for the same audio. SPIDEr-max demonstrate that SPIDEr
-can exceed state-of-the-art scores on AudioCaps and Clotho and even human
-scores on AudioCaps [[7]](#spider-max). ### SPIDEr-max: usage This usage is
-very similar to other captioning metrics, with the main difference of take a
-multiple candidates list as input. ```python from aac_metrics.functional import
-spider_max from aac_metrics.utils.tokenization import preprocess_mult_sents
-mult_candidates: list[list[str]] = [["a man is speaking", "maybe someone
-speaking"]] mult_references: list[list[str]] = [["a man speaks.", "someone
-speaks.", "a man is speaking while a bird is chirping in the background"]]
-mult_candidates = preprocess_mult_sents(mult_candidates) mult_references =
-preprocess_mult_sents(mult_references) corpus_scores, sents_scores = spider_max
-(mult_candidates, mult_references) print(corpus_scores) # {"spider": tensor
-(0.1), ...} print(sents_scores) # {"spider": tensor([0.9, ...]), ...} ``` ##
-Requirements ### Python packages The pip requirements are automatically
+Combines SBERT-sim and Fluency Error | | SPIDEr-FL [[9]](#spider-fl) |
+`SPIDErFL` | audio captioning | [0, 5.5] | Combines SPIDEr and Fluency Error |
+## Requirements ### Python packages The pip requirements are automatically
 installed when using `pip install` on this repository. ``` torch >= 1.10.1
 numpy >= 1.21.2 pyyaml >= 6.0 tqdm >= 4.64.0 sentence-transformers>=2.2.2 ```
-### External requirements - `java` >= 1.8 is required to compute METEOR, SPICE
-and use the PTBTokenizer. Most of these functions can specify a java executable
-path with `java_path` argument. - `unzip` command to extract SPICE zipped
-files. ## Additional notes ### CIDEr or CIDEr-D ? The CIDEr metric differs from
-CIDEr-D because it applies a stemmer to each word before computing the n-grams
-of the sentences. In AAC, only the CIDEr-D is reported and used for SPIDEr in
-[caption-evaluation-tools](https://github.com/audio-captioning/caption-
-evaluation-tools), but some papers called it "CIDEr". ### Does metrics work on
-multi-GPU ? No. Most of these metrics use numpy or external java programs to
-run, which prevents multi-GPU testing for now. ### Is torchmetrics needed for
-this package ? No. But if torchmetrics is installed, all metrics classes will
-inherit from the base class `torchmetrics.Metric`. It is because most of the
-metrics does not use PyTorch tensors to compute scores and numpy and strings
-cannot be added to states of `torchmetrics.Metric`. ## References #### BLEU [1]
-K. Papineni, S. Roukos, T. Ward, and W.-J. Zhu, âBLEU: a method for automatic
-evaluation of machine translation,â in Proceed- ings of the 40th Annual
-Meeting on Association for Computational Linguistics - ACL â02. Philadelphia,
-Pennsylvania: Association for Computational Linguistics, 2001, p. 311.
-[Online]. Available: http://portal.acm.org/citation.cfm?doid=1073083.1073135
-#### ROUGE-L [2] C.-Y. Lin, âROUGE: A package for automatic evaluation of
-summaries,â in Text Summarization Branches Out. Barcelona, Spain: Association
-for Computational Linguistics, Jul. 2004, pp. 74â81. [Online]. Available:
-https://aclanthology.org/W04-1013 #### METEOR [3] M. Denkowski and A. Lavie,
-âMeteor Universal: Language Specific Translation Evaluation for Any Target
-Language,â in Proceedings of the Ninth Workshop on Statistical Machine
-Translation. Baltimore, Maryland, USA: Association for Computational
-Linguistics, 2014, pp. 376â380. [Online]. Available: http://aclweb.org/
-anthology/W14-3348 #### CIDEr [4] R. Vedantam, C. L. Zitnick, and D. Parikh,
-âCIDEr: Consensus-based Image Description Evaluation,â arXiv:1411.5726
-[cs], Jun. 2015, arXiv: 1411.5726. [Online]. Available: http://arxiv.org/abs/
-1411.5726 #### SPICE [5] P. Anderson, B. Fernando, M. Johnson, and S. Gould,
-âSPICE: Semantic Propositional Image Caption Evaluation,â arXiv:1607.08822
-[cs], Jul. 2016, arXiv: 1607.08822. [Online]. Available: http://arxiv.org/abs/
-1607.08822 #### SPIDEr [6] S. Liu, Z. Zhu, N. Ye, S. Guadarrama, and K. Murphy,
-âImproved Image Captioning via Policy Gradient optimization of SPIDEr,â
-2017 IEEE Inter- national Conference on Computer Vision (ICCV), pp. 873â881,
-Oct. 2017, arXiv: 1612.00370. [Online]. Available: http://arxiv.org/abs/
-1612.00370 #### SPIDEr-max [7] E. LabbÃ©, T. Pellegrini, and J. Pinquier, âIs
-my automatic audio captioning system so bad? spider-max: a metric to consider
-several caption candidates,â Nov. 2022. [Online]. Available: https://
-hal.archives-ouvertes.fr/hal-03810396 #### FENSE [8] Z. Zhou, Z. Zhang, X. Xu,
-Z. Xie, M. Wu, and K. Q. Zhu, Can Audio Captions Be Evaluated with Image
-Caption Metrics? arXiv, 2022. [Online]. Available: http://arxiv.org/abs/
-2110.04684 ## Citation If you use **SPIDEr-max**, you can cite the following
-paper using BibTex: ``` @inproceedings{labbe:hal-03810396, TITLE = {{Is my
-automatic audio captioning system so bad? spider-max: a metric to consider
-several caption candidates}}, AUTHOR = {Labb{\'e}, Etienne and Pellegrini,
-Thomas and Pinquier, Julien}, URL = {https://hal.archives-ouvertes.fr/hal-
-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy, France}, YEAR =
-{2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation metric ; beam
-search ; multiple candidates}, PDF = {https://hal.archives-ouvertes.fr/hal-
-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396}, HAL_VERSION =
-{v1}, } ``` ## Contact Maintainer: - Etienne LabbÃ© "Labbeti":
-labbeti.pub@gmail.com
+### External requirements - `java` **>= 1.8 and <= 1.11** is required to
+compute METEOR, SPICE and use the PTBTokenizer. Most of these functions can
+specify a java executable path with `java_path` argument. - `unzip` command to
+extract SPICE zipped files. ## Additional notes ### CIDEr or CIDEr-D ? The
+CIDEr metric differs from CIDEr-D because it applies a stemmer to each word
+before computing the n-grams of the sentences. In AAC, only the CIDEr-D is
+reported and used for SPIDEr in [caption-evaluation-tools](https://github.com/
+audio-captioning/caption-evaluation-tools), but some papers called it "CIDEr".
+### Does metrics work on multi-GPU ? No. Most of these metrics use numpy or
+external java programs to run, which prevents multi-GPU testing for now. ### Is
+torchmetrics needed for this package ? No. But if torchmetrics is installed,
+all metrics classes will inherit from the base class `torchmetrics.Metric`. It
+is because most of the metrics does not use PyTorch tensors to compute scores
+and numpy and strings cannot be added to states of `torchmetrics.Metric`. ##
+SPIDEr-max metric SPIDEr-max [[7]](#spider-max) is a metric based on SPIDEr
+that takes into account multiple candidates for the same audio. It computes the
+maximum of the SPIDEr scores for each candidate to balance the high sensitivity
+to the frequency of the words generated by the model. For more detail, please
+see the [documentation about SPIDEr-max](https://aac-metrics.readthedocs.io/en/
+stable/spider_max.html). ## References #### BLEU [1] K. Papineni, S. Roukos, T.
+Ward, and W.-J. Zhu, âBLEU: a method for automatic evaluation of machine
+translation,â in Proceed- ings of the 40th Annual Meeting on Association for
+Computational Linguistics - ACL â02. Philadelphia, Pennsylvania: Association
+for Computational Linguistics, 2001, p. 311. [Online]. Available: http://
+portal.acm.org/citation.cfm?doid=1073083.1073135 #### ROUGE-L [2] C.-Y. Lin,
+âROUGE: A package for automatic evaluation of summaries,â in Text
+Summarization Branches Out. Barcelona, Spain: Association for Computational
+Linguistics, Jul. 2004, pp. 74â81. [Online]. Available: https://
+aclanthology.org/W04-1013 #### METEOR [3] M. Denkowski and A. Lavie, âMeteor
+Universal: Language Specific Translation Evaluation for Any Target Language,â
+in Proceedings of the Ninth Workshop on Statistical Machine Translation.
+Baltimore, Maryland, USA: Association for Computational Linguistics, 2014, pp.
+376â380. [Online]. Available: http://aclweb.org/anthology/W14-3348 #### CIDEr
+[4] R. Vedantam, C. L. Zitnick, and D. Parikh, âCIDEr: Consensus-based Image
+Description Evaluation,â arXiv:1411.5726 [cs], Jun. 2015, arXiv: 1411.5726.
+[Online]. Available: http://arxiv.org/abs/1411.5726 #### SPICE [5] P. Anderson,
+B. Fernando, M. Johnson, and S. Gould, âSPICE: Semantic Propositional Image
+Caption Evaluation,â arXiv:1607.08822 [cs], Jul. 2016, arXiv: 1607.08822.
+[Online]. Available: http://arxiv.org/abs/1607.08822 #### SPIDEr [6] S. Liu, Z.
+Zhu, N. Ye, S. Guadarrama, and K. Murphy, âImproved Image Captioning via
+Policy Gradient optimization of SPIDEr,â 2017 IEEE Inter- national Conference
+on Computer Vision (ICCV), pp. 873â881, Oct. 2017, arXiv: 1612.00370.
+[Online]. Available: http://arxiv.org/abs/1612.00370 #### SPIDEr-max [7] E.
+LabbÃ©, T. Pellegrini, and J. Pinquier, âIs my automatic audio captioning
+system so bad? spider-max: a metric to consider several caption candidates,â
+Nov. 2022. [Online]. Available: https://hal.archives-ouvertes.fr/hal-03810396
+#### FENSE [8] Z. Zhou, Z. Zhang, X. Xu, Z. Xie, M. Wu, and K. Q. Zhu, Can
+Audio Captions Be Evaluated with Image Caption Metrics? arXiv, 2022. [Online].
+Available: http://arxiv.org/abs/2110.04684 #### SPIDEr-FL [9] DCASE website
+task6a description: https://dcase.community/challenge2023/task-automated-audio-
+captioning#evaluation ## Citation If you use **SPIDEr-max**, you can cite the
+following paper using BibTex : ``` @inproceedings{labbe:hal-03810396, TITLE = {
+{Is my automatic audio captioning system so bad? spider-max: a metric to
+consider several caption candidates}}, AUTHOR = {Labb{\'e}, Etienne and
+Pellegrini, Thomas and Pinquier, Julien}, URL = {https://hal.archives-
+ouvertes.fr/hal-03810396}, BOOKTITLE = {{Workshop DCASE}}, ADDRESS = {Nancy,
+France}, YEAR = {2022}, MONTH = Nov, KEYWORDS = {audio captioning ; evaluation
+metric ; beam search ; multiple candidates}, PDF = {https://hal.archives-
+ouvertes.fr/hal-03810396/file/Labbe_DCASE2022.pdf}, HAL_ID = {hal-03810396},
+HAL_VERSION = {v1}, } ``` If you use this software, please consider cite it as
+below : ``` @software{ Labbe_aac-metrics_2023, author = {LabbÃ©, Etienne},
+license = {MIT}, month = {4}, title = {{aac-metrics}}, url = {https://
+github.com/Labbeti/aac-metrics/}, version = {0.4.0}, year = {2023}, } ``` ##
+Contact Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac-metrics-0.3.0/src/aac_metrics.egg-info/SOURCES.txt` & `aac-metrics-0.4.0/src/aac_metrics.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENCE
 MANIFEST.in
 README.md
 install_spice.sh
-setup.cfg
+pyproject.toml
 setup.py
 ./setup.py
 ./.github/workflows/python-package-pip.yaml
 ./src/aac_metrics/__init__.py
 ./src/aac_metrics/__main__.py
 ./src/aac_metrics/download.py
 ./src/aac_metrics/evaluate.py
@@ -62,33 +62,44 @@
 src/aac_metrics/classes/__init__.py
 src/aac_metrics/classes/base.py
 src/aac_metrics/classes/bleu.py
 src/aac_metrics/classes/cider_d.py
 src/aac_metrics/classes/evaluate.py
 src/aac_metrics/classes/fense.py
 src/aac_metrics/classes/fluency_error.py
+src/aac_metrics/classes/fluerr.py
 src/aac_metrics/classes/meteor.py
 src/aac_metrics/classes/rouge_l.py
 src/aac_metrics/classes/sbert.py
+src/aac_metrics/classes/sbert_sim.py
 src/aac_metrics/classes/spice.py
 src/aac_metrics/classes/spider.py
 src/aac_metrics/classes/spider_err.py
+src/aac_metrics/classes/spider_fl.py
 src/aac_metrics/classes/spider_max.py
 src/aac_metrics/functional/__init__.py
 src/aac_metrics/functional/bleu.py
 src/aac_metrics/functional/cider_d.py
 src/aac_metrics/functional/evaluate.py
 src/aac_metrics/functional/fense.py
 src/aac_metrics/functional/fluency_error.py
+src/aac_metrics/functional/fluerr.py
 src/aac_metrics/functional/meteor.py
 src/aac_metrics/functional/mult_cands.py
 src/aac_metrics/functional/rouge_l.py
 src/aac_metrics/functional/sbert.py
+src/aac_metrics/functional/sbert_sim.py
 src/aac_metrics/functional/spice.py
 src/aac_metrics/functional/spider.py
 src/aac_metrics/functional/spider_err.py
+src/aac_metrics/functional/spider_fl.py
 src/aac_metrics/functional/spider_max.py
 src/aac_metrics/utils/__init__.py
 src/aac_metrics/utils/checks.py
 src/aac_metrics/utils/collections.py
 src/aac_metrics/utils/imports.py
-src/aac_metrics/utils/tokenization.py
+src/aac_metrics/utils/tokenization.py
+tests/test_bleu_tchmet.py
+tests/test_compare_cet.py
+tests/test_compare_fense.py
+tests/test_pickable.py
+tests/test_utils.py
```

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/cider/cider_scorer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/eval.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/rouge/rouge.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/spice/spice.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocoevalcap/tokenizer/ptbtokenizer.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/coco_caption/pycocotools/coco.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/caption-evaluation-tools/eval_metrics.py` & `aac-metrics-0.4.0/tests/caption-evaluation-tools/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aac-metrics-0.3.0/tests/test_bleu_tchmet.py` & `aac-metrics-0.4.0/tests/test_bleu_tchmet.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from aac_metrics.utils.imports import _TORCHMETRICS_AVAILABLE
 
 if _TORCHMETRICS_AVAILABLE:
     from torchmetrics.text.bleu import BLEUScore
 
 
 class TestBleu(TestCase):
+    # Tests methods
     def test_bleu(self) -> None:
         if not _TORCHMETRICS_AVAILABLE:
             return None
 
         cands = ["a man is speaking", "birds chirping"]
         mrefs = [
             [
```

### Comparing `aac-metrics-0.3.0/tests/test_pickable.py` & `aac-metrics-0.4.0/tests/test_pickable.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # -*- coding: utf-8 -*-
 
 import pickle
 import unittest
 
 from unittest import TestCase
 
-from aac_metrics.classes.evaluate import _get_metrics_classes_list
+from aac_metrics.classes.evaluate import _instantiate_metrics_classes
 
 
 class TestCompare(TestCase):
+    # Tests methods
     def test_pickle_dump(self) -> None:
-        metrics = _get_metrics_classes_list("all")
+        metrics = _instantiate_metrics_classes("all")
 
         for metric in metrics:
             try:
                 pickle.dumps(metric)
             except pickle.PicklingError:
                 self.assert_(False, f"Cannot pickle {metric.__class__.__name__}.")
```

