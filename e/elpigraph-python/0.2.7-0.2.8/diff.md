# Comparing `tmp/elpigraph-python-0.2.7.tar.gz` & `tmp/elpigraph-python-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elpigraph-python-0.2.7.tar", last modified: Wed Jul  6 16:05:42 2022, max compression
+gzip compressed data, was "elpigraph-python-0.2.8.tar", last modified: Thu Apr 13 10:32:47 2023, max compression
```

## Comparing `elpigraph-python-0.2.7.tar` & `elpigraph-python-0.2.8.tar`

### file list

```diff
@@ -1,88 +1,36 @@
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/
--rwxrwxrwx   0 jo        (1000) jo        (1000)      472 2020-08-06 15:59:02.000000 elpigraph-python-0.2.7/.coveragerc
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/.github/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/.github/workflows/
--rwxrwxrwx   0 jo        (1000) jo        (1000)      895 2022-06-29 09:42:33.000000 elpigraph-python-0.2.7/.github/workflows/python-publish.yml
--rwxrwxrwx   0 jo        (1000) jo        (1000)      110 2022-03-29 16:32:39.000000 elpigraph-python-0.2.7/.gitignore
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2022-05-18 12:48:15.000000 elpigraph-python-0.2.7/.readthedocs.yml
--rwxrwxrwx   0 jo        (1000) jo        (1000)    35823 2020-07-06 13:34:30.000000 elpigraph-python-0.2.7/LICENSE
--rwxrwxrwx   0 jo        (1000) jo        (1000)       26 2020-07-09 16:08:29.000000 elpigraph-python-0.2.7/MANIFEST.in
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2735 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/PKG-INFO
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2190 2022-05-19 10:17:10.000000 elpigraph-python-0.2.7/README.md
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/data/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     7509 2020-07-06 13:34:30.000000 elpigraph-python-0.2.7/data/circle_data.csv
--rwxrwxrwx   0 jo        (1000) jo        (1000)    27830 2020-07-06 13:34:30.000000 elpigraph-python-0.2.7/data/curve_data.csv
--rwxrwxrwx   0 jo        (1000) jo        (1000)    17394 2020-07-06 13:34:30.000000 elpigraph-python-0.2.7/data/tree_data.csv
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/doc/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     7037 2020-08-20 14:04:35.000000 elpigraph-python-0.2.7/doc/Makefile
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/doc/_static/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/doc/_static/css/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     4315 2020-12-08 10:36:38.000000 elpigraph-python-0.2.7/doc/_static/css/custom.css
--rwxrwxrwx   0 jo        (1000) jo        (1000)      273 2020-08-20 14:04:35.000000 elpigraph-python-0.2.7/doc/_static/css/project-template.css
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/doc/_templates/
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/doc/_templates/autosummary/
--rwxrwxrwx   0 jo        (1000) jo        (1000)      194 2021-01-02 16:48:02.000000 elpigraph-python-0.2.7/doc/_templates/autosummary/base.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      690 2021-01-03 14:51:52.000000 elpigraph-python-0.2.7/doc/_templates/autosummary/class.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      670 2022-05-23 15:48:45.000000 elpigraph-python-0.2.7/doc/api.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)   459550 2022-05-23 15:41:19.000000 elpigraph-python-0.2.7/doc/basics.ipynb
--rwxrwxrwx   0 jo        (1000) jo        (1000)    17185 2022-05-18 12:26:51.000000 elpigraph-python-0.2.7/doc/conf.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     4966 2022-05-18 08:51:41.000000 elpigraph-python-0.2.7/doc/contributing.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      245 2022-05-23 16:37:07.000000 elpigraph-python-0.2.7/doc/elpigraph.CollapseBranches.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      232 2022-05-23 16:37:07.000000 elpigraph-python-0.2.7/doc/elpigraph.ExtendLeaves.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      239 2022-05-23 16:37:07.000000 elpigraph-python-0.2.7/doc/elpigraph.ShiftBranching.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      217 2022-05-23 16:18:58.000000 elpigraph-python-0.2.7/doc/elpigraph.addPath.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      278 2022-05-23 16:18:58.000000 elpigraph-python-0.2.7/doc/elpigraph.computeElasticPrincipalCircle.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      277 2022-05-23 16:18:58.000000 elpigraph-python-0.2.7/doc/elpigraph.computeElasticPrincipalCurve.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      274 2022-05-23 16:18:58.000000 elpigraph-python-0.2.7/doc/elpigraph.computeElasticPrincipalTree.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      218 2022-05-23 16:18:58.000000 elpigraph-python-0.2.7/doc/elpigraph.delPath.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      223 2022-05-23 16:18:58.000000 elpigraph-python-0.2.7/doc/elpigraph.findPaths.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      224 2022-05-23 16:37:07.000000 elpigraph-python-0.2.7/doc/elpigraph.fineTuneBR.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      279 2022-05-23 16:37:07.000000 elpigraph-python-0.2.7/doc/elpigraph.generateInitialConfiguration.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      221 2022-05-23 15:41:41.000000 elpigraph-python-0.2.7/doc/elpigraph.plot.PlotPG.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      242 2022-05-23 15:49:08.000000 elpigraph-python-0.2.7/doc/elpigraph.utils.getProjection.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      243 2022-05-23 15:49:08.000000 elpigraph-python-0.2.7/doc/elpigraph.utils.getPseudotime.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      235 2022-05-23 15:49:08.000000 elpigraph-python-0.2.7/doc/elpigraph.utils.getWeights.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)   243613 2022-06-01 11:47:38.000000 elpigraph-python-0.2.7/doc/graph_editing.ipynb
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1470 2022-05-24 07:25:26.000000 elpigraph-python-0.2.7/doc/index.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1018 2022-05-18 08:51:41.000000 elpigraph-python-0.2.7/doc/installation.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)     6721 2020-07-09 16:08:29.000000 elpigraph-python-0.2.7/doc/make.bat
--rwxrwxrwx   0 jo        (1000) jo        (1000)      594 2022-05-18 12:29:26.000000 elpigraph-python-0.2.7/doc/quick_start.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      689 2022-05-18 12:34:06.000000 elpigraph-python-0.2.7/doc/references.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      288 2021-04-21 19:26:06.000000 elpigraph-python-0.2.7/doc/release_notes.rst
--rwxrwxrwx   0 jo        (1000) jo        (1000)      198 2022-02-25 09:29:36.000000 elpigraph-python-0.2.7/doc/requirements.txt
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/elpigraph/
--rwxrwxrwx   0 jo        (1000) jo        (1000)    53248 2020-07-10 20:03:12.000000 elpigraph-python-0.2.7/elpigraph/.coverage
--rwxrwxrwx   0 jo        (1000) jo        (1000)    37260 2022-06-15 16:32:43.000000 elpigraph-python-0.2.7/elpigraph/_AlterStructure.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    23429 2022-06-01 10:15:51.000000 elpigraph-python-0.2.7/elpigraph/_BaseElPiWrapper.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1074 2022-05-23 16:31:02.000000 elpigraph-python-0.2.7/elpigraph/_EMAdjustment.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)      563 2022-06-16 14:30:09.000000 elpigraph-python-0.2.7/elpigraph/__init__.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    38645 2022-07-06 15:52:59.000000 elpigraph-python-0.2.7/elpigraph/_graph_editing.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    62370 2022-06-01 10:15:14.000000 elpigraph-python-0.2.7/elpigraph/_topologies.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)       23 2022-07-06 12:11:07.000000 elpigraph-python-0.2.7/elpigraph/_version.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    78943 2022-05-23 16:36:38.000000 elpigraph-python-0.2.7/elpigraph/plot.py
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/elpigraph/src/
--rwxrwxrwx   0 jo        (1000) jo        (1000)    39106 2022-06-01 10:37:46.000000 elpigraph-python-0.2.7/elpigraph/src/BaseElPi.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     6811 2020-07-20 18:44:00.000000 elpigraph-python-0.2.7/elpigraph/src/PCA.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)      184 2022-03-29 16:32:40.000000 elpigraph-python-0.2.7/elpigraph/src/__init__.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    69252 2022-05-23 16:35:30.000000 elpigraph-python-0.2.7/elpigraph/src/core.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    19376 2022-05-23 16:30:37.000000 elpigraph-python-0.2.7/elpigraph/src/distutils.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    71100 2022-05-23 16:31:04.000000 elpigraph-python-0.2.7/elpigraph/src/grammar_operations.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    16072 2022-05-23 16:31:02.000000 elpigraph-python-0.2.7/elpigraph/src/graphs.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     9721 2022-05-23 16:31:02.000000 elpigraph-python-0.2.7/elpigraph/src/reporting.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    32378 2022-03-29 16:33:34.000000 elpigraph-python-0.2.7/elpigraph/src/supervised.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     3823 2022-05-23 16:31:02.000000 elpigraph-python-0.2.7/elpigraph/src/synthetic.py
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/elpigraph/tests/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1607 2020-07-09 16:08:29.000000 elpigraph-python-0.2.7/elpigraph/tests/__init__.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)     4669 2020-07-20 17:49:18.000000 elpigraph-python-0.2.7/elpigraph/tests/test_all_params.py
--rwxrwxrwx   0 jo        (1000) jo        (1000)    16836 2022-06-28 09:15:04.000000 elpigraph-python-0.2.7/elpigraph/utils.py
-drwxrwxrwx   0 jo        (1000) jo        (1000)        0 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2735 2022-07-06 16:05:39.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/PKG-INFO
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1920 2022-07-06 16:05:41.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)        1 2022-07-06 16:05:39.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)        1 2022-06-01 11:53:57.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/not-zip-safe
--rwxrwxrwx   0 jo        (1000) jo        (1000)      225 2022-07-06 16:05:39.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/requires.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)       10 2022-07-06 16:05:39.000000 elpigraph-python-0.2.7/elpigraph_python.egg-info/top_level.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)     1234 2022-05-12 08:05:24.000000 elpigraph-python-0.2.7/meta.yaml
--rwxrwxrwx   0 jo        (1000) jo        (1000)      137 2022-05-11 09:50:36.000000 elpigraph-python-0.2.7/requirements.txt
--rwxrwxrwx   0 jo        (1000) jo        (1000)      106 2022-07-06 16:05:42.000000 elpigraph-python-0.2.7/setup.cfg
--rwxrwxrwx   0 jo        (1000) jo        (1000)     2580 2022-05-12 08:17:27.000000 elpigraph-python-0.2.7/setup.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.923720 elpigraph-python-0.2.8/
+-rw-r--r--   0 jbac       (502) staff       (20)    35823 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/LICENSE
+-rw-r--r--   0 jbac       (502) staff       (20)       26 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/MANIFEST.in
+-rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-13 10:32:47.923808 elpigraph-python-0.2.8/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)     2190 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/README.md
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.920682 elpigraph-python-0.2.8/elpigraph/
+-rw-r--r--   0 jbac       (502) staff       (20)    37260 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_AlterStructure.py
+-rw-r--r--   0 jbac       (502) staff       (20)    23429 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_BaseElPiWrapper.py
+-rw-r--r--   0 jbac       (502) staff       (20)     1074 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_EMAdjustment.py
+-rw-r--r--   0 jbac       (502) staff       (20)      563 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    36962 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_graph_editing.py
+-rw-r--r--   0 jbac       (502) staff       (20)    62370 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_topologies.py
+-rw-r--r--   0 jbac       (502) staff       (20)       23 2023-04-13 10:19:41.000000 elpigraph-python-0.2.8/elpigraph/_version.py
+-rw-r--r--   0 jbac       (502) staff       (20)    78943 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/plot.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.922574 elpigraph-python-0.2.8/elpigraph/src/
+-rw-r--r--   0 jbac       (502) staff       (20)    39106 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/BaseElPi.py
+-rw-r--r--   0 jbac       (502) staff       (20)     6811 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/PCA.py
+-rw-r--r--   0 jbac       (502) staff       (20)      184 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    69252 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/core.py
+-rw-r--r--   0 jbac       (502) staff       (20)    19376 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/distutils.py
+-rw-r--r--   0 jbac       (502) staff       (20)    71100 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/grammar_operations.py
+-rw-r--r--   0 jbac       (502) staff       (20)    16072 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/graphs.py
+-rw-r--r--   0 jbac       (502) staff       (20)     9721 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/reporting.py
+-rw-r--r--   0 jbac       (502) staff       (20)    32378 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/supervised.py
+-rw-r--r--   0 jbac       (502) staff       (20)     3823 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/synthetic.py
+-rw-r--r--   0 jbac       (502) staff       (20)    18040 2023-04-13 10:18:22.000000 elpigraph-python-0.2.8/elpigraph/utils.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.923573 elpigraph-python-0.2.8/elpigraph_python.egg-info/
+-rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)      787 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/not-zip-safe
+-rw-r--r--   0 jbac       (502) staff       (20)      225 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/requires.txt
+-rw-r--r--   0 jbac       (502) staff       (20)       10 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/top_level.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      137 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/requirements.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      106 2023-04-13 10:32:47.924130 elpigraph-python-0.2.8/setup.cfg
+-rw-r--r--   0 jbac       (502) staff       (20)     2580 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elpigraph-python-0.2.7/LICENSE` & `elpigraph-python-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/PKG-INFO` & `elpigraph-python-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpigraph-python
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://github.com/j-bac/elpigraph-python
 Maintainer: Jonathan Bac
 Maintainer-email: 
 Project-URL: Bug Reports, https://github.com/j-bac/elpigraph-python/issues
 Project-URL: Source, https://github.com/j-bac/elpigraph-python/
 Keywords: machine_learning graphs dimension_reduction single_cell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elpigraph-python-0.2.7/README.md` & `elpigraph-python-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/_AlterStructure.py` & `elpigraph-python-0.2.8/elpigraph/_AlterStructure.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/_BaseElPiWrapper.py` & `elpigraph-python-0.2.8/elpigraph/_BaseElPiWrapper.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/_EMAdjustment.py` & `elpigraph-python-0.2.8/elpigraph/_EMAdjustment.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/__init__.py` & `elpigraph-python-0.2.8/elpigraph/__init__.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/_graph_editing.py` & `elpigraph-python-0.2.8/elpigraph/_graph_editing.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,24 +236,24 @@
     X,
     PG,
     min_path_len=None,
     nnodes=None,
     max_inner_fraction=0.1,
     min_node_n_points=2,
     max_n_points=None,
