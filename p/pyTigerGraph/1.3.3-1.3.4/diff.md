# Comparing `tmp/pyTigerGraph-1.3.3.tar.gz` & `tmp/pyTigerGraph-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTigerGraph-1.3.3.tar", last modified: Mon Apr  3 18:34:50 2023, max compression
+gzip compressed data, was "pyTigerGraph-1.3.4.tar", last modified: Thu Apr 13 17:56:04 2023, max compression
```

## Comparing `pyTigerGraph-1.3.3.tar` & `pyTigerGraph-1.3.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.585025 pyTigerGraph-1.3.3/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3653 2023-04-03 18:34:50.585163 pyTigerGraph-1.3.3/PKG-INFO
--rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2022-12-09 01:43:49.000000 pyTigerGraph-1.3.3/README.md
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.554253 pyTigerGraph-1.3.3/pyTigerGraph/
--rw-r--r--   0 parkererickson   (502) staff       (20)      108 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/__init__.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5291 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.3/pyTigerGraph/datasets.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.559523 pyTigerGraph-1.3.3/pyTigerGraph/gds/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.566635 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)      398 2023-03-13 16:30:47.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    94025 2023-03-13 16:28:17.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    19922 2023-01-13 15:10:11.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    51764 2023-01-13 15:10:10.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    11393 2023-03-13 16:29:14.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9232 2023-01-13 15:10:11.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     7243 2023-03-13 16:28:17.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     5509 2023-03-13 16:29:14.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)   173340 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/dataloaders.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    33157 2023-04-03 15:27:02.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/featurizer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    69236 2023-03-13 15:45:37.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gds.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.545963 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.568605 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3874 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     6673 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)      242 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/get_anchors.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     5667 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8422 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8853 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8063 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     5788 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.569647 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/
--rw-r--r--   0 parkererickson   (502) staff       (20)     1308 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     2715 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     2703 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     4874 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/metrics.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.546142 pyTigerGraph-1.3.3/pyTigerGraph/gds/models/
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.571419 pyTigerGraph-1.3.3/pyTigerGraph/gds/models/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)     6125 2023-02-15 15:29:03.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)      195 2023-02-15 15:29:03.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     1364 2023-02-15 15:29:03.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9661 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/splitters.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.546452 pyTigerGraph-1.3.3/pyTigerGraph/gds/transforms/
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.572312 pyTigerGraph-1.3.3/pyTigerGraph/gds/transforms/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)      165 2023-03-13 16:30:48.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/transforms/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)      799 2023-03-13 16:30:48.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9395 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.3/pyTigerGraph/gds/utilities.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2388 2022-11-23 18:58:50.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraph.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17679 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphAuth.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    16032 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphBase.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3910 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphDataset.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    47508 2023-02-20 22:23:49.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphEdge.py
--rw-r--r--   0 parkererickson   (502) staff       (20)      265 2022-04-21 16:09:16.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphException.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     8364 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphGSQL.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3631 2022-11-02 21:02:01.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphLoading.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11419 2022-11-02 21:02:01.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphPath.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    23431 2023-04-03 15:27:02.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphQuery.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9169 2023-02-20 22:23:49.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphSchema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2184 2022-11-02 21:02:01.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphUDT.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5996 2022-11-15 18:52:57.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphUtils.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    32833 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphVertex.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3930 2022-11-15 18:52:57.000000 pyTigerGraph-1.3.3/pyTigerGraph/visualization.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.556067 pyTigerGraph-1.3.3/pyTigerGraph.egg-info/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3653 2023-04-03 18:34:50.000000 pyTigerGraph-1.3.3/pyTigerGraph.egg-info/PKG-INFO
--rw-r--r--   0 parkererickson   (502) staff       (20)     3087 2023-04-03 18:34:50.000000 pyTigerGraph-1.3.3/pyTigerGraph.egg-info/SOURCES.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)        1 2023-04-03 18:34:50.000000 pyTigerGraph-1.3.3/pyTigerGraph.egg-info/dependency_links.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)       72 2023-04-03 18:34:50.000000 pyTigerGraph-1.3.3/pyTigerGraph.egg-info/requires.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)       19 2023-04-03 18:34:50.000000 pyTigerGraph-1.3.3/pyTigerGraph.egg-info/top_level.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)      229 2022-04-20 17:25:11.000000 pyTigerGraph-1.3.3/pyproject.toml
--rw-r--r--   0 parkererickson   (502) staff       (20)       78 2023-04-03 18:34:50.585608 pyTigerGraph-1.3.3/setup.cfg
--rw-r--r--   0 parkererickson   (502) staff       (20)     2573 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.3/setup.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-03 18:34:50.584662 pyTigerGraph-1.3.3/tests/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2022-04-20 17:25:11.000000 pyTigerGraph-1.3.3/tests/__init__.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     1481 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/pyTigerGraphUnitTest.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2037 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.3/tests/test_datasets.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    29857 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.3/tests/test_gds_BaseLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    10546 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.3/tests/test_gds_EdgeLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5677 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_gds_EdgeNeighborLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     6719 2023-03-13 15:45:37.000000 pyTigerGraph-1.3.3/tests/test_gds_GDS.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17297 2022-12-12 17:59:45.000000 pyTigerGraph-1.3.3/tests/test_gds_GraphLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7362 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.3/tests/test_gds_HGTLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    26565 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/tests/test_gds_NeighborLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11380 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.3/tests/test_gds_NodePieceLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11773 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.3/tests/test_gds_VertexLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    14864 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.3/tests/test_gds_featurizer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2424 2023-03-31 20:07:37.000000 pyTigerGraph-1.3.3/tests/test_gds_metrics.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     8349 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.3/tests/test_gds_splitters.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2025 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_gds_utilities.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2847 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphAuth.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2860 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphBase.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    14229 2023-02-20 22:23:49.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphEdge.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     1700 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphGSQL.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     6631 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphPath.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3530 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphQuery.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11799 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphSchema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)      706 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphUDT.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     1648 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphUtils.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9548 2023-04-03 18:34:31.000000 pyTigerGraph-1.3.3/tests/test_pyTigerGraphVertex.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.194143 pyTigerGraph-1.3.4/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3653 2023-04-13 17:56:04.194259 pyTigerGraph-1.3.4/PKG-INFO
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2022-12-09 01:43:49.000000 pyTigerGraph-1.3.4/README.md
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.171216 pyTigerGraph-1.3.4/pyTigerGraph/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      108 2023-04-13 17:55:41.000000 pyTigerGraph-1.3.4/pyTigerGraph/__init__.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5291 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.4/pyTigerGraph/datasets.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.175239 pyTigerGraph-1.3.4/pyTigerGraph/gds/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.179190 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      398 2023-03-13 16:30:47.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    94025 2023-03-13 16:28:17.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    19922 2023-01-13 15:10:11.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    51764 2023-01-13 15:10:10.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11393 2023-03-13 16:29:14.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9232 2023-01-13 15:10:11.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7243 2023-03-13 16:28:17.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5509 2023-03-13 16:29:14.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)   173570 2023-04-13 16:52:05.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/dataloaders.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    33157 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/featurizer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    69236 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gds.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.162489 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.181590 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3874 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6673 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)      242 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/get_anchors.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5667 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8422 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8853 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8437 2023-04-13 16:52:05.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5788 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.182685 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1546 2023-04-13 16:52:05.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2715 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2703 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4874 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/metrics.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.162677 pyTigerGraph-1.3.4/pyTigerGraph/gds/models/
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.183922 pyTigerGraph-1.3.4/pyTigerGraph/gds/models/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6125 2023-02-15 15:29:03.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)      195 2023-02-15 15:29:03.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1364 2023-02-15 15:29:03.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9661 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/splitters.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.162847 pyTigerGraph-1.3.4/pyTigerGraph/gds/transforms/
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.184583 pyTigerGraph-1.3.4/pyTigerGraph/gds/transforms/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      165 2023-03-13 16:30:48.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/transforms/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)      799 2023-03-13 16:30:48.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9395 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.4/pyTigerGraph/gds/utilities.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2388 2022-11-23 18:58:50.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraph.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17679 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphAuth.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    16032 2023-04-05 22:21:39.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphBase.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3910 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphDataset.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    47508 2023-02-20 22:23:49.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphEdge.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)      265 2022-04-21 16:09:16.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphException.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8364 2023-04-05 22:21:39.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphGSQL.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3631 2022-11-02 21:02:01.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphLoading.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11419 2022-11-02 21:02:01.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphPath.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    23431 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphQuery.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9169 2023-02-20 22:23:49.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphSchema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2184 2022-11-02 21:02:01.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphUDT.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5996 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphUtils.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    32833 2023-04-05 22:21:39.000000 pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphVertex.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3930 2022-11-15 18:52:57.000000 pyTigerGraph-1.3.4/pyTigerGraph/visualization.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.172450 pyTigerGraph-1.3.4/pyTigerGraph.egg-info/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3653 2023-04-13 17:56:04.000000 pyTigerGraph-1.3.4/pyTigerGraph.egg-info/PKG-INFO
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3087 2023-04-13 17:56:04.000000 pyTigerGraph-1.3.4/pyTigerGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)        1 2023-04-13 17:56:04.000000 pyTigerGraph-1.3.4/pyTigerGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)       72 2023-04-13 17:56:04.000000 pyTigerGraph-1.3.4/pyTigerGraph.egg-info/requires.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)       19 2023-04-13 17:56:04.000000 pyTigerGraph-1.3.4/pyTigerGraph.egg-info/top_level.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)      229 2022-04-20 17:25:11.000000 pyTigerGraph-1.3.4/pyproject.toml
+-rw-r--r--   0 parkererickson   (502) staff       (20)       78 2023-04-13 17:56:04.194682 pyTigerGraph-1.3.4/setup.cfg
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2573 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.4/setup.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2023-04-13 17:56:04.193857 pyTigerGraph-1.3.4/tests/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2022-04-20 17:25:11.000000 pyTigerGraph-1.3.4/tests/__init__.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1481 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/pyTigerGraphUnitTest.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2037 2022-12-07 20:53:19.000000 pyTigerGraph-1.3.4/tests/test_datasets.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    29857 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.4/tests/test_gds_BaseLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    10546 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.4/tests/test_gds_EdgeLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5677 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_gds_EdgeNeighborLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6719 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/tests/test_gds_GDS.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17297 2022-12-12 17:59:45.000000 pyTigerGraph-1.3.4/tests/test_gds_GraphLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7362 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.4/tests/test_gds_HGTLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    29086 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/tests/test_gds_NeighborLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11380 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.4/tests/test_gds_NodePieceLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11773 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.4/tests/test_gds_VertexLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    14864 2023-02-16 15:58:12.000000 pyTigerGraph-1.3.4/tests/test_gds_featurizer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2424 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/tests/test_gds_metrics.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8349 2023-01-09 15:28:36.000000 pyTigerGraph-1.3.4/tests/test_gds_splitters.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2025 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_gds_utilities.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2847 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphAuth.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2860 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphBase.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    14229 2023-02-20 22:23:49.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphEdge.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1700 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphGSQL.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6631 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphPath.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3530 2023-04-12 13:21:14.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphQuery.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11799 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphSchema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)      706 2022-12-12 17:45:12.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphUDT.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1648 2023-04-13 16:51:53.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphUtils.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9548 2023-04-05 22:21:39.000000 pyTigerGraph-1.3.4/tests/test_pyTigerGraphVertex.py
```

### Comparing `pyTigerGraph-1.3.3/PKG-INFO` & `pyTigerGraph-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTigerGraph
-Version: 1.3.3
+Version: 1.3.4
 Summary: Library to connect to TigerGraph databases
 Home-page: https://docs.tigergraph.com/pytigergraph/current/intro/
 Download-URL: 
 Author: TigerGraph Inc.
 Author-email: support@tigergraph.com
 License: Apache 2
 Project-URL: Bug Reports, https://github.com/tigergraph/pyTigerGraph/issues
