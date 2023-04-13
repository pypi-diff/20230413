# Comparing `tmp/sleepecg-0.5.3.tar.gz` & `tmp/sleepecg-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepecg-0.5.3.tar", last modified: Mon Dec  5 11:08:37 2022, max compression
+gzip compressed data, was "sleepecg-0.5.4.tar", last modified: Thu Apr 13 05:51:12 2023, max compression
```

## Comparing `sleepecg-0.5.3.tar` & `sleepecg-0.5.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.515879 sleepecg-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.499879 sleepecg-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.503879 sleepecg-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1526 2022-12-05 11:08:30.000000 sleepecg-0.5.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      882 2022-12-05 11:08:30.000000 sleepecg-0.5.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      163 2022-12-05 11:08:30.000000 sleepecg-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      778 2022-12-05 11:08:30.000000 sleepecg-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5932 2022-12-05 11:08:30.000000 sleepecg-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2022-12-05 11:08:30.000000 sleepecg-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1538 2022-12-05 11:08:30.000000 sleepecg-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      240 2022-12-05 11:08:30.000000 sleepecg-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4706 2022-12-05 11:08:37.515879 sleepecg-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3261 2022-12-05 11:08:30.000000 sleepecg-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.503879 sleepecg-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.503879 sleepecg-0.5.3/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3369 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/benchmark/benchmark_detectors.py
--rw-r--r--   0 runner    (1001) docker     (122)      824 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/benchmark/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/benchmark/plot_benchmark_results.py
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/benchmark/requirements-benchmark.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.503879 sleepecg-0.5.3/examples/classifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     2500 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/classifiers/wrn_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (122)     2563 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/classifiers/wrn_gru_mesa_weighted.py
--rw-r--r--   0 runner    (1001) docker     (122)     2483 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/classifiers/ws_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/heartbeat_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2022-12-05 11:08:30.000000 sleepecg-0.5.3/examples/try_ws_gru_mesa.py
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-12-05 11:08:30.000000 sleepecg-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      324 2022-12-05 11:08:30.000000 sleepecg-0.5.3/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2022-12-05 11:08:37.515879 sleepecg-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      263 2022-12-05 11:08:30.000000 sleepecg-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.507879 sleepecg-0.5.3/sleepecg/
--rw-r--r--   0 runner    (1001) docker     (122)      539 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23823 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/_heartbeat_detection.c
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/_heartbeat_detection.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    18850 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.511879 sleepecg-0.5.3/sleepecg/classifiers/
--rw-r--r--   0 runner    (1001) docker     (122)   775585 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
--rw-r--r--   0 runner    (1001) docker     (122)   764383 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/classifiers/wrn-gru-mesa.zip
--rw-r--r--   0 runner    (1001) docker     (122)   775057 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/classifiers/ws-gru-mesa.zip
--rw-r--r--   0 runner    (1001) docker     (122)     3158 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/config.py
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)    26052 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    27521 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/heartbeats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.511879 sleepecg-0.5.3/sleepecg/io/
--rw-r--r--   0 runner    (1001) docker     (122)      426 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10104 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/ecg_readers.py
--rw-r--r--   0 runner    (1001) docker     (122)    29259 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/gudb.py
--rw-r--r--   0 runner    (1001) docker     (122)     6200 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/nsrr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4290 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/physionet.py
--rw-r--r--   0 runner    (1001) docker     (122)    24166 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/sleep_readers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2715 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8547 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.515879 sleepecg-0.5.3/sleepecg/test/
--rw-r--r--   0 runner    (1001) docker     (122)      700 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (122)     6496 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_heartbeat_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (122)     6045 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/test/test_sleep_readers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2022-12-05 11:08:30.000000 sleepecg-0.5.3/sleepecg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 11:08:37.507879 sleepecg-0.5.3/sleepecg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4706 2022-12-05 11:08:36.000000 sleepecg-0.5.3/sleepecg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1605 2022-12-05 11:08:37.000000 sleepecg-0.5.3/sleepecg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 11:08:36.000000 sleepecg-0.5.3/sleepecg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      675 2022-12-05 11:08:36.000000 sleepecg-0.5.3/sleepecg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-05 11:08:36.000000 sleepecg-0.5.3/sleepecg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.763930 sleepecg-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.751929 sleepecg-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 05:51:04.000000 sleepecg-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-13 05:51:04.000000 sleepecg-0.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-13 05:51:04.000000 sleepecg-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-13 05:51:04.000000 sleepecg-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 05:51:04.000000 sleepecg-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-13 05:51:12.763930 sleepecg-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-13 05:51:04.000000 sleepecg-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/benchmark_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/plot_benchmark_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/requirements-benchmark.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/examples/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/classifiers/ws_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/heartbeat_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 05:51:04.000000 sleepecg-0.5.4/examples/try_ws_gru_mesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 05:51:04.000000 sleepecg-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-13 05:51:04.000000 sleepecg-0.5.4/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-13 05:51:12.763930 sleepecg-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 05:51:04.000000 sleepecg-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.755930 sleepecg-0.5.4/sleepecg/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/_heartbeat_detection.c
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/_heartbeat_detection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.759930 sleepecg-0.5.4/sleepecg/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)   775585 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa-weighted.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   764383 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   775057 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/classifiers/ws-gru-mesa.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26627 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27521 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/heartbeats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.759930 sleepecg-0.5.4/sleepecg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/ecg_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29259 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/gudb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/nsrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/physionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24290 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/sleep_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.763930 sleepecg-0.5.4/sleepecg/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_heartbeat_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/test/test_sleep_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-13 05:51:04.000000 sleepecg-0.5.4/sleepecg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:51:12.759930 sleepecg-0.5.4/sleepecg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 05:51:12.000000 sleepecg-0.5.4/sleepecg.egg-info/top_level.txt
```

### Comparing `sleepecg-0.5.3/.github/workflows/release.yml` & `sleepecg-0.5.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/.github/workflows/test.yml` & `sleepecg-0.5.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/.pre-commit-config.yaml` & `sleepecg-0.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/CHANGELOG.md` & `sleepecg-0.5.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## [0.5.4] - 2023-04-13
+### Changed
+- Remove dependency on pandas for `read_gudb` ([#134](https://github.com/cbrnr/sleepecg/pull/134) by [Florian Hofer](https://github.com/hofaflo))
+- Update SHHS encoding and missing data handling for `read_shhs` ([#139](https://github.com/cbrnr/sleepecg/pull/139) by [Andrew Gilbert](https://github.com/adgilbert))
+- Ignore expected warnings during feature extraction ([#142](https://github.com/cbrnr/sleepecg/pull/142) by [Florian Hofer](https://github.com/hofaflo))
+
 ## [0.5.3] - 2022-12-05
 ### Added
 - Do not redownload GUDB data sets if they are already stored locally ([#112](https://github.com/cbrnr/sleepecg/pull/112) by [Clemens Brunner](https://github.com/cbrnr))
 - Add `sleepecg.plot_ecg` and `sleepecg.ECGRecord.plot` functions for plotting ECG with beat annotations ([#116](https://github.com/cbrnr/sleepecg/pull/116) by [Clemens Brunner](https://github.com/cbrnr))
 
 ### Changed
 - The detector benchmark example now requires only those packages that are actually used in the benchmark ([#114](https://github.com/cbrnr/sleepecg/pull/114) by [Clemens Brunner](https://github.com/cbrnr))
```

### Comparing `sleepecg-0.5.3/CONTRIBUTING.md` & `sleepecg-0.5.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/LICENSE` & `sleepecg-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/PKG-INFO` & `sleepecg-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepecg
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for sleep stage classification using ECG data
 Home-page: https://github.com/cbrnr/sleepecg
 Author: Florian Hofer
 Author-email: hofaflo@gmail.com
 Maintainer: Clemens Brunner
 Maintainer-email: clemens.brunner@gmail.com
 License: BSD 3-Clause License
@@ -38,15 +38,14 @@
         
         Optional dependencies provide additional features:
         
         - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
         - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
         - [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
         - [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-        - [pandas](https://pandas.pydata.org/) ≥ 1.4.0 (read data from [GUDB](https://berndporr.github.io/ECG-GUDB))
         - [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
         - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
         
         ### Installation
         SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
         
         ```
```

### Comparing `sleepecg-0.5.3/README.md` & `sleepecg-0.5.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 Optional dependencies provide additional features:
 
 - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
 - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
 - [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
 - [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-- [pandas](https://pandas.pydata.org/) ≥ 1.4.0 (read data from [GUDB](https://berndporr.github.io/ECG-GUDB))
 - [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
 - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
 
 ### Installation
 SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
 
 ```
```

### Comparing `sleepecg-0.5.3/examples/benchmark/README.md` & `sleepecg-0.5.4/examples/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/benchmark/benchmark_detectors.py` & `sleepecg-0.5.4/examples/benchmark/benchmark_detectors.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/benchmark/config.yml` & `sleepecg-0.5.4/examples/benchmark/config.yml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/benchmark/plot_benchmark_results.py` & `sleepecg-0.5.4/examples/benchmark/plot_benchmark_results.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/benchmark/utils.py` & `sleepecg-0.5.4/examples/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/classifiers/wrn_gru_mesa.py` & `sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/classifiers/wrn_gru_mesa_weighted.py` & `sleepecg-0.5.4/examples/classifiers/wrn_gru_mesa_weighted.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/classifiers/ws_gru_mesa.py` & `sleepecg-0.5.4/examples/classifiers/ws_gru_mesa.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/feature_extraction.py` & `sleepecg-0.5.4/examples/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/heartbeat_detection.py` & `sleepecg-0.5.4/examples/heartbeat_detection.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/examples/try_ws_gru_mesa.py` & `sleepecg-0.5.4/examples/try_ws_gru_mesa.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/pyproject.toml` & `sleepecg-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/setup.cfg` & `sleepecg-0.5.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -34,28 +34,26 @@
 
 [options.extras_require]
 full = 
 	joblib>=1.0.0
 	matplotlib>=3.5.0
 	mne>=1.0.0
 	numba>=0.55.0;python_version<'3.11'
-	pandas>=1.4.0
 	tensorflow>=2.7.0;python_version<'3.11'
 	wfdb>=3.4.0
 dev = 
 	black>=22.6.0
 	flake8>=4.0.0
 	joblib>=1.0.0
 	matplotlib>=3.5.0
 	mkdocs-material>=8.4.0
 	mkdocstrings-python>=0.7.1
 	mne>=1.0.0
 	mypy>=0.991
 	numba>=0.55.0;python_version<'3.11'
-	pandas>=1.4.0
 	pre-commit>=2.13.0
 	pyEDFlib>=0.1.25
 	pytest>=6.2.0
 	setuptools>=56.0.0
 	sphinx>=4.1.0
 	tensorflow>=2.7.0;python_version<'3.11'
 	wfdb>=3.4.0
```

### Comparing `sleepecg-0.5.3/sleepecg/__init__.py` & `sleepecg-0.5.4/sleepecg/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 )
 from .config import get_config, set_config
 from .feature_extraction import extract_features, preprocess_rri
 from .heartbeats import compare_heartbeats, detect_heartbeats, rri_similarity
 from .io import *  # noqa: F403
 from .plot import plot_ecg, plot_hypnogram
 
-__version__ = "0.5.3"
+__version__ = "0.5.4"
```

### Comparing `sleepecg-0.5.3/sleepecg/_heartbeat_detection.c` & `sleepecg-0.5.4/sleepecg/_heartbeat_detection.c`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/classification.py` & `sleepecg-0.5.4/sleepecg/classification.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/classifiers/wrn-gru-mesa-weighted.zip` & `sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa-weighted.zip`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/classifiers/wrn-gru-mesa.zip` & `sleepecg-0.5.4/sleepecg/classifiers/wrn-gru-mesa.zip`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/classifiers/ws-gru-mesa.zip` & `sleepecg-0.5.4/sleepecg/classifiers/ws-gru-mesa.zip`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/config.py` & `sleepecg-0.5.4/sleepecg/config.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/feature_extraction.py` & `sleepecg-0.5.4/sleepecg/feature_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,23 @@
         "HF_norm",
         "LF_HF_ratio",
     ),
     "metadata": ("recording_start_time", "age", "gender", "weight"),
 }
 _FEATURE_ID_TO_GROUP = {id: group for group, ids in _FEATURE_GROUPS.items() for id in ids}
 
+_TIME_DOMAIN_EXPECTED_WARNING_MESSAGES = (
+    "All-NaN slice encountered",
+    "Degrees of freedom <= 0 for slice",
+    "divide by zero encountered in divide",
+    "divide by zero encountered in log10",
+    "invalid value encountered in sqrt",
+    "Mean of empty slice",
+)
+
 
 def _create_ragged_array(data: list[np.ndarray]) -> np.ndarray:
     """
     Convert a list of arrays with different lengths to a numpy array.
 
     Each element in `data` is a row in the resulting array. Rows shorter than the longest
     row will be padded with `np.nan`.
@@ -292,15 +301,14 @@
     rri: np.ndarray,
     rri_times: np.ndarray,
     stage_times: np.ndarray,
     lookback: int,
     lookforward: int,
     fs_rri_resample: float,
     max_nans: float,
-    feature_ids: list[str],
 ) -> np.ndarray:
     """
     Calculate seven frequency domain heart rate variability (HRV) features.
 
     Features are implemented according to [1]_.
 
     Parameters
@@ -318,54 +326,27 @@
         Forward extension of the analysis window from each sleep stage time.
     fs_rri_resample : float
         Frequency in Hz at which the RRI time series should be resampled before spectral
         analysis.
     max_nans : float
         Maximum fraction of NaNs in an analysis window, for which frequency features are
         computed. Should be a value between `0.0` and `1.0`.
-    feature_ids : list[str]
-        A list containing the identifiers of all features to be extracted. This does not
-        change the returned array. It is only used to avoid issuing a warning about the
-        analysis window being too short for some frequency range which is not requested.
 
     Returns
     -------
     np.ndarray
         Array of shape `(len(stage_times), 7)` containing the extracted frequency domain
         features.
 
     Notes
     -----
     .. [1] Task Force of the European Society of Cardiology. (1996). Heart rate variability:
        standards of measurement, physiological interpretation and clinical use. Circulation,
        93, 1043-1065. https://doi.org/10.1161/01.CIR.93.5.1043
     """
-    # The recording should last for at least 10 times the wavelength of the lower frequency
-    # bound of the investigated component.
-    window_time = lookback + lookforward
-    min_frequencies = {
-        "VLF": 0.0033,
-        "LF": 0.04,
-        "LF_norm": 0.04,
-        "HF": 0.15,
-        "HF_norm": 0.04,
-        "LF_HF_ratio": 0.04,
-    }
-
-    for name, min_frequency in min_frequencies.items():
-        min_window_time = 10 / min_frequency
-        if name not in feature_ids:
-            continue
-        if window_time < min_window_time:
-            msg = (
-                f"HR analysis window too short for estimating PSD for feature {name}. "
-                f"{min_window_time:.1f}s required, got {window_time}s"
-            )
-            warnings.warn(msg, category=RuntimeWarning)
-
     rri_interp_times = np.arange(
         start=stage_times[0] - lookback,
         stop=stage_times[-1] + lookforward,
         step=1 / fs_rri_resample,
     )
     rri_interp = interp1d(rri_times, rri, bounds_error=False)(rri_interp_times)
 
@@ -484,14 +465,48 @@
     duplicate_ids = {x for x in feature_ids if feature_ids.count(x) > 1}
     if duplicate_ids:
         warnings.warn(f"Duplicates in feature selection: {duplicate_ids}", RuntimeWarning)
 
     return list(required_groups), feature_ids, selected_cols
 
 
+def _check_frequencydomain_window_time(window_time: int, feature_ids: list[str]) -> None:
+    """
+    Warn if the duration of the analysis window is too short for a frequency domain feature.
+
+    Each window duration should be at least 10 times the wavelength of the lower frequency
+    bound of the investigated component.
+
+    Parameters
+    ----------
+    window_time : int
+        The duration of the analysis window.
+    feature_ids : list[str]
+        A list containing the identifiers of all features to be extracted.
+    """
+    min_frequencies = {
+        "VLF": 0.0033,
+        "LF": 0.04,
+        "LF_norm": 0.04,
+        "HF": 0.15,
+        "HF_norm": 0.04,
+        "LF_HF_ratio": 0.04,
+    }
+    for name, min_frequency in min_frequencies.items():
+        min_window_time = 10 / min_frequency
+        if name not in feature_ids:
+            continue
+        if window_time < min_window_time:
+            msg = (
+                f"HR analysis window too short for estimating PSD for feature {name}. "
+                f"{min_window_time:.1f}s required, got {window_time}s"
+            )
+            warnings.warn(msg, category=RuntimeWarning)
+
+
 def preprocess_rri(
     rri: np.ndarray,
     min_rri: Optional[float] = None,
     max_rri: Optional[float] = None,
 ) -> np.ndarray:
     """
     Replace invalid RRI samples with `np.nan`.
@@ -610,34 +625,36 @@
             max_rri=max_rri,
         )
         rri_times = record.heartbeat_times[1:]
 
     X = []
     for feature_group in required_groups:
         if feature_group == "hrv-time":
-            X.append(
-                _hrv_timedomain_features(
-                    rri,
-                    rri_times,
-                    stage_times,
-                    lookback,
-                    lookforward,
-                ),
-            )
+            with warnings.catch_warnings():
+                for message in _TIME_DOMAIN_EXPECTED_WARNING_MESSAGES:
+                    warnings.filterwarnings("ignore", message=message)
+                X.append(
+                    _hrv_timedomain_features(
+                        rri,
+                        rri_times,
+                        stage_times,
+                        lookback,
+                        lookforward,
+                    ),
+                )
         elif feature_group == "hrv-frequency":
             X.append(
                 _hrv_frequencydomain_features(
                     rri,
                     rri_times,
                     stage_times,
                     lookback,
                     lookforward,
                     fs_rri_resample,
                     max_nans,
-                    feature_ids,
                 ),
             )
         elif feature_group == "metadata":
             X.append(_metadata_features(record, num_stages))
     features = np.hstack(X)[:, col_indices]
 
     if record.sleep_stages is None or sleep_stage_duration == record.sleep_stage_duration:
@@ -732,14 +749,15 @@
         in `feature_selection` are expanded to all individual features they contain. The
         order matches the column order of the feature matrix.
     """
     if feature_selection is None:
         feature_selection = list(_FEATURE_GROUPS)
 
     required_groups, feature_ids, col_indices = _parse_feature_selection(feature_selection)
+    _check_frequencydomain_window_time(lookback + lookforward, feature_ids)
 
     # _extract_features_single has two return values, so the list returned by _parallel
     # needs to be unpacked
     Xy = _parallel(
         n_jobs,
         _extract_features_single,
         records,
```

### Comparing `sleepecg-0.5.3/sleepecg/heartbeats.py` & `sleepecg-0.5.4/sleepecg/heartbeats.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/io/ecg_readers.py` & `sleepecg-0.5.4/sleepecg/io/ecg_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,16 +254,14 @@
     Yields
     ------
     ECGRecord
         Each element in the generator is of type `ECGRecord` and contains the ECG signal
         (`.ecg`), sampling frequency (`.fs`), annotated beat indices (`.annotations`),
         `.lead`, and `.id`.
     """
-    import pandas as pd
-
     DB_URL = "https://berndporr.github.io/ECG-GUDB/experiment_data"
     EXPERIMENTS = ["sitting", "maths", "walking", "hand_bike", "jogging"]
     FS = 250
 
     if data_dir is None:
         data_dir = get_config("data_dir")
 
@@ -282,19 +280,26 @@
                     target_filepath = db_dir / experiment_subdir / tsv_filename
                     try:
                         checksum = _GUDB_MD5[f"{experiment_subdir}/{tsv_filename}"]
                     except KeyError:
                         pass  # file not available
                     else:
                         _download_file(ecg_file_url, target_filepath, checksum, "md5")
-            ecg_data = pd.read_csv(
-                db_dir / experiment_subdir / "ECG.tsv",
-                sep=" ",  # contrary to what .tsv suggests, the data is space-separated
-                names=["chest", "II", "III", "X", "Y", "Z"],
-            )
+            ecg_data = {
+                lead: signal
+                for lead, signal in zip(
+                    ("chest", "II", "III"),
+                    np.loadtxt(
+                        db_dir / experiment_subdir / "ECG.tsv",
+                        delimiter=" ",  # space-separated (contrary to what .tsv suggests)
+                        usecols=(0, 1, 2),
+                        unpack=True,
+                    ),
+                )
+            }
             annotations_chest_file = db_dir / experiment_subdir / "annotation_cs.tsv"
             if annotations_chest_file.is_file():
                 yield ECGRecord(
                     ecg=ecg_data["chest"].to_numpy(),
                     fs=FS,
                     annotation=np.loadtxt(annotations_chest_file, dtype=np.int32),
                     lead="chest",
```

### Comparing `sleepecg-0.5.3/sleepecg/io/gudb.py` & `sleepecg-0.5.4/sleepecg/io/gudb.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/io/nsrr.py` & `sleepecg-0.5.4/sleepecg/io/nsrr.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/io/physionet.py` & `sleepecg-0.5.4/sleepecg/io/physionet.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/io/sleep_readers.py` & `sleepecg-0.5.4/sleepecg/io/sleep_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,32 +582,32 @@
         xml_paths = sorted(annotations_dir.rglob(f"{records_pattern}-nsrr.xml"))
         requested_records = [str(file)[-27:-9] for file in xml_paths]
 
     subject_data = {}
 
     if any(r.startswith("shhs1") for r in requested_records):
         subject_data_file_shhs1 = next((db_dir / "datasets").glob("shhs1-dataset-*.csv"))
-        with open(subject_data_file_shhs1, newline="") as csvfile:
+        with open(subject_data_file_shhs1, newline="", encoding="windows-1252") as csvfile:
             reader = csv.DictReader(csvfile)
             for row in reader:
                 record_id = f"shhs1-{row['nsrrid']}"
                 subject_data[record_id] = SubjectData(
-                    gender=GENDER_MAPPING[row["gender"]],
-                    age=int(row["age_s1"]),
+                    gender=GENDER_MAPPING.get(row["gender"]),
+                    age=int(row["age_s1"]) if row["age_s1"] != "" else None,
                     weight=float(row["weight"]) if row["weight"] else None,
                 )
     if any(r.startswith("shhs2") for r in requested_records):
         subject_data_file_shhs2 = next((db_dir / "datasets").glob("shhs2-dataset-*.csv"))
-        with open(subject_data_file_shhs2, newline="") as csvfile:
+        with open(subject_data_file_shhs2, newline="", encoding="windows-1252") as csvfile:
             reader = csv.DictReader(csvfile)
             for row in reader:
                 record_id = f"shhs2-{row['nsrrid']}"
                 subject_data[record_id] = SubjectData(
-                    gender=GENDER_MAPPING[row["gender"]],
-                    age=int(row["age_s2"]),
+                    gender=GENDER_MAPPING.get(row["gender"]),
+                    age=int(row["age_s2"]) if row["age_s2"] != "" else None,
                     weight=None,  # subject weight was not recorded in shhs2
                 )
 
     for record_id in requested_records:
         heartbeats_file = heartbeats_dir / f"{record_id}.npy"
         if heartbeats_source == "annotation":
             rpoints_filename = f"{RPOINTS_DIRNAME}/{record_id}-rpoint.csv"
```

### Comparing `sleepecg-0.5.3/sleepecg/io/utils.py` & `sleepecg-0.5.4/sleepecg/io/utils.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/plot.py` & `sleepecg-0.5.4/sleepecg/plot.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/test/test_classification.py` & `sleepecg-0.5.4/sleepecg/test/test_classification.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/test/test_config.py` & `sleepecg-0.5.4/sleepecg/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/test/test_examples.py` & `sleepecg-0.5.4/sleepecg/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/test/test_feature_extraction.py` & `sleepecg-0.5.4/sleepecg/test/test_feature_extraction.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,26 +38,22 @@
         rri_times,
         stage_times,
         lookback=0,
         lookforward=30,
     )
     assert X_time.shape[1] == len(_FEATURE_GROUPS["hrv-time"])
 
-    # The analysis window (i.e. the sum of lookback and lookforward) must
-    # be at least 3030.3 seconds long to give useful PSD estimates in all
-    # frequency ranges, otherwise a warning is issued.
     X_frequency = _hrv_frequencydomain_features(
         rri,
         rri_times,
         stage_times,
-        lookback=3001,
+        lookback=0,
         lookforward=30,
         fs_rri_resample=4,
         max_nans=0,
-        feature_ids=_FEATURE_GROUPS["hrv-frequency"],
     )
     assert X_frequency.shape[1] == len(_FEATURE_GROUPS["hrv-frequency"])
 
 
 @pytest.mark.parametrize(
     ["metadata", "feature_vec"],
     [
```

### Comparing `sleepecg-0.5.3/sleepecg/test/test_heartbeat_detection.py` & `sleepecg-0.5.4/sleepecg/test/test_heartbeat_detection.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/test/test_heartbeats.py` & `sleepecg-0.5.4/sleepecg/test/test_heartbeats.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/test/test_sleep_readers.py` & `sleepecg-0.5.4/sleepecg/test/test_sleep_readers.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg/utils.py` & `sleepecg-0.5.4/sleepecg/utils.py`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg.egg-info/PKG-INFO` & `sleepecg-0.5.4/sleepecg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepecg
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for sleep stage classification using ECG data
 Home-page: https://github.com/cbrnr/sleepecg
 Author: Florian Hofer
 Author-email: hofaflo@gmail.com
 Maintainer: Clemens Brunner
 Maintainer-email: clemens.brunner@gmail.com
 License: BSD 3-Clause License
@@ -38,15 +38,14 @@
         
         Optional dependencies provide additional features:
         
         - [joblib](https://joblib.readthedocs.io/en/latest/) ≥ 1.0.0 (parallelized feature extraction)
         - [matplotlib](https://matplotlib.org/) ≥ 3.5.0 (plot ECG time courses, hypnograms, and confusion matrices)
         - [mne](https://mne.tools/stable/index.html) ≥ 1.0.0 (read data from [MESA](https://sleepdata.org/datasets/mesa) and [SHHS](https://sleepdata.org/datasets/shhs))
         - [numba](https://numba.pydata.org/) ≥ 0.55.0 (JIT-compiled heartbeat detector)
-        - [pandas](https://pandas.pydata.org/) ≥ 1.4.0 (read data from [GUDB](https://berndporr.github.io/ECG-GUDB))
         - [tensorflow](https://www.tensorflow.org/) ≥ 2.7.0 (sleep stage classification with Keras models)
         - [wfdb](https://github.com/MIT-LCP/wfdb-python/) ≥ 3.4.0 (read data from [SLPDB](https://physionet.org/content/slpdb), [MITDB](https://physionet.org/content/mitdb), and [LTDB](https://physionet.org/content/ltdb))
         
         ### Installation
         SleepECG is available on PyPI and can be installed with [pip](https://pip.pypa.io/en/stable/):
         
         ```
```

### Comparing `sleepecg-0.5.3/sleepecg.egg-info/SOURCES.txt` & `sleepecg-0.5.4/sleepecg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sleepecg-0.5.3/sleepecg.egg-info/requires.txt` & `sleepecg-0.5.4/sleepecg.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 flake8>=4.0.0
 joblib>=1.0.0
 matplotlib>=3.5.0
 mkdocs-material>=8.4.0
 mkdocstrings-python>=0.7.1
 mne>=1.0.0
 mypy>=0.991
-pandas>=1.4.0
 pre-commit>=2.13.0
 pyEDFlib>=0.1.25
 pytest>=6.2.0
 setuptools>=56.0.0
 sphinx>=4.1.0
 wfdb>=3.4.0
 
@@ -37,13 +36,12 @@
 mkdocs-material>=8.4.0
 mkdocstrings-python>=0.8.2
 
 [full]
 joblib>=1.0.0
 matplotlib>=3.5.0
 mne>=1.0.0
-pandas>=1.4.0
 wfdb>=3.4.0
 
 [full:python_version < "3.11"]
 numba>=0.55.0
 tensorflow>=2.7.0
```