-    # max_empty_curve_fraction=.2,
     min_compactness=0.5,
     radius=None,
     allow_same_branch=True,
     fit_loops=True,
     Lambda=None,
     Mu=None,
     cycle_Lambda=None,
     cycle_Mu=None,
     weights=None,
+    ignore_equivalent=False,
     plot=False,
     verbose=False,
 ):
     """
     This function tries to add extra paths to the graph
     by computing a series of principal curves connecting two nodes
     and retaining plausible ones using heuristic parameters
@@ -275,18 +275,16 @@
     allow_same_branch: bool, default=True
         Whether to allow new paths to connect two nodes from the same branch
     fit_loops: bool, default=True
         Whether to refit the graph to data after adding the new paths
     plot: bool, default=False
         Whether to plot selected candidate paths
     verbose: bool, default=False
-    copy: bool, default=False
-    use_weights: bool, default=False
+    weights: bool, default=False
         Whether to use point weights
-    use_partition: bool or list, default=False
     """
 
     _PG = deepcopy(PG)
     if "projection" in _PG.keys():
         del _PG["projection"]
     init_nodes_pos, init_edges = _PG["NodePositions"], _PG["Edges"][0]
 
@@ -307,17 +305,17 @@
     )
 
     if Mu is None:
         Mu = _PG["Mu"]
     if Lambda is None:
         Lambda = _PG["Lambda"]
     if cycle_Mu is None:
-        cycle_Mu = Mu / 10
+        cycle_Mu = Mu 
     if cycle_Lambda is None:
-        cycle_Lambda = Lambda / 10
+        cycle_Lambda = Lambda 
     if radius is None:
         radius = np.mean(edge_lengths) * len(init_nodes_pos) / 10
     if min_path_len is None:
         min_path_len = len(init_nodes_pos) // 5
     if max_n_points is None:
         max_n_points = int(len(X) * 0.05)
     if min_node_n_points is None:
@@ -344,17 +342,17 @@
     )
     net = elpigraph.src.graphs.ConstructGraph({"Edges": [init_edges]})
 
     if all(np.array(net.degree()) <= 2):
         branches = net.get_shortest_paths(leaves[0], leaves[-1])
     else:
         (
-            dict_tree,
+            _,
             dict_branches,
-            dict_branches_single_end,
+            _,
         ) = elpigraph.src.supervised.get_tree(init_edges, leaves[0])
         branches = list(dict_branches.values())
 
     candidate_nodes = []
     for i in range(len(leaves)):
         root_branch = [b for b in branches if leaves[i] in b][0]
 
@@ -411,17 +409,15 @@
                 ):
                     continue
                 else:
                     raise e
 
             # ---get nodep, edges, create new graph with added loop
             nodep, edges = pg["NodePositions"], pg["Edges"][0]