```

### Comparing `pyTigerGraph-1.3.3/README.md` & `pyTigerGraph-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/datasets.py` & `pyTigerGraph-1.3.4/pyTigerGraph/datasets.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/dataloaders.py` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/dataloaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1741,14 +1741,15 @@
             v_extra_feats = v_extra_feats,
             v_attr_types = v_attr_types,
             e_in_feats = self.e_in_feats,
             e_out_labels = self.e_out_labels,
             e_extra_feats = self.e_extra_feats,
             e_attr_types = e_attr_types,
             add_self_loop = self.add_self_loop,
+            delimiter = self.delimiter,
             reindex = True,
             primary_id = i["pids"],
             is_hetero = self.is_hetero,
             callback_fn = self.callback_fn
         )
         # Return data
         return data
@@ -3220,15 +3221,15 @@
                 os.path.dirname(os.path.abspath(__file__)),
                 "gsql",
                 "dataloaders",
                 "get_anchors.gsql",
             )
             params = {"anchor_attr": anchor_attribute, "v_types": self._vtypes}
             install_query_file(self._graph, query_path)
-            ancs = self._graph.runInstalledQuery("get_anchors", params=params)[0]["@@vids"]
+            ancs = self._graph.runInstalledQuery("get_anchors", params=params, timeout=self.timeout)[0]["@@vids"]
             print("Number of Anchors:", len(ancs))
             for tok in self.baseTokens + ancs:
                 self.idToIdx[str(tok)] = self.curIdx
                 self.curIdx += 1
             
         self.num_tokens = len(self.idToIdx.keys())
 
@@ -3451,25 +3452,27 @@
             v_attr_types = self._v_schema
         if self.is_hetero:
             data = self._parse_data(resp[0]["vertex_batch"], 
                                     v_in_feats=attributes, 
                                     v_out_labels = {},
                                     v_extra_feats = {},
                                     v_attr_types=v_attr_types,
-                                    reindex=False, 
+                                    reindex=False,
+                                    delimiter = self.delimiter, 
                                     is_hetero=self.is_hetero, 
                                     primary_id=resp[0]["pids"],
                                     callback_fn=self.nodepiece_process)
         else:
             data = self._parse_data(resp[0]["vertex_batch"], 
                                     v_in_feats=attributes, 
                                     v_out_labels = [],
                                     v_extra_feats = [],
                                     v_attr_types=v_attr_types,
-                                    reindex=False, 
+                                    reindex=False,
+                                    delimiter = self.delimiter, 
                                     is_hetero=self.is_hetero, 
                                     primary_id=resp[0]["pids"],
                                     callback_fn=self.nodepiece_process)
         return data
 
     def precompute(self) -> None:
         """Compute NodePiece results (anchors and their distances) to cache attribute.
@@ -3875,14 +3878,15 @@
             v_extra_feats = v_extra_feats,
             v_attr_types = v_attr_types,
             e_in_feats = self.e_in_feats,
             e_out_labels = self.e_out_labels,
             e_extra_feats = self.e_extra_feats,
             e_attr_types = e_attr_types,
             add_self_loop = self.add_self_loop,
+            delimiter = self.delimiter,
             reindex = True,
             primary_id = i["pids"],
             is_hetero = self.is_hetero,
             callback_fn = self.callback_fn
         )
         # Return data
         return data
```

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/featurizer.py` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/featurizer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gds.py` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gds.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     SumAccum<INT> @tmp_id;
     SumAccum<STRING> @@kafka_error;
     SetAccum<VERTEX> @next_pass, @to_pass, @received;
     HeapAccum<Distance_Tuple> (max_anchors, distance ASC) @token_heap;
     SumAccum<STRING> @rel_context_set;
     SumAccum<STRING> @ancs;
     OrAccum @prev_sampled;
