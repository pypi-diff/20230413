# Comparing `tmp/xgi-0.5.6.tar.gz` & `tmp/xgi-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgi-0.5.6.tar", last modified: Mon Apr  3 19:04:37 2023, max compression
+gzip compressed data, was "xgi-0.5.7.tar", last modified: Thu Apr 13 18:56:33 2023, max compression
```

## Comparing `xgi-0.5.6.tar` & `xgi-0.5.7.tar`

### file list

```diff
@@ -1,86 +1,93 @@
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.668688 xgi-0.5.6/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      541 2023-04-03 19:00:13.000000 xgi-0.5.6/CITATION.cff
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    13466 2022-10-13 17:38:17.000000 xgi-0.5.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3140 2023-03-09 16:27:55.000000 xgi-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-03-17 19:59:13.000000 xgi-0.5.6/LICENSE.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-01-03 14:13:27.000000 xgi-0.5.6/MANIFEST.in
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3391 2023-04-03 19:04:37.668556 xgi-0.5.6/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5633 2023-03-23 13:51:40.000000 xgi-0.5.6/README.md
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.659366 xgi-0.5.6/logo/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.5.6/logo/logo.pdf
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.5.6/logo/logo.png
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.5.6/logo/logo.svg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2574 2023-03-23 13:51:29.000000 xgi-0.5.6/long_description.rst
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.5.6/pytest.ini
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.660444 xgi-0.5.6/requirements/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.5.6/requirements/README.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.5.6/requirements/benchmarks.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-03-17 19:59:30.000000 xgi-0.5.6/requirements/default.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-03-17 19:59:22.000000 xgi-0.5.6/requirements/developer.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       95 2022-10-13 17:38:17.000000 xgi-0.5.6/requirements/documentation.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.5.6/requirements/release.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       40 2023-03-17 19:59:30.000000 xgi-0.5.6/requirements/test.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2022-10-13 17:38:17.000000 xgi-0.5.6/requirements/tutorial.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-04-03 19:04:37.668727 xgi-0.5.6/setup.cfg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1856 2023-04-03 19:00:11.000000 xgi-0.5.6/setup.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.662582 xgi-0.5.6/tutorials/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-03-14 19:28:19.000000 xgi-0.5.6/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-03-14 19:28:19.000000 xgi-0.5.6/tutorials/Tutorial 2 - Read and Write.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-01-03 14:13:27.000000 xgi-0.5.6/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2022-10-13 17:38:17.000000 xgi-0.5.6/tutorials/Tutorial 4 - Generative_Models.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)  1036171 2023-03-27 19:34:24.000000 xgi-0.5.6/tutorials/Tutorial 5 - Plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57228 2023-03-14 19:28:19.000000 xgi-0.5.6/tutorials/Tutorial 6 - Statistics.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-03-28 14:59:38.000000 xgi-0.5.6/tutorials/case_study_zhang2022.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    21241 2023-03-22 23:23:15.000000 xgi-0.5.6/tutorials/quickstart.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-03-14 19:28:19.000000 xgi-0.5.6/tutorials/simplicial_kuramoto_example.ipynb
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.663089 xgi-0.5.6/xgi/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.5.6/xgi/__init__.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.664580 xgi-0.5.6/xgi/algorithms/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      131 2023-04-03 17:05:40.000000 xgi-0.5.6/xgi/algorithms/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4552 2023-03-27 20:55:15.000000 xgi-0.5.6/xgi/algorithms/assortativity.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8946 2023-04-03 17:05:40.000000 xgi-0.5.6/xgi/algorithms/centrality.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5425 2022-10-13 17:38:17.000000 xgi-0.5.6/xgi/algorithms/connected.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.665426 xgi-0.5.6/xgi/classes/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      151 2023-03-17 19:59:13.000000 xgi-0.5.6/xgi/classes/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    26166 2023-03-28 14:59:38.000000 xgi-0.5.6/xgi/classes/function.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    41420 2023-03-28 14:59:39.000000 xgi-0.5.6/xgi/classes/hypergraph.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2729 2023-03-28 13:51:25.000000 xgi-0.5.6/xgi/classes/hypergraphviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    20877 2023-03-30 11:30:13.000000 xgi-0.5.6/xgi/classes/reportviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    26081 2023-03-28 14:59:38.000000 xgi-0.5.6/xgi/classes/simplicialcomplex.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    20582 2023-04-03 17:05:40.000000 xgi-0.5.6/xgi/convert.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.665815 xgi-0.5.6/xgi/drawing/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-03-22 23:23:15.000000 xgi-0.5.6/xgi/drawing/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    33907 2023-04-02 20:57:13.000000 xgi-0.5.6/xgi/drawing/draw.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10608 2023-03-28 14:59:38.000000 xgi-0.5.6/xgi/drawing/layout.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.666070 xgi-0.5.6/xgi/dynamics/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.5.6/xgi/dynamics/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8888 2023-03-28 14:59:38.000000 xgi-0.5.6/xgi/dynamics/synchronization.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.5.6/xgi/exception.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.666518 xgi-0.5.6/xgi/generators/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      115 2022-10-13 17:38:17.000000 xgi-0.5.6/xgi/generators/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9979 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/generators/classic.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    14154 2023-03-17 19:59:30.000000 xgi-0.5.6/xgi/generators/nonuniform.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10033 2023-03-17 19:59:30.000000 xgi-0.5.6/xgi/generators/uniform.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.666746 xgi-0.5.6/xgi/linalg/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       43 2022-10-13 17:38:17.000000 xgi-0.5.6/xgi/linalg/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    19107 2023-04-03 17:05:40.000000 xgi-0.5.6/xgi/linalg/matrix.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.667747 xgi-0.5.6/xgi/readwrite/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      179 2022-10-13 17:38:17.000000 xgi-0.5.6/xgi/readwrite/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6002 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/readwrite/bipartite.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/readwrite/edgelist.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2177 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/readwrite/incidence.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1904 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/readwrite/json.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5167 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/readwrite/xgi_data.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.668125 xgi-0.5.6/xgi/stats/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    17688 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/stats/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6544 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/stats/edgestats.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10279 2023-03-31 23:24:07.000000 xgi-0.5.6/xgi/stats/nodestats.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.668348 xgi-0.5.6/xgi/utils/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.5.6/xgi/utils/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3858 2023-03-17 19:59:22.000000 xgi-0.5.6/xgi/utils/utilities.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-03 19:04:37.663735 xgi-0.5.6/xgi.egg-info/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3391 2023-04-03 19:04:37.000000 xgi-0.5.6/xgi.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1772 2023-04-03 19:04:37.000000 xgi-0.5.6/xgi.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-04-03 19:04:37.000000 xgi-0.5.6/xgi.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      767 2023-04-03 19:04:37.000000 xgi-0.5.6/xgi.egg-info/requires.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-04-03 19:04:37.000000 xgi-0.5.6/xgi.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.293846 xgi-0.5.7/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      541 2023-04-13 18:54:30.000000 xgi-0.5.7/CITATION.cff
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-04-13 15:46:50.000000 xgi-0.5.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3123 2023-04-13 15:46:50.000000 xgi-0.5.7/CONTRIBUTING.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-03-17 19:59:13.000000 xgi-0.5.7/LICENSE.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-01-03 14:13:27.000000 xgi-0.5.7/MANIFEST.in
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3204 2023-04-13 18:56:33.293714 xgi-0.5.7/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5531 2023-04-13 15:46:50.000000 xgi-0.5.7/README.md
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.283970 xgi-0.5.7/logo/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.5.7/logo/logo.pdf
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.5.7/logo/logo.png
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.5.7/logo/logo.svg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2438 2023-04-13 15:46:50.000000 xgi-0.5.7/long_description.rst
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.5.7/pytest.ini
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.284826 xgi-0.5.7/requirements/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.5.7/requirements/README.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.5.7/requirements/benchmarks.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-03-17 19:59:30.000000 xgi-0.5.7/requirements/default.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-03-17 19:59:22.000000 xgi-0.5.7/requirements/developer.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       95 2022-10-13 17:38:17.000000 xgi-0.5.7/requirements/documentation.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.5.7/requirements/release.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-04-13 15:46:50.000000 xgi-0.5.7/requirements/test.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2022-10-13 17:38:17.000000 xgi-0.5.7/requirements/tutorial.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-04-13 18:56:33.293885 xgi-0.5.7/setup.cfg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1805 2023-04-13 18:47:46.000000 xgi-0.5.7/setup.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.286970 xgi-0.5.7/tutorials/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-03-14 19:28:19.000000 xgi-0.5.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-03-14 19:28:19.000000 xgi-0.5.7/tutorials/Tutorial 2 - Read and Write.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-01-03 14:13:27.000000 xgi-0.5.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2022-10-13 17:38:17.000000 xgi-0.5.7/tutorials/Tutorial 4 - Generative_Models.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)  1036142 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/Tutorial 5 - Plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/Tutorial 6 - Statistics.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   214665 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-03-28 14:59:38.000000 xgi-0.5.7/tutorials/case_study_zhang2022.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    21289 2023-04-05 18:31:56.000000 xgi-0.5.7/tutorials/quickstart.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-03-14 19:28:19.000000 xgi-0.5.7/tutorials/simplicial_kuramoto_example.ipynb
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.287457 xgi-0.5.7/xgi/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.5.7/xgi/__init__.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.288813 xgi-0.5.7/xgi/algorithms/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      169 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/algorithms/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4552 2023-03-27 20:55:15.000000 xgi-0.5.7/xgi/algorithms/assortativity.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9027 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/algorithms/centrality.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7198 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/algorithms/clustering.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5425 2022-10-13 17:38:17.000000 xgi-0.5.7/xgi/algorithms/connected.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.289681 xgi-0.5.7/xgi/classes/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      151 2023-03-17 19:59:13.000000 xgi-0.5.7/xgi/classes/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    25479 2023-04-11 13:26:40.000000 xgi-0.5.7/xgi/classes/function.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    41403 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/classes/hypergraph.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2729 2023-03-28 13:51:25.000000 xgi-0.5.7/xgi/classes/hypergraphviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    22713 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/classes/reportviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    26351 2023-04-11 13:26:40.000000 xgi-0.5.7/xgi/classes/simplicialcomplex.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    20902 2023-04-08 17:36:23.000000 xgi-0.5.7/xgi/convert.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.290126 xgi-0.5.7/xgi/drawing/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-03-22 23:23:15.000000 xgi-0.5.7/xgi/drawing/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    42809 2023-04-08 17:36:59.000000 xgi-0.5.7/xgi/drawing/draw.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10608 2023-03-28 14:59:38.000000 xgi-0.5.7/xgi/drawing/layout.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.290386 xgi-0.5.7/xgi/dynamics/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.5.7/xgi/dynamics/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8872 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/dynamics/synchronization.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.5.7/xgi/exception.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.291593 xgi-0.5.7/xgi/generators/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2616 2023-04-05 18:46:03.000000 xgi-0.5.7/xgi/generators/classic.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1410 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/lattice.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10635 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/random.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-04-05 18:49:06.000000 xgi-0.5.7/xgi/generators/simple.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7754 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/generators/simplicial_complexes.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10033 2023-04-08 17:36:59.000000 xgi-0.5.7/xgi/generators/uniform.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.292104 xgi-0.5.7/xgi/linalg/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/linalg/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7016 2023-04-05 18:50:00.000000 xgi-0.5.7/xgi/linalg/hodge_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8403 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/linalg/hypergraph_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6711 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/linalg/laplacian_matrix.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.292806 xgi-0.5.7/xgi/readwrite/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      179 2022-10-13 17:38:17.000000 xgi-0.5.7/xgi/readwrite/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6002 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/bipartite.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/edgelist.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2177 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/incidence.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1904 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/readwrite/json.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5235 2023-04-05 18:31:56.000000 xgi-0.5.7/xgi/readwrite/xgi_data.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.293210 xgi-0.5.7/xgi/stats/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    17825 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/stats/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-04-13 15:46:50.000000 xgi-0.5.7/xgi/stats/edgestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    12556 2023-04-13 13:41:14.000000 xgi-0.5.7/xgi/stats/nodestats.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.293507 xgi-0.5.7/xgi/utils/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.5.7/xgi/utils/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3858 2023-03-17 19:59:22.000000 xgi-0.5.7/xgi/utils/utilities.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-04-13 18:56:33.288120 xgi-0.5.7/xgi.egg-info/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3204 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2018 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      741 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/requires.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-04-13 18:56:33.000000 xgi-0.5.7/xgi.egg-info/top_level.txt
```

### Comparing `xgi-0.5.6/CITATION.cff` & `xgi-0.5.7/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
   - family-names: Schwarze
     given-names: Alice
 
 cff-version: "1.1.0"
 license: "BSD-3"
 message: "If you use this software, please cite it using these metadata."
 title: XGI
-version: "0.5.6"
+version: "0.5.7"
```

### Comparing `xgi-0.5.6/CODE_OF_CONDUCT.md` & `xgi-0.5.7/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 Community members asked to stop any inappropriate behavior are expected to comply immediately.
 
 
 ## XGI Community Online Spaces
 
 This Code of Conduct applies to the following online spaces:
 