-            # _part, _part_dist = elpigraph.src.core.PartitionData(
-            #    X_fit, nodep, 10 ** 6, np.sum(X_fit ** 2, axis=1, keepdims=1)
-            # )
+
             _edges = edges.copy()
             _edges[(edges != 0) & (edges != 1)] += init_edges.max() - 1
             _edges[edges == 0] = c
             _edges[edges == 1] = l
             _merged_edges = np.concatenate((init_edges, _edges))
             _merged_nodep = np.concatenate((init_nodes_pos, nodep[2:]))
 
@@ -432,40 +428,24 @@
                 Lambda=Lambda,
                 Mu=Mu,
                 cycle_Lambda=cycle_Lambda,
                 cycle_Mu=cycle_Mu,
                 cycle_nodes=cycle_nodes,
             )
 
-            (
-                _merged_nodep,
-                _,
-                _,
-                _,
-                _,
-                _,
-                _,
-            ) = elpigraph.src.core.PrimitiveElasticGraphEmbedment(
+            _merged_nodep = elpigraph.src.core.PrimitiveElasticGraphEmbedment(
                 X,
                 _merged_nodep,
                 ElasticMatrix,
                 PointWeights=weights,
                 FixNodesAtPoints=[],
-            )
+            )[0]
 
             ### candidate validity tests ###
             valid = True