+    OrAccum @heapFull;
 
     MapAccum<VERTEX, SumAccum<INT>> @@token_count;
     MapAccum<INT, MinAccum<INT>> @conv_map;
     BOOL cache_empty = FALSE;
     INT distance;
     start = {v_types};
     # Perform fetch operation if desired
@@ -83,20 +84,28 @@
                 POST-ACCUM s.@tmp_id = floor(rand()*num_vertices);
         ELSE
             res = SELECT s 
                 FROM start:s
                 POST-ACCUM s.@tmp_id = getvid(s);
         END;
         FOREACH i IN RANGE [1, max_distance] DO
-          ancs = SELECT t
-                 FROM ancs:s -(e_types:e)-v_types:t
+          LOG(TRUE, "ANCHOR MESSAGE DISTANCE", i);
+          FOREACH j IN RANGE [0, 9] DO
+            LOG(TRUE, "ANCHOR BATCH", j);
+            ancs = SELECT t
+                 FROM ancs:s -(e_types:e)-v_types:t WHERE t.@heapFull == False AND getvid(s) % 10 == j
                  ACCUM 
                   FOREACH tup IN s.@token_heap DO 
                     t.@token_heap += Distance_Tuple(tup.v_id, i)
+                  END
+                POST-ACCUM
+                  IF s.@token_heap.size() == max_anchors THEN
+                    s.@heapFull += TRUE
                   END;
