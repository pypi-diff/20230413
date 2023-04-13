# Comparing `tmp/vectorlab-1.0.0.tar.gz` & `tmp/vectorlab-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorlab-1.0.0.tar", last modified: Tue Oct 18 12:27:26 2022, max compression
+gzip compressed data, was "vectorlab-1.0.1.tar", last modified: Thu Apr 13 14:55:08 2023, max compression
```

## Comparing `vectorlab-1.0.0.tar` & `vectorlab-1.0.1.tar`

### file list

```diff
@@ -1,76 +1,99 @@
--rw-r--r--   0        0        0     1544 2022-10-18 12:26:16.623061 vectorlab-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2200 2022-10-18 12:26:16.623486 vectorlab-1.0.0/README.md
--rw-r--r--   0        0        0     1281 2022-10-18 12:26:16.625168 vectorlab-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      255 2022-10-18 12:26:16.627109 vectorlab-1.0.0/vectorlab/__init__.py
--rw-r--r--   0        0        0    11484 2022-10-18 12:26:16.627411 vectorlab-1.0.0/vectorlab/base.py
--rw-r--r--   0        0        0      113 2022-10-18 12:26:16.627580 vectorlab-1.0.0/vectorlab/data/__init__.py
--rw-r--r--   0        0        0     1129 2022-10-18 12:26:16.627827 vectorlab-1.0.0/vectorlab/data/_argument_generator.py
--rw-r--r--   0        0        0     1308 2022-10-18 12:26:16.628180 vectorlab-1.0.0/vectorlab/data/_data_generator.py
--rw-r--r--   0        0        0       76 2022-10-18 12:26:16.628420 vectorlab-1.0.0/vectorlab/data/dataloader/__init__.py
--rw-r--r--   0        0        0     3544 2022-10-18 12:26:16.628668 vectorlab-1.0.0/vectorlab/data/dataloader/_torch_dataloader.py
--rw-r--r--   0        0        0     4867 2022-10-18 12:26:16.628920 vectorlab-1.0.0/vectorlab/data/dataloader/_torch_geometric_dataloader.py
--rw-r--r--   0        0        0     1662 2022-10-18 12:26:16.629153 vectorlab-1.0.0/vectorlab/data/dataloader/tests/test_torch_dataloader.py
--rw-r--r--   0        0        0       57 2022-10-18 12:26:16.629359 vectorlab-1.0.0/vectorlab/data/dataset/__init__.py
--rw-r--r--   0        0        0     6253 2022-10-18 12:26:16.629590 vectorlab-1.0.0/vectorlab/data/dataset/_torch_dataset.py
--rw-r--r--   0        0        0    31883 2022-10-18 12:26:16.630206 vectorlab-1.0.0/vectorlab/data/dataset/_ts_dataset.py
--rw-r--r--   0        0        0      385 2022-10-18 12:26:16.630668 vectorlab-1.0.0/vectorlab/data/tests/test_argument_generator.py
--rw-r--r--   0        0        0      533 2022-10-18 12:26:16.648196 vectorlab-1.0.0/vectorlab/data/tests/test_data_generator.py
--rw-r--r--   0        0        0       23 2022-10-18 12:26:16.648537 vectorlab-1.0.0/vectorlab/ensemble/__init__.py
--rw-r--r--   0        0        0     3677 2022-10-18 12:26:16.648854 vectorlab-1.0.0/vectorlab/ensemble/_voting.py
--rw-r--r--   0        0        0     4070 2022-10-18 12:26:16.649089 vectorlab-1.0.0/vectorlab/ensemble/tests/test_ensemble_voting.py
--rw-r--r--   0        0        0       70 2022-10-18 12:26:16.649260 vectorlab-1.0.0/vectorlab/graph/__init__.py
--rw-r--r--   0        0        0    11604 2022-10-18 12:26:16.649456 vectorlab-1.0.0/vectorlab/graph/_generator.py
--rw-r--r--   0        0        0    15921 2022-10-18 12:26:16.649921 vectorlab-1.0.0/vectorlab/graph/_utils.py
--rw-r--r--   0        0        0     1169 2022-10-18 12:26:16.650118 vectorlab-1.0.0/vectorlab/graph/tests/test_graph_generator.py
--rw-r--r--   0        0        0     6818 2022-10-18 12:26:16.650417 vectorlab-1.0.0/vectorlab/graph/tests/test_graph_utils.py
--rw-r--r--   0        0        0       68 2022-10-18 12:26:16.650716 vectorlab-1.0.0/vectorlab/graph/walking/__init__.py
--rw-r--r--   0        0        0     1920 2022-10-18 12:26:16.650914 vectorlab-1.0.0/vectorlab/graph/walking/_bfs.py
--rw-r--r--   0        0        0     1869 2022-10-18 12:26:16.651263 vectorlab-1.0.0/vectorlab/graph/walking/_dfs.py
--rw-r--r--   0        0        0     1275 2022-10-18 12:26:16.651449 vectorlab-1.0.0/vectorlab/graph/walking/_random_walk.py
--rw-r--r--   0        0        0     2235 2022-10-18 12:26:16.651741 vectorlab-1.0.0/vectorlab/graph/walking/tests/test_graph_walking.py
--rw-r--r--   0        0        0       23 2022-10-18 12:26:16.652169 vectorlab-1.0.0/vectorlab/metrics/__init__.py
--rw-r--r--   0        0        0       87 2022-10-18 12:26:16.652455 vectorlab-1.0.0/vectorlab/metrics/pairwise/__init__.py
--rw-r--r--   0        0        0     8721 2022-10-18 12:26:16.652876 vectorlab-1.0.0/vectorlab/metrics/pairwise/_dtw.py
--rw-r--r--   0        0        0     3423 2022-10-18 12:26:16.653142 vectorlab-1.0.0/vectorlab/metrics/pairwise/_kl_div.py
--rw-r--r--   0        0        0     1183 2022-10-18 12:26:16.653383 vectorlab-1.0.0/vectorlab/metrics/pairwise/_lp_norm.py
--rw-r--r--   0        0        0     3206 2022-10-18 12:26:16.653655 vectorlab-1.0.0/vectorlab/metrics/pairwise/_sbd.py
--rw-r--r--   0        0        0     2560 2022-10-18 12:26:16.653944 vectorlab-1.0.0/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py
--rw-r--r--   0        0        0       45 2022-10-18 12:26:16.654240 vectorlab-1.0.0/vectorlab/optimize/__init__.py
--rw-r--r--   0        0        0     6294 2022-10-18 12:26:16.654546 vectorlab-1.0.0/vectorlab/optimize/_estimate.py
--rw-r--r--   0        0        0    16484 2022-10-18 12:26:16.654886 vectorlab-1.0.0/vectorlab/optimize/_qap.py
--rw-r--r--   0        0        0     2521 2022-10-18 12:26:16.655150 vectorlab-1.0.0/vectorlab/optimize/tests/test_estimate.py
--rw-r--r--   0        0        0       69 2022-10-18 12:26:16.655369 vectorlab-1.0.0/vectorlab/plot/__init__.py
--rw-r--r--   0        0        0      412 2022-10-18 12:26:16.655569 vectorlab-1.0.0/vectorlab/plot/_helper.py
--rw-r--r--   0        0        0     2980 2022-10-18 12:26:16.655760 vectorlab-1.0.0/vectorlab/plot/_palettes.py
--rw-r--r--   0        0        0    16083 2022-10-18 12:26:16.655991 vectorlab-1.0.0/vectorlab/plot/_plot.py
--rw-r--r--   0        0        0      732 2022-10-18 12:26:16.656214 vectorlab-1.0.0/vectorlab/plot/tests/test_plot.py
--rw-r--r--   0        0        0       76 2022-10-18 12:26:16.656335 vectorlab-1.0.0/vectorlab/series/__init__.py
--rw-r--r--   0        0        0     8732 2022-10-18 12:26:16.656556 vectorlab-1.0.0/vectorlab/series/_preprocessing.py
--rw-r--r--   0        0        0     2796 2022-10-18 12:26:16.656755 vectorlab-1.0.0/vectorlab/series/_utils.py
--rw-r--r--   0        0        0      116 2022-10-18 12:26:16.656962 vectorlab-1.0.0/vectorlab/series/smoothing/__init__.py
--rw-r--r--   0        0        0     6309 2022-10-18 12:26:16.657160 vectorlab-1.0.0/vectorlab/series/smoothing/_arima.py
--rw-r--r--   0        0        0     7455 2022-10-18 12:26:16.657360 vectorlab-1.0.0/vectorlab/series/smoothing/_holt_winters.py
--rw-r--r--   0        0        0    12395 2022-10-18 12:26:16.657559 vectorlab-1.0.0/vectorlab/series/smoothing/_moving_average.py
--rw-r--r--   0        0        0     6854 2022-10-18 12:26:16.657719 vectorlab-1.0.0/vectorlab/series/smoothing/_spectral_residual.py
--rw-r--r--   0        0        0     2333 2022-10-18 12:26:16.657930 vectorlab-1.0.0/vectorlab/series/smoothing/tests/test_series_smoothing.py
--rw-r--r--   0        0        0     1520 2022-10-18 12:26:16.658161 vectorlab-1.0.0/vectorlab/series/tests/test_series_preprocessing.py
--rw-r--r--   0        0        0       77 2022-10-18 12:26:16.658368 vectorlab-1.0.0/vectorlab/stats/__init__.py
--rw-r--r--   0        0        0    15478 2022-10-18 12:26:16.658637 vectorlab-1.0.0/vectorlab/stats/_deg_graph.py
--rw-r--r--   0        0        0    18260 2022-10-18 12:26:16.658927 vectorlab-1.0.0/vectorlab/stats/_freq_tree.py
--rw-r--r--   0        0        0    14207 2022-10-18 12:26:16.659213 vectorlab-1.0.0/vectorlab/stats/_t_digest.py
--rw-r--r--   0        0        0     1312 2022-10-18 12:26:16.659497 vectorlab-1.0.0/vectorlab/stats/tests/test_deg_graph.py
--rw-r--r--   0        0        0     1311 2022-10-18 12:26:16.659727 vectorlab-1.0.0/vectorlab/stats/tests/test_freq_tree.py
--rw-r--r--   0        0        0     1310 2022-10-18 12:26:16.659921 vectorlab-1.0.0/vectorlab/stats/tests/test_t_digest.py
--rw-r--r--   0        0        0      110 2022-10-18 12:26:16.660122 vectorlab-1.0.0/vectorlab/utils/__init__.py
--rw-r--r--   0        0        0     9958 2022-10-18 12:26:16.660338 vectorlab-1.0.0/vectorlab/utils/_check.py
--rw-r--r--   0        0        0      617 2022-10-18 12:26:16.660508 vectorlab-1.0.0/vectorlab/utils/_env.py
--rw-r--r--   0        0        0     2026 2022-10-18 12:26:16.660689 vectorlab-1.0.0/vectorlab/utils/_loading.py
--rw-r--r--   0        0        0     2707 2022-10-18 12:26:16.660882 vectorlab-1.0.0/vectorlab/utils/_parser.py
--rw-r--r--   0        0        0     5081 2022-10-18 12:26:16.661155 vectorlab-1.0.0/vectorlab/utils/_time.py
--rw-r--r--   0        0        0     1123 2022-10-18 12:26:16.661286 vectorlab-1.0.0/vectorlab/utils/tests/test_time.py
--rw-r--r--   0        0        0       45 2022-10-18 12:26:16.661507 vectorlab-1.0.0/vectorlab/vector/__init__.py
--rw-r--r--   0        0        0    11924 2022-10-18 12:26:16.661786 vectorlab-1.0.0/vectorlab/vector/_array.py
--rw-r--r--   0        0        0     2933 2022-10-18 12:26:16.662034 vectorlab-1.0.0/vectorlab/vector/_tensor.py
--rw-r--r--   0        0        0     4232 2022-10-18 12:26:16.662172 vectorlab-1.0.0/vectorlab/vector/tests/test_array.py
--rw-r--r--   0        0        0     1217 2022-10-18 12:26:16.662393 vectorlab-1.0.0/vectorlab/vector/tests/test_tensor.py
--rw-r--r--   0        0        0     3691 1970-01-01 00:00:00.000000 vectorlab-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2022-10-19 08:15:02.000000 vectorlab-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2212 2023-04-13 14:52:09.284268 vectorlab-1.0.1/README.md
+-rw-r--r--   0        0        0     1331 2023-04-13 14:52:09.292262 vectorlab-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8196 2022-11-24 06:03:57.630870 vectorlab-1.0.1/vectorlab/.DS_Store
+-rw-r--r--   0        0        0      272 2023-04-13 14:53:42.990467 vectorlab-1.0.1/vectorlab/__init__.py
+-rw-r--r--   0        0        0    11168 2023-04-13 14:52:09.294277 vectorlab-1.0.1/vectorlab/base.py
+-rw-r--r--   0        0        0      113 2022-10-25 03:41:44.000000 vectorlab-1.0.1/vectorlab/data/__init__.py
+-rw-r--r--   0        0        0     1129 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/_argument_generator.py
+-rw-r--r--   0        0        0     1308 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/_data_generator.py
+-rw-r--r--   0        0        0       76 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/dataloader/__init__.py
+-rw-r--r--   0        0        0     3809 2023-04-13 14:52:09.294877 vectorlab-1.0.1/vectorlab/data/dataloader/_torch_dataloader.py
+-rw-r--r--   0        0        0     4801 2023-04-13 14:52:09.295769 vectorlab-1.0.1/vectorlab/data/dataloader/_torch_geometric_dataloader.py
+-rw-r--r--   0        0        0     1662 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/dataloader/tests/test_torch_dataloader.py
+-rw-r--r--   0        0        0       57 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/dataset/__init__.py
+-rw-r--r--   0        0        0     6196 2023-04-13 14:52:09.296470 vectorlab-1.0.1/vectorlab/data/dataset/_torch_dataset.py
+-rw-r--r--   0        0        0    31856 2023-04-13 14:52:09.297053 vectorlab-1.0.1/vectorlab/data/dataset/_ts_dataset.py
+-rw-r--r--   0        0        0      385 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/tests/test_argument_generator.py
+-rw-r--r--   0        0        0      533 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/data/tests/test_data_generator.py
+-rw-r--r--   0        0        0       23 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/ensemble/__init__.py
+-rw-r--r--   0        0        0     3677 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/ensemble/_voting.py
+-rw-r--r--   0        0        0     4070 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/ensemble/tests/test_ensemble_voting.py
+-rw-r--r--   0        0        0       70 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/__init__.py
+-rw-r--r--   0        0        0    11604 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/_generator.py
+-rw-r--r--   0        0        0    15921 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/_utils.py
+-rw-r--r--   0        0        0     1169 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/tests/test_graph_generator.py
+-rw-r--r--   0        0        0     6818 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/tests/test_graph_utils.py
+-rw-r--r--   0        0        0       68 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/__init__.py
+-rw-r--r--   0        0        0     1920 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/_bfs.py
+-rw-r--r--   0        0        0     1869 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/_dfs.py
+-rw-r--r--   0        0        0     1275 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/_random_walk.py
+-rw-r--r--   0        0        0     2235 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/graph/walking/tests/test_graph_walking.py
+-rw-r--r--   0        0        0       23 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/__init__.py
+-rw-r--r--   0        0        0       87 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/__init__.py
+-rw-r--r--   0        0        0     8721 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/_dtw.py
+-rw-r--r--   0        0        0     3329 2023-04-13 14:52:09.297651 vectorlab-1.0.1/vectorlab/metrics/pairwise/_kl_div.py
+-rw-r--r--   0        0        0     1183 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/_lp_norm.py
+-rw-r--r--   0        0        0     3206 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/metrics/pairwise/_sbd.py
+-rw-r--r--   0        0        0     2365 2023-04-13 14:52:09.298082 vectorlab-1.0.1/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py
+-rw-r--r--   0        0        0      119 2023-04-13 14:52:09.298380 vectorlab-1.0.1/vectorlab/nn/__init__.py
+-rw-r--r--   0        0        0     4305 2023-04-13 14:52:09.298680 vectorlab-1.0.1/vectorlab/nn/_earlystopping.py
+-rw-r--r--   0        0        0     6318 2023-04-13 14:52:09.299021 vectorlab-1.0.1/vectorlab/nn/_resolver.py
+-rw-r--r--   0        0        0    46446 2023-04-13 14:52:09.299466 vectorlab-1.0.1/vectorlab/nn/explorer.py
+-rw-r--r--   0        0        0     2906 2023-04-13 14:52:09.299821 vectorlab-1.0.1/vectorlab/nn/functional.py
+-rw-r--r--   0        0        0      201 2023-04-13 14:52:09.300127 vectorlab-1.0.1/vectorlab/nn/models/__init__.py
+-rw-r--r--   0        0        0    18081 2023-04-13 14:52:09.300609 vectorlab-1.0.1/vectorlab/nn/models/_autoencoder.py
+-rw-r--r--   0        0        0     2303 2023-04-13 14:52:09.300957 vectorlab-1.0.1/vectorlab/nn/models/_basic_gnn.py
+-rw-r--r--   0        0        0     3679 2023-04-13 14:52:09.301388 vectorlab-1.0.1/vectorlab/nn/models/_classifier.py
+-rw-r--r--   0        0        0    11804 2023-04-13 14:52:09.301831 vectorlab-1.0.1/vectorlab/nn/models/_decoder.py
+-rw-r--r--   0        0        0    32841 2023-04-13 14:52:09.302107 vectorlab-1.0.1/vectorlab/nn/models/_encoder.py
+-rw-r--r--   0        0        0     2571 2023-04-13 14:52:09.302342 vectorlab-1.0.1/vectorlab/nn/models/_gnn_decoder.py
+-rw-r--r--   0        0        0     7574 2023-04-13 14:52:09.303205 vectorlab-1.0.1/vectorlab/nn/models/_mlp.py
+-rw-r--r--   0        0        0     5855 2023-04-13 14:52:09.303721 vectorlab-1.0.1/vectorlab/nn/models/_seq2seq.py
+-rw-r--r--   0        0        0     2155 2023-04-13 14:52:09.304252 vectorlab-1.0.1/vectorlab/nn/models/tests/test_decoder.py
+-rw-r--r--   0        0        0     2255 2023-04-13 14:52:09.304596 vectorlab-1.0.1/vectorlab/nn/models/tests/test_encoder.py
+-rw-r--r--   0        0        0     1276 2023-04-13 14:52:09.304912 vectorlab-1.0.1/vectorlab/nn/models/tests/test_seq2seq.py
+-rw-r--r--   0        0        0       44 2023-04-13 14:52:09.306267 vectorlab-1.0.1/vectorlab/nn/modules/__init__.py
+-rw-r--r--   0        0        0     1529 2023-04-13 14:52:09.306669 vectorlab-1.0.1/vectorlab/nn/modules/gnn_loss.py
+-rw-r--r--   0        0        0     2556 2023-04-13 14:52:09.306963 vectorlab-1.0.1/vectorlab/nn/modules/loss.py
+-rw-r--r--   0        0        0      743 2023-04-13 14:52:09.307274 vectorlab-1.0.1/vectorlab/nn/tests/test_explorer.py
+-rw-r--r--   0        0        0      873 2023-04-13 14:52:09.307569 vectorlab-1.0.1/vectorlab/nn/tests/test_functional.py
+-rw-r--r--   0        0        0       45 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/optimize/__init__.py
+-rw-r--r--   0        0        0     6294 2023-04-13 14:52:09.308010 vectorlab-1.0.1/vectorlab/optimize/_estimate.py
+-rw-r--r--   0        0        0    16484 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/optimize/_qap.py
+-rw-r--r--   0        0        0     2521 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/optimize/tests/test_estimate.py
+-rw-r--r--   0        0        0       69 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/__init__.py
+-rw-r--r--   0        0        0      412 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/_helper.py
+-rw-r--r--   0        0        0     2980 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/_palettes.py
+-rw-r--r--   0        0        0    16083 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/_plot.py
+-rw-r--r--   0        0        0      732 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/plot/tests/test_plot.py
+-rw-r--r--   0        0        0       76 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/__init__.py
+-rw-r--r--   0        0        0     8732 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/_preprocessing.py
+-rw-r--r--   0        0        0     2796 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/_utils.py
+-rw-r--r--   0        0        0      116 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/smoothing/__init__.py
+-rw-r--r--   0        0        0     6298 2023-04-13 14:52:09.308452 vectorlab-1.0.1/vectorlab/series/smoothing/_arima.py
+-rw-r--r--   0        0        0     7438 2023-04-13 14:52:09.308890 vectorlab-1.0.1/vectorlab/series/smoothing/_holt_winters.py
+-rw-r--r--   0        0        0    12319 2023-04-13 14:52:09.309332 vectorlab-1.0.1/vectorlab/series/smoothing/_moving_average.py
+-rw-r--r--   0        0        0     6832 2023-04-13 14:52:09.310075 vectorlab-1.0.1/vectorlab/series/smoothing/_spectral_residual.py
+-rw-r--r--   0        0        0     2333 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/smoothing/tests/test_series_smoothing.py
+-rw-r--r--   0        0        0     1520 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/series/tests/test_series_preprocessing.py
+-rw-r--r--   0        0        0       77 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/__init__.py
+-rw-r--r--   0        0        0    15478 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/_deg_graph.py
+-rw-r--r--   0        0        0    18242 2023-04-13 14:52:09.310614 vectorlab-1.0.1/vectorlab/stats/_freq_tree.py
+-rw-r--r--   0        0        0    14207 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/_t_digest.py
+-rw-r--r--   0        0        0     1312 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/tests/test_deg_graph.py
+-rw-r--r--   0        0        0     1311 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/tests/test_freq_tree.py
+-rw-r--r--   0        0        0     1310 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/stats/tests/test_t_digest.py
+-rw-r--r--   0        0        0      110 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/__init__.py
+-rw-r--r--   0        0        0     9958 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_check.py
+-rw-r--r--   0        0        0      617 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_env.py
+-rw-r--r--   0        0        0     2026 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_loading.py
+-rw-r--r--   0        0        0     2707 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/_parser.py
+-rw-r--r--   0        0        0     5089 2023-04-13 14:52:09.311123 vectorlab-1.0.1/vectorlab/utils/_time.py
+-rw-r--r--   0        0        0     1123 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/utils/tests/test_time.py
+-rw-r--r--   0        0        0       45 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/__init__.py
+-rw-r--r--   0        0        0    11924 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/_array.py
+-rw-r--r--   0        0        0     2933 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/_tensor.py
+-rw-r--r--   0        0        0     4140 2023-04-13 14:52:09.311629 vectorlab-1.0.1/vectorlab/vector/tests/test_array.py
+-rw-r--r--   0        0        0     1217 2022-10-19 08:15:02.000000 vectorlab-1.0.1/vectorlab/vector/tests/test_tensor.py
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 vectorlab-1.0.1/PKG-INFO
```

### Comparing `vectorlab-1.0.0/LICENSE.txt` & `vectorlab-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/README.md` & `vectorlab-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/Kr4t0n/vectorlab/main/static/logo.png"/>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/vectorlab)](https://pypi.org/project/vectorlab/)
 [![Package Status](https://img.shields.io/pypi/status/vectorlab)](https://pypi.org/project/vectorlab/)
-[![Testing Status](https://img.shields.io/github/workflow/status/Kr4t0n/vectorlab/Testing?label=Testing&logo=github)](https://github.com/Kr4t0n/vectorlab/actions/workflows/testing.yml)
+[![Testing Status](https://img.shields.io/github/actions/workflow/status/Kr4t0n/vectorlab/testing.yml?label=Testing&logo=github)](https://github.com/Kr4t0n/vectorlab/actions/workflows/testing.yml)
 [![Coverage](https://codecov.io/github/Kr4t0n/vectorlab/coverage.svg?branch=dev-feat)](https://codecov.io/gh/Kr4t0n/vectorlab)
 [![License](https://img.shields.io/pypi/l/vectorlab)](https://github.com/Kr4t0n/vectorlab/blob/main/LICENSE.txt)
 [![Python Version](https://img.shields.io/pypi/pyversions/vectorlab)](https://pypi.org/project/vectorlab/)
 
 VectorLab is a library to help solve scientific and engineering problems of mathematics and machine learning. It is built upon various fabulous softwares and tries to fill the gap when playing around with those softwares.
 
 VectorLab consists of many modules including data generation, graph processing, series processing, statistics, optimization, ensemble mechanism and more.
```

### Comparing `vectorlab-1.0.0/pyproject.toml` & `vectorlab-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     "scikit-learn>=1.1.2",
     "matplotlib>=3.5.3",
     "seaborn>=0.11.2",
     "pillow>=9.2.0",
     "pytz>=2022.2.1",
     "dill>=0.3.5.1",
     "halo>=0.0.31",
-    "pyyaml>=6.0"
+    "pyyaml>=6.0",
+    "torchinfo>=1.6.3",
+    "tensorboard>=2.6.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1.2",
     "pytest-cov>=3.0.0",
     "pytest-repeat>=0.9.1",
```

### Comparing `vectorlab-1.0.0/vectorlab/base.py` & `vectorlab-1.0.1/vectorlab/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         A Python object represents the entity.
     value_ : int, float, object
         The value to be compared.
     """
 
     def __init__(self, key, value):
 
-        super(KVNode, self).__init__()
+        super().__init__()
 
         self.key_ = key
         self.value_ = value
 
         return
 
     def __lt__(self, other):
@@ -104,17 +104,15 @@
         return (self.key_ == other.key_) & (self.value_ == other.value_)
 
     def __hash__(self):
         return hash(self.__repr__())
 
     def __repr__(self):
 
-        print_str = 'Key: {}, Value: {}'.format(
-            self.key_, self.value_
-        )
+        print_str = f'Key: {self.key_}, Value: {self.value_}'
 
         return print_str
 
 
 class Stack(SLMixin):
     r"""The base Stack class
 
@@ -135,15 +133,15 @@
         The stack to store elements.
     dtype_ : type
         The element type desired to store in the stack.
     """
 
     def __init__(self, dtype=None):
 
-        super(Stack, self).__init__()
+        super().__init__()
 
         self.stack_ = []
         self.dtype_ = dtype
 
         return
 
     def push(self, element):
@@ -160,19 +158,17 @@
             When the stack's dtype is not None and new element
             type is not equal to it, a ValueError is raised.
         """
 
         if self.dtype_ is not None:
             if not isinstance(element, self.dtype_):
                 raise ValueError(
-                    'New element type is not allowed. '
-                    'New element type is {}, allowed type is {}'.format(
-                        type(element),
-                        self.dtype_
-                    )
+                    f'New element type is not allowed. '
+                    f'New element type is {type(element)}, '
+                    f'allowed type is {self.dtype_}.'
                 )
 
         self.stack_.append(element)
 
         return
 
     def pop(self):
@@ -235,15 +231,15 @@
         The queue to store elements.
     dtype_ : type
         The element type desired to store in the queue.
     """
 
     def __init__(self, dtype=None):
 
-        super(Queue, self).__init__()
+        super().__init__()
 
         self.queue_ = []
         self.dtype_ = dtype
 
         return
 
     def push(self, element):
@@ -260,19 +256,17 @@
             When the queue's dtype is not None and new element
             type is not equal to it, a ValueError is raised.
         """
 
         if self.dtype_ is not None:
             if not isinstance(element, self.dtype_):
                 raise ValueError(
-                    'New element type is not allowed. '
-                    'New element type is {}, allowed type is {}'.format(
-                        type(element),
-                        self.dtype_
-                    )
+                    f'New element type is not allowed. '
+                    f'New element type is {type(element)}, '
+                    f'allowed type is {self.dtype_}.'
                 )
 
         self.queue_.append(element)
 
         return
 
     def pop(self):
@@ -348,21 +342,18 @@
         are not equal, a ValueError will be raised.
     """
 
     def __init__(self, n_attrs, attrs):
 
         if attrs is not None and len(attrs) != n_attrs:
             raise ValueError(
-                'The number of attributes and the number of provided '
-                'attribute names are not equal. The number of attributes '
-                'is {} and the number of provided attribute '
-                'names is {}.'.format(
-                    n_attrs,
-                    len(attrs)
-                )
+                f'The number of attributes and the number of provided '
+                f'attribute names are not equal. The number of attributes '
+                f'is {n_attrs} and the number of provided attribute '
+                f'names is {len(attrs)}.'
             )
 
         self.n_attrs_ = n_attrs
 
         self.attrs_ = {attr: idx for idx, attr in enumerate(attrs)}
         self.attrs_stats_ = np.zeros(self.n_attrs_, dtype=np.float_)
 
@@ -411,21 +402,18 @@
             isinstance(attrs_stats, np.ndarray)
         ):
 
             attrs_stats = np.array(attrs_stats)
 
             if self.attrs_stats_.shape != attrs_stats.shape:
                 raise ValueError(
-                    'The number of adding attributes statistics is different '
-                    'from the number of elements initialized. '
-                    'The accumulator contains {} elements '
-                    'but provided with {}.'.format(
-                        self.n_attrs_,
-                        attrs_stats.shape[0]
-                    )
+                    f'The number of adding attributes statistics is different '
+                    f'from the number of elements initialized. '
+                    f'The accumulator contains {self.n_attrs_} elements '
+                    f'but provided with {attrs_stats.shape[0]}.'
                 )
 
             self.attrs_stats_ += attrs_stats
 
         if isinstance(attrs_stats, dict):
 
             attrs_stats_ = np.zeros(self.n_attrs_, dtype=np.float_)
```

### Comparing `vectorlab-1.0.0/vectorlab/data/_argument_generator.py` & `vectorlab-1.0.1/vectorlab/data/_argument_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/data/_data_generator.py` & `vectorlab-1.0.1/vectorlab/data/_data_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/data/dataloader/_torch_dataloader.py` & `vectorlab-1.0.1/vectorlab/data/dataloader/_torch_dataloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -83,43 +83,57 @@
     PadSeqDataLoader inherits from original Dataloader,
     while using a customized pad sequence collate function.
 
     Parameters
     ----------
     batch_first : bool
         Whether pad sequence in a batch first manner or not.
+
+    Attributes
+    ----------
+    batch_first : bool
+        Whether pad sequence in a batch first manner or not.
     """
 
     def __init__(self, *args, batch_first=False, **kwargs):
 
-        super(PadSeqDataLoader, self).__init__(
+        super().__init__(
             *args, **kwargs,
             collate_fn=lambda batch: pad_sequence_collate(
                 batch, batch_first=batch_first
             )
         )
 
+        self.batch_first = batch_first
+
         return
 
 
 class PadSeqsDataLoader(DataLoader):
     r"""Load data in a padding manner.
 
     PadSeqsDataLoader inherits from original Dataloader,
     while using a customized pad sequence collate function.
 
     Parameters
     ----------
     batch_first : bool
         Whether pad sequence in a batch first manner or not.
+
+    Attributes
+    ----------
+    batch_first : bool
+        Whether pad sequence in a batch first manner or not.
     """
 
     def __init__(self, *args, batch_first=False, **kwargs):
 
-        super(PadSeqsDataLoader, self).__init__(
+        super().__init__(
             *args, **kwargs,
             collate_fn=lambda batch: pad_sequences_collate(
                 batch, batch_first=batch_first
             )
         )
 
+        self.batch_first = batch_first
+
         return
```

### Comparing `vectorlab-1.0.0/vectorlab/data/dataloader/_torch_geometric_dataloader.py` & `vectorlab-1.0.1/vectorlab/data/dataloader/_torch_geometric_dataloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     NodeDataLoader inherits from original DataLoader,
     while using a customized collate function.
     """
 
     def __init__(self, *args, **kwargs):
 
-        super(NodeDataLoader, self).__init__(
+        super().__init__(
             *args, **kwargs,
             collate_fn=gnn_node_collate
         )
 
         return
 
 
@@ -158,15 +158,15 @@
 
     GraphDataLoader inherits from original DataLoader,
     while using a customized collate function.
     """
 
     def __init__(self, *args, **kwargs):
 
-        super(GraphDataLoader, self).__init__(
+        super().__init__(
             *args, **kwargs,
             collate_fn=gnn_graph_collate
         )
 
         return
 
 
@@ -183,15 +183,15 @@
         The percentage nodes to be masked.
     mask_method : str, optional
         The method to replace the masked node features.
     """
 
     def __init__(self, *args, p=0.5, mask_method='zeros', **kwargs):
 
-        super(MaskGraphDataLoader, self).__init__(
+        super().__init__(
             *args, **kwargs,
             collate_fn=lambda batch: mask_gnn_collate(
                 batch, p=p, mask_method=mask_method
             )
         )
 
         return
```

### Comparing `vectorlab-1.0.0/vectorlab/data/dataloader/tests/test_torch_dataloader.py` & `vectorlab-1.0.1/vectorlab/data/dataloader/tests/test_torch_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/data/dataset/_torch_dataset.py` & `vectorlab-1.0.1/vectorlab/data/dataset/_torch_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         The number of data stored in MultiDataset.
     tensors_ : tuple
         The multiple tensors stored in MultiDataset.
     """
 
     def __init__(self, *args):
 
-        super(MultiDataset, self).__init__()
+        super().__init__()
 
         tensors = tuple(_check_tensor(arg) for arg in args)
 
         assert all(
             tensors[0].size(0) == tensor.size(0) for tensor in tensors
         ), 'Size mismatch between tensors.'
 
@@ -107,15 +107,15 @@
         A series of transform(s) applied over the given image(s).
     len_ : int
         The number of data stored in ImageDataset.
     """
 
     def __init__(self, root, annotation, transform=None):
 
-        super(ImageDataset, self).__init__()
+        super().__init__()
 
         self.root_ = root
         self.annotations_ = pd.read_csv(annotation)
         self.transform_ = transform
 
         self.len_ = len(self.annotations_)
 
@@ -193,15 +193,15 @@
         The output sequences.
     len_ : int
         The number of sequences stored in SequenceDataset.
     """
 
     def __init__(self, input_seq, output_seq):
 
-        super(SequenceDataset, self).__init__()
+        super().__init__()
 
         assert len(input_seq) == len(output_seq)
 
         self.input_seq_ = tuple(_check_tensor(_) for _ in input_seq)
         self.output_seq_ = tuple(_check_tensor(_) for _ in output_seq)
 
         self.len_ = len(self.input_seq_)
```

### Comparing `vectorlab-1.0.0/vectorlab/data/dataset/_ts_dataset.py` & `vectorlab-1.0.1/vectorlab/data/dataset/_ts_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         The number of samples contained in the TSData.
     n_attrs_ : int
         The number of attributes contained in the TSData.
     """
 
     def __init__(self):
 
-        super(TSData, self).__init__()
+        super().__init__()
 
         return
 
     def _validate(self):
         r"""The data validation for TSData.
 
         In this function, time stamps and attributes data of TSData are
@@ -694,15 +694,15 @@
         The dataset of the entities, every element is TSData.
     n_entities_ : int
         The number of entities contains in the TSDataset.
     """
 
     def __init__(self):
 
-        super(TSDataset, self).__init__()
+        super().__init__()
 
         return
 
     def _validate(self):
         r"""The data validation for TSDataset.
 
         In this function, entities and dataset of TSDataset are checked.
```

### Comparing `vectorlab-1.0.0/vectorlab/data/tests/test_data_generator.py` & `vectorlab-1.0.1/vectorlab/data/tests/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/ensemble/_voting.py` & `vectorlab-1.0.1/vectorlab/ensemble/_voting.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/ensemble/tests/test_ensemble_voting.py` & `vectorlab-1.0.1/vectorlab/ensemble/tests/test_ensemble_voting.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/_generator.py` & `vectorlab-1.0.1/vectorlab/graph/_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/_utils.py` & `vectorlab-1.0.1/vectorlab/graph/_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/tests/test_graph_generator.py` & `vectorlab-1.0.1/vectorlab/graph/tests/test_graph_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/tests/test_graph_utils.py` & `vectorlab-1.0.1/vectorlab/graph/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/walking/_bfs.py` & `vectorlab-1.0.1/vectorlab/graph/walking/_bfs.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/walking/_dfs.py` & `vectorlab-1.0.1/vectorlab/graph/walking/_dfs.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/walking/_random_walk.py` & `vectorlab-1.0.1/vectorlab/graph/walking/_random_walk.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/graph/walking/tests/test_graph_walking.py` & `vectorlab-1.0.1/vectorlab/graph/walking/tests/test_graph_walking.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/metrics/pairwise/_dtw.py` & `vectorlab-1.0.1/vectorlab/metrics/pairwise/_dtw.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/metrics/pairwise/_lp_norm.py` & `vectorlab-1.0.1/vectorlab/metrics/pairwise/_lp_norm.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/metrics/pairwise/_sbd.py` & `vectorlab-1.0.1/vectorlab/metrics/pairwise/_sbd.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py` & `vectorlab-1.0.1/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,23 +102,14 @@
 
 def test_kl_div():
 
     # test identity of indiscernibles
     assert np.isclose(kl_div(X1, X1), 0)
     assert np.isclose(kl_div(Y1, Y1), 0)
 
-    # test symmetry
-    # kl_div may need a larger atol since the result
-    # may vary every time
-    assert np.isclose(
-        kl_div(X1, Y1),
-        kl_div(Y1, X1),
-        atol=1e-3
-    )
-
 
 def kl_div_efficency():
     kl_div(X1, Y1)
 
 
 def test_kl_div_efficency(benchmark):
     benchmark(kl_div_efficency)
```

### Comparing `vectorlab-1.0.0/vectorlab/optimize/_estimate.py` & `vectorlab-1.0.1/vectorlab/optimize/_estimate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-This module provides several estimation methods to find the best parameters for a certain algorithm.
+This module provides several estimation methods to find the best
+parameters for a certain algorithm.
 """
 
 import numpy as np
 
 from scipy import signal
 from sklearn.preprocessing import MinMaxScaler
```

### Comparing `vectorlab-1.0.0/vectorlab/optimize/_qap.py` & `vectorlab-1.0.1/vectorlab/optimize/_qap.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/optimize/tests/test_estimate.py` & `vectorlab-1.0.1/vectorlab/optimize/tests/test_estimate.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/plot/_palettes.py` & `vectorlab-1.0.1/vectorlab/plot/_palettes.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/plot/_plot.py` & `vectorlab-1.0.1/vectorlab/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/plot/tests/test_plot.py` & `vectorlab-1.0.1/vectorlab/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/series/_preprocessing.py` & `vectorlab-1.0.1/vectorlab/series/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/series/_utils.py` & `vectorlab-1.0.1/vectorlab/series/_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/series/smoothing/_arima.py` & `vectorlab-1.0.1/vectorlab/series/smoothing/_arima.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     ValueError
         If order is not in {'auto', list, tuple}, or list or tuple length is
         not equal to three, a ValueError is raised.
     """
 
     def __init__(self, order='auto'):
 
-        super(ARIMA, self).__init__()
+        super().__init__()
 
         self.p_, self.d_, self.q_ = None, None, None
 
         _order_error_msg = (
             f'Order parameter is {order}. '
             'However, order only supports auto or a tuple of (p, d, q).'
         )
```

### Comparing `vectorlab-1.0.0/vectorlab/series/smoothing/_holt_winters.py` & `vectorlab-1.0.1/vectorlab/series/smoothing/_holt_winters.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         The smoothed input array.
     """
 
     def __init__(self, trend=None,
                  seasonal=None, seasonal_periods=None,
                  initialization_method='estimated'):
 
-        super(HoltWinters, self).__init__()
+        super().__init__()
 
         if trend:
             trend = check_valid_option(
                 trend,
                 options=['add', 'mul', 'additive', 'multiplicative'],
                 variable_name='trend'
             )
```

### Comparing `vectorlab-1.0.0/vectorlab/series/smoothing/_moving_average.py` & `vectorlab-1.0.1/vectorlab/series/smoothing/_moving_average.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ValueError
         If window_size is not an integer larger than 0,
         a ValueError is raised.
     """
 
     def __init__(self, window_size):
 
-        super(MovingAverage, self).__init__()
+        super().__init__()
 
         window_size = check_valid_int(
             window_size,
             lower=1,
             variable_name='window_size'
         )
 
@@ -193,15 +193,15 @@
     ValueError
         If window_size is not an integer larger than 0,
         a ValueError is raised.
     """
 
     def __init__(self, window_size):
 
-        super(WeightedMovingAverage, self).__init__()
+        super().__init__()
 
         window_size = check_valid_int(
             window_size,
             lower=1,
             variable_name='window_size'
         )
 
@@ -340,15 +340,15 @@
     ValueError
         If alpha is a float larger than 1 or smaller than 0,
         a ValueError is raised.
     """
 
     def __init__(self, alpha):
 
-        super(ExpWeightedMovingAverage, self).__init__()
+        super().__init__()
 
         alpha = check_valid_float(
             alpha,
             lower=0, upper=1,
             variable_name='alpha'
         )
```

### Comparing `vectorlab-1.0.0/vectorlab/series/smoothing/_spectral_residual.py` & `vectorlab-1.0.1/vectorlab/series/smoothing/_spectral_residual.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     smoothed_X_ : array_like, shape (n_samples + extend_num)
         The smoothed extended input array.
     """
 
     def __init__(self, window_size,
                  extend_num=0, look_ahead=5):
 
-        super(SpectralResidual, self).__init__()
+        super().__init__()
 
         window_size = check_valid_int(
             window_size,
             lower=1,
             variable_name='window_size'
         )
         extend_num = check_valid_int(
```

### Comparing `vectorlab-1.0.0/vectorlab/series/smoothing/tests/test_series_smoothing.py` & `vectorlab-1.0.1/vectorlab/series/smoothing/tests/test_series_smoothing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/series/tests/test_series_preprocessing.py` & `vectorlab-1.0.1/vectorlab/series/tests/test_series_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/stats/_deg_graph.py` & `vectorlab-1.0.1/vectorlab/stats/_deg_graph.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/stats/_freq_tree.py` & `vectorlab-1.0.1/vectorlab/stats/_freq_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         The parent node for the current node.
     children_ : dict
         The children nodes for the current node.
     """
 
     def __init__(self, key, value):
 
-        super(FreqTreeNode, self).__init__(key, value)
+        super().__init__(key, value)
 
         self.parent_ = None
         self.children_ = {}
 
         return
 
     def value_add_one(self):
```

### Comparing `vectorlab-1.0.0/vectorlab/stats/_t_digest.py` & `vectorlab-1.0.1/vectorlab/stats/_t_digest.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/stats/tests/test_deg_graph.py` & `vectorlab-1.0.1/vectorlab/stats/tests/test_deg_graph.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/stats/tests/test_freq_tree.py` & `vectorlab-1.0.1/vectorlab/stats/tests/test_freq_tree.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/stats/tests/test_t_digest.py` & `vectorlab-1.0.1/vectorlab/stats/tests/test_t_digest.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/utils/_check.py` & `vectorlab-1.0.1/vectorlab/utils/_check.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/utils/_env.py` & `vectorlab-1.0.1/vectorlab/utils/_env.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/utils/_loading.py` & `vectorlab-1.0.1/vectorlab/utils/_loading.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/utils/_parser.py` & `vectorlab-1.0.1/vectorlab/utils/_parser.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/utils/_time.py` & `vectorlab-1.0.1/vectorlab/utils/_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 from ._check import check_valid_float, check_valid_option
 
 # Check if DATE is an environment variable
 if 'DATE' not in os.environ:
     os.environ['DATE'] = datetime.now().strftime('%Y%m%d')
 
-# timestamp and date conversion utils #
-#-------------------------------------#
+#  timestamp and date conversion utils  #
+# ------------------------------------- #
 
 
 def _auto_convert_ts(ts):
     r"""Auto convert timestamp in to seconds
 
     Parameters
     ----------
@@ -159,16 +159,16 @@
     """
 
     ts = datetime.timestamp(dttz)
 
     return ts
 
 
-# date parser utils #
-#-------------------#
+#  date parser utils  #
+# ------------------- #
 
 
 def _calculate_date_structure(date_structure):
     r"""Calculate date representation according to the
     date string format, `{DATE}` or `{DATE[+/-]int}`.
 
     Parameters
```

### Comparing `vectorlab-1.0.0/vectorlab/utils/tests/test_time.py` & `vectorlab-1.0.1/vectorlab/utils/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/vector/_array.py` & `vectorlab-1.0.1/vectorlab/vector/_array.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/vector/_tensor.py` & `vectorlab-1.0.1/vectorlab/vector/_tensor.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/vectorlab/vector/tests/test_array.py` & `vectorlab-1.0.1/vectorlab/vector/tests/test_array.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,19 +63,16 @@
             mat, trans_mat, method=method
         )
 
         if np.all(swap_matrix(mat, forward_transform) == trans_mat):
             success_number += 1
 
     print(
-        'Method: {}, node size: {}, success_rate: {:.2%}'.format(
-            method,
-            k,
-            success_number * 1.0 / rerun
-        )
+        f'Method: {method}, node size: {k}, '
+        f'success_rate: {success_number * 1.0 / rerun:.2%}'
     )
 
 
 def find_forward_transform_efficency(method):
 
     k = 30
 
@@ -122,19 +119,16 @@
             mat, trans_mat, method=method
         )
 
         if np.all(swap_matrix(trans_mat, forward_transform) == mat):
             success_number += 1
 
     print(
-        'Method: {}, node size: {}, success_rate: {:.2%}'.format(
-            method,
-            k,
-            success_number * 1.0 / rerun
-        )
+        f'Method: {method}, node size: {k}, '
+        f'success_rate: {success_number * 1.0 / rerun:.2%}'
     )
 
 
 def find_backward_transform_efficency(method):
 
     k = 30
```

### Comparing `vectorlab-1.0.0/vectorlab/vector/tests/test_tensor.py` & `vectorlab-1.0.1/vectorlab/vector/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.0/PKG-INFO` & `vectorlab-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorlab
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lab for vectors.
 Author-email: Kyle Yang <kyle.yang1995@gmail.com>, Emma Qin <emmaqin0722@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -20,14 +20,16 @@
 Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: seaborn>=0.11.2
 Requires-Dist: pillow>=9.2.0
 Requires-Dist: pytz>=2022.2.1
 Requires-Dist: dill>=0.3.5.1
 Requires-Dist: halo>=0.0.31
 Requires-Dist: pyyaml>=6.0
+Requires-Dist: torchinfo>=1.6.3
+Requires-Dist: tensorboard>=2.6.0
 Requires-Dist: torch>=1.10.0 ; extra == "full"
 Requires-Dist: torch-sparse>=0.6.12 ; extra == "full"
 Requires-Dist: torch-cluster>=1.6.0 ; extra == "full"
 Requires-Dist: torch-scatter>=2.0.9 ; extra == "full"
 Requires-Dist: torch-spline-conv>=1.2.1 ; extra == "full"
 Requires-Dist: torch-geometric>=2.0.4 ; extra == "full"
 Requires-Dist: pytest>=7.1.2 ; extra == "test"
@@ -39,15 +41,15 @@
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/Kr4t0n/vectorlab/main/static/logo.png"/>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/vectorlab)](https://pypi.org/project/vectorlab/)
 [![Package Status](https://img.shields.io/pypi/status/vectorlab)](https://pypi.org/project/vectorlab/)
-[![Testing Status](https://img.shields.io/github/workflow/status/Kr4t0n/vectorlab/Testing?label=Testing&logo=github)](https://github.com/Kr4t0n/vectorlab/actions/workflows/testing.yml)
+[![Testing Status](https://img.shields.io/github/actions/workflow/status/Kr4t0n/vectorlab/testing.yml?label=Testing&logo=github)](https://github.com/Kr4t0n/vectorlab/actions/workflows/testing.yml)
 [![Coverage](https://codecov.io/github/Kr4t0n/vectorlab/coverage.svg?branch=dev-feat)](https://codecov.io/gh/Kr4t0n/vectorlab)
 [![License](https://img.shields.io/pypi/l/vectorlab)](https://github.com/Kr4t0n/vectorlab/blob/main/LICENSE.txt)
 [![Python Version](https://img.shields.io/pypi/pyversions/vectorlab)](https://pypi.org/project/vectorlab/)
 
 VectorLab is a library to help solve scientific and engineering problems of mathematics and machine learning. It is built upon various fabulous softwares and tries to fill the gap when playing around with those softwares.
 
 VectorLab consists of many modules including data generation, graph processing, series processing, statistics, optimization, ensemble mechanism and more.
```