-            # --- curve validity test
-            # if (max_empty_curve_fraction is not None) and valid: # if X_fit projected to curve has long gaps
-            #    infer_pseudotime(_adata,source=0)
-            #    sorted_X_proj=_adata.obsm['X_epg_proj'][_adata.obs['epg_pseudotime'].argsort()]
-            #    dist = np.sqrt((np.diff(sorted_X_proj,axis=0)**2).sum(axis=1))
-            #    curve_len = np.sum(_adata.uns['epg']['edge_len'])
-            #    if np.max(dist) > (curve_len * max_empty_curve_fraction):
-            #        valid = False
 
             # --- cycle validity test
             if valid:
                 G = nx.Graph(_merged_edges.tolist())
                 cycle_nodes = find_all_cycles(G)[0]
                 cycle_nodep = np.array([_merged_nodep[e] for e in cycle_nodes])
                 cent_part, cent_dists = elpigraph.src.core.PartitionData(
@@ -495,33 +475,28 @@
                         w = mahalanobis(X_inside, cycle_centroid)
 
                     # points belonging to cycle shrunk by 10% or within 2 std of centroid (mahalanobis < 2)
                     shrunk_cycle_2d = shrink_or_swell_shapely_polygon(
                         cycle_2d, factor=0.1
                     )
 
-                    # prevent shapely bugs when multi-polygon is returned. Fall back to mahalanobis
+                    # prevent shapely edge case bug when multi-polygon is returned. Fall back to mahalanobis
                     if type(shrunk_cycle_2d) == MultiPolygon:
                         in_shrunk_cycle = np.ones(len(X_inside), dtype=bool)
                     else:
                         shrunk_cycle_2d = np.array(shrunk_cycle_2d.exterior.coords)
 
                         # prevent bug when self-intersection
                         if len(shrunk_cycle_2d) == 0:
                             in_shrunk_cycle = np.ones(len(X_inside), dtype=bool)
                         else:
                             in_shrunk_cycle = in_hull(shrunk_cycle_2d, X_inside)
                     idx_close = in_shrunk_cycle | (w < 1)
                     w = 1 - w / w.max()
                     w[idx_close] = 1
-
-                    # cycle_nodes_array = np.append(np.array(list(zip(range(len(cycle_2d)-1),
-                    #                                  range(1,len(cycle_2d))))),[[len(cycle_2d)-1,0]],axis=0)
-                    # w, idx_close = get_weights_lineproj(X_inside,cycle_2d,cycle_nodes_array,cycle_centroid[0],threshold=.2)
-
                     inner_fraction = np.sum(w) / np.sum(cycle_points)
 
                 if init_nodes_pos.shape[1] == 2:
                     intersect = not (
                         MultiLineString(
                             [LineString(_merged_nodep[e]) for e in _merged_edges]
                         ).is_simple
@@ -542,16 +517,16 @@
                         < min_node_n_points
                     )  # if empty cycle node
                     or (
                         inner_fraction > max_inner_fraction
                     )  # if high fraction of points inside
                     or (not np.isfinite(inner_fraction))  # prevent no points error
                     or (np.sum(idx_close) > max_n_points)  # if too many points inside
-                    or pp_compactness(cycle_2d) < min_compactness
-                ):  # if loop is very narrow
+                    or pp_compactness(cycle_2d) < min_compactness # if loop is very narrow
+                ):  
                     valid = False
 
             # ---> if cycle is invalid, continue
             if not valid:
                 inner_fractions.append(np.inf)
                 energies.append(np.inf)
                 merged_edges.append(np.inf)
@@ -567,19 +542,14 @@
                 (_merged_part, _merged_part_dist,) = elpigraph.src.core.PartitionData(
                     X, _merged_nodep, 10 ** 6, SquaredX=SquaredX
                 )
                 proj = elpigraph.src.reporting.project_point_onto_graph(
                     X, _merged_nodep, _merged_edges, _merged_part
                 )
                 MSE = proj["MSEP"]