+          END;
         END;
     END;
     IF batch_size IS NULL THEN
       batch_s = ceil(res.size()/num_batches);
     ELSE  
       batch_s = batch_size;
     END;
@@ -131,15 +140,15 @@
                         POST-ACCUM @@batch_heap += ID_Tuple(s.@tmp_id, s);
             END;
             FOREACH elem IN @@batch_heap DO
               @@seeds += elem.v;
             END;
             seeds = {@@seeds};
             seeds = SELECT s 
-                    FROM start:s
+                    FROM seeds:s
                     POST-ACCUM
                         s.@prev_sampled += TRUE,
                         @@printed_vertices += s;
         END;
       ELSE
         start = input_vertices;
         seeds = SELECT s
```

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-CREATE QUERY random_anchor_selection(
+CREATE DISTRIBUTED QUERY random_anchor_selection(
   FLOAT percentage,
   STRING filter_by,
   SET<STRING> v_type,
   SET<STRING> tgt_v_type,
   STRING anchor_attr,
   INT random_seed) SYNTAX v2{
-
+  TYPEDEF TUPLE<FLOAT score, VERTEX v> Anchor_Tuple;
   SumAccum<FLOAT> @score;
   SetAccum<STRING> @@not_tgt_type;
-
+  HeapAccum<Anchor_Tuple> (1, score DESC) @@anchor_heap;
   INT anchor_sample_size, digit_mod;
 
   INT _mod, _mult, _inc;
   _mod = pow(2, 31)-1;
   _mult = 1664525;
   _inc = 1013904223;
   digit_mod =pow(10, 5);
 
   nodes = {v_type};
-  PRINT nodes.size();
   anchor_sample_size = nodes.size() * percentage;
+  @@anchor_heap.resize(anchor_sample_size);
   @@not_tgt_type = v_type MINUS tgt_v_type;
-
   IF filter_by IS NOT NULL THEN
     anchors =
       SELECT s FROM nodes:s
       WHERE s.getAttr(filter_by, "BOOL") OR (s.type IN @@not_tgt_type)
       POST-ACCUM 
         s.@score = ((((getvid(s)*_mult)+_inc)+_mult*random_seed) % _mod) % digit_mod / (digit_mod * 1.0), 
-        s.setAttr(anchor_attr, FALSE)
-      ORDER BY s.@score
-      LIMIT anchor_sample_size;
+        s.setAttr(anchor_attr, FALSE);
   ELSE
     anchors =
       SELECT s FROM nodes:s
       POST-ACCUM 
         s.@score = ((((getvid(s)*_mult)+_inc)+_mult*random_seed) % _mod) % digit_mod / (digit_mod * 1.0), 
-        s.setAttr(anchor_attr, FALSE)
-      ORDER BY s.@score
-      LIMIT anchor_sample_size;
+        s.setAttr(anchor_attr, FALSE);
   END;
    
   anchors =
     SELECT s FROM anchors:s
-    POST-ACCUM s.setAttr(anchor_attr, TRUE);
+    POST-ACCUM @@anchor_heap += Anchor_Tuple(s.@score, s);
+  SetAccum<VERTEX> @@seeds;
+  FOREACH elem IN @@anchor_heap DO
+    @@seeds += elem.v;
+  END;
     
+  anchors = {@@seeds};
+  anchors = SELECT s FROM anchors:s POST-ACCUM s.setAttr(anchor_attr, TRUE);
   PRINT anchor_sample_size, anchors.size();
 }
```

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/metrics.py` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/metrics.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/splitters.py` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/splitters.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/gds/utilities.py` & `pyTigerGraph-1.3.4/pyTigerGraph/gds/utilities.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraph.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraph.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphAuth.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphAuth.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphBase.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphBase.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphDataset.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphDataset.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphEdge.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphEdge.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphGSQL.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphGSQL.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphLoading.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphLoading.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphPath.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphPath.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphQuery.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphQuery.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphSchema.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphSchema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphUDT.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphUDT.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphUtils.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphUtils.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/pyTigerGraphVertex.py` & `pyTigerGraph-1.3.4/pyTigerGraph/pyTigerGraphVertex.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph/visualization.py` & `pyTigerGraph-1.3.4/pyTigerGraph/visualization.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph.egg-info/PKG-INFO` & `pyTigerGraph-1.3.4/pyTigerGraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTigerGraph
-Version: 1.3.3
+Version: 1.3.4
 Summary: Library to connect to TigerGraph databases
 Home-page: https://docs.tigergraph.com/pytigergraph/current/intro/
 Download-URL: 
 Author: TigerGraph Inc.
 Author-email: support@tigergraph.com
 License: Apache 2
 Project-URL: Bug Reports, https://github.com/tigergraph/pyTigerGraph/issues