-- The [XGI GitHub Project](https://github.com/ComplexGroupInteractions/xgi)
+- The [XGI GitHub Project](https://github.com/xgi-org/xgi)
 
 This Code of Conduct applies to every member in official XGI Community online spaces, including:
 
 - Moderators
 
 - Maintainers
```

### Comparing `xgi-0.5.6/CONTRIBUTING.md` & `xgi-0.5.7/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 8. [Optional, but STRONGLY preferred] Run `black .` for consistent styling.
 9. Update the "Current Version" section of CHANGELOG.md with overview of changes to the interface and add the usernames of all contributors.
 10. Submit Pull Request with a list of changes, links to issues that it addresses (if applicable)
 11. You may merge the Pull Request in once you have the sign-off of at least one other developer, or if you do not have permission to do that, you may request the reviewer to merge it for you.
 
 ## New Version process
 1. Make sure that the Github Actions workflow runs without any errors.
-2. Using the `github-changelog` package (a dependency in the [release](requirements/release.txt) requirements file), run `changelog -m ComplexGroupInteractions xgi [last release tag]` to get the merged pull requests with their links. Paste this into the changelog file under a new heading and edit to make more legible. Associate a GitHub username with each pull request.
+2. Using the `github-changelog` package (a dependency in the [release](requirements/release.txt) requirements file), run `changelog -m xgi-org xgi [last release tag]` to get the merged pull requests with their links. Paste this into the changelog file under a new heading and edit to make more legible. Associate a GitHub username with each pull request.
 3. Increase the version number in [setup.py](setup.py), [conf.py](docs/source/conf.py), and [CITATION.cff](CITATION.cff) to the new version agreed upon by the core developers. The versioning scheme we use is [SemVer](http://semver.org/).
 4. Commit these changes.
 5. Create a new release on GitHub by selecting "Releases", then clicking "Draft a new release". Click "Choose a tag" and type "v" followed by the version number and then click "Create new tag". The release title will be this same string. Paste the contents of the CHANGELOG into the "Describe this release" field. Click "Publish release".
 6. Run `python setup.py sdist` from the main folder. This will create a zipped file to upload to PyPI and save it to the "dist" folder.
 6. Using `twine` (a dependency in the [release](requirements/release.txt) requirements file), run `twine upload dist/xgi-[version number].tar.gz`. Enter your username and password.
 4. The new version is now on PyPI.
```

### Comparing `xgi-0.5.6/LICENSE.md` & `xgi-0.5.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/PKG-INFO` & `xgi-0.5.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: xgi
-Version: 0.5.6
+Version: 0.5.7
 Summary: XGI is a Python library for the representation
 Author: Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze
 Author-email: nicholas.landry@uvm.edu
 Project-URL: Documentation, https://xgi.readthedocs.io/en/latest/
-Project-URL: Bug Reports, https://github.com/ComplexGroupInteractions/xgi/issues
-Project-URL: Source, https://github.com/ComplexGroupInteractions/xgi
+Project-URL: Bug Reports, https://github.com/xgi-org/xgi/issues
+Project-URL: Source, https://github.com/xgi-org/xgi
 Project-URL: PyPI, https://pypi.org/project/xgi/
-Project-URL: GitHub Discussions, https://github.com/ComplexGroupInteractions/xgi/discussions
+Project-URL: GitHub Discussions, https://github.com/xgi-org/xgi/discussions
 Provides-Extra: benchmarks
 Provides-Extra: developer
 Provides-Extra: documentation
 Provides-Extra: release
 Provides-Extra: test
 Provides-Extra: tutorial
 Provides-Extra: all
 License-File: LICENSE.md
 
 XGI
 ===
 
-.. image:: https://github.com/ComplexGroupInteractions/xgi/raw/main/logo/logo.svg
+.. image:: https://github.com/xgi-org/xgi/raw/main/logo/logo.svg
   :width: 200
 
 CompleX Group Interactions (XGI) is a Python package for the representation, manipulation,
 and study of the structure, dynamics, and functions of complex systems with group (higher-order) interactions.
 
 Installation
 ------------
@@ -42,41 +42,41 @@
 -  Run the following command::
 
    $ pip install -e .["all"]
 
 
 Getting Started
 ---------------
-To get started, take a look at the `tutorials <https://github.com/ComplexGroupInteractions/xgi/tree/main/tutorials>`_
+To get started, take a look at the `tutorials <https://github.com/xgi-org/xgi/tree/main/tutorials>`_
 illustrating the library's basic functionality.
 
 Contributing
 ------------
-Contributions are always welcome. Please report any bugs that you find `here <https://github.com/ComplexGroupInteractions/xgi/issues>`_.
-Or, even better, fork the repository on `GitHub <https://github.com/ComplexGroupInteractions/xgi>`_ and create a pull request (PR).
+Contributions are always welcome. Please report any bugs that you find `here <https://github.com/xgi-org/xgi/issues>`_.
+Or, even better, fork the repository on `GitHub <https://github.com/xgi-org/xgi>`_ and create a pull request (PR).
 We welcome all changes, big or small, and we will help you make the PR if you are new to `git`
-(just ask on the issue and/or see our `contributing guidelines <https://github.com/ComplexGroupInteractions/xgi/tree/main/CONTRIBUTING.md>`_.
+(just ask on the issue and/or see our `contributing guidelines <https://github.com/xgi-org/xgi/tree/main/CONTRIBUTING.md>`_.
 
 How to Cite
 -----------
 We acknowledge the importance of good software to support research, and we note
 that research becomes more valuable when it is communicated effectively. To
 demonstrate the value of XGI, we ask that you cite XGI in your work.
 Currently, the best way to cite XGI is to go to our
-`repository page <https://github.com/ComplexGroupInteractions/xgi>`_ and
+`repository page <https://github.com/xgi-org/xgi>`_ and
 click the "cite this repository" button on the right sidebar. This will generate
 a citation in your preferred format, and will also integrate well with citation managers.
 
 Code of Conduct
 ---------------
-Our full code of conduct, and how we enforce it, can be read in `our repository <https://github.com/ComplexGroupInteractions/xgi/tree/main/CODE_OF_CONDUCT.md>`_.
+Our full code of conduct, and how we enforce it, can be read in `our repository <https://github.com/xgi-org/xgi/tree/main/CODE_OF_CONDUCT.md>`_.
 
 License
 -------
-Released under the 3-Clause BSD license (see the `license file <https://github.com/ComplexGroupInteractions/xgi/tree/main/license.md>`_)
+Released under the 3-Clause BSD license (see the `license file <https://github.com/xgi-org/xgi/tree/main/license.md>`_)
 
 Copyright (C) 2021-2023 XGI Developers
 
 Nicholas Landry <nicholas.landry@colorado.edu>
 
 Leo Torres <leo@leotrs.com>
```

### Comparing `xgi-0.5.6/README.md` & `xgi-0.5.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # XGI
 <img src='logo/logo.svg' width='150px' align="right" style="float:right;margin-left:10pt"></img>
 Comple**X** **G**roup **I**nteractions (**XGI**) is a Python package for the representation, manipulation, and study of the structure, dynamics, and functions of complex systems with group (higher-order) interactions.
 
-[![Test Status](https://github.com/ComplexGroupInteractions/xgi/workflows/test/badge.svg?branch=main)](https://github.com/ComplexGroupInteractions/xgi/actions?query=workflow%3A%22test%22)
-[![codecov](https://codecov.io/gh/ComplexGroupInteractions/xgi/branch/main/graph/badge.svg?token=BI6TX2WDSG)](https://codecov.io/gh/ComplexGroupInteractions/xgi)
-[![Good First Issue](https://img.shields.io/badge/contribute-Good%20First%20Issue-%232EBC4F)](https://github.com/ComplexGroupInteractions/xgi/issues?q=is%3Aopen+is%3Aissue+label%3A%22Good+First+Issue%22)
+[![Test Status](https://github.com/xgi-org/xgi/workflows/test/badge.svg?branch=main)](https://github.com/xgi-org/xgi/actions?query=workflow%3A%22test%22)
+[![codecov](https://codecov.io/gh/xgi-org/xgi/branch/main/graph/badge.svg?token=BI6TX2WDSG)](https://codecov.io/gh/xgi-org/xgi)
+[![Good First Issue](https://img.shields.io/badge/contribute-Good%20First%20Issue-%232EBC4F)](https://github.com/xgi-org/xgi/issues?q=is%3Aopen+is%3Aissue+label%3A%22Good+First+Issue%22)
 
 * [**Source**](../../)
 * [**Bug reports**](../../issues)
 * [**GitHub Discussions**](../../discussions)
 * [**Documentation**](https://xgi.readthedocs.io/en/latest/)
 
 Sign up for our [mailing list](http://eepurl.com/igE6ez) and follow XGI on [Twitter](https://twitter.com/xginets) or [Mastodon](https://mathstodon.xyz/@xginets)!
@@ -59,15 +59,15 @@
 
 ## Contributing
 If you want to contribute to this project, please make sure to read the
 [code of conduct](CODE_OF_CONDUCT.md)
 and the [contributing guidelines](CONTRIBUTING.md).
 
 The best way to contribute to XGI is by submitting a bug or request a new feature by
-opening a [new issue](https://github.com/ComplexGroupInteractions/xgi/issues/new).
+opening a [new issue](https://github.com/xgi-org/xgi/issues/new).
 
 To get more actively involved, you are invited to browse the [issues page](../../issues) and choose one that you can
 work on.  The core developers will be happy to help you understand the codebase and any
 other doubts you may have while working on your contribution.
 
 If you are interested in the daily goings-on of XGI, you are invited to join our [Zulip
 channel](https://xgi.zulipchat.com/join/7agfwo7dh7jo56ppnk5kc23r/).
```

### Comparing `xgi-0.5.6/logo/logo.pdf` & `xgi-0.5.7/logo/logo.pdf`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/logo/logo.png` & `xgi-0.5.7/logo/logo.png`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/logo/logo.svg` & `xgi-0.5.7/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/long_description.rst` & `xgi-0.5.7/long_description.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 XGI
 ===
 
-.. image:: https://github.com/ComplexGroupInteractions/xgi/raw/main/logo/logo.svg
+.. image:: https://github.com/xgi-org/xgi/raw/main/logo/logo.svg
   :width: 200
 
 CompleX Group Interactions (XGI) is a Python package for the representation, manipulation,
 and study of the structure, dynamics, and functions of complex systems with group (higher-order) interactions.
 
 Installation
 ------------
@@ -22,41 +22,41 @@
 -  Run the following command::
 
    $ pip install -e .["all"]
 
 
 Getting Started
 ---------------
-To get started, take a look at the `tutorials <https://github.com/ComplexGroupInteractions/xgi/tree/main/tutorials>`_
+To get started, take a look at the `tutorials <https://github.com/xgi-org/xgi/tree/main/tutorials>`_
 illustrating the library's basic functionality.
 
 Contributing
 ------------
-Contributions are always welcome. Please report any bugs that you find `here <https://github.com/ComplexGroupInteractions/xgi/issues>`_.
-Or, even better, fork the repository on `GitHub <https://github.com/ComplexGroupInteractions/xgi>`_ and create a pull request (PR).
+Contributions are always welcome. Please report any bugs that you find `here <https://github.com/xgi-org/xgi/issues>`_.
+Or, even better, fork the repository on `GitHub <https://github.com/xgi-org/xgi>`_ and create a pull request (PR).
 We welcome all changes, big or small, and we will help you make the PR if you are new to `git`
-(just ask on the issue and/or see our `contributing guidelines <https://github.com/ComplexGroupInteractions/xgi/tree/main/CONTRIBUTING.md>`_.
+(just ask on the issue and/or see our `contributing guidelines <https://github.com/xgi-org/xgi/tree/main/CONTRIBUTING.md>`_.
 
 How to Cite
 -----------
 We acknowledge the importance of good software to support research, and we note
 that research becomes more valuable when it is communicated effectively. To
 demonstrate the value of XGI, we ask that you cite XGI in your work.
 Currently, the best way to cite XGI is to go to our
-`repository page <https://github.com/ComplexGroupInteractions/xgi>`_ and
+`repository page <https://github.com/xgi-org/xgi>`_ and
 click the "cite this repository" button on the right sidebar. This will generate
 a citation in your preferred format, and will also integrate well with citation managers.
 
 Code of Conduct
 ---------------
-Our full code of conduct, and how we enforce it, can be read in `our repository <https://github.com/ComplexGroupInteractions/xgi/tree/main/CODE_OF_CONDUCT.md>`_.
+Our full code of conduct, and how we enforce it, can be read in `our repository <https://github.com/xgi-org/xgi/tree/main/CODE_OF_CONDUCT.md>`_.
 
 License
 -------
-Released under the 3-Clause BSD license (see the `license file <https://github.com/ComplexGroupInteractions/xgi/tree/main/license.md>`_)
+Released under the 3-Clause BSD license (see the `license file <https://github.com/xgi-org/xgi/tree/main/license.md>`_)
 
 Copyright (C) 2021-2023 XGI Developers
 
 Nicholas Landry <nicholas.landry@colorado.edu>
 
 Leo Torres <leo@leotrs.com>
```

### Comparing `xgi-0.5.6/requirements/README.md` & `xgi-0.5.7/requirements/README.md`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/setup.py` & `xgi-0.5.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import sys
 
 import setuptools
 from setuptools import setup
 
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 
 if sys.version_info < (3, 8):
     sys.exit("XGI requires Python 3.8 or later.")
 
 name = "xgi"
 
 version = __version__
 
 authors = "Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze"
 
 author_email = "nicholas.landry@uvm.edu"
 
 project_urls = {
     "Documentation": "https://xgi.readthedocs.io/en/latest/",
-    "Bug Reports": "https://github.com/ComplexGroupInteractions/xgi/issues",
-    "Source": "https://github.com/ComplexGroupInteractions/xgi",
+    "Bug Reports": "https://github.com/xgi-org/xgi/issues",
+    "Source": "https://github.com/xgi-org/xgi",
     "PyPI": "https://pypi.org/project/xgi/",
-    "GitHub Discussions": "https://github.com/ComplexGroupInteractions/xgi/discussions",
+    "GitHub Discussions": "https://github.com/xgi-org/xgi/discussions",
 }
 
 description = """XGI is a Python library for the representation
 and analysis of complex systems with group (higher-order) interactions."""
 
 with open("long_description.rst") as file:
     long_description = file.read()
```

### Comparing `xgi-0.5.6/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb` & `xgi-0.5.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/tutorials/Tutorial 2 - Read and Write.ipynb` & `xgi-0.5.7/tutorials/Tutorial 2 - Read and Write.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb` & `xgi-0.5.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/tutorials/Tutorial 4 - Generative_Models.ipynb` & `xgi-0.5.7/tutorials/Tutorial 4 - Generative_Models.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/tutorials/Tutorial 5 - Plotting.ipynb` & `xgi-0.5.7/tutorials/Tutorial 5 - Plotting.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991170634920635%*

 * *Differences: {"'cells'": "{11: {delete: ['attachments']}, 13: {delete: ['attachments']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'version': '3.9.13'}}"}*

```diff
@@ -182,15 +182,14 @@
                 }
             ],
             "source": [
                 "xgi.draw(H, pos, node_labels=True, hyperedge_labels=True)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "bad32b53",
             "metadata": {},
             "source": [
                 "For some hypergraphs, it can be helpful to rotate the positions of the nodes relative to the principal axis. We can do this by generating node positions with any of the functions previously described and then using the function `pca_transform()`. For example:"
             ]
         },
@@ -223,15 +222,14 @@
             ],
             "source": [
                 "transformed_pos = xgi.pca_transform(pos)\n",
                 "xgi.draw(H, transformed_pos)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "fc7cf849",
             "metadata": {},
             "source": [
                 "We can also rotate the node positions relative to the principal axis:"
             ]
         },
@@ -668,27 +666,27 @@
                 "ax.set_xlabel(\"Degree\")\n",
                 "ax.set_xticks(np.arange(1, max(centers) + 1, step=1));"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "hyper",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.0"
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xgi-0.5.6/tutorials/Tutorial 6 - Statistics.ipynb` & `xgi-0.5.7/tutorials/Tutorial 6 - Statistics.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994368399908172%*

 * *Differences: {"'cells'": '{47: {\'source\': [\'(\\n\', \'    H.nodes.filterby("degree", 2)\\n\', \'    '*

 * *            '.filterby_attr("color", "blue")\\n\', \'    .clustering_coefficient.asdict()\\n\', '*

 * *            '\')\']}, 57: {\'source\': [\'H.nodes.multi(["degree", "clustering_coefficient"])\']}, '*

 * *            '59: {\'source\': [\'H.nodes.multi(["degree", "clustering_coefficient"]).asdict()\']}, '*

 * *            '61: {\'source\': {insert: [(0, \'ms = H.nodes.multi(["degree", '*

 * *            '"clustering_coefficient"])\\n […]*

```diff
@@ -706,15 +706,19 @@
                     },
                     "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "(H.nodes.filterby(\"degree\", 2).filterby_attr(\"color\", \"blue\").clustering.asdict())"
+                "(\n",
+                "    H.nodes.filterby(\"degree\", 2)\n",
+                "    .filterby_attr(\"color\", \"blue\")\n",
+                "    .clustering_coefficient.asdict()\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d830bb95",
             "metadata": {},
             "source": [
@@ -844,15 +848,15 @@
                     },
                     "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "H.nodes.multi([\"degree\", \"clustering\"])"
+                "H.nodes.multi([\"degree\", \"clustering_coefficient\"])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "741b381a",
             "metadata": {},
             "source": [
@@ -879,15 +883,15 @@
                     },
                     "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "H.nodes.multi([\"degree\", \"clustering\"]).asdict()"
+                "H.nodes.multi([\"degree\", \"clustering_coefficient\"]).asdict()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4cdb4bd5",
             "metadata": {},
             "source": [
@@ -930,15 +934,15 @@
                         " {'clustering': 1.3333333333333333, 'degree': 3},\n",
                         " {'clustering': 3.0, 'degree': 2},\n",
                         " {'clustering': 3.0, 'degree': 2}]\n"
                     ]
                 }
             ],
             "source": [
-                "ms = H.nodes.multi([\"degree\", \"clustering\"])\n",
+                "ms = H.nodes.multi([\"degree\", \"clustering_coefficient\"])\n",
                 "\n",
                 "from pprint import pprint\n",
                 "\n",
                 "print(\"# dict of dicts, nodes first:\")\n",
                 "pprint(ms.asdict())\n",
                 "print()\n",
                 "print(\"# dict of dicts, stats first:\")\n",
@@ -1045,15 +1049,15 @@
                     },
                     "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df = H.nodes.multi([\"degree\", \"clustering\"]).aspandas()\n",
+                "df = H.nodes.multi([\"degree\", \"clustering_coefficient\"]).aspandas()\n",
                 "df"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "25357b7b",
             "metadata": {},
@@ -1153,15 +1157,15 @@
                     "metadata": {
                         "needs_background": "light"
                     },
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "H.nodes.multi([\"degree\", \"clustering\"]).aspandas().plot();"
+                "H.nodes.multi([\"degree\", \"clustering_coefficient\"]).aspandas().plot();"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "977c336f",
             "metadata": {},
             "source": [
```

### Comparing `xgi-0.5.6/tutorials/case_study_zhang2022.ipynb` & `xgi-0.5.7/tutorials/case_study_zhang2022.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/tutorials/quickstart.ipynb` & `xgi-0.5.7/tutorials/quickstart.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997702205882353%*

 * *Differences: {"'cells'": '{55: {\'source\': [\'H_stats.nodes.multi(["degree", '*

 * *            '"clustering_coefficient"]).aspandas().groupby(\\n\', \'    "degree"\\n\', '*

 * *            '\').agg("mean")\']}, 56: {\'source\': {insert: [(1, \'    '*

 * *            'H_stats.nodes.multi(["degree", "clustering_coefficient", '*

 * *            '"average_neighbor_degree"])\\n\')], delete: [1]}}}'}*

```diff
@@ -601,25 +601,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "H_stats.nodes.multi([\"degree\", \"clustering\"]).aspandas().groupby(\"degree\").agg(\"mean\")"
+                "H_stats.nodes.multi([\"degree\", \"clustering_coefficient\"]).aspandas().groupby(\n",
+                "    \"degree\"\n",
+                ").agg(\"mean\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "(\n",
-                "    H_stats.nodes.multi([\"degree\", \"clustering\", \"average_neighbor_degree\"])\n",
+                "    H_stats.nodes.multi([\"degree\", \"clustering_coefficient\", \"average_neighbor_degree\"])\n",
                 "    .aspandas()\n",
                 "    .groupby(\"degree\")\n",
                 "    .agg(\"mean\")\n",
                 "    .plot(marker=\"o\")\n",
                 ")"
             ]
         },
```

### Comparing `xgi-0.5.6/tutorials/simplicial_kuramoto_example.ipynb` & `xgi-0.5.7/tutorials/simplicial_kuramoto_example.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/algorithms/assortativity.py` & `xgi-0.5.7/xgi/algorithms/assortativity.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/algorithms/centrality.py` & `xgi-0.5.7/xgi/algorithms/centrality.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 from ..classes import convert_labels_to_integers, is_uniform
 from ..convert import to_line_graph
 from ..exception import XGIError
 from ..linalg import clique_motif_matrix, incidence_matrix
 
 __all__ = [
-    "CEC_centrality",
-    "HEC_centrality",
+    "clique_eigenvector_centrality",
+    "h_eigenvector_centrality",
     "node_edge_centrality",
     "line_vector_centrality",
 ]
 
 
-def CEC_centrality(H, tol=1e-6):
-    """Compute the CEC centrality of a hypergraph.
+def clique_eigenvector_centrality(H, tol=1e-6):
+    """Compute the clique motif eigenvector centrality of a hypergraph.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest.
     tol : float, default: 1e-6
         The tolerance when computing the eigenvector.
@@ -43,27 +43,27 @@
     """
     from ..algorithms import is_connected
 
     # if there aren't any nodes, return an empty dict
     if H.num_nodes == 0:
         return dict()
     # if the hypergraph is not connected,
-    # this metric doesn't make sense and should return NaN.
+    # this metric doesn't make sense and should return nan.
     if not is_connected(H):
-        return {n: np.NaN for n in H.nodes}
+        return {n: np.nan for n in H.nodes}
     W, node_dict = clique_motif_matrix(H, index=True)
     _, v = eigsh(W.asfptype(), k=1, which="LM", tol=tol)
 
     # multiply by the sign to try and enforce positivity
     v = np.sign(v[0]) * v / norm(v, 1)
     return {node_dict[n]: v[n].item() for n in node_dict}
 
 
-def HEC_centrality(H, max_iter=100, tol=1e-6):
-    """Compute the HEC centrality of a uniform hypergraph.
+def h_eigenvector_centrality(H, max_iter=100, tol=1e-6):
+    """Compute the H-eigenvector centrality of a uniform hypergraph.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest.
     max_iter : int, default: 100
         The maximum number of iterations before the algorithm terminates.
@@ -89,17 +89,17 @@
     """
     from ..algorithms import is_connected
 
     # if there aren't any nodes, return an empty dict
     if H.num_nodes == 0:
         return dict()
     # if the hypergraph is not connected,
-    # this metric doesn't make sense and should return NaN.
+    # this metric doesn't make sense and should return nan.
     if not is_connected(H):
-        return {n: np.NaN for n in H.nodes}
+        return {n: np.nan for n in H.nodes}
 
     m = is_uniform(H)
     if not m:
         raise XGIError("This method is not defined for non-uniform hypergraphs.")
 
     new_H = convert_labels_to_integers(H, "old-label")
 
@@ -201,19 +201,19 @@
     Francesco Tudisco & Desmond J. Higham,
     https://doi.org/10.1038/s42005-021-00704-2
     """
     from ..algorithms import is_connected
 
     # if there aren't any nodes or edges, return an empty dict
     if H.num_nodes == 0 or H.num_edges == 0 or not is_connected(H):
-        return {n: np.NaN for n in H.nodes}, {e: np.NaN for e in H.edges}
+        return {n: np.nan for n in H.nodes}, {e: np.nan for e in H.edges}
     # if the hypergraph is not connected,
-    # this metric doesn't make sense and should return NaN.
+    # this metric doesn't make sense and should return nan.
     # if not is_connected(H):
-    #     return {n: np.NaN for n in H.nodes}, {e: np.NaN for e in H.edges}
+    #     return {n: np.nan for n in H.nodes}, {e: np.nan for e in H.edges}
 
     n = H.num_nodes
     m = H.num_edges
     x = np.ones(n) / n
     y = np.ones(m) / m
 
     I, node_dict, edge_dict = incidence_matrix(H, index=True)
```

### Comparing `xgi-0.5.6/xgi/algorithms/connected.py` & `xgi-0.5.7/xgi/algorithms/connected.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/classes/function.py` & `xgi-0.5.7/xgi/classes/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "is_frozen",
     "create_empty_copy",
     "set_node_attributes",
     "get_node_attributes",
     "set_edge_attributes",
     "get_edge_attributes",
     "is_empty",
-    "maximal_simplices",
     "convert_labels_to_integers",
     "density",
     "incidence_density",
     "subfaces",
 ]
 
 
@@ -173,15 +172,17 @@
     if include_self:
         return [H.edges.members(e) for e in H.nodes.memberships(n)]
     else:
         return [H.edges.members(e) - {n} for e in H.nodes.memberships(n)]
 
 
 def degree_counts(H, order=None):
-    """Returns a list of the frequency of each degree value.
+    """Returns a list of the the number of occurrences of each degree value.
+
+    The counts correspond to degrees from 0 to max(degree).
 
     Parameters
     ----------
     H : Hypergraph object
         The hypergraph of interest
     order: int, optional
         Order of edges to take into account. If None (default),
@@ -194,14 +195,18 @@
         The degree values are the index in the list.
 
     Notes
     -----
     Note: the bins are width one, hence len(list) can be large
     (Order(num_edges))
 
+    The degree is defined as the number of edges to which a node belongs.
+    A node belonging only to a singleton edge will thus have degree 1 and
+    contribute accordingly to the degree count.
+
     Examples
     --------
     >>> import xgi
     >>> hyperedge_list = [[1, 2], [2, 3, 4]]
     >>> H = xgi.Hypergraph(hyperedge_list)
     >>> xgi.degree_counts(H)
     [0, 3, 1]
@@ -611,48 +616,14 @@
     >>> H = xgi.Hypergraph(hyperedge_list)
     >>> xgi.is_empty(H)
     False
     """
     return len(H.edges) == 0
 
 
-def maximal_simplices(SC):
-    """Return the IDs of the maximal simplices of the input.
-
-    Parameters
-    ----------
-    SC : xgi SimplicialComplex
-
-    Returns
-    -------
-    maximal_simplices : list(int)
-        A list of IDs correspondent to the maximal simplices in `SC`.
-
-    """
-    # This import needs to happen when this function is called, not when it is
-    # defined.  Otherwise, a circular import error would happen.
-    from .simplicialcomplex import SimplicialComplex
-
-    if not isinstance(SC, SimplicialComplex):
-        raise XGIError("The input must be a SimplicialComplex")
-
-    max_simplices = []
-
-    for i in SC.edges:
-        maximal = True
-        for j in SC.edges:
-            # i is a subface of j, I remove it
-            if SC.edges.members(i) < SC.edges.members(j):
-                maximal = False
-                break
-        if maximal:
-            max_simplices.append(i)
-    return max_simplices
-
-
 def convert_labels_to_integers(H, label_attribute="label"):
     """Relabel node and edge IDs to be sequential integers.
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest
```

### Comparing `xgi-0.5.6/xgi/classes/hypergraph.py` & `xgi-0.5.7/xgi/classes/hypergraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     The `attr` keyword arguments are added as hypergraph attributes. To add node or edge
     attributes see :meth:`add_node` and :meth:`add_edge`.
 
     In addition to the methods listed in this page, other methods defined in the `stats`
     package are also accessible via the `Hypergraph` class.  For more details, see the
     `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     Examples
     --------
     >>> import xgi
     >>> H = xgi.Hypergraph([[1, 2, 3], [4], [5, 6], [6, 7, 8]])
     >>> H.nodes
     NodeView((1, 2, 3, 4, 5, 6, 7, 8))
```

### Comparing `xgi-0.5.6/xgi/classes/hypergraphviews.py` & `xgi-0.5.7/xgi/classes/hypergraphviews.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/classes/reportviews.py` & `xgi-0.5.7/xgi/classes/reportviews.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 allow modification.  This module provides View classes for nodes, edges, degree, and
 edge size of a hypergraph.  Views are automatically updaed when the hypergraph changes.
 
 """
 
 from collections import defaultdict
 from collections.abc import Mapping, Set
+from functools import reduce
 
 from ..exception import IDNotFound, XGIError
 from ..stats import IDStat, dispatch_many_stats, dispatch_stat
 
 __all__ = [
     "NodeView",
     "EdgeView",
@@ -201,15 +202,15 @@
             * 'geq': Return IDs whose value is greater than or equal to `val`.
             * 'between': In this mode, `val` must be a tuple `(val1, val2)`.  Return IDs
               whose value `v` satisfies `val1 <= v <= val2`.
 
         See Also
         --------
         For more details, see the `tutorial
-        <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+        <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
         Examples
         --------
         By default, return the IDs whose value of the statistic is exactly equal to
         `val`.
 
         >>> import xgi
@@ -284,15 +285,15 @@
             The default value if the attribute is missing. If None,
             ignores those IDs.
 
 
         See Also
         --------
         Works identically to `filterby`.  For more details, see the `tutorial
-        <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+        <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
         Notes
         -----
         Beware of using comparison modes ("lt", "gt", "leq", "geq")
         when the attribute is a string. For example, the string comparison
         `'10' < '9'` evaluates to `True`.
         """
@@ -416,15 +417,18 @@
         """
         dups = []
         hashes = defaultdict(list)
         for idx, members in self._id_dict.items():
             hashes[frozenset(members)].append(idx)
         for _, edges in hashes.items():
             if len(edges) > 1:
-                dups.extend(sorted(edges)[1:])
+                try:
+                    dups.extend(sorted(edges)[1:])
+                except TypeError:
+                    dups.extend(edges[1:])
         return self.__class__.from_view(self, bunch=dups)
 
     def lookup(self, neighbors):
         """Find IDs with the specified bipartite neighbors.
 
         Parameters
         ----------
@@ -525,15 +529,15 @@
         The node ids to keep track of.  If None (default), keep track of all node ids.
 
     Notes
     -----
     In addition to the methods listed in this page, other methods defined in the `stats`
     package are also accessible via the `NodeView` class.  For more details, see the
     `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     _id_kind = "node"
 
     def __init__(self, H, bunch=None):
         if H is None:
@@ -617,15 +621,15 @@
         The edge ids to keep track of.  If None (default), keep track of all edge ids.
 
     Notes
     -----
     In addition to the methods listed in this page, other methods defined in the `stats`
     package are also accessible via the `EdgeView` class.  For more details, see the
     `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     _id_kind = "edge"
 
     def __init__(self, H, bunch=None):
         if H is None:
@@ -684,7 +688,59 @@
 
         See Also
         --------
         :meth:`NodeView.isolates`
 
         """
         return self.filterby("size", 1)
+
+    def maximal(self):
+        """Returns the maximal edges as an EdgeView. Maximal edges are those that are not subsets of any other edges in the hypergraph.
+
+        Returns
+        -------
+        EdgeView
+            The maximal edges
+
+        Notes
+        -----
+        When there are maximal edges that are also multi-edges,
+        `maximal()` returns all of these multi-edges rather than
+        choosing one of them to return. There are methods for
+        eliminating these duplicates by running `H.cleanup()`
+        or `H.remove_edges_from(H.edges.duplicates())`
+
+        References
+        ----------
+        https://stackoverflow.com/questions/14106121/efficient-algorithm-for-finding-all-maximal-subsets
+
+        Example
+        -------
+
+        >>> import xgi
+        >>> H = xgi.Hypergraph([{1, 2, 3},{1, 2}, {2, 3}, {2}, {2}, {3, 4}, {1, 2, 3}])
+        >>> H.edges.maximal()
+        EdgeView((0, 5, 6))
+        >>> H.edges.maximal().members()
+        [{1, 2, 3}, {3, 4}, {1, 2, 3}]
+        """
+        edges = self._id_dict
+        nodes = self._bi_id_dict
+        max_edges = set()
+
+        # This data structure so that the algorithm can handle multi-edges
+        dups = defaultdict(list)
+        for idx, members in edges.items():
+            dups[frozenset(members)].append(idx)
+
+        _intersection = lambda x, y: x & y
+
+        for i, e in edges.items():
+            # If a multi-edge has already been added to the set of
+            # maximal edges, we don't need to check.
+            if i not in max_edges:
+                in_common = reduce(_intersection, (nodes[n] for n in e))
+
+                if in_common == set(dups[frozenset(e)]):
+                    max_edges.update(in_common)
+
+        return self.from_view(self, bunch=max_edges)
```

### Comparing `xgi-0.5.6/xgi/classes/simplicialcomplex.py` & `xgi-0.5.7/xgi/classes/simplicialcomplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,18 @@
             may be a dict of the form `{simplex_id: simplex_members}` (Format 5).
 
             Formats 2 and 3 are unambiguous because `attr` dicts are not hashable, while `id`s must be.
             In Formats 2-4, each element of `ebunch_to_add` must have the same length,
             i.e. you cannot mix different formats.  The iterables containing simplex
             members cannot be strings.
 
+        max_order : None or int
+            Maximal dimension of simplices to add. If None (default), adds all simplices.
+            If int, and `ebunch_to_add` contains simplices of order > `max_order`, creates
+            and adds all its subfaces up to `max_order`.
         attr : \*\*kwargs, optional
             Additional attributes to be assigned to all simplices. Attribues specified via
             `ebunch_to_add` take precedence over `attr`.
 
         See Also
         --------
         add_simplex : add a single simplex
```

### Comparing `xgi-0.5.6/xgi/convert.py` & `xgi-0.5.7/xgi/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,15 @@
     csc_matrix,
     csr_array,
     csr_matrix,
     lil_array,
     lil_matrix,
 )
 
-from .classes import (
-    Hypergraph,
-    SimplicialComplex,
-    maximal_simplices,
-    set_edge_attributes,
-)
+from .classes import Hypergraph, SimplicialComplex, set_edge_attributes
 from .exception import XGIError
 from .generators import empty_hypergraph, empty_simplicial_complex
 from .linalg import adjacency_matrix, incidence_matrix
 from .utils.utilities import dual_dict
 
 __all__ = [
     "convert_to_hypergraph",
@@ -496,15 +491,15 @@
     -------
     Hypergraph
 
     """
     if type(SC) != SimplicialComplex:
         raise XGIError("The input must be a SimplicialComplex")
 
-    max_simplices = maximal_simplices(SC)
+    max_simplices = SC.edges.maximal()
     H = Hypergraph()
     H.add_nodes_from(SC.nodes)  # to keep node order and isolated nodes
     H.add_edges_from([list(SC.edges.members(e)) for e in max_simplices])
     return H
 
 
 def to_incidence_matrix(H, sparse=True, index=False):
@@ -609,56 +604,64 @@
     H.add_nodes_from(nodes)
     for edge in edges:
         nodes_in_edge = list(G.neighbors(edge))
         H.add_edge(nodes_in_edge, id=edge)
     return H.dual() if dual else H
 
 
-def to_bipartite_graph(H):
-    """
-    Create a NetworkX bipartite network from a hypergraph.
+def to_bipartite_graph(H, index=False):
+    """Create a NetworkX bipartite network from a hypergraph.
 
     Parameters
     ----------
     H: xgi.Hypergraph
         The XGI hypergraph object of interest
+    index: bool (default False)
+        If False (default), return only the graph.  If True, additionally return the
+        index-to-node and index-to-edge mappings.
 
     Returns
     -------
-    nx.Graph
-        The resulting equivalent bipartite graph
+    nx.Graph[, dict, dict]
+        The resulting equivalent bipartite graph, and optionally the index-to-unit
+        mappings.
 
     References
     ----------
     The Why, How, and When of Representations for Complex Systems,
     Leo Torres, Ann S. Blevins, Danielle Bassett, and Tina Eliassi-Rad,
     https://doi.org/10.1137/20M1355896
 
     Examples
     --------
     >>> import xgi
     >>> hyperedge_list = [[1, 2], [2, 3, 4]]
     >>> H = xgi.Hypergraph(hyperedge_list)
     >>> G = xgi.to_bipartite_graph(H)
+    >>> G, itn, ite = xgi.to_bipartite_graph(H, index=True)
+
     """
     G = nx.Graph()
 
     node_dict = dict(zip(H.nodes, range(H.num_nodes)))
     edge_dict = dict(zip(H.edges, range(H.num_nodes, H.num_nodes + H.num_edges)))
     G.add_nodes_from(node_dict.values(), bipartite=0)
     G.add_nodes_from(edge_dict.values(), bipartite=1)
     for node in H.nodes:
         for edge in H.nodes.memberships(node):
             G.add_edge(node_dict[node], edge_dict[edge])
 
-    return (
-        G,
-        dict(zip(range(H.num_nodes), H.nodes)),
-        dict(zip(range(H.num_nodes, H.num_nodes + H.num_edges), H.edges)),
-    )
+    if index:
+        return (
+            G,
+            dict(zip(range(H.num_nodes), H.nodes)),
+            dict(zip(range(H.num_nodes, H.num_nodes + H.num_edges), H.edges)),
+        )
+    else:
+        return G
 
 
 def dict_to_hypergraph(data, nodetype=None, edgetype=None, max_order=None):
     """
     A function to read a file in a standardized JSON format.
 
     Parameters
```

### Comparing `xgi-0.5.6/xgi/drawing/draw.py` & `xgi-0.5.7/xgi/drawing/draw.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from inspect import signature
 from itertools import combinations
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import cm
 from matplotlib.colors import LinearSegmentedColormap, ListedColormap
+from scipy.spatial import ConvexHull
 
 from .. import convert
 from ..classes import Hypergraph, SimplicialComplex, max_edge_order
 from ..exception import XGIError
 from ..stats import EdgeStat, NodeStat
 from .layout import barycenter_spring_layout
 
 __all__ = [
     "draw",
     "draw_nodes",
     "draw_hyperedges",
     "draw_simplices",
     "draw_node_labels",
     "draw_hyperedge_labels",
+    "draw_hypergraph_hull",
 ]
 
 
 def draw(
     H,
     pos=None,
     ax=None,
@@ -42,18 +44,20 @@
     **kwargs,
 ):
     """Draw hypergraph or simplicial complex.
 
     Parameters
     ----
     H : Hypergraph or SimplicialComplex.
+        Hypergraph to draw
     pos : dict (default=None)
         If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
         If None (default), use the `barycenter_spring_layout` to compute the positions.
     ax : matplotlib.pyplot.axes (default=None)
+        Axis to draw on
     dyad_color : str, dict, iterable, or EdgeStat (default='black')
         Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
         contain (edge_id: color_str) pairs.  If iterable, assume the colors are
         specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
         (specified with dyad_color_cmap) associated to it.
     dyad_lw : int, float, dict, iterable, or EdgeStat (default=1.5)
         Line width of edges of order 1 (dyadic links).  If int or float, use the same width for all edges.
@@ -216,14 +220,15 @@
     """Draw the nodes of a hypergraph
 
     Parameters
     ----------
     H : Hypergraph or SimplicialComplex
         Higher-order network to plot.
     ax : matplotlib.pyplot.axes
+        Axis to draw on
     pos : dict (default=None)
         If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
         If None (default), use the `barycenter_spring_layout` to compute the positions.
     node_fc : str, dict, iterable, or NodeStat (default='white')
         Color of the nodes.  If str, use the same color for all nodes.  If a dict, must
         contain (node_id: color_str) pairs.  If other iterable, assume the colors are
         specified in the same order as the nodes are found in H.nodes. If NodeStat,
@@ -348,14 +353,15 @@
 ):
     """Draw hyperedges.
 
     Parameters
     ----------
     H : Hypergraph
     ax : matplotlib.pyplot.axes
+        Axis to draw on
     pos : dict (default=None)
         If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
         If None (default), use the `barycenter_spring_layout` to compute the positions.
     dyad_color : str, dict, iterable, or EdgeStat (default='black')
         Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
         contain (edge_id: color_str) pairs.  If iterable, assume the colors are
         specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
@@ -492,15 +498,17 @@
     **kwargs,
 ):
     """Draw maximal simplices and pairwise faces.
 
     Parameters
     ----------
     SC : SimplicialComplex
+        Simplicial complex to draw
     ax : matplotlib.pyplot.axes
+        Axis to draw on
     pos : dict (default=None)
         If passed, this dictionary of positions node_id:(x,y) is used for placing the 0-simplices.
         If None (default), use the `barycenter_spring_layout` to compute the positions.
     dyad_color : str, dict, iterable, or EdgeStat
         Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
         contain (edge_id: color_str) pairs.  If iterable, assume the colors are
         specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
@@ -981,7 +989,245 @@
     h = maxy - miny
 
     # update view after drawing
     padx, pady = 0.05 * w, 0.05 * h
     corners = (minx - padx, miny - pady), (maxx + padx, maxy + pady)
     ax.update_datalim(corners)
     ax.autoscale_view()
+
+
+def _draw_hull(node_pos, ax, edges_ec, facecolor, alpha, zorder, radius):
+    """Draw a convex hull encompassing the nodes in node_pos
+
+    Parameters
+    ----------
+    node_pos : np.array
+        nx2 dimensional array containing positions of the nodes
+    ax : matplotlib.pyplot.axes
+    edges_ec : str
+        Color of the border of the convex hull
+    facecolor : str
+        Filling color of the convex hull
+    alpha : float
+        Transparency of the convex hull
+    radius : float
+        Radius of the convex hull in the vicinity of the nodes.
+
+    Returns
+    -------
+    ax : matplotlib.pyplot.axes
+
+    """
+
+    thetas = np.linspace(0, 2 * np.pi, num=100, endpoint=False)
+    offsets = radius * np.array([np.cos(thetas), np.sin(thetas)]).T
+    points = np.vstack([p + offsets for p in node_pos])
+    points = np.vstack([node_pos, points])
+
+    hull = ConvexHull(points)
+
+    for simplex in hull.simplices:
+        ax.plot(points[simplex, 0], points[simplex, 1], color=edges_ec, zorder=zorder)
+    ax.fill(
+        points[hull.vertices, 0],
+        points[hull.vertices, 1],
+        color=facecolor,
+        alpha=alpha,
+        zorder=zorder,
+    )
+
+    return ax
+
+
+def draw_hypergraph_hull(
+    H,
+    pos=None,
+    ax=None,
+    dyad_color="black",
+    edge_fc=None,
+    edge_ec=None,
+    node_fc="tab:blue",
+    node_ec="black",
+    node_lw=1,
+    node_size=7,
+    max_order=None,
+    node_labels=False,
+    hyperedge_labels=False,
+    radius=0.05,
+    **kwargs,
+):
+    """Draw hypergraphs displaying the hyperedges of order k>1 as convex hulls
+
+
+    Parameters
+    ----------
+    H : Hypergraph
+    pos : dict (default=None)
+        If passed, this dictionary of positions node_id:(x,y) is used for placing the nodes.
+        If None (default), use the `barycenter_spring_layout` to compute the positions.
+    ax : matplotlib.pyplot.axes (default=None)
+    dyad_color : str, dict, iterable, or EdgeStat (default='black')
+        Color of the dyadic links.  If str, use the same color for all edges. If a dict, must
+        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
+        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
+        (specified with dyad_color_cmap) associated to it.
+    edge_fc : str, dict, iterable, or EdgeStat (default=None)
+        str, dict, iterable, or EdgeStat (default=None)
+        Color of the hyperedges of order k>1.  If str, use the same color for all hyperedges of order k>1.  If a dict, must
+        contain (edge_id: color_str) pairs.  If other iterable, assume the colors are
+        specified in the same order as the hyperedges are found in H.edges. If EdgeStat,
+        use the colormap specified with edge_fc_cmap. If None (default),
+        use the H.edges.size.
+    edge_ec : str, dict, iterable, or EdgeStat (default=None)
+        Color of the borders of the hyperdges of order k>1.  If str, use the same color for all edges. If a dict, must
+        contain (edge_id: color_str) pairs.  If iterable, assume the colors are
+        specified in the same order as the edges are found in H.edges. If EdgeStat, use a colormap
+        (specified with edge_ec_cmap) associated to it. If None (default),
+        use the H.edges.size.
+    node_fc : node_fc : str, dict, iterable, or NodeStat (default='tab:blue')
+        Color of the nodes.  If str, use the same color for all nodes.  If a dict, must
+        contain (node_id: color_str) pairs.  If other iterable, assume the colors are
+        specified in the same order as the nodes are found in H.nodes. If NodeStat,
+        use the colormap specified with node_fc_cmap.
+    node_ec : str, dict, iterable, or NodeStat (default='black')
+        Color of node borders.  If str, use the same color for all nodes.  If a dict, must
+        contain (node_id: color_str) pairs.  If other iterable, assume the colors are
+        specified in the same order as the nodes are found in H.nodes. If NodeStat,
+        use the colormap specified with node_ec_cmap.
+    node_lw : int, float, dict, iterable, or EdgeStat (default=1)
+        Line width of the node borders in pixels.  If int or float, use the same width for all node borders.
+        If a dict, must contain (node_id: width) pairs.  If iterable, assume the widths are
+        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
+        linear interpolation defined between min_node_lw and max_node_lw.
+    node_size : int, float, dict, iterable, or NodeStat (default=7)
+        Radius of the nodes in pixels.  If int or float, use the same radius for all nodes.
+        If a dict, must contain (node_id: radius) pairs.  If iterable, assume the radiuses are
+        specified in the same order as the nodes are found in H.nodes. If NodeStat, use a monotonic
+        linear interpolation defined between min_node_size and max_node_size.
+    max_order : int (default=None)
+        Maximum of hyperedges to plot. If None (default), plots all orders.
+    node_labels : bool, or dict (default=False)
+        If True, draw ids on the nodes. If a dict, must contain (node_id: label) pairs.
+    hyperedge_labels : bool, or dict (default=False)
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label) pairs.
+    radius : float (deafault=0.05)
+        Radius of the convex hull in the vicinity of the nodes.
+    **kwargs : optional args
+        Alternate default values. Values that can be overwritten are the following:
+        * min_node_size
+        * max_node_size
+        * min_node_lw
+        * max_node_lw
+        * node_fc_cmap
+        * node_ec_cmap
+        * dyad_color_cmap
+        * edge_fc_cmap
+        * edge_ec_cmap
+        * alpha
+
+    Returns
+    -------
+    ax : matplotlib.pyplot.axes
+
+    """
+
+    settings = {
+        "min_node_size": 5.0,
+        "max_node_size": 30.0,
+        "min_node_lw": 1.0,
+        "max_node_lw": 5.0,
+        "node_fc_cmap": cm.Reds,
+        "node_ec_cmap": cm.Greys,
+        "dyad_color_cmap": cm.Greys,
+        "edge_fc_cmap": cm.Blues,
+        "edge_ec_cmap": cm.Greys,
+        "alpha": 0.4,
+    }
+
+    alpha = settings["alpha"]
+
+    if edge_fc is None:
+        edge_fc = H.edges.size
+
+    edge_fc = _color_arg_to_dict(edge_fc, H.edges, settings["edge_fc_cmap"])
+
+    if edge_ec is None:
+        edge_ec = H.edges.size
+
+    edge_ec = _color_arg_to_dict(edge_ec, H.edges, settings["edge_ec_cmap"])
+
+    settings.update(kwargs)
+
+    if pos is None:
+        pos = barycenter_spring_layout(H)
+
+    if ax is None:
+        ax = plt.gca()
+
+    ax.get_xaxis().set_ticks([])
+    ax.get_yaxis().set_ticks([])
+    ax.axis("off")
+
+    if not max_order:
+        max_order = max_edge_order(H)
+
+    dyad_color = _color_arg_to_dict(dyad_color, H.edges, settings["dyad_color_cmap"])
+
+    for id, he in H._edge.items():
+        d = len(he) - 1
+        if d > max_order:
+            continue
+        if d == 1:
+            # Drawing the edges
+            he = list(he)
+            x_coords = [pos[he[0]][0], pos[he[1]][0]]
+            y_coords = [pos[he[0]][1], pos[he[1]][1]]
+            line = plt.Line2D(
+                x_coords,
+                y_coords,
+                color=dyad_color[id],
+                zorder=max_order - 1,
+                alpha=1,
+            )
+            ax.add_line(line)
+
+        else:
+            coordinates = [[pos[n][0], pos[n][1]] for n in he]
+            _draw_hull(
+                node_pos=np.array(coordinates),
+                ax=ax,
+                edges_ec=edge_ec[id],
+                facecolor=edge_fc[id],
+                alpha=alpha,
+                zorder=max_order - d,
+                radius=radius,
+            )
+
+    if hyperedge_labels:
+        # Get all valid keywords by inspecting the signatures of draw_node_labels
+        valid_label_kwds = signature(draw_hyperedge_labels).parameters.keys()
+        # Remove the arguments of this function (draw_networkx)
+        valid_label_kwds = valid_label_kwds - {"H", "pos", "ax", "hyperedge_labels"}
+        if any([k not in valid_label_kwds for k in kwargs]):
+            invalid_args = ", ".join([k for k in kwargs if k not in valid_label_kwds])
+            raise ValueError(f"Received invalid argument(s): {invalid_args}")
+        label_kwds = {k: v for k, v in kwargs.items() if k in valid_label_kwds}
+        draw_hyperedge_labels(H, pos, hyperedge_labels, ax_edges=ax, **label_kwds)
+
+    draw_nodes(
+        H,
+        pos,
+        ax,
+        node_fc,
+        node_ec,
+        node_lw,
+        node_size,
+        max_order,
+        settings,
+        node_labels,
+        **kwargs,
+    )
+
+    # compute axis limits
+    _update_lims(pos, ax)
+
+    return ax
```

### Comparing `xgi-0.5.6/xgi/drawing/layout.py` & `xgi-0.5.7/xgi/drawing/layout.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/dynamics/synchronization.py` & `xgi-0.5.7/xgi/dynamics/synchronization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Simulation of the Kuramoto model."""
 
 import numpy as np
 
 import xgi
 
 from ..exception import XGIError
+from ..linalg.hodge_matrix import boundary_matrix
 
 __all__ = [
     "simulate_kuramoto",
     "compute_kuramoto_order_parameter",
     "simulate_simplicial_kuramoto",
     "compute_simplicial_order_parameter",
 ]
@@ -204,25 +205,23 @@
 
     if not isinstance(S, xgi.SimplicialComplex):
         raise XGIError(
             "The simplicial Kuramoto model can be simulated only on a SimplicialComplex object"
         )
 
     if index:
-        B_o, om1_dict, o_dict = xgi.matrix.boundary_matrix(S, order, orientations, True)
+        B_o, om1_dict, o_dict = boundary_matrix(S, order, orientations, True)
     else:
-        B_o = xgi.matrix.boundary_matrix(S, order, orientations, False)
+        B_o = boundary_matrix(S, order, orientations, False)
     D_om1 = np.transpose(B_o)
 
     if index:
-        B_op1, __, op1_dict = xgi.matrix.boundary_matrix(
-            S, order + 1, orientations, True
-        )
+        B_op1, __, op1_dict = boundary_matrix(S, order + 1, orientations, True)
     else:
-        B_op1 = xgi.matrix.boundary_matrix(S, order + 1, orientations, False)
+        B_op1 = boundary_matrix(S, order + 1, orientations, False)
     D_o = np.transpose(B_op1)
 
     # Compute the number of oscillating simplices
     n_o = np.shape(B_o)[1]
 
     dt = T / n_steps
     theta = np.zeros((n_o, n_steps))
```

### Comparing `xgi-0.5.6/xgi/generators/classic.py` & `xgi-0.5.7/xgi/generators/uniform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,395 +1,375 @@
-"""Generators for some classic hypergraphs.
-
-All the functions in this module return a Hypergraph class (i.e. a simple, undirected
-hypergraph).
-
-"""
-
+"""Generate random uniform hypergraphs."""
+import itertools
+import operator
 import random
-from collections import defaultdict
-from itertools import combinations
-from warnings import warn
+import warnings
+from functools import reduce
 
-import networkx as nx
+import numpy as np
 
-from ..classes.function import subfaces
 from ..exception import XGIError
-from ..utils.utilities import find_triangles
+from .classic import empty_hypergraph
 
 __all__ = [
-    "empty_hypergraph",
-    "empty_simplicial_complex",
-    "star_clique",
-    "flag_complex",
-    "flag_complex_d2",
-    "sunflower",
-    "ring_lattice",
+    "uniform_hypergraph_configuration_model",
+    "uniform_HSBM",
+    "uniform_HPPM",
+    "uniform_erdos_renyi_hypergraph",
 ]
 
 
-def _empty_network(create_using, default):
-    """Return an empty network.
-
-    See Also
-    --------
-    empty_hypergraph
-    empty_simplicial_complex
-
+def uniform_hypergraph_configuration_model(k, m, seed=None):
     """
-    if create_using is None:
-        H = default()
-    elif hasattr(create_using, "_node"):
-        # create_using is a Hypergraph object
-        create_using.clear()
-        H = create_using
-    else:
-        # try create_using as constructor
-        H = create_using()
-    return H
-
-
-def empty_hypergraph(create_using=None, default=None):
-    """Returns the empty hypergraph with zero nodes and edges.
+    A function to generate an m-uniform configuration model
 
     Parameters
     ----------
-    create_using : Hypergraph Instance, Constructor or None
-        If None, use the `default` constructor.
-        If a constructor, call it to create an empty hypergraph.
-    default : Hypergraph constructor (default None)
-        The constructor to use if create_using is None.
-        If None, then xgi.Hypergraph is used.
+    k : dictionary
+        This is a dictionary where the keys are node ids
+        and the values are node degrees.
+    m : int
+        specifies the hyperedge size
+    seed : integer or None (default)
+        The seed for the random number generator
 
     Returns
     -------
     Hypergraph object
-        An empty hypergraph
-
-    Examples
-    --------
-    >>> import xgi
-    >>> H = xgi.empty_hypergraph()
-    >>> H.num_nodes, H.num_edges
-    (0, 0)
-
-    """
-    # this import needs to happen when the function runs, not when the module is first
-    # imported, to avoid circular imports
-    import xgi
-
-    if default is None:
-        default = xgi.Hypergraph
-    return _empty_network(create_using, default)
+        The generated hypergraph
 
+    Warns
+    -----
+    warnings.warn
+        If the sums of the degrees are not divisible by m, the
+        algorithm still runs, but raises a warning and adds an
+        additional connection to random nodes to satisfy this
+        condition.
 
-def empty_simplicial_complex(create_using=None, default=None):
-    """Returns the empty simplicial complex with zero nodes and simplices.
+    Notes
+    -----
+    This algorithm normally creates multi-edges and loopy hyperedges.
+    We remove the loopy hyperedges.
 
-    Parameters
+    References
     ----------
-    create_using : SimplicialComplex Instance, Constructor or None
-        If None, use the `default` constructor.
-        If a constructor, call it to create an empty simplicial complex.
-    default : SimplicialComplex constructor (default None)
-        The constructor to use if create_using is None.
-        If None, then xgi.SimplicialComplex is used.
+    "The effect of heterogeneity on hypergraph contagion models"
+    by Nicholas W. Landry and Juan G. Restrepo
+    https://doi.org/10.1063/5.0020034
 
-    Returns
-    -------
-    SimplicialComplex
-        An empty simplicial complex.
-
-    Examples
-    --------
-    >>> import xgi
-    >>> H = xgi.empty_simplicial_complex()
-    >>> H.num_nodes, H.num_edges
-    (0, 0)
 
-    """
-    # this import needs to happen when the function runs, not when the module is first
-    # imported, to avoid circular imports
-    import xgi
-
-    if default is None:
-        default = xgi.SimplicialComplex
-    return _empty_network(create_using, default)
-
-
-def star_clique(n_star, n_clique, d_max):
-    """Generate a star-clique structure
-
-    That is a star network and a clique network,
-    connected by one pairwise edge connecting the centre of the star to the clique.
-    network, the each clique is promoted to a hyperedge
-    up to order d_max.
-
-    Parameters
-    ----------
-    n_star : int
-        Number of legs of the star
-    n_clique : int
-        Number of nodes in the clique
-    d_max : int
-        Maximum order up to which to promote
-        cliques to hyperedges
-
-    Returns
+    Example
     -------
-    H : Hypergraph
-
-    Examples
-    --------
     >>> import xgi
-    >>> H = xgi.star_clique(6, 7, 2)
-
-    Notes
-    -----
-    The total number of nodes is n_star + n_clique.
+    >>> import random
+    >>> n = 1000
+    >>> m = 3
+    >>> k = {1: 1, 2: 2, 3: 3, 4: 3}
+    >>> H = xgi.uniform_hypergraph_configuration_model(k, m)
 
     """
+    if seed is not None:
+        random.seed(seed)
 
-    if n_star <= 0:
-        raise ValueError("n_star must be an integer > 0.")
-    if n_clique <= 0:
-        raise ValueError("n_clique must be an integer > 0.")
-    if d_max < 0:
-        raise ValueError("d_max must be an integer >= 0.")
-    elif d_max > n_clique - 1:
-        raise ValueError("d_max must be <= n_clique - 1.")
-
-    nodes_star = range(n_star)
-    nodes_clique = range(n_star, n_star + n_clique)
-    nodes = list(nodes_star) + list(nodes_clique)
+    # Making sure we have the right number of stubs
+    remainder = sum(k.values()) % m
+    if remainder != 0:
+        warnings.warn(
+            "This degree sequence is not realizable. Increasing the degree of random nodes so that it is."
+        )
+        random_ids = random.sample(list(k.keys()), int(round(m - remainder)))
+        for id in random_ids:
+            k[id] = k[id] + 1
+
+    stubs = []
+    # Creating the list to index through
+    for id in k:
+        stubs.extend([id] * int(k[id]))
 
     H = empty_hypergraph()
-    H.add_nodes_from(nodes)
-
-    # add star edges (center of the star is 0-th node)
-    H.add_edges_from([(nodes_star[0], nodes_star[i]) for i in range(1, n_star)])
+    H.add_nodes_from(k.keys())
 
-    # connect clique and star by adding last star leg
-    H.add_edge((nodes_star[0], nodes_clique[0]))
+    while len(stubs) != 0:
+        u = random.sample(range(len(stubs)), m)
+        edge = set()
+        for index in u:
+            edge.add(stubs[index])
+        if len(edge) == m:
+            H.add_edge(edge)
 
-    # add clique hyperedges up to order d_max
-    H.add_edges_from(
-        [e for d in range(1, d_max + 1) for e in combinations(nodes_clique, d + 1)]
-    )
+        for index in sorted(u, reverse=True):
+            del stubs[index]
 
     return H
 
 
-def flag_complex(G, max_order=2, ps=None, seed=None):
-    """Generate a flag (or clique) complex from a
-    NetworkX graph by filling all cliques up to dimension max_order.
+def uniform_HSBM(n, m, p, sizes, seed=None):
+    """Create a uniform hypergraph stochastic block model (HSBM).
 
     Parameters
     ----------
-    G : Networkx Graph
-
-    max_order : int
-        maximal dimension of simplices to add to the output simplicial complex
-    ps: list of float
-        List of probabilities (between 0 and 1) to create a
-        hyperedge from a clique, at each order d. For example,
-        ps[0] is the probability of promoting any 3-node clique (triangle) to
-        a 3-hyperedge.
-    seed: int or None (default)
+    n : int
+        The number of nodes
+    m : int
+        The hyperedge size
+    p : m-dimensional numpy array
+        tensor of probabilities between communities
+    sizes : list or 1D numpy array
+        The sizes of the community blocks in order
+    seed : integer or None (default)
         The seed for the random number generator
 
     Returns
     -------
-    S : SimplicialComplex
+    Hypergraph
+        The constructed SBM hypergraph
 
-    Notes
-    -----
-    Computing all cliques quickly becomes heavy for large networks. `flag_complex_d2`
-    is faster to compute up to order 2.
+    Raises
+    ------
+    XGIError
+        - If the length of sizes and p do not match.
+        - If p is not a tensor with every dimension equal
+        - If p is not m-dimensional
+        - If the entries of p are not in the range [0, 1]
+        - If the sum of the vector of sizes does not equal the number of nodes.
+    Exception
+        If there is an integer overflow error
 
-    See also
+    See Also
     --------
-    flag_complex_d2
+    uniform_HPPM
 
+    References
+    ----------
+    Nicholas W. Landry and Juan G. Restrepo.
+    "Polarization in hypergraphs with community structure."
+    Preprint, 2023. https://doi.org/10.48550/arXiv.2302.13967
     """
-    # This import needs to happen when this function is called, not when it is
-    # defined.  Otherwise, a circular import error would happen.
-    from ..classes import SimplicialComplex
-
-    if seed is not None:
-        random.seed(seed)
 
-    nodes = G.nodes()
-    edges = G.edges()
+    # Check if dimensions match
+    if len(sizes) != np.size(p, axis=0):
+        raise XGIError("'sizes' and 'p' do not match.")
+    if len(np.shape(p)) != m:
+        raise XGIError("The dimension of p does not match m")
+    # Check that p has the same length over every dimension.
+    if len(set(np.shape(p))) != 1:
+        raise XGIError("'p' must be a square tensor.")
+    if np.max(p) > 1 or np.min(p) < 0:
+        raise XGIError("Entries of 'p' not in [0,1].")
+    if np.sum(sizes) != n:
+        raise XGIError("Sum of sizes does not match n")
 
-    # compute all maximal cliques to fill
-    max_cliques = list(nx.find_cliques(G))
-
-    S = SimplicialComplex()
-    S.add_nodes_from(nodes)
-    S.add_simplices_from(edges)
-    if not ps:  # promote all cliques
-        S.add_simplices_from(max_cliques, max_order=max_order)
-        return S
-
-    if max_order:  # compute subfaces of order max_order (allowed max cliques)
-        max_cliques_to_add = subfaces(max_cliques, order=max_order)
-    else:
-        max_cliques_to_add = max_cliques
+    if seed is not None:
+        np.random.seed(seed)
 
-    # store max cliques per order
-    cliques_d = defaultdict(list)
-    for x in max_cliques_to_add:
-        cliques_d[len(x)].append(x)
+    node_labels = range(n)
+    H = empty_hypergraph()
+    H.add_nodes_from(node_labels)
 
-    # promote cliques with a given probability
-    for i, p in enumerate(ps[: max_order - 1]):
-        d = i + 2  # simplex order
-        cliques_d_to_add = [el for el in cliques_d[d + 1] if random.random() <= p]
-        S.add_simplices_from(cliques_d_to_add, max_order=max_order)
+    block_range = range(len(sizes))
+    # Split node labels in a partition (list of sets).
+    size_cumsum = [sum(sizes[0:x]) for x in range(0, len(sizes) + 1)]
+    partition = [
+        list(node_labels[size_cumsum[x] : size_cumsum[x + 1]])
+        for x in range(0, len(size_cumsum) - 1)
+    ]
 
-    return S
+    for block in itertools.product(block_range, repeat=m):
+        if p[block] == 1:  # Test edges cases p_ij = 0 or 1
+            edges = itertools.product((partition[i] for i in block_range))
+            for e in edges:
+                H.add_edge(e)
+        elif p[block] > 0:
+            partition_sizes = [len(partition[i]) for i in block]
+            max_index = reduce(operator.mul, partition_sizes, 1)
+            if max_index < 0:
+                raise Exception("Index overflow error!")
+            index = np.random.geometric(p[block]) - 1
+
+            while index < max_index:
+                indices = _index_to_edge_partition(index, partition_sizes, m)
+                e = {partition[block[i]][indices[i]] for i in range(m)}
+                if len(e) == m:
+                    H.add_edge(e)
+                index += np.random.geometric(p[block])
+    return H
 
 
-def flag_complex_d2(G, p2=None, seed=None):
-    """Generate a flag (or clique) complex from a
-    NetworkX graph by filling all cliques up to dimension 2.
+def uniform_HPPM(n, m, rho, k, epsilon, seed=None):
+    """Construct the m-uniform hypergraph planted partition model (m-HPPM)
 
     Parameters
     ----------
-    G : networkx Graph
-        Graph to consider
-    p2: float
-        Probability (between 0 and 1) of filling empty triangles in graph G
-    seed: int or None (default)
+    n : int > 0
+        Number of nodes
+    m : int > 0
+        Hyperedge size
+    rho : float between 0 and 1
+        The fraction of nodes in community 1
+    k : float > 0
+        Mean degree
+    epsilon : float > 0
+        Imbalance parameter
+    seed : integer or None (default)
         The seed for the random number generator
 
     Returns
     -------
-    S : xgi.SimplicialComplex
+    Hypergraph
+        The constructed m-HPPM hypergraph.
 
-    Notes
-    -----
-    Computing all cliques quickly becomes heavy for large networks. This
-    is faster than `flag_complex` to compute up to order 2.
+    Raises
+    ------
+    XGIError
+        - If rho is not between 0 and 1
+        - If the mean degree is negative.
+        - If epsilon is not between 0 and 1
 
-    See also
+    See Also
     --------
-    flag_complex
-    """
-    # This import needs to happen when this function is called, not when it is
-    # defined.  Otherwise, a circular import error would happen.
-    from ..classes import SimplicialComplex
-
-    if seed is not None:
-        random.seed(seed)
+    uniform_HSBM
 
-    nodes = G.nodes()
-    edges = G.edges()
+    References
+    ----------
+    Nicholas W. Landry and Juan G. Restrepo.
+    "Polarization in hypergraphs with community structure."
+    Preprint, 2023. https://doi.org/10.48550/arXiv.2302.13967
+    """
 
-    S = SimplicialComplex()
-    S.add_nodes_from(nodes)
-    S.add_simplices_from(edges)
+    if rho < 0 or rho > 1:
+        raise XGIError("The value of rho must be between 0 and 1")
+    if k < 0:
+        raise XGIError("The mean degree must be non-negative")
+    if epsilon < 0 or epsilon > 1:
+        raise XGIError("epsilon must be between 0 and 1")
 
-    triangles_empty = find_triangles(G)
+    sizes = [int(rho * n), n - int(rho * n)]
 
-    if p2 is not None:
-        triangles = [el for el in triangles_empty if random.random() <= p2]
-    else:
-        triangles = triangles_empty
+    p = k / (m * n ** (m - 1))
+    # ratio of inter- to intra-community edges
+    q = rho**m + (1 - rho) ** m
+    r = 1 / q - 1
+    p_in = (1 + r * epsilon) * p
+    p_out = (1 - epsilon) * p
 
-    S.add_simplices_from(triangles)
+    p = p_out * np.ones([2] * m)
+    p[tuple([0] * m)] = p_in
+    p[tuple([1] * m)] = p_in
 
-    return S
+    return uniform_HSBM(n, m, p, sizes, seed=seed)
 
 
-def ring_lattice(n, d, k, l):
-    """A ring lattice hypergraph.
+def uniform_erdos_renyi_hypergraph(n, m, p, p_type="degree", seed=None):
+    """Generate an m-uniform Erdős–Rényi hypergraph
 
-    A d-uniform hypergraph on n nodes where each node is part of k edges and the
-    overlap between consecutive edges is d-l.
+    This creates a hypergraph with `n` nodes where
+    hyperedges of size `m` are created at random to
+    obtain a mean degree of `k`.
 
     Parameters
     ----------
-    n : int
+    n : int > 0
         Number of nodes
-    d : int
-        Edge size
-    k : int
-        Number of edges of which a node is a part. Should be a multiple of 2.
-    l : int
-        Overlap between edges
+    m : int > 0
+        Hyperedge size
+    p : float or int > 0
+        Mean expected degree if p_type="degree" and
+        probability of an m-hyperedge if p_type="prob"
+    p_type : str
+        "degree" or "prob", by default "degree"
+    seed : integer or None (default)
+        The seed for the random number generator
 
     Returns
     -------
     Hypergraph
-        The generated hypergraph
+        The Erdos Renyi hypergraph
 
-    Raises
-    ------
-    XGIError
-        If k is negative.
 
-    Notes
-    -----
-    ring_lattice(n, 2, k, 0) is a ring lattice graph where each node has k//2 edges on either
-    side.
+    See Also
+    --------
+    random_hypergraph
     """
-    from ..classes import Hypergraph
+    if seed is not None:
+        np.random.seed(seed)
 
-    if k < 0:
-        raise XGIError("Invalid k value!")
+    node_labels = range(n)
+    H = empty_hypergraph()
+    H.add_nodes_from(node_labels)
 
-    if k < 2:
-        warn("This creates a completely disconnected hypergraph!")
+    if p_type == "degree":
+        q = p / (m * n ** (m - 1))  # wiring probability
+    elif p_type == "prob":
+        q = p
+    else:
+        raise XGIError("Invalid p_type!")
 
-    if k % 2 != 0:
-        warn("k is not divisible by 2")
+    if q > 1 or q < 0:
+        raise XGIError("Probability not in [0,1].")
 
-    edges = [
-        [node] + [(start + l + i) % n for i in range(d - 1)]
-        for node in range(n)
-        for start in range(node + 1, node + k // 2 + 1)
-    ]
-    H = Hypergraph(edges)
-    H.add_nodes_from(range(n))
+    index = np.random.geometric(q) - 1  # -1 b/c zero indexing
+    max_index = n**m
+    while index < max_index:
+        e = set(_index_to_edge(index, n, m))
+        if len(e) == m:
+            H.add_edge(e)
+        index += np.random.geometric(q)
     return H
 
 
-def sunflower(l, c, m):
-    """Create a sunflower hypergraph.
-
-    This creates an m-uniform hypergraph
-    according to the sunflower model.
+def _index_to_edge(index, n, m):
+    """Generate a hyperedge given an index in the list of possible edges.
 
     Parameters
     ----------
-    l : int
-        Number of petals
-    c : int
-        Size of the core
-    m : int
-        Size of each edge
-
-    Raises
-    ------
-    XGIError
-        If the edge size is smaller than the core.
+    index : int > 0
+        The index of the hyperedge in the list of all possible hyperedges.
+    n : int > 0
+        The number of nodes
+    m : int > 0
+        The hyperedge size.
 
     Returns
     -------
+    list
+        The reconstructed hyperedge
+
+    See Also
+    --------
+    _index_to_edge_partition
 
+    References
+    ----------
+    https://stackoverflow.com/questions/53834707/element-at-index-in-itertools-product
     """
-    from ..classes import Hypergraph
+    return [(index // (n**r) % n) for r in range(m - 1, -1, -1)]
+
 
-    if m < c:
-        raise XGIError("m cannot be smaller than c.")
+def _index_to_edge_partition(index, partition_sizes, m):
+    """Generate a hyperedge given an index in the list of possible edges
+    and a partition of community labels.
 
-    core_nodes = list(range(c))
+    Parameters
+    ----------
+    index : int > 0
+        The index of the hyperedge in the list of all possible hyperedges.
+    n : int > 0
+        The number of nodes
+    m : int > 0
+        The hyperedge size.
 
-    H = Hypergraph()
-    start_label = c
-    while start_label + (m - c) <= c + (m - c) * l:
-        H.add_edge(core_nodes + [start_label + i for i in range(m - c)])
-        start_label = start_label + (m - c)
+    Returns
+    -------
+    list
+        The reconstructed hyperedge
 
-    return H
+    See Also
+    --------
+    _index_to_edge
+    """
+    try:
+        return [
+            int(index // np.prod(partition_sizes[r + 1 :]) % partition_sizes[r])
+            for r in range(m)
+        ]
+    except:
+        raise Exception("Invalid parameters")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xgi-0.5.6/xgi/generators/nonuniform.py` & `xgi-0.5.7/xgi/generators/random.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,99 @@
 """Generate random (non-uniform) hypergraphs."""
 import math
 import random
 import warnings
 from collections import defaultdict
 from itertools import combinations
 
-import networkx as nx
 import numpy as np
 from scipy.special import comb
 
-from ..classes import SimplicialComplex
-from .classic import empty_hypergraph, flag_complex_d2, ring_lattice
+from .classic import empty_hypergraph
+from .lattice import ring_lattice
 
 __all__ = [
+    "random_hypergraph",
     "chung_lu_hypergraph",
     "dcsbm_hypergraph",
-    "random_hypergraph",
-    "random_simplicial_complex",
-    "random_flag_complex_d2",
-    "random_flag_complex",
     "watts_strogatz_hypergraph",
 ]
 
 
+def random_hypergraph(N, ps, order=None, seed=None):
+    """Generates a random hypergraph
+
+    Generate N nodes, and connect any d+1 nodes
+    by a hyperedge with probability ps[d-1].
+
+    Parameters
+    ----------
+    N : int
+        Number of nodes
+    ps : list of float
+        List of probabilities (between 0 and 1) to create a
+        hyperedge at each order d between any d+1 nodes. For example,
+        ps[0] is the wiring probability of any edge (2 nodes), ps[1]
+        of any triangles (3 nodes).
+    order: int of None (default)
+        If None, ignore. If int, generates a uniform hypergraph with edges
+        of order `order` (ps must have only one element).
+    seed : integer or None (default)
+            Seed for the random number generator.
+
+    Returns
+    -------
+    Hypergraph object
+        The generated hypergraph
+
+    References
+    ----------
+    Described as 'random hypergraph' by M. Dewar et al. in https://arxiv.org/abs/1703.07686
+
+    Example
+    -------
+    >>> import xgi
+    >>> H = xgi.random_hypergraph(50, [0.1, 0.01])
+
+    """
+    if seed is not None:
+        np.random.seed(seed)
+
+    if order is not None:
+        if len(ps) != 1:
+            raise ValueError("ps must contain a single element if order is an int")
+
+    if (np.any(np.array(ps) < 0)) or (np.any(np.array(ps) > 1)):
+        raise ValueError("All elements of ps must be between 0 and 1 included.")
+
+    nodes = range(N)
+    hyperedges = []
+
+    for i, p in enumerate(ps):
+
+        if order is not None:
+            d = order
+        else:
+            d = i + 1  # order, ps[0] is prob of edges (d=1)
+
+        potential_edges = combinations(nodes, d + 1)
+        n_comb = comb(N, d + 1, exact=True)
+        mask = np.random.random(size=n_comb) <= p  # True if edge to keep
+
+        edges_to_add = [e for e, val in zip(potential_edges, mask) if val]
+
+        hyperedges += edges_to_add
+
+    H = empty_hypergraph()
+    H.add_nodes_from(nodes)
+    H.add_edges_from(hyperedges)
+
+    return H
+
+
 def chung_lu_hypergraph(k1, k2, seed=None):
     """A function to generate a Chung-Lu hypergraph
 
     Parameters
     ----------
     k1 : dictionary
         Dictionary where the keys are node ids
@@ -110,15 +177,16 @@
                 p = q
                 j = j + 1
 
     return H
 
 
 def dcsbm_hypergraph(k1, k2, g1, g2, omega, seed=None):
-    """A function to generate a DCSBM hypergraph.
+    """A function to generate a Degree-Corrected Stochastic Block Model
+    (DCSBM) hypergraph.
 
     Parameters
     ----------
     k1 : dict
         This is a dictionary where the keys are node ids
         and the values are node degrees.
     k2 : dict
@@ -247,215 +315,14 @@
                             # no duplicates
                             H.add_node_to_edge(v, u)
                         p = q
                         j = j + 1
     return H
 
 
-def random_hypergraph(N, ps, seed=None):
-    """Generates a random hypergraph
-
-    Generate N nodes, and connect any d+1 nodes
-    by a hyperedge with probability ps[d-1].
-
-    Parameters
-    ----------
-    N : int
-        Number of nodes
-    ps : list of float
-        List of probabilities (between 0 and 1) to create a
-        hyperedge at each order d between any d+1 nodes. For example,
-        ps[0] is the wiring probability of any edge (2 nodes), ps[1]
-        of any triangles (3 nodes).
-    seed : integer or None (default)
-            Seed for the random number generator.
-
-    Returns
-    -------
-    Hypergraph object
-        The generated hypergraph
-
-    References
-    ----------
-    Described as 'random hypergraph' by M. Dewar et al. in https://arxiv.org/abs/1703.07686
-
-    Example
-    -------
-    >>> import xgi
-    >>> H = xgi.random_hypergraph(50, [0.1, 0.01])
-
-    """
-    if seed is not None:
-        np.random.seed(seed)
-
-    if (np.any(np.array(ps) < 0)) or (np.any(np.array(ps) > 1)):
-        raise ValueError("All elements of ps must be between 0 and 1 included.")
-
-    nodes = range(N)
-    hyperedges = []
-
-    for i, p in enumerate(ps):
-        d = i + 1  # order, ps[0] is prob of edges (d=1)
-
-        potential_edges = combinations(nodes, d + 1)
-        n_comb = comb(N, d + 1, exact=True)
-        mask = np.random.random(size=n_comb) <= p  # True if edge to keep
-
-        edges_to_add = [e for e, val in zip(potential_edges, mask) if val]
-
-        hyperedges += edges_to_add
-
-    H = empty_hypergraph()
-    H.add_nodes_from(nodes)
-    H.add_edges_from(hyperedges)
-
-    return H
-
-
-def random_simplicial_complex(N, ps, seed=None):
-    """Generates a random hypergraph
-
-    Generate N nodes, and connect any d+1 nodes
-    by a simplex with probability ps[d-1]. For each simplex,
-    add all its subfaces if they do not already exist.
-
-    Parameters
-    ----------
-    N : int
-        Number of nodes
-    ps : list of float
-        List of probabilities (between 0 and 1) to create a
-        hyperedge at each order d between any d+1 nodes. For example,
-        ps[0] is the wiring probability of any edge (2 nodes), ps[1]
-        of any triangles (3 nodes).
-    seed : int or None (default)
-        The seed for the random number generator
-
-    Returns
-    -------
-    Simplicialcomplex object
-        The generated simplicial complex
-
-    References
-    ----------
-    Described as 'random simplicial complex' in
-    "Simplicial Models of Social Contagion", Nature Communications 10(1), 2485,
-    by I. Iacopini, G. Petri, A. Barrat & V. Latora (2019).
-    https://doi.org/10.1038/s41467-019-10431-6
-
-    Example
-    -------
-    >>> import xgi
-    >>> H = xgi.random_simplicial_complex(20, [0.1, 0.01])
-
-    """
-
-    if seed is not None:
-        np.random.seed(seed)
-
-    if (np.any(np.array(ps) < 0)) or (np.any(np.array(ps) > 1)):
-        raise ValueError("All elements of ps must be between 0 and 1 included.")
-
-    nodes = range(N)
-    simplices = []
-
-    for i, p in enumerate(ps):
-        d = i + 1  # order, ps[0] is prob of edges (d=1)
-
-        potential_simplices = combinations(nodes, d + 1)
-        n_comb = comb(N, d + 1, exact=True)
-        mask = np.random.random(size=n_comb) <= p  # True if simplex to keep
-
-        simplices_to_add = [e for e, val in zip(potential_simplices, mask) if val]
-
-        simplices += simplices_to_add
-
-    S = SimplicialComplex()
-    S.add_nodes_from(nodes)
-    S.add_simplices_from(simplices)
-
-    return S
-
-
-def random_flag_complex_d2(N, p, seed=None):
-    """Generate a maximal simplicial complex (up to order 2) from a
-    :math:`G_{N,p}` Erdős-Rényi random graph by filling all empty triangles with 2-simplices.
-
-    Parameters
-    ----------
-    N : int
-        Number of nodes
-    p : float
-        Probabilities (between 0 and 1) to create an edge
-        between any 2 nodes
-    seed : int or None (default)
-        The seed for the random number generator
-
-    Returns
-    -------
-    SimplicialComplex
-
-    Notes
-    -----
-    Computing all cliques quickly becomes heavy for large networks.
-    """
-    if seed is not None:
-        random.seed(seed)
-
-    if (p < 0) or (p > 1):
-        raise ValueError("p must be between 0 and 1 included.")
-
-    G = nx.fast_gnp_random_graph(N, p, seed=seed)
-
-    return flag_complex_d2(G)
-
-
-def random_flag_complex(N, p, max_order=2, seed=None):
-    """Generate a flag (or clique) complex from a
-    :math:`G_{N,p}` Erdős-Rényi random graph by filling all cliques up to dimension max_order.
-
-    Parameters
-    ----------
-    N : int
-        Number of nodes
-    p : float
-        Probability (between 0 and 1) to create an edge
-        between any 2 nodes
-    max_order : int
-        maximal dimension of simplices to add to the output simplicial complex
-    seed : int or None (default)
-        The seed for the random number generator
-
-    Returns
-    -------
-    SimplicialComplex
-
-    Notes
-    -----
-    Computing all cliques quickly becomes heavy for large networks.
-    """
-
-    if (p < 0) or (p > 1):
-        raise ValueError("p must be between 0 and 1 included.")
-
-    G = nx.fast_gnp_random_graph(N, p, seed=seed)
-
-    nodes = G.nodes()
-    edges = list(G.edges())
-
-    # compute all triangles to fill
-    max_cliques = list(nx.find_cliques(G))
-
-    S = SimplicialComplex()
-    S.add_nodes_from(nodes)
-    S.add_simplices_from(max_cliques, max_order=max_order)
-
-    return S
-
-
 def watts_strogatz_hypergraph(n, d, k, l, p, seed=None):
     if seed is not None:
         np.random.seed(seed)
     H = ring_lattice(n, d, k, l)
     to_remove = []
     to_add = []
     for e in H.edges:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xgi-0.5.6/xgi/readwrite/bipartite.py` & `xgi-0.5.7/xgi/readwrite/bipartite.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/readwrite/edgelist.py` & `xgi-0.5.7/xgi/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/readwrite/incidence.py` & `xgi-0.5.7/xgi/readwrite/incidence.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/readwrite/json.py` & `xgi-0.5.7/xgi/readwrite/json.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi/readwrite/xgi_data.py` & `xgi-0.5.7/xgi/readwrite/xgi_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Load a data set from the xgi-data repository or a local file."""
 import json
 import os
 from functools import lru_cache
 from warnings import warn
 
 import requests
```

### Comparing `xgi-0.5.6/xgi/stats/__init__.py` & `xgi-0.5.7/xgi/stats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 >>> H.nodes.attrs('color').aslist()
 ['red', 'blue', 'yellow', 'red', 'blue']
 >>> H.nodes.filterby_attr('color', 'red')
 NodeView((1, 4))
 
 Many other features are available, including edge-statistics, and user-defined
 statistics.  For more details, see the `tutorial
-<https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+<https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
 """
 
 from collections import defaultdict
 from typing import Callable
 
 import numpy as np
@@ -202,25 +202,25 @@
 
 
 class NodeStat(IDStat):
     """An arbitrary node-quantity mapping.
 
     `NodeStat` objects represent a mapping that assigns a value to each node in a
     network.  For more details, see the `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
 
 class EdgeStat(IDStat):
     """An arbitrary edge-quantity mapping.
 
     `EdgeStat` objects represent a mapping that assigns a value to each edge in a
     network.  For more details, see the `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
 
 class MultiIDStat(IDStat):
     """Multiple mappings."""
 
@@ -279,25 +279,28 @@
             keys are the specified stats.  If True, the outer and inner keys are
             reversed.  Only used when `inner` is `dict`.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-        >>> m = H.nodes.multi(['degree', 'clustering'])
+        >>> m = H.nodes.multi(['degree', 'clustering_coefficient'])
         >>> m.asdict() # doctest: +NORMALIZE_WHITESPACE
-        {1: {'degree': 1, 'clustering': 0.0},
-         2: {'degree': 2, 'clustering': 4.0},
-         3: {'degree': 3, 'clustering': 1.3333333333333333},
-         4: {'degree': 2, 'clustering': 3.0},
-         5: {'degree': 2, 'clustering': 3.0}}
+        {1: {'degree': 1, 'clustering_coefficient': 1.0},
+         2: {'degree': 2, 'clustering_coefficient': 0.6666666666666666},
+         3: {'degree': 3, 'clustering_coefficient': 0.6666666666666666},
+         4: {'degree': 2, 'clustering_coefficient': 1.0},
+         5: {'degree': 2, 'clustering_coefficient': 1.0}}
         >>> m.asdict(transpose=True) # doctest: +NORMALIZE_WHITESPACE
         {'degree': {1: 1, 2: 2, 3: 3, 4: 2, 5: 2},
-        'clustering': {1: 0.0, 2: 4.0, 3: 1.3333333333333333, 4: 3.0, 5: 3.0}}
-
+        'clustering_coefficient': {1: 1.0,
+        2: 0.6666666666666666,
+        3: 0.6666666666666666,
+        4: 1.0,
+        5: 1.0}}
         """
         val = self._val
         if inner is dict:
             if not transpose:
                 return {n: val[n] for n in self.view}
             else:
                 return {s.name: s.asdict() for s in self.stats}
@@ -320,20 +323,19 @@
             of a single node.  If True, each inner list contains the values of a single
             stat of all nodes.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-        >>> m = H.nodes.multi(['degree', 'clustering'])
+        >>> m = H.nodes.multi(['degree', 'clustering_coefficient'])
         >>> m.aslist() # doctest:
-        [[1, 0.0], [2, 4.0], [3, 1.3333333333333333], [2, 3.0], [2, 3.0]]
+        [[1, 1.0], [2, 0.6666666666666666], [3, 0.6666666666666666], [2, 1.0], [2, 1.0]]
         >>> m.aslist(transpose=True)
-        [[1, 2, 3, 2, 2], [0.0, 4.0, 1.3333333333333333, 3.0, 3.0]]
-
+        [[1, 2, 3, 2, 2], [1.0, 0.6666666666666666, 0.6666666666666666, 1.0, 1.0]]
         """
         val = self._val
         if inner is list:
             if not transpose:
                 return [list(val[n].values()) for n in self.view]
             else:
                 return [s.aslist() for s in self.stats]
@@ -349,65 +351,65 @@
         -----
         Equivalent to `np.array(self.aslist(inner=list))`.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-        >>> H.nodes.multi(['degree', 'clustering']).asnumpy()  # doctest: +NORMALIZE_WHITESPACE
-        array([[1.        , 0.        ],
-               [2.        , 4.        ],
-               [3.        , 1.33333333],
-               [2.        , 3.        ],
-               [2.        , 3.        ]])
+        >>> H.nodes.multi(['degree', 'clustering_coefficient']).asnumpy()  # doctest: +NORMALIZE_WHITESPACE
+        array([[1.        , 1.        ],
+               [2.        , 0.66666667],
+               [3.        , 0.66666667],
+               [2.        , 1.        ],
+               [2.        , 1.        ]])
 
         """
         return np.array(self.aslist(inner=list))
 
     def aspandas(self):
         """Output the stats as a pandas dataframe.
 
         Examples
         --------
         >>> import xgi
         >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-        >>> H.nodes.multi(['degree', 'clustering']).aspandas()  # doctest: +NORMALIZE_WHITESPACE
-           degree  clustering
-        1       1    0.000000
-        2       2    4.000000
-        3       3    1.333333
-        4       2    3.000000
-        5       2    3.000000
+        >>> H.nodes.multi(['degree', 'clustering_coefficient']).aspandas()  # doctest: +NORMALIZE_WHITESPACE
+           degree  clustering_coefficient
+        1       1    1.000000
+        2       2    0.666667
+        3       3    0.666667
+        4       2    1.000000
+        5       2    1.000000
 
         """
         result = {s.name: s._val for s in self.stats}
         series = [pd.Series(v, name=k) for k, v in result.items()]
         return pd.concat(series, axis=1)
 
     def dist(self):
         return [np.histogram(data, density=True) for data in self.asnumpy().T]
 
 
 class MultiNodeStat(MultiIDStat):
     """Multiple node-quantity mappings.
 
     For more details, see the `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     statsclass = NodeStat
     statsmodule = nodestats
 
 
 class MultiEdgeStat(MultiIDStat):
     """Multiple edge-quantity mappings.
 
     For more details, see the `tutorial
-    <https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     statsclass = EdgeStat
     statsmodule = edgestats
```

### Comparing `xgi-0.5.6/xgi/stats/edgestats.py` & `xgi-0.5.7/xgi/stats/edgestats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Edge statistics.
 
 This module is part of the stats package, and it defines edge-level statistics.  That
 is, each function defined in this module is assumed to define an edge-quantity mapping.
 Each callable defined here is accessible via a `Network` object, or a
 :class:`~xgi.classes.reportviews.EdgeView` object.  For more details, see the `tutorial
-<https://github.com/ComplexGroupInteractions/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+<https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
 Examples
 --------
 
 >>> import xgi
 >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
 >>> H.order()
```

### Comparing `xgi-0.5.6/xgi/stats/nodestats.py` & `xgi-0.5.7/xgi/stats/nodestats.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 
 import xgi
 
 __all__ = [
     "attrs",
     "degree",
     "average_neighbor_degree",
-    "clustering",
-    "cec_centrality",
-    "hec_centrality",
+    "local_clustering_coefficient",
+    "clustering_coefficient",
+    "two_node_clustering_coefficient",
+    "clique_eigenvector_centrality",
+    "h_eigenvector_centrality",
     "node_edge_centrality",
 ]
 
 
 def attrs(net, bunch, attr=None, missing=None):
     """Access node attributes.
 
@@ -184,20 +186,24 @@
     for n in bunch:
         neighbors = net.nodes.neighbors(n)
         result[n] = sum(len(net._node[nbr]) for nbr in neighbors)
         result[n] = result[n] / len(neighbors) if neighbors else 0
     return result
 
 
-def clustering(net, bunch):
+def clustering_coefficient(net, bunch):
     """Local clustering coefficient.
 
-    The clustering coefficient of a node `n` is defined as `num / denom`, where `num`
-    equals `A^3[n, n]` and `denom` equals `d*(d-1)/2`.  Here `A` is the adjacency matrix
-    of the network and `d` is the degree of `n`.
+    This clustering coefficient is defined as the
+    clustering coefficient of the unweighted pairwise
+    projection of the hypergraph, i.e., `num / denom`,
+    where `num` equals `A^3[n, n]` and `denom` equals
+    `nu*(nu-1)/2`.  Here `A` is the adjacency matrix
+    of the network and `nu` is the number of pairwise
+    neighbors of `n`.
 
     Parameters
     ----------
     net : xgi.Hypergraph
         The network.
     bunch : Iterable
         Nodes in `net`.
@@ -211,35 +217,109 @@
     This is a direct generalization of the definition of local clustering coefficient
     for graphs.  It has not been tested on hypergraphs.
 
     Examples
     --------
     >>> import xgi, numpy as np
     >>> H = xgi.Hypergraph([[1, 2, 3], [2, 3, 4, 5], [3, 4, 5]])
-    >>> np.round(H.nodes.clustering.asnumpy(), 3)
-    array([0.   , 4.   , 1.333, 3.   , 3.   ])
+    >>> H.nodes.two_node_clustering_coefficient.asnumpy()
+    array([0.41666667, 0.45833333, 0.58333333, 0.66666667, 0.66666667])
 
     """
-    adj, index = xgi.adjacency_matrix(net, index=True)
-    node_to_index = {n: i for i, n in index.items()}
-    mat = adj.dot(adj).dot(adj)
-    result = {}
-    for n in bunch:
-        deg = len(net.nodes.memberships(n))
-        denom = deg * (deg - 1) / 2
-        if denom <= 0:
-            result[n] = 0.0
-        else:
-            i = node_to_index[n]
-            result[n] = mat[i, i] / denom / 2
-    return result
+    cc = xgi.clustering_coefficient(net)
+    return {n: cc[n] for n in cc if n in bunch}
+
+
+def local_clustering_coefficient(net, bunch):
+    """Compute the local clustering coefficient.
+
+    This clustering coefficient is based on the
+    overlap of the edges connected to a given node,
+    normalized by the size of the node's neighborhood.
+
+    Parameters
+    ----------
+    net : xgi.Hypergraph
+        The network.
+    bunch : Iterable
+        Nodes in `net`.
+
+    Returns
+    -------
+    dict
+        keys are node IDs and values are the
+        clustering coefficients.
+
+    References
+    ----------
+    "Properties of metabolic graphs: biological organization or representation artifacts?"
+    by Wanding Zhou and Luay Nakhleh.
+    https://doi.org/10.1186/1471-2105-12-132
+
+    "Hypergraphs for predicting essential genes using multiprotein complex data"
+    by Florian Klimm, Charlotte M. Deane, and Gesine Reinert.
+    https://doi.org/10.1093/comnet/cnaa028
+
+    Example
+    -------
+    >>> import xgi
+    >>> H = xgi.random_hypergraph(3, [1, 1])
+    >>> H.nodes.local_clustering_coefficient.asdict()
+    {0: 1.0, 1: 1.0, 2: 1.0}
+    """
+    cc = xgi.local_clustering_coefficient(net)
+    return {n: cc[n] for n in cc if n in bunch}
+
+
+def two_node_clustering_coefficient(net, bunch, kind="union"):
+    """Return the clustering coefficients for
+    each node in a Hypergraph.
+
+    This definition averages over all of the
+    two-node clustering coefficients involving the node.
+
+    Parameters
+    ----------
+    net : xgi.Hypergraph
+        The network.
+    bunch : Iterable
+        Nodes in `net`.
+    kind : str
+        The type of two-node clustering coefficient.
+        Types are:
+
+        - "union"
+        - "min"
+        - "max"
+        by default, "union".
+
+    Returns
+    -------
+    dict
+        nodes are keys, clustering coefficients are values.
+
+    References
+    ----------
+    "Clustering Coefficients in Protein Interaction Hypernetworks"
+    by Suzanne Gallagher and Debra Goldberg.
+    DOI: 10.1145/2506583.2506635
+
+    Example
+    -------
+    >>> import xgi
+    >>> H = xgi.random_hypergraph(3, [1, 1])
+    >>> H.nodes.two_node_clustering_coefficient.asdict()
+    {0: 0.5, 1: 0.5, 2: 0.5}
+    """
+    cc = xgi.two_node_clustering_coefficient(net, kind=kind)
+    return {n: cc[n] for n in cc if n in bunch}
 
 
-def cec_centrality(net, bunch, tol=1e-6):
-    """Compute the CEC centrality of a hypergraph.
+def clique_eigenvector_centrality(net, bunch, tol=1e-6):
+    """Compute the clique motif eigenvector centrality of a hypergraph.
 
     Parameters
     ----------
     net : xgi.Hypergraph
         The hypergraph of interest.
     bunch : Iterable
         Nodes in `net`.
@@ -253,20 +333,20 @@
 
     References
     ----------
     Three Hypergraph Eigenvector Centralities,
     Austin R. Benson,
     https://doi.org/10.1137/18M1203031
     """
-    c = xgi.CEC_centrality(net, tol)
+    c = xgi.clique_eigenvector_centrality(net, tol)
     return {n: c[n] for n in c if n in bunch}
 
 
-def hec_centrality(net, bunch, max_iter=10, tol=1e-6):
-    """Compute the HEC centrality of a hypergraph.
+def h_eigenvector_centrality(net, bunch, max_iter=10, tol=1e-6):
+    """Compute the H-eigenvector centrality of a hypergraph.
 
     Parameters
     ----------
     net : xgi.Hypergraph
         The hypergraph of interest.
     bunch : Iterable
         Nodes in `net`.
@@ -282,15 +362,15 @@
 
     References
     ----------
     Three Hypergraph Eigenvector Centralities,
     Austin R. Benson,
     https://doi.org/10.1137/18M1203031
     """
-    c = xgi.HEC_centrality(net, max_iter, tol)
+    c = xgi.h_eigenvector_centrality(net, max_iter, tol)
     return {n: c[n] for n in c if n in bunch}
 
 
 def node_edge_centrality(
     net,
     bunch,
     f=lambda x: np.power(x, 2),
```

### Comparing `xgi-0.5.6/xgi/utils/utilities.py` & `xgi-0.5.7/xgi/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `xgi-0.5.6/xgi.egg-info/PKG-INFO` & `xgi-0.5.7/xgi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: xgi
-Version: 0.5.6
+Version: 0.5.7
 Summary: XGI is a Python library for the representation
 Author: Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze
 Author-email: nicholas.landry@uvm.edu
 Project-URL: Documentation, https://xgi.readthedocs.io/en/latest/
-Project-URL: Bug Reports, https://github.com/ComplexGroupInteractions/xgi/issues
-Project-URL: Source, https://github.com/ComplexGroupInteractions/xgi
+Project-URL: Bug Reports, https://github.com/xgi-org/xgi/issues
+Project-URL: Source, https://github.com/xgi-org/xgi
 Project-URL: PyPI, https://pypi.org/project/xgi/
-Project-URL: GitHub Discussions, https://github.com/ComplexGroupInteractions/xgi/discussions
+Project-URL: GitHub Discussions, https://github.com/xgi-org/xgi/discussions
 Provides-Extra: benchmarks
 Provides-Extra: developer
 Provides-Extra: documentation
 Provides-Extra: release
 Provides-Extra: test
 Provides-Extra: tutorial
 Provides-Extra: all
 License-File: LICENSE.md
 
 XGI
 ===
 
-.. image:: https://github.com/ComplexGroupInteractions/xgi/raw/main/logo/logo.svg
+.. image:: https://github.com/xgi-org/xgi/raw/main/logo/logo.svg
   :width: 200
 
 CompleX Group Interactions (XGI) is a Python package for the representation, manipulation,
 and study of the structure, dynamics, and functions of complex systems with group (higher-order) interactions.
 
 Installation
 ------------
@@ -42,41 +42,41 @@
 -  Run the following command::
 
    $ pip install -e .["all"]
 
 
 Getting Started
 ---------------
-To get started, take a look at the `tutorials <https://github.com/ComplexGroupInteractions/xgi/tree/main/tutorials>`_
+To get started, take a look at the `tutorials <https://github.com/xgi-org/xgi/tree/main/tutorials>`_
 illustrating the library's basic functionality.
 
 Contributing
 ------------
-Contributions are always welcome. Please report any bugs that you find `here <https://github.com/ComplexGroupInteractions/xgi/issues>`_.
-Or, even better, fork the repository on `GitHub <https://github.com/ComplexGroupInteractions/xgi>`_ and create a pull request (PR).
+Contributions are always welcome. Please report any bugs that you find `here <https://github.com/xgi-org/xgi/issues>`_.
+Or, even better, fork the repository on `GitHub <https://github.com/xgi-org/xgi>`_ and create a pull request (PR).
 We welcome all changes, big or small, and we will help you make the PR if you are new to `git`
-(just ask on the issue and/or see our `contributing guidelines <https://github.com/ComplexGroupInteractions/xgi/tree/main/CONTRIBUTING.md>`_.
+(just ask on the issue and/or see our `contributing guidelines <https://github.com/xgi-org/xgi/tree/main/CONTRIBUTING.md>`_.
 
 How to Cite
 -----------
 We acknowledge the importance of good software to support research, and we note
 that research becomes more valuable when it is communicated effectively. To
 demonstrate the value of XGI, we ask that you cite XGI in your work.
 Currently, the best way to cite XGI is to go to our
-`repository page <https://github.com/ComplexGroupInteractions/xgi>`_ and
+`repository page <https://github.com/xgi-org/xgi>`_ and
 click the "cite this repository" button on the right sidebar. This will generate
 a citation in your preferred format, and will also integrate well with citation managers.
 
 Code of Conduct
 ---------------
-Our full code of conduct, and how we enforce it, can be read in `our repository <https://github.com/ComplexGroupInteractions/xgi/tree/main/CODE_OF_CONDUCT.md>`_.
+Our full code of conduct, and how we enforce it, can be read in `our repository <https://github.com/xgi-org/xgi/tree/main/CODE_OF_CONDUCT.md>`_.
 
 License
 -------
-Released under the 3-Clause BSD license (see the `license file <https://github.com/ComplexGroupInteractions/xgi/tree/main/license.md>`_)
+Released under the 3-Clause BSD license (see the `license file <https://github.com/xgi-org/xgi/tree/main/license.md>`_)
 
 Copyright (C) 2021-2023 XGI Developers
 
 Nicholas Landry <nicholas.landry@colorado.edu>
 
 Leo Torres <leo@leotrs.com>
```

### Comparing `xgi-0.5.6/xgi.egg-info/SOURCES.txt` & `xgi-0.5.7/xgi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,46 +20,53 @@
 requirements/tutorial.txt
 tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
 tutorials/Tutorial 2 - Read and Write.ipynb
 tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
 tutorials/Tutorial 4 - Generative_Models.ipynb
 tutorials/Tutorial 5 - Plotting.ipynb
 tutorials/Tutorial 6 - Statistics.ipynb
+tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
 tutorials/case_study_zhang2022.ipynb
 tutorials/quickstart.ipynb
 tutorials/simplicial_kuramoto_example.ipynb
 xgi/__init__.py
 xgi/convert.py
 xgi/exception.py
 xgi.egg-info/PKG-INFO
 xgi.egg-info/SOURCES.txt
 xgi.egg-info/dependency_links.txt
 xgi.egg-info/requires.txt
 xgi.egg-info/top_level.txt
 xgi/algorithms/__init__.py
 xgi/algorithms/assortativity.py
 xgi/algorithms/centrality.py
+xgi/algorithms/clustering.py
 xgi/algorithms/connected.py
 xgi/classes/__init__.py
 xgi/classes/function.py
 xgi/classes/hypergraph.py
 xgi/classes/hypergraphviews.py
 xgi/classes/reportviews.py
 xgi/classes/simplicialcomplex.py
 xgi/drawing/__init__.py
 xgi/drawing/draw.py
 xgi/drawing/layout.py
 xgi/dynamics/__init__.py
 xgi/dynamics/synchronization.py
 xgi/generators/__init__.py
 xgi/generators/classic.py
-xgi/generators/nonuniform.py
+xgi/generators/lattice.py
+xgi/generators/random.py
+xgi/generators/simple.py
+xgi/generators/simplicial_complexes.py
 xgi/generators/uniform.py
 xgi/linalg/__init__.py
-xgi/linalg/matrix.py
+xgi/linalg/hodge_matrix.py
+xgi/linalg/hypergraph_matrix.py
+xgi/linalg/laplacian_matrix.py
 xgi/readwrite/__init__.py
 xgi/readwrite/bipartite.py
 xgi/readwrite/edgelist.py
 xgi/readwrite/incidence.py
 xgi/readwrite/json.py
 xgi/readwrite/xgi_data.py
 xgi/stats/__init__.py
```

### Comparing `xgi-0.5.6/xgi.egg-info/requires.txt` & `xgi-0.5.7/xgi.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 scipy>=1.8
 pandas>=1.3
 networkx>=2.7
 requests>=2.0
 matplotlib>=3.4
 
 [all]
-black[jupyter]==22.3.0
-twine>=3.4
+github-changelog
 pytest>=7.2
-hypernetx>=1.0
-wheel>=0.36
-sphinx~=4.0
-isort==5.10.1
+pre-commit>=2.12
+black[jupyter]==22.3.0
 sphinx-rtd-theme>=0.4.2
-seaborn>=0.10
-github-changelog
+sphinx_copybutton
+pylint>=2.10
+isort==5.10.1
 matplotlib>=3.3
-pre-commit>=2.12
-asv>=0.5
-numpydoc>=1.1
+seaborn>=0.10
 pytest-cov>=4.0
-jupyter>=1.0
-codecov>=2.1
+numpydoc>=1.1
+twine>=3.4
+sphinx~=4.0
+hypernetx>=1.0
 pillow>=8.2
-sphinx_copybutton
-pylint>=2.10
+wheel>=0.36
+jupyter>=1.0
+asv>=0.5
 
 [benchmarks]
 hypernetx>=1.0
 asv>=0.5
 
 [developer]
 black[jupyter]==22.3.0
@@ -49,13 +48,12 @@
 twine>=3.4
 wheel>=0.36
 github-changelog
 
 [test]
 pytest>=7.2
 pytest-cov>=4.0
-codecov>=2.1
 
 [tutorial]
 jupyter>=1.0
 matplotlib>=3.3
 seaborn>=0.10
```