-                # dist2proj = np.sum(np.square(X - X_proj), axis=1)
-                # ElasticMatrix = elpigraph.src.core.Encode2ElasticMatrix(_merged_edges, Lambdas=Lambda, Mus=Mu)
-                # ElasticEnergy, MSE, EP, RP = elpigraph.src.core.ComputePenalizedPrimitiveGraphElasticEnergy(_merged_nodep,
-                #                                                                                            ElasticMatrix,
-                #                                                                                            dist2proj,alpha=0.01,beta=0)
                 inner_fractions.append(inner_fraction)
                 energies.append(MSE)
                 merged_edges.append(_merged_edges)
                 merged_nodep.append(_merged_nodep)
                 merged_part.append(np.where(np.isin(_merged_part.flat, cycle_nodes))[0])
                 loop_edges.append(edges)
                 loop_nodep.append(nodep[2:])
@@ -678,48 +648,54 @@
                     _ = plt.scatter(*X[cycle_points][inside_idx, :2].T, c=w.flat, s=5)
                     plt.colorbar(_)
 
                     plt.show()
 
     # ignore equivalent loops (with more than 2/3 shared points and nodes)
     valid = np.ones(len(new_part))
-    for i in range(len(new_part) - 1):
-        for j in range(i + 1, len(new_part)):
-            if (
-                len(np.intersect1d(new_part[i], new_part[j]))
-                / max(len(new_part[i]), len(new_part[j]))
-            ) > (2 / 3):
-                if np.argmin([new_inner_fraction[i], new_inner_fraction[j]]) == 0:
-                    valid[i] = 0
-                else:
-                    valid[j] = 0
 
-    new_edges = [e for i, e in enumerate(new_edges) if valid[i]]
-    new_nodep = [e for i, e in enumerate(new_nodep) if valid[i]]
-    new_leaves = [e for i, e in enumerate(new_leaves) if valid[i]]
-    new_part = [e for i, e in enumerate(new_part) if valid[i]]
-    new_energy = [e for i, e in enumerate(new_energy) if valid[i]]
-    new_inner_fraction = [e for i, e in enumerate(new_inner_fraction) if valid[i]]
+    if ignore_equivalent:
+        for i in range(len(new_part) - 1):
+            for j in range(i + 1, len(new_part)):
+                if (
+                    len(np.intersect1d(new_part[i], new_part[j]))
+                    / max(len(new_part[i]), len(new_part[j]))
+                ) > (2 / 3):
+
+                    #all_leaves_i = np.isin(new_leaves[i],leaves).all()
+                    #all_leaves_j = np.isin(new_leaves[j],leaves).all()
+                    ## prioritize connecting leaves
+                    #if all_leaves_j and not(all_leaves_i):
+                    #    valid[i] = 0
+                    #elif all_leaves_i and not(all_leaves_j):
+                    #    valid[j] = 0
+                    # else take lowest energy
+                    if np.argmin([new_energy[i], new_energy[j]]) == 0:
+                        valid[j] = 0
+                    else:
+                        valid[i] = 0
+
+        new_edges = [e for i, e in enumerate(new_edges) if valid[i]]
+        new_nodep = [e for i, e in enumerate(new_nodep) if valid[i]]
+        new_leaves = [e for i, e in enumerate(new_leaves) if valid[i]]
+        new_part = [e for i, e in enumerate(new_part) if valid[i]]
+        new_energy = [e for i, e in enumerate(new_energy) if valid[i]]
+        new_inner_fraction = [e for i, e in enumerate(new_inner_fraction) if valid[i]]
 
     ### form graph with all valid loops found ###
     if (new_edges == []) or (sum(valid) == 0):
         print("Found no valid path to add")
         return None
 
+    merged_edges=init_edges.copy()
     for i, loop_edges in enumerate(new_edges):