```

### Comparing `pyTigerGraph-1.3.3/pyTigerGraph.egg-info/SOURCES.txt` & `pyTigerGraph-1.3.4/pyTigerGraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/setup.py` & `pyTigerGraph-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/pyTigerGraphUnitTest.py` & `pyTigerGraph-1.3.4/tests/pyTigerGraphUnitTest.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_datasets.py` & `pyTigerGraph-1.3.4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_BaseLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_BaseLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_EdgeLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_EdgeLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_EdgeNeighborLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_EdgeNeighborLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_GDS.py` & `pyTigerGraph-1.3.4/tests/test_gds_GDS.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_GraphLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_GraphLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_HGTLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_HGTLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_NeighborLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_NeighborLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,48 @@
         self.assertIn("55", data["primary_id"])
         for i, d in enumerate(data["primary_id"]):
             if d == "100" or d == "55":
                 self.assertTrue(data["is_seed"][i].item())
             else:
                 self.assertFalse(data["is_seed"][i].item())
 
+    def test_fetch_delimiter(self):
+        loader = NeighborLoader(
+            graph=self.conn,
+            v_in_feats=["x"],
+            v_out_labels=["y"],
+            v_extra_feats=["train_mask", "val_mask", "test_mask"],
+            batch_size=16,
+            num_neighbors=10,
+            num_hops=2,
+            shuffle=True,
+            delimiter="$|",
+            filter_by="train_mask",
+            output_format="PyG",
+            add_self_loop=False,
+            loader_id=None,
+            buffer_size=4,
+        )
+        data = loader.fetch(
+            [
+                {"primary_id": "100", "type": "Paper"},
+                {"primary_id": "55", "type": "Paper"},
+            ]
+        )
+        self.assertIn("primary_id", data)
+        self.assertGreater(data["x"].shape[0], 2)
+        self.assertGreater(data["edge_index"].shape[1], 0)
+        self.assertIn("100", data["primary_id"])
+        self.assertIn("55", data["primary_id"])
+        for i, d in enumerate(data["primary_id"]):
+            if d == "100" or d == "55":
+                self.assertTrue(data["is_seed"][i].item())
+            else:
+                self.assertFalse(data["is_seed"][i].item())
+
     def test_iterate_spektral(self):
         loader = NeighborLoader(
             graph=self.conn,
             v_in_feats=["x"],
             v_out_labels=["y"],
             v_extra_feats=["train_mask", "val_mask", "test_mask"],
             batch_size=16,
@@ -670,30 +704,62 @@
         self.assertIn("55", data["v0"]["primary_id"])
         for i, d in enumerate(data["v0"]["primary_id"]):
             if d == "10" or d == "55":
                 self.assertTrue(data["v0"]["is_seed"][i].item())
             else:
                 self.assertFalse(data["v0"]["is_seed"][i].item())
 
+    def test_fetch_delimiter(self):
+        loader = NeighborLoader(
+            graph=self.conn,
+            v_in_feats={"v0": ["x"], "v1": ["x"], "v2": ["x"]},
+            v_out_labels={"v0": ["y"]},
+            v_extra_feats={"v0": ["train_mask", "val_mask", "test_mask"]},
+            batch_size=16,
+            num_neighbors=10,
+            num_hops=2,
+            shuffle=False,
+            output_format="PyG",
+            delimiter="$|",
+            add_self_loop=False,
+            loader_id=None,
+            buffer_size=4,
+        )
+        data = loader.fetch(
+            [{"primary_id": "10", "type": "v0"}, {"primary_id": "55", "type": "v0"}]
+        )
+        self.assertIn("primary_id", data["v0"])
+        self.assertGreater(data["v0"]["x"].shape[0], 2)
+        self.assertGreater(data["v0v0"]["edge_index"].shape[1], 0)
+        self.assertIn("10", data["v0"]["primary_id"])
+        self.assertIn("55", data["v0"]["primary_id"])
+        for i, d in enumerate(data["v0"]["primary_id"]):
+            if d == "10" or d == "55":
+                self.assertTrue(data["v0"]["is_seed"][i].item())
+            else:
+                self.assertFalse(data["v0"]["is_seed"][i].item())
+
 
 if __name__ == "__main__":
     suite = unittest.TestSuite()
     suite.addTest(TestGDSNeighborLoaderKafka("test_init"))
     suite.addTest(TestGDSNeighborLoaderKafka("test_iterate_pyg"))
     suite.addTest(TestGDSNeighborLoaderKafka("test_whole_graph_pyg"))
     suite.addTest(TestGDSNeighborLoaderKafka("test_edge_attr"))
     # suite.addTest(TestGDSNeighborLoaderKafka("test_sasl_plaintext"))
     # suite.addTest(TestGDSNeighborLoaderKafka("test_sasl_ssl"))
     suite.addTest(TestGDSNeighborLoaderREST("test_init"))
     suite.addTest(TestGDSNeighborLoaderREST("test_iterate_pyg"))
     suite.addTest(TestGDSNeighborLoaderREST("test_whole_graph_pyg"))
     suite.addTest(TestGDSNeighborLoaderREST("test_edge_attr"))
     suite.addTest(TestGDSNeighborLoaderREST("test_fetch"))
+    suite.addTest(TestGDSNeighborLoaderREST("test_fetch_delimiter"))
     suite.addTest(TestGDSHeteroNeighborLoaderREST("test_init"))
     suite.addTest(TestGDSHeteroNeighborLoaderREST("test_whole_graph_df"))
     suite.addTest(TestGDSHeteroNeighborLoaderREST("test_whole_graph_pyg"))
     suite.addTest(TestGDSHeteroNeighborLoaderREST("test_iterate_pyg"))
     suite.addTest(TestGDSHeteroNeighborLoaderREST("test_iterate_pyg_multichar_delimiter"))
     suite.addTest(TestGDSHeteroNeighborLoaderREST("test_fetch"))
+    suite.addTest(TestGDSHeteroNeighborLoaderREST("test_fetch_delimiter"))
 
     runner = unittest.TextTestRunner(verbosity=2, failfast=True)
     runner.run(suite)
```

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_NodePieceLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_NodePieceLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_VertexLoader.py` & `pyTigerGraph-1.3.4/tests/test_gds_VertexLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_featurizer.py` & `pyTigerGraph-1.3.4/tests/test_gds_featurizer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_metrics.py` & `pyTigerGraph-1.3.4/tests/test_gds_metrics.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_splitters.py` & `pyTigerGraph-1.3.4/tests/test_gds_splitters.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_gds_utilities.py` & `pyTigerGraph-1.3.4/tests/test_gds_utilities.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphAuth.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphAuth.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphBase.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphBase.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphEdge.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphEdge.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphGSQL.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphGSQL.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphPath.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphPath.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphQuery.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphQuery.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphSchema.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphSchema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphUDT.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphUDT.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphUtils.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphUtils.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.3.3/tests/test_pyTigerGraphVertex.py` & `pyTigerGraph-1.3.4/tests/test_pyTigerGraphVertex.py`

 * *Files identical despite different names*