-        if i == 0:
-            loop_edges[(loop_edges != 0) & (loop_edges != 1)] += init_edges.max() - 1
-            loop_edges[loop_edges == 0] = new_leaves[i][0]
-            loop_edges[loop_edges == 1] = new_leaves[i][1]
-            merged_edges = np.concatenate((init_edges, loop_edges))
-        else:
-            loop_edges[(loop_edges != 0) & (loop_edges != 1)] += merged_edges.max() - 1
-            loop_edges[loop_edges == 0] = new_leaves[i][0]
-            loop_edges[loop_edges == 1] = new_leaves[i][1]
-            merged_edges = np.concatenate((merged_edges, loop_edges))
+        loop_edges[(loop_edges != 0) & (loop_edges != 1)] += merged_edges.max() - 1
+        ix0, ix1 = loop_edges == 0, loop_edges == 1
+        loop_edges[ix0],loop_edges[ix1] = new_leaves[i][0], new_leaves[i][1]
+        merged_edges = np.concatenate((merged_edges, loop_edges))
     merged_nodep = np.concatenate((init_nodes_pos, *new_nodep))
 
     ### optionally refit the entire graph ###
     if fit_loops:
         cycle_nodes = np.concatenate(find_all_cycles(nx.Graph(merged_edges.tolist())))
 
         ElasticMatrix = elpigraph.src.core.MakeUniformElasticMatrix_with_cycle(
@@ -727,25 +703,17 @@
             Lambda=Lambda,
             Mu=Mu,
             cycle_Lambda=cycle_Lambda,
             cycle_Mu=cycle_Mu,
             cycle_nodes=cycle_nodes,
         )
 
-        (
-            merged_nodep,
-            _,
-            _,
-            _,
-            _,
-            _,
-            _,
-        ) = elpigraph.src.core.PrimitiveElasticGraphEmbedment(
-            X, merged_nodep, ElasticMatrix, PointWeights=weights, FixNodesAtPoints=[],
-        )
+        merged_nodep = elpigraph.src.core.PrimitiveElasticGraphEmbedment(
+        X, merged_nodep, ElasticMatrix, PointWeights=weights, FixNodesAtPoints=[])[0]
+
         # check intersection
         if merged_nodep.shape[1] == 2:
             intersect = not (
                 MultiLineString(
                     [LineString(merged_nodep[e]) for e in merged_edges]
                 ).is_simple
             )
@@ -759,14 +727,16 @@
     _PG["Lambda"] = Lambda
     _PG["Mu"] = Mu
     _PG["cycle_Lambda"] = cycle_Lambda
     _PG["cycle_Mu"] = cycle_Mu
     _PG["addLoopsdict"] = dict(
         new_edges=new_edges,
         new_nodep=new_nodep,
+        merged_nodep=merged_nodep,
+        merged_edges=merged_edges,
         new_leaves=new_leaves,
         new_part=new_part,
         new_energy=new_energy,
         new_inner_fraction=new_inner_fraction,
     )
 
     if verbose:
```

### Comparing `elpigraph-python-0.2.7/elpigraph/_topologies.py` & `elpigraph-python-0.2.8/elpigraph/_topologies.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/plot.py` & `elpigraph-python-0.2.8/elpigraph/plot.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/BaseElPi.py` & `elpigraph-python-0.2.8/elpigraph/src/BaseElPi.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/PCA.py` & `elpigraph-python-0.2.8/elpigraph/src/PCA.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/core.py` & `elpigraph-python-0.2.8/elpigraph/src/core.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/distutils.py` & `elpigraph-python-0.2.8/elpigraph/src/distutils.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/grammar_operations.py` & `elpigraph-python-0.2.8/elpigraph/src/grammar_operations.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/graphs.py` & `elpigraph-python-0.2.8/elpigraph/src/graphs.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/reporting.py` & `elpigraph-python-0.2.8/elpigraph/src/reporting.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/supervised.py` & `elpigraph-python-0.2.8/elpigraph/src/supervised.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/src/synthetic.py` & `elpigraph-python-0.2.8/elpigraph/src/synthetic.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.7/elpigraph/utils.py` & `elpigraph-python-0.2.8/elpigraph/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def getProjection(X, PG):
     """Compute graph projection from principal graph dict
     (result stored in PG dict under 'projection' key)
     """
 
     G = nx.Graph()
     G.add_edges_from(PG["Edges"][0].tolist(), weight=1)
-    mat_conn = nx.to_scipy_sparse_matrix(
+    mat_conn = nx.to_scipy_sparse_array(
         G, nodelist=np.arange(len(PG["NodePositions"])), weight="weight"
     )
 
     # partition points
     node_id, node_dist = PartitionData(
         X=X,
         NodePositions=PG["NodePositions"],
@@ -170,24 +170,23 @@
     """Get point weights as the inverse density of data
     X: np.array, (n_sample x n_dims)
     bandwidth: sklearn KernelDensity bandwidth if method == 'sklearn'
     griddelta: FFTKDE grid step size if method =='fft'
     exponent: density values are raised to the power of exponent
     """
     if method == "sklearn":
-        kde = KernelDensity(
-            kernel="gaussian", bandwidth=bandwidth, **kwargs
+        kde = KernelDensity(bandwidth=bandwidth, **kwargs
         ).fit(X)
         scores = kde.score_samples(X)
         scores = np.exp(scores)[:, None]
 
     elif method == "fft":
         import KDEpy
 
-        kde = KDEpy.FFTKDE(**kwargs).fit(X)
+        kde = KDEpy.FFTKDE(bw=bandwidth,**kwargs).fit(X)
         x, y = kde.evaluate(griddelta)
         scores = scipy.interpolate.griddata(x, y, X)
 
     p = 1 / (scores ** exponent)
     p /= np.sum(p)
     return p
 
@@ -376,19 +375,19 @@
         return merged_dists, merged_idx
 
 
 def geodesic_pseudotime(X, k, root, g=None):
     """pseudotime as graph distance from root point"""
     if g is None:
         nn = NearestNeighbors(n_neighbors=k, n_jobs=8).fit(X)
-        g = nx.convert_matrix.from_scipy_sparse_matrix(
+        g = nx.convert_matrix.from_scipy_sparse_array(
             nn.kneighbors_graph(mode="distance")
         )
     else:
-        g = nx.convert_matrix.from_scipy_sparse_matrix(g)
+        g = nx.convert_matrix.from_scipy_sparse_array(g)
     if len(list(nx.connected_components(g))) > 1:
         raise ValueError(
             f"detected more than 1 components with k={k} neighbors. Please"
             " increase k"
         )
     lengths = nx.single_source_dijkstra_path_length(g, root)
     pseudotime = np.array(pd.Series(lengths).sort_index())
@@ -464,11 +463,50 @@
         cprev = clusters==c
         cnext = clusters==(c-1)
         ypath[cnext] = _propagate_labels(Xs=Xpath[cprev],Xt=Xpath[cnext],ys=ypath[cprev],
                                     flavor=flavor,n_neighbors=n_neighbors,reg_e=ot_reg_e,reg_m=ot_reg_m)
         
     s = '-'.join(str(x) for x in branch_nodes)
     
-    y[ix] = ypath
-    PG[f'early_groups_{source}->{s}']=y.astype(str)
-    y[ix] = clusters
-    PG[f'early_groups_{source}->{s}_clusters']=y.astype(str)
+    y_groups = y.copy()
+    y_groups[ix] = ypath
+    PG[f'early_groups_{source}->{s}'] = y_groups.astype(str)
+    
+    y_clus = y.astype(str)
+    y_clus[ix] = ['c'+c for c in clusters.astype(str)]
+    PG[f'early_groups_{source}->{s}_clusters'] = y_clus.copy()
+
+def residuals(X, Xr, nodep, r2_threshold=.5):
+
+    partition = PartitionData(
+        X=Xr,
+        NodePositions=nodep,
+        MaxBlockSize=100000,
+        TrimmingRadius=np.inf,
+        SquaredX=np.sum(Xr ** 2, axis=1, keepdims=1),
+    )[0]
+
+    means, residue_matrix, r2scores = _residuals_matrix(X, partition.flatten(), len(nodep))
+    ind = np.where(r2scores > r2_threshold)[0]
+    return (means, residue_matrix, r2scores, ind)
+
+def _residuals_matrix(X, partition, n_nodes):
+    # Building mapping partition -> set of points
+    inds = [[] for _ in range(n_nodes)]
+    for i in range(X.shape[0]):
+        inds[partition[i]].append(i)
+    if any([len(ind) == 0 for ind in inds]):
+        print("Warning: empty nodes.")
+
+    # Computing barycenter of each cluster
+    means = np.array(
+        [
+            (np.mean(X[ind, :], axis=0) if len(ind) > 0 else np.zeros((X.shape[1],)))
+            for ind in inds
+        ]
+    )
+
+    # Computing residuals
+    residue_matrix = means[partition, :]
+    r2_scores = np.var(residue_matrix, axis=0) / np.var(X, axis=0)
+    
+    return((means, residue_matrix, r2_scores))
```

### Comparing `elpigraph-python-0.2.7/elpigraph_python.egg-info/PKG-INFO` & `elpigraph-python-0.2.8/elpigraph_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpigraph-python
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://github.com/j-bac/elpigraph-python
 Maintainer: Jonathan Bac
 Maintainer-email: 
 Project-URL: Bug Reports, https://github.com/j-bac/elpigraph-python/issues
 Project-URL: Source, https://github.com/j-bac/elpigraph-python/
 Keywords: machine_learning graphs dimension_reduction single_cell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elpigraph-python-0.2.7/setup.py` & `elpigraph-python-0.2.8/setup.py`

 * *Files identical despite different names*

