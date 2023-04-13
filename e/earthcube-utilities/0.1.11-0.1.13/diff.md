# Comparing `tmp/earthcube_utilities-0.1.11.tar.gz` & `tmp/earthcube_utilities-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthcube_utilities-0.1.11.tar", last modified: Mon Mar 27 20:45:26 2023, max compression
+gzip compressed data, was "earthcube_utilities-0.1.13.tar", last modified: Thu Apr 13 19:37:45 2023, max compression
```

## Comparing `earthcube_utilities-0.1.11.tar` & `earthcube_utilities-0.1.13.tar`

### file list

```diff
@@ -1,90 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.763236 earthcube_utilities-0.1.11/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.771236 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-27 20:45:26.000000 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-27 20:45:26.000000 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:45:26.000000 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-27 20:45:26.000000 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-27 20:45:26.000000 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-27 20:45:26.000000 earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.771236 earthcube_utilities-0.1.11/src/ec/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/check_sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.771236 earthcube_utilities-0.1.11/src/ec/collection/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/collection/rocrate_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/collection/rocrate_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.771236 earthcube_utilities-0.1.11/src/ec/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/datastore/s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/generate_repo_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.771236 earthcube_utilities-0.1.11/src/ec/gleanerio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/gleanerio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/gleanerio/gleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.771236 earthcube_utilities-0.1.11/src/ec/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/manageGraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.783236 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_count_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_count_variablename.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_repo_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_repo_count_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_repo_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_repo_with_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_select_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_select_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_summary_query.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/get_triples_for_a_graph.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_graph_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_keywords.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_triples.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_types.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_count_variablename.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_graphs_startwith.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_select_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_select_graphs.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_summary_query.sparql
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/select_one.sparql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.783236 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/sparql_static/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/graph/sparql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.783236 earthcube_utilities-0.1.11/src/ec/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/notebook/geocodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/notebook/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.783236 earthcube_utilities-0.1.11/src/ec/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/ec_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/ecobjectmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/objects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/src/ec/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/reporting/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/src/ec/sitemap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/sitemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/sitemap/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/src/ec/sos_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/sos_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/sos_json/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/src/ec/sos_json/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/sos_json/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/sos_json/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:26.787236 earthcube_utilities-0.1.11/src/ec/summarize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-03-27 20:45:15.000000 earthcube_utilities-0.1.11/src/ec/summarize/summarize_materializedview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.830700 earthcube_utilities-0.1.13/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.834700 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:37:45.000000 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-13 19:37:45.000000 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:37:45.000000 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 19:37:45.000000 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 19:37:45.000000 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-13 19:37:45.000000 earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.834700 earthcube_utilities-0.1.13/src/ec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/check_sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.834700 earthcube_utilities-0.1.13/src/ec/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/collection/rocrate_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/collection/rocrate_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.834700 earthcube_utilities-0.1.13/src/ec/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/datastore/s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2799 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/generate_graph_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.834700 earthcube_utilities-0.1.13/src/ec/gleanerio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/gleanerio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/gleanerio/gleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.834700 earthcube_utilities-0.1.13/src/ec/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/manageGraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.838701 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_types_top_level.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_count_variablename.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_graph_sizes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_count_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_with_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_select_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_select_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_summary_query.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_urn_w_types_toplevel.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/org_all_org_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/org_all_returns_properties.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/org_all_returns_urns.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_keywords.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_triples.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_types.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_count_variablename.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_graph_sizes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_graphs_startwith.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_select_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_select_graphs.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_summary_query.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/select_one.sparql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.838701 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/sparql_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_files/urn_triples_for_a_graph.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/graph/sparql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.838701 earthcube_utilities-0.1.13/src/ec/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/logger/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/missing_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.838701 earthcube_utilities-0.1.13/src/ec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/notebook/geocodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/notebook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.838701 earthcube_utilities-0.1.13/src/ec/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/ec_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/ecobjectmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/objects/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/query_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.838701 earthcube_utilities-0.1.13/src/ec/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/reporting/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/src/ec/sitemap/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/sitemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/sitemap/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/src/ec/sos_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/sos_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/sos_json/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/src/ec/sos_json/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/sos_json/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/sos_json/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:37:45.842701 earthcube_utilities-0.1.13/src/ec/summarize/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-13 19:37:35.000000 earthcube_utilities-0.1.13/src/ec/summarize/summarize_materializedview.py
```

### Comparing `earthcube_utilities-0.1.11/PKG-INFO` & `earthcube_utilities-0.1.13/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthcube_utilities
-Version: 0.1.11
+Version: 0.1.13
 Summary: A package of utilities for NSF Earthcube Geocodes Project
 Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Maintainer-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Project-URL: Homepage, https://www.earthcube.org/
 Project-URL: Bug Tracker, https://github.com/earthcube/earthcube_utilities/issues
 Project-URL: Geocodes Documentation, https://earthcube.github.io/geocodes_documentation/
 Project-URL: Source, https://github.com/earthcube/earthcube_utilities
@@ -30,16 +30,22 @@
 `python3 -m pip install  earthcube-utilities`
 
 
 
 ## Developers
 
 ### scripts
-In theory, if pip installed, theree is one script at present,
-`generaterepostats --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ -s3 localhost:9000 --s3bucket gleaner`
+When installed via pip:
+
+`query_graph SPARQL_FILE --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ `
+
+`check_sitemap SITEMAP_URL --output FILE --no-check-url  `
+
+`generategraphstats --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ -s3 localhost:9000 --s3bucket gleaner`
+
 
 from [console scripts](https://setuptools.pypa.io/en/latest/userguide/entry_point.html#console-scripts)
 
 ### local development mode
 ```shell
 cd earthcube_utiltiies
 pip3 install -e .
```

### Comparing `earthcube_utilities-0.1.11/README.md` & `earthcube_utilities-0.1.13/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,22 @@
 `python3 -m pip install  earthcube-utilities`
 
 
 
 ## Developers
 
 ### scripts
-In theory, if pip installed, theree is one script at present,
-`generaterepostats --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ -s3 localhost:9000 --s3bucket gleaner`
+When installed via pip:
+
+`query_graph SPARQL_FILE --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ `
+
+`check_sitemap SITEMAP_URL --output FILE --no-check-url  `
+
+`generategraphstats --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ -s3 localhost:9000 --s3bucket gleaner`
+
 
 from [console scripts](https://setuptools.pypa.io/en/latest/userguide/entry_point.html#console-scripts)
 
 ### local development mode
 ```shell
 cd earthcube_utiltiies
 pip3 install -e .
```

### Comparing `earthcube_utilities-0.1.11/pyproject.toml` & `earthcube_utilities-0.1.13/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "earthcube_utilities"
-version = "0.1.11"
+version = "0.1.13"
 dynamic = ["dependencies"]
 description = "A package of utilities for NSF Earthcube Geocodes Project"
 readme =  "README.md"
 
 authors = [
     {name = "Mike Bobak", email = "mbobak@illinois.edu"},
     {name= "David Valentine", email="dwvalentine@ucsd.edu"}
@@ -29,16 +29,18 @@
 "Bug Tracker" = "https://github.com/earthcube/earthcube_utilities/issues"
 "Geocodes Documentation" = "https://earthcube.github.io/geocodes_documentation/"
 "Source" = "https://github.com/earthcube/earthcube_utilities"
 
 # if the name of the module is the same as the name of the script, then you get
 #    'module' object is not callable
 [project.scripts]
-generaterepostats = "ec.generate_repo_stats:start"
+generategraphstats = "ec.generate_graph_stats:start"
 check_sitemap = "ec.check_sitemap:start"
+query_graph = "ec.query_graph:start"
+missing_report = "ec.missing_report:start"
 
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 [tool.setuptools.packages.find]
 where = ["src"]
 [tool.setuptools.package-data]
@@ -47,8 +49,8 @@
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel"
 ]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
```

### Comparing `earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/PKG-INFO` & `earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthcube-utilities
-Version: 0.1.11
+Version: 0.1.13
 Summary: A package of utilities for NSF Earthcube Geocodes Project
 Author-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Maintainer-email: Mike Bobak <mbobak@illinois.edu>, David Valentine <dwvalentine@ucsd.edu>
 Project-URL: Homepage, https://www.earthcube.org/
 Project-URL: Bug Tracker, https://github.com/earthcube/earthcube_utilities/issues
 Project-URL: Geocodes Documentation, https://earthcube.github.io/geocodes_documentation/
 Project-URL: Source, https://github.com/earthcube/earthcube_utilities
@@ -30,16 +30,22 @@
 `python3 -m pip install  earthcube-utilities`
 
 
 
 ## Developers
 
 ### scripts
-In theory, if pip installed, theree is one script at present,
-`generaterepostats --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ -s3 localhost:9000 --s3bucket gleaner`
+When installed via pip:
+
+`query_graph SPARQL_FILE --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ `
+
+`check_sitemap SITEMAP_URL --output FILE --no-check-url  `
+
+`generategraphstats --graphendpoint https://graph.geocodes-dev.earthcube.org/blazegraph/namespace/earthcube/ -s3 localhost:9000 --s3bucket gleaner`
+
 
 from [console scripts](https://setuptools.pypa.io/en/latest/userguide/entry_point.html#console-scripts)
 
 ### local development mode
 ```shell
 cd earthcube_utiltiies
 pip3 install -e .
```

### Comparing `earthcube_utilities-0.1.11/src/earthcube_utilities.egg-info/SOURCES.txt` & `earthcube_utilities-0.1.13/src/earthcube_utilities.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,55 +4,73 @@
 src/earthcube_utilities.egg-info/PKG-INFO
 src/earthcube_utilities.egg-info/SOURCES.txt
 src/earthcube_utilities.egg-info/dependency_links.txt
 src/earthcube_utilities.egg-info/entry_points.txt
 src/earthcube_utilities.egg-info/requires.txt
 src/earthcube_utilities.egg-info/top_level.txt
 src/ec/check_sitemap.py
-src/ec/generate_repo_stats.py
+src/ec/generate_graph_stats.py
+src/ec/missing_report.py
+src/ec/query_graph.py
+src/ec/collection/__init__.py
 src/ec/collection/rocrate_archive.py
 src/ec/collection/rocrate_collection.py
 src/ec/datastore/__init__.py
 src/ec/datastore/s3.py
 src/ec/gleanerio/__init__.py
 src/ec/gleanerio/gleaner.py
+src/ec/graph/__init__.py
 src/ec/graph/manageGraph.py
 src/ec/graph/sparql_query.py
 src/ec/graph/sparql_files/__init__.py
 src/ec/graph/sparql_files/all_count_datasets.sparql
 src/ec/graph/sparql_files/all_count_keywords.sparql
 src/ec/graph/sparql_files/all_count_multiple_versioned_datasets.sparql
 src/ec/graph/sparql_files/all_count_triples.sparql
 src/ec/graph/sparql_files/all_count_types.sparql
+src/ec/graph/sparql_files/all_count_types_top_level.sparql
 src/ec/graph/sparql_files/all_count_variablename.sparql
+src/ec/graph/sparql_files/all_graph_sizes.sparql
 src/ec/graph/sparql_files/all_repo_count_datasets.sparql
 src/ec/graph/sparql_files/all_repo_count_graphs.sparql
 src/ec/graph/sparql_files/all_repo_count_keywords.sparql
+src/ec/graph/sparql_files/all_repo_count_types.sparql
 src/ec/graph/sparql_files/all_repo_count_versioned_datasets.sparql
 src/ec/graph/sparql_files/all_repo_with_keywords.sparql
 src/ec/graph/sparql_files/all_select_datasets.sparql
 src/ec/graph/sparql_files/all_select_graphs.sparql
 src/ec/graph/sparql_files/all_summary_query.sparql
+src/ec/graph/sparql_files/all_urn_w_types_toplevel.sparql
 src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql
-src/ec/graph/sparql_files/get_triples_for_a_graph.sparql
+src/ec/graph/sparql_files/org_all_org_triples.sparql
+src/ec/graph/sparql_files/org_all_returns_properties.sparql
+src/ec/graph/sparql_files/org_all_returns_urns.sparql
+src/ec/graph/sparql_files/q_n_o_exact_query__returns_properties.sparql
+src/ec/graph/sparql_files/q_n_o_query_returns_urn.sparql
 src/ec/graph/sparql_files/repo_count_datasets.sparql
-src/ec/graph/sparql_files/repo_count_graph_triples.sparql
 src/ec/graph/sparql_files/repo_count_graphs.sparql
 src/ec/graph/sparql_files/repo_count_keywords.sparql
 src/ec/graph/sparql_files/repo_count_multi_versioned_datasets.sparql
 src/ec/graph/sparql_files/repo_count_triples.sparql
+src/ec/graph/sparql_files/repo_count_triples_by_graph.sparql
 src/ec/graph/sparql_files/repo_count_types.sparql
 src/ec/graph/sparql_files/repo_count_variablename.sparql
+src/ec/graph/sparql_files/repo_graph_sizes.sparql
 src/ec/graph/sparql_files/repo_graphs_startwith.sparql
 src/ec/graph/sparql_files/repo_select_datasets.sparql
 src/ec/graph/sparql_files/repo_select_graphs.sparql
 src/ec/graph/sparql_files/repo_summary_query.sparql
+src/ec/graph/sparql_files/repo_urn_w_types_toplevel.sparql
 src/ec/graph/sparql_files/select_one.sparql
+src/ec/graph/sparql_files/subj_construct_w_blanknodes.sparql
+src/ec/graph/sparql_files/urn_triples_for_a_graph.sparql
 src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql
 src/ec/graph/sparql_files/sparql_static/repo_graphs_opentopo.sparql
+src/ec/logger/__init__.py
+src/ec/logger/log.py
 src/ec/notebook/__init__.py
 src/ec/notebook/geocodes.py
 src/ec/notebook/utils.py
 src/ec/objects/__init__.py
 src/ec/objects/datacatalog.py
 src/ec/objects/datasets.py
 src/ec/objects/ec_object.py
```

### Comparing `earthcube_utilities-0.1.11/src/ec/check_sitemap.py` & `earthcube_utilities-0.1.13/src/ec/check_sitemap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 from io import StringIO
 
 from ec.sitemap.sitemap import Sitemap
 import argparse
-from distutils.util import strtobool
+
+from ec.logger import config_app
+
+log = config_app()
+
 def sitemap_checker(args):
+    log.debug(" Sitemap")
+    """Sitemap checker. Default option  checks if url is sitemap exist"""
     sitemap = Sitemap(args.sitemapurl, no_progress_bar=args.no_progress)
     if  not args.nocheck :
         sitemap.check_urls()
 
     return sitemap.get_url_report()
 
 def start():
+    """
+        Run the sitemap_checker program.
+        Sitemap checker. Default option  checks if url is sitemap exist.
+        Arguments:
+            args: Arguments passed from the command line.
+        Returns:
+            result of check as csv.
+
+    """
     parser = argparse.ArgumentParser()
     parser.add_argument("sitemapurl", help='sitemapurl')
     parser.add_argument("--output", type=argparse.FileType('w'), help='output file')
     parser.add_argument("--no-url-check",action='store_true', dest="nocheck" ,help='output file', default=False)
-    parser.add_argument("--no-progress", action='store_false',   dest="no_progress" ,help='no progress bad', default=True)
+    parser.add_argument("--no-progress", action='store_false',   dest="no_progress" ,help='no progress bar', default=True)
     args = parser.parse_args()
 
     result = sitemap_checker(args)
     if args.output:
+        log.info(" Sitemap written to file"  )
         args.output.write(result)
     else:
         print(result)
+
 if __name__ == '__main__':
 
     result = start()
```

### Comparing `earthcube_utilities-0.1.11/src/ec/collection/rocrate_collection.py` & `earthcube_utilities-0.1.13/src/ec/collection/rocrate_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,34 @@
 from os import path
 import uuid
 
 import uuid as uuid
 from rocrate.rocrate import ROCrate
 from rocrate.model.person import Person
 from rocrate.model.softwareapplication import SoftwareApplication
+from rocrate.model.contextentity import ContextEntity
+from rocrate.model.data_entity import DataEntity
+from rocrate.model.computationalworkflow import ComputationalWorkflow
 
 from rocrate.model.dataset import Dataset
 from rocrate.model.metadata import Metadata
 from rocrate.model.file import File
 from rocrate.model.file_or_dir import FileOrDir
 
 from rocrateValidator import validate
-from datastore.s3 import MinioDatastore
+from ec.datastore.s3 import MinioDatastore
+
+## Fair Signposting
+# https://pypi.org/project/signposting/
+# https://signposting.org/FAIR/
+# https://fair-impact.eu/enabling-fair-signposting-and-ro-crate-contentmetadata-discovery-and-consumption
+#######
 
 # issue https://github.com/earthcube/GeoCODES-Metadata/issues/5
-# logic that might be utilizle
+# logic that might be utilize
 # https://github.com/MBcode/ec/blob/8255d7c1312faca721000535b85cd1e22470a73e/ec.py#L2472
 
 ##### THOUGHTS #####
 # creating a crate
 # it will have multiple objects that are in a collection.
 # for a collection on the client, we will ask the user to select the distribution to be utilize
 # that will be added to the rocrate
@@ -33,15 +42,16 @@
 
 # then create a friggin tool that read the firrig crate from frigging s3,
 # now, that it is downloaded, head the distribitions.
 # create tool to download the frigging links from the firring distributions.
 # then tell the tool where the files are, and execute the tool
 #  how frigging hard can that workflow be to understand.
 #  linking tool to the datasets to the tool will be the fun part
-#
+
+
 
 #####
 # add distribution... up here to prevent some linting errors
 ######
 """
  web etities: https://www.researchobject.org/ro-crate/1.1/data-entities.html#web-based-data-entities
  {
@@ -76,15 +86,15 @@
     "contentSize": "82818928"
   }
 """
 
 
 
 # this tool will read information from an s3 bucket, or a local zip crate
-def readDecaoderRoCrate(crate, bucket="gleaner", s3endpoint=None) -> ROCrate:
+def readDecoderRoCrate(crate, bucket="gleaner", s3endpoint=None) -> ROCrate:
     if (s3endpoint is not None):
         client = MinioDatastore(s3endpoint)
         data = client.getRoCrateFile(crate, bucket=bucket)
         p = path.join(tempfile.gettempdir(), crate)
         with open(p, mode='wb') as f:
             f.write(crate)
         crate = p
@@ -108,21 +118,31 @@
 
         m = hashlib.md5(proposedid.encode(encoding='UTF-8', errors='strict')).hexdigest()
     else:
         # random id
         m = uuid.uuid4().hex
     return f"uuid:{m}"
 
-DATASET_DATADOWNLOAD = '@DataDownload'  # distribution
-DATASET_DATASET = '@Dataset'  # Dataset
-DATASET_WEBENTITY = '@File'  # url, aka web link
+DATASET__DATA_DOWNLOAD = '@DataDownload'  # distribution
+DATASET__DATASET = '@Dataset'  # Dataset
+DATASET__WEB_ENTITY = '@File'  # url, aka web link
+# DATASET__WEB_SERVICE = '@SERVICE'   #how do we do a service?
 
 ## we do not want to override the methods, we want to add methods
-class sosRocrate(ROCrate):
+# crates are a bit of a pain because they use disk layout, rather than just metadata file
+
+class SosRocrate(ROCrate):
+    """ Science on Schema(SOS) ROCrate Object.
+    ROCrate plus methods to easily add SOS information to an ROCrate
+
+    USE:
+     [Consuming an RO-Crate](https://github.com/ResearchObject/ro-crate-py#consuming-an-ro-crate):
+    use SosRocrate instead of RoCrate
 
+    """
     def nameCrate(self, aName):
         self.nameCrate(aName)
 
     # this is the creator of the crate, it should be a sos_person
     # probably not correct, but it's a start
     def addSosCreator(self, crate, username):
         properties = {"name": username}
@@ -140,32 +160,50 @@
         self.publisher = creator
 
         # pption 1 it's a file
 
 
 
 
-    def addSosDistribution(self, crate, dataset_jsonld, distribution_to_add=None, distType=DATASET_DATADOWNLOAD):
+    def addSosDistribution(self, crate, dataset_jsonld, distribution_to_add=None, distType=DATASET__DATA_DOWNLOAD):
         aurl = dataset_jsonld.get('url')
         name = dataset_jsonld.get('name')
         if distribution_to_add is None:
             #kw = {"fetch_remote": fetch_remote, "validate_url": validate_url}
             kw = {"name": name}
             self.add_file(aurl, properties=kw)
-        elif distType == DATASET_DATADOWNLOAD :
-            pass
-        elif distType == DATASET_DATASET:
+        elif distType == DATASET__DATA_DOWNLOAD :
             pass
+        elif distType == DATASET__DATASET:
+            self.add_dataset(source=dataset_jsonld)
 
     def addSosServicesAsEntity(self,crate, url=None, name=None):
         kw = {"name": name}
         self.add_file(source=url, properties=kw)
         pass
 
-    def addSosURL(self,crate, url=None, name=None):
-        kw = {"name": name}
-        self.add_file(source=url, properties=kw)
+    def addSosURL(self, url=None, name=None):
+        properties = {"name":name}
+        self.add_file(source=url, properties=properties)
         #self.add_file(url, identifier=CreateIdentifier(url), properties=kw)
 
+# two possible ways to add the whole JSONLD.
+    # 1. File: url plus the jsonld
+    # 2. Dataset (aka directory): url to geocodes, plus jsonld
+
+    # these need to check that these are datasets ;)
+    def addSosDatasetAsFile(self, dataset_jsonld,  url):
+        properties = dataset_jsonld
+        self.add_file(source=url, properties=properties)
+### humm https://github.com/ResearchObject/ro-crate-py#adding-entities-with-an-arbitrary-type
+    def addSosDatasetAsDataset(self, dataset_jsonld, urn, distType=DATASET__DATASET):
+        self.add_dataset(dest_path=urn, properties=dataset_jsonld)
+
+
+    # this does not get added to hasParts... aka does not get Identifieed as a Dataset
+    def addSosDatasetAsCtxEntity(self, dataset_jsonld, urn, distType=DATASET__DATASET):
+        """Not useful. this does not get added to hasParts... aka does not get Identifieed as a Dataset """
+        datasetCtxEntity =ContextEntity(self, identifier=urn, properties=dataset_jsonld)
 
-def addContact(self, sos_contact):
-        pass
+        self.add(datasetCtxEntity)
+    def addSosContact(self, sos_contact):
+            pass
```

### Comparing `earthcube_utilities-0.1.11/src/ec/datastore/s3.py` & `earthcube_utilities-0.1.13/src/ec/datastore/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from io import BytesIO
 
 import minio
 import pydash
 from pydash.collections import find
 
-def shaFroms3Path(path):
-    split = path.split()
-    return split[len(split)-1]
+def shaFroms3Path(path, extension=None):
+    split = path.split("/")
+    sha = split[len(split)-1]
+    if extension is not None:
+        sha = pydash.strings.replace_end(sha, extension, '')
+    return sha
 
 
 """
 Basic abstraction, in case someone want to store files in a 
 different method
 """
 class bucketDatastore():
@@ -62,22 +65,31 @@
         return count
 
     def getJsonLD(self, bucket, repo, sha):
         path = f"{self.paths['summon']}/{repo}/{sha}.jsonld"
         s3ObjectInfo = {"bucket_name": bucket, "object_name": path}
         resp = self.getFileFromStore(s3ObjectInfo)
         return resp
+
     def listSummonedUrls(self,bucket, repo):
         """  returns list of urns with urls"""
         jsonlds = self.listJsonld(bucket, repo, include_user_meta=True)
         objs = map(lambda f: self.s3client.stat_object(f.bucket_name, f.object_name), jsonlds)
         # for ob in objs:
         #     print(ob)
         o_list = list(map(lambda f: {"sha": shaFroms3Path(f.object_name), "url": f.metadata["X-Amz-Meta-Url"]}, objs))
         return o_list
+    def listSummonedSha(self,bucket, repo):
+        """  returns list of urns with urls"""
+        jsonlds = self.listJsonld(bucket, repo, include_user_meta=False)
+        objs = map(lambda f: shaFroms3Path( f.object_name, extension=".jsonld"), jsonlds)
+        # for ob in objs:
+        #     print(ob)
+        o_list = list(objs)
+        return o_list
 
     def getJsonLDMetadata(self, bucket, repo, sha):
         path = f"{self.paths['summon']}/{repo}/{sha}.jsonld"
         s3ObjectInfo = {"bucket_name": bucket, "object_name": path}
         tags = self.getFileMetadataFromStore(s3ObjectInfo)
 
         return tags
@@ -89,14 +101,18 @@
     '''Cleans the name of slashes... might need more in the future.'''
     def getCleanObjectName(s3ObjectName) -> str:
         return s3ObjectName.replace('/','__')
 
     def listMilledRdf(self,bucket, repo,urnonly=False):
         path = f"{self.paths['milled']}/{repo}/"
         return self.listPath(bucket, path)
+    def listMilledSha(self,bucket, repo,urnonly=False):
+        paths = self.listMilledRdf(bucket,repo)
+        shas = list(map(lambda p: shaFroms3Path(p.object_name, extension=".rdf"), paths))
+        return shas
 
     def countMilledRdf(self,bucket, repo) -> int:
         count = len(list(self.listMilledRdf(bucket,repo)))
         return count
     ### methods for reporting
     '''
     Reporting will have to pull the original and put back to the datastore
@@ -192,23 +208,23 @@
         s3obj = self.s3client.stat_object(s3ObjectInfo.bucket_name, s3ObjectInfo.object_name)
         for o in s3obj:
             user_meta = pydash.collections.filter_(o,lambda m: m.startswith("X-Amz-Meta") )
         # this needs to return the metadata
         return user_meta
 
     def putReportFile(self, bucket, repo, filename, json_str, date="latest"):
-        path = f"{self.paths['reports']}/{repo}/{date}/{filename}"
+        path = f"{self.paths['report']}/{repo}/{date}/{filename}"
         f = BytesIO()
         length = f.write(bytes(json_str, 'utf-8'))
         f.seek(0)
         resp = self.s3client.put_object(bucket, path, f,length=length)
         return resp.bucket_name, resp.object_name
 
     def getReportFile(self, bucket, repo, filename):
-        path = f"{self.paths['reports']}/{repo}/{filename}"
+        path = f"{self.paths['report']}/{repo}/{filename}"
         s3ObjectInfo = {"bucket_name": bucket, "object_name": path}
         resp = self.getFileFromStore(s3ObjectInfo)
         return resp
 
     def getLatestRelaseFile(self, bucket, repo):
         path = f"{self.paths['graph']}/latest/summonded{repo}_latest_release.nq"
         s3ObjectInfo = {"bucket_name":bucket,"object_name": path}
@@ -218,11 +234,11 @@
     def getRelasePaths(self, bucket):
         path = f"{self.paths['graph']}/latest/"
         files = self.listPath(bucket, path)
         paths = list(map(lambda f:  f.object_name, files))
         return paths
 
     def getRoCrateFile(self, filename, bucket="gleaner", user="public"):
-        path = f"/{self.paths['collections']}/{user}/{filename}"
+        path = f"/{self.paths['collection']}/{user}/{filename}"
         crate = self.s3client.get_object(bucket, path)
         return crate
```

### Comparing `earthcube_utilities-0.1.11/src/ec/gleanerio/gleaner.py` & `earthcube_utilities-0.1.13/src/ec/gleanerio/gleaner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import io
 import json
 import os
 import shutil
 import subprocess
-from typing import Tuple
+from typing import Tuple, Any
 
 import yaml
 
 
 def endpointUpdateNamespace( fullendpoint: str, namepsace='temp') -> str:
     paths = fullendpoint.split('/')
     paths[len(paths)-2] = namepsace
@@ -70,15 +70,15 @@
         # delete config file here
         return result.stdout
     else:
         raise Exception(f"glcon not found at {glcon}. Pass path to glcon with --glcon")
 
 
 
-def getGleaner( cfgfile):
+def getGleaner( cfgfile) -> Tuple[str,str,Any]:
     with open(cfgfile, "r") as stream:
         try:
             cfg =(yaml.safe_load(stream))
         except yaml.YAMLError as exc:
             print(exc)
     bucket = cfg['minio']['bucket']
     s3endpoint = cfg['minio']['address']
@@ -98,29 +98,29 @@
 
 def getSourcesFromGleaner(cfgfile, sourcename=None):
     s3endpoint,  bucket, cfg = getGleaner(cfgfile)
     sources = cfg['sources']
     if sourcename is None:
         return sources
     else:
-        matched = list(filter(lambda source: source.name == sourcename, sources))
+        matched = list(filter(lambda source: source.get('name') == sourcename, sources))
         if len(matched) == 1:
             return matched[0]
         else:
             return None
 
 
 def getSitemapSourcesFromGleaner(cfgfile, sourcename=None):
     s3endpoint,  bucket, cfg = getGleaner(cfgfile)
     sources = cfg['sources']
-    sources =list(filter(lambda source: source.sourcetype == "sitemap", sources))
+    sources = list(filter(lambda source: source.get('sourcetype') == "sitemap", sources))
     if sourcename is None:
         return sources
     else:
-        matched = list(filter(lambda source: source.name == sourcename, sources))
+        matched = list(filter(lambda source: source.get('name') == sourcename, sources))
         if len(matched) == 1:
             return matched[0]
         else:
             return None
 
 
 def reviseGleanerConf(cfg: str, bucket:str) -> object:
@@ -181,8 +181,8 @@
 
 ## needs to be in utils
 def _validateJSON(jsonData):
     try:
         json.loads(jsonData)
     except ValueError as err:
         return False, err
-    return True, None
+    return True, None
```

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/manageGraph.py` & `earthcube_utilities-0.1.13/src/ec/graph/manageGraph.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_repo_count_graphs.sparql` & `earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_repo_count_graphs.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_summary_query.sparql` & `earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_summary_query.sparql`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 prefix schema: <https://schema.org/>
 SELECT distinct ?subj ?g ?resourceType ?name ?description  ?pubname
         (GROUP_CONCAT(DISTINCT ?placename; SEPARATOR=", ") AS ?placenames)
-        (GROUP_CONCAT(DISTINCT ?kwu; SEPARATOR=", ") AS ?kw) ?datep
+        (GROUP_CONCAT(DISTINCT ?kwu; SEPARATOR=", ") AS ?kw) ?datep ?sosType
         #(GROUP_CONCAT(DISTINCT ?url; SEPARATOR=", ") AS ?disurl)
         WHERE {
           graph ?g {
              ?subj schema:name ?name .
              ?subj schema:description ?description .
-            ?subj a schema:Dataset
+            values ?sosType {
+            schema:Dataset
+#        schema:DataCatalog
+            }
+        #     ?subj a ?sosType .
             Minus {?subj a schema:Person } .
- #BIND (IF (exists {?subj a schema:Dataset .} ||exists{?subj a schema:DataCatalog .} , "data", "tool") AS ?resourceType).
-                   ?subj a ?resourceType .
+ BIND (IF (exists {?subj a schema:Dataset .} ||exists{?subj a schema:DataCatalog .} , "data", "tool") AS ?resourceType).
+
             optional {?subj schema:distribution/schema:url|schema:subjectOf/schema:url ?url .}
             OPTIONAL {?subj schema:datePublished ?date_p .}
             OPTIONAL {?subj schema:publisher/schema:name|schema:sdPublisher|schema:provider/schema:name ?pub_name .}
             OPTIONAL {?subj schema:spatialCoverage/schema:name ?place_name .}
             OPTIONAL {?subj schema:keywords ?kwu .}
            # Query should not return "No datePublished" is not a valid Date "YYYY-MM-DD" so
             # UI Date Select failed, because it expects an actual date
            # BIND ( IF ( BOUND(?date_p), ?date_p, "No datePublished") as ?datep ) .
              BIND ( IF ( BOUND(?date_p), ?date_p, "1900-01-01") as ?datep ) .
             BIND ( IF ( BOUND(?pub_name), ?pub_name, "No Publisher") as ?pubname ) .
             BIND ( IF ( BOUND(?place_name), ?place_name, "No spatialCoverage") as ?placename ) .
              }
+
         }
-        GROUP BY ?subj ?pubname ?placenames ?kw ?datep   ?name ?description  ?resourceType ?g
+        GROUP BY ?subj ?pubname ?placenames ?kw ?datep   ?name ?description  ?resourceType ?sosType ?g
```

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql` & `earthcube_utilities-0.1.13/src/ec/graph/sparql_files/all_versioned_datasets_multiple_versions.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/sparql_files/repo_summary_query.sparql` & `earthcube_utilities-0.1.13/src/ec/graph/sparql_files/repo_summary_query.sparql`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 prefix schema: <https://schema.org/>
 SELECT distinct ?subj ?g ?resourceType ?name ?description  ?pubname
         (GROUP_CONCAT(DISTINCT ?placename; SEPARATOR=", ") AS ?placenames)
-        (GROUP_CONCAT(DISTINCT ?kwu; SEPARATOR=", ") AS ?kw) ?datep
+        (GROUP_CONCAT(DISTINCT ?kwu; SEPARATOR=", ") AS ?kw) ?datep ?sosType
         #(GROUP_CONCAT(DISTINCT ?url; SEPARATOR=", ") AS ?disurl)
         WHERE {
           graph ?g {
              ?subj schema:name ?name .
              ?subj schema:description ?description .
-            ?subj a schema:Dataset
+                         values ?sosType {
+               schema:Dataset
+#               schema:DataCatalog
+            }
+            #?subj a schema:Dataset .
+           #  ?subj a ?sosType .
             Minus {?subj a schema:Person } .
- #BIND (IF (exists {?subj a schema:Dataset .} ||exists{?subj a schema:DataCatalog .} , "data", "tool") AS ?resourceType).
-                   ?subj a ?resourceType .
+ BIND (IF (exists {?subj a schema:Dataset .} ||exists{?subj a schema:DataCatalog .} , "data", "tool") AS ?resourceType).
+
             optional {?subj schema:distribution/schema:url|schema:subjectOf/schema:url ?url .}
             OPTIONAL {?subj schema:datePublished ?date_p .}
             OPTIONAL {?subj schema:publisher/schema:name|schema:sdPublisher|schema:provider/schema:name ?pub_name .}
             OPTIONAL {?subj schema:spatialCoverage/schema:name ?place_name .}
             OPTIONAL {?subj schema:keywords ?kwu .}
            # Query should not return "No datePublished" is not a valid Date "YYYY-MM-DD" so
             # UI Date Select failed, because it expects an actual date
            # BIND ( IF ( BOUND(?date_p), ?date_p, "No datePublished") as ?datep ) .
              BIND ( IF ( BOUND(?date_p), ?date_p, "1900-01-01") as ?datep ) .
             BIND ( IF ( BOUND(?pub_name), ?pub_name, "No Publisher") as ?pubname ) .
             BIND ( IF ( BOUND(?place_name), ?place_name, "No spatialCoverage") as ?placename ) .
              }
         FILTER( CONTAINS(str(?g), "${repo}") )
         }
-        GROUP BY ?subj ?pubname ?placenames ?kw ?datep   ?name ?description  ?resourceType ?g
+        GROUP BY ?subj ?pubname ?placenames ?kw ?datep   ?name ?description  ?resourceType ?sosType ?g
```

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql` & `earthcube_utilities-0.1.13/src/ec/graph/sparql_files/sparql_static/earthref_versioned_datasets.sparql`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.11/src/ec/graph/sparql_query.py` & `earthcube_utilities-0.1.13/src/ec/graph/sparql_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This basically wraps sparqldataframe,
 and contains a way to get resources that are the sparql queries,
 and few helpers to basic queries
 """
 import pandas
+from  pydash import  ends_with, replace_end, sort
 import sparqldataframe
 from string import Template
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
@@ -28,34 +29,41 @@
     """ Query a SPARQL endpoint, and return a Pandas Dataframe
 
     Parameters:
        template_name: name of templates in the ec.graph.sparql_files directory
        endpoint: SPARQL endpoint url
        parameters: object with the names to fill in template eg {"repo": "reponame"}
     """
-    query = _getFileFromResources(f"{template_name}")
+    query = _getSparqlFileFromResources(f"{template_name}")
     q_template = Template(query)
     thsGraphQuery = q_template.substitute(parameters)
     q_df = sparqldataframe.query(endpoint, thsGraphQuery)
     return q_df
 
 ## this will need to be done to package specifications.
 # https://stackoverflow.com/questions/6028000/how-to-read-a-static-file-from-inside-a-python-package
-def _getFileFromResources(filename) -> str:
+def _getSparqlFileFromResources(filename) -> str:
     """ retrieves sparql file from the sparql_files folder when in a package"""
     resourcename = f"{filename}.sparql"
     resource = pkg_resources.read_text(sparqlfiles, resourcename)
     return resource
     # with open(f"./resources/{filename}", "r") as stream:
     #     try:
     #         return stream.read()
     #     except Exception as exc:
     #         print(exc)
+def listSparqlFilesFromResources() -> str:
+    """ retrieves sparql file from the sparql_files folder when in a package"""
+    resource = pkg_resources.contents(sparqlfiles)
+    files = filter( lambda f: ends_with(f, ".sparql"), resource)
+    files = map(lambda f: replace_end(f,".sparql",""), files)
+    files = sort(list(files))
+    return files
 
 def getAGraph(  g, endpoint: str) -> pandas.DataFrame:
     """Query a SPARQL endpoint and return a Pandas Dataframe for a geocodes object"""
-    query = _getFileFromResources('get_triples_for_a_graph')
+    query = _getSparqlFileFromResources('get_triples_for_a_graph')
     q_template = Template(query)
-    thsGraphQuery = q_template.substitute(g=g)
+    thsGraphQuery = q_template.substitute(urn=g)
     g_df = sparqldataframe.query(endpoint, thsGraphQuery)
 
     return g_df
```

### Comparing `earthcube_utilities-0.1.11/src/ec/notebook/utils.py` & `earthcube_utilities-0.1.13/src/ec/notebook/utils.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.11/src/ec/objects/ecobjectmanager.py` & `earthcube_utilities-0.1.13/src/ec/objects/ecobjectmanager.py`

 * *Files identical despite different names*

### Comparing `earthcube_utilities-0.1.11/src/ec/sitemap/sitemap.py` & `earthcube_utilities-0.1.13/src/ec/sitemap/sitemap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import csv
 import logging
 from io import StringIO
 
 import advertools as adv
+import numpy as np
 import pandas
 from numpy import ndarray
 from pandarallel import pandarallel
 from pandas import DataFrame
 
 import requests, sys, os
 import yaml
@@ -58,19 +60,19 @@
         """ does the provided sitemap URL exist."""
         return self._validSitemap
 
     def errors(self):
         return self.errors
     def uniqueItems(self):
         """list of unqiue sitemaps records"""
-        return self.sitemap_df.sitemap.unique()
+        return self.sitemap_df.sitemap.unique().tolist()
 
     def uniqueUrls(self) :
         """Returns a pandas series of the URLS'"""
-        return self.sitemap_df["loc"].unique()
+        return self.sitemap_df["loc"].unique().tolist()
 
     def check_urls(self) -> DataFrame:
         """This will run head on the list of url's in the pandas dataframe.
         It will append columns ("url_response","content_type") to the sitemap_df
         """
 
         # add columns to the dataframe. clear out any previous values
@@ -90,15 +92,15 @@
         return df
 
     def get_url_report(self) -> str:
         """returns a csv of the 'loc','lastmod','url_response', 'content_type' """
         if not self._checkedUrls:
             self.check_urls()
         out= StringIO()
-        self.sitemap_df.to_csv(out, index=False,
+        self.sitemap_df.to_csv(out, index=False, quoting=csv.QUOTE_ALL,
                 columns=['loc','lastmod','url_response', 'content_type']
               #                 columns=['loc','lastmod',"url_response/content_type"]
                                )
         return out.getvalue()
 
 class GleanerioSourceSitemap(Sitemap):
     """ For a provided GleanerIO source record, create a Sitemap object to utilize"""
```

### Comparing `earthcube_utilities-0.1.11/src/ec/sos_json/rdf.py` & `earthcube_utilities-0.1.13/src/ec/sos_json/rdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 import pandas
 import json
 from string import Template
 
 from pyld import jsonld
 from rdflib import URIRef, BNode, Literal, Graph, Dataset
 
@@ -15,15 +17,15 @@
 def is_http(u: str) -> bool:
     if not isinstance(u, str) :
         print("might need to set LD_cache") #have this where predicate called
         return None
     #might also check that the str has no spaces in it,&warn/die if it does
     return u.startswith("http")
 
-def createRDFNode(nodeValue: str) -> Literal | BNode | URIRef:
+def createRDFNode(nodeValue: str) -> Union[Literal, BNode ,URIRef]:
     "fix_url and quote otherwise"
     if not isinstance(nodeValue,str):
         if  (nodeValue is None) or  (pandas.isnull(nodeValue)):
             return Literal("")
         return Literal(nodeValue)
     else:
         if nodeValue.startswith("<ht"):
@@ -74,40 +76,48 @@
     return g
 
 def graph2jsonld(g, form="jsonld", schemaType="Dataset") -> str:
     """get jsonld from endpoint
 
     Parameters:
         g: ?g from sparql query. URN of the graph eg. urn:gleaner.io:earthcube:geocodes_demo_datasets:257108e0760f96ef7a480e1d357bcf8720cd11e4
-        form: jsonld  future. other forms
+        form: jsonld| compact, frame
+        schemaType: if form=frame then this type is passed to the frame
     """
     # auto_compact=False might change
     jld_str = g.serialize(format="json-ld")
 
-    return formatted_jsonld(jld_str)
+    return formatted_jsonld(jld_str, form=form, schemaType=schemaType)
 
 # returns a framd JSON
 # form= framed|compact
-def get_graph2jsonld(urn: str, endpoint:str, form="jsonld", schemaType="Dataset") -> str:
-    "get jsonld from endpoint"
+def get_graph2jsonld(urn: str, endpoint:str, form="compact", schemaType="Dataset") -> str:
+    """get jsonld from endpoint
+
+    Parameters:
+        urn: ?g from sparql query. URN of the graph eg. urn:gleaner.io:earthcube:geocodes_demo_datasets:257108e0760f96ef7a480e1d357bcf8720cd11e4
+        form: jsonld| compact, frame
+        schemaType: if form=frame then this type is passed to the frame
+        endpoint: sparql endpoint
+
+    """
     g = get_rdfgraph(urn, endpoint)
-    # auto_compact=False might change
-    jld_str = g.serialize(format="json-ld")
 
-    return formatted_jsonld(jld_str)
+    return graph2jsonld(g, form=form, schemaType=schemaType)
 
 
 def get_rdf2jld_str(urn: str, endpoint:str) -> str:
     "get jsonld from endpoint"
     g= get_rdfgraph(urn, endpoint)
     jld_str = g.serialize(format="json-ld")
     return compact_jld_str(jld_str)
 
 ####
-def load_release(releaseurl:str) -> pandas.DataFrame:
+def load_release(releaseurl:str) -> Graph:
+    """retrieves a release from the url"""
     g= Dataset()
     g.parse(releaseurl, format='nquads')
     return g
 #  using https://github.com/cadmiumkitty/rdfpandas
     #g = Graph()
 #    g.parse(releaseurl, format='nt')
 #    df = to_dataframe(g)
```

### Comparing `earthcube_utilities-0.1.11/src/ec/summarize/summarize_materializedview.py` & `earthcube_utilities-0.1.13/src/ec/summarize/summarize_materializedview.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from io import StringIO
 from string import Template
+from typing import Union
 
 import pandas
 import sparqldataframe
 from rdflib import URIRef, BNode, Literal, Graph,Namespace, RDF
 import json
 
 from  ec.graph.sparql_query import queryWithSparql
@@ -50,26 +51,27 @@
     #
     # df = sparqldataframe.query(endpoint,thsGraphQuery)
     # return df
 
 ###
 # from dataframe
 ####
-def summaryDF2ttl(df: pandas.DataFrame, repo: str) -> tuple[ str|bytes, Graph]:
-    "summarize sparql qry (or main quad store)s ret DataFrame, as triples in ttl format w/g as the new subj"
+def summaryDF2ttl(df: pandas.DataFrame, repo: str) -> tuple[ Union[str,bytes], Graph]:
+    "summarize sparql query returns turtle string and rdf lib Graph"
     urns = {}
     def is_str(v):
         return type(v) is str
     g = Graph()
     ## ##########
     # Not officially a standard schema format.
     # we might want to use our own namespace in the future
     ###########
     g.bind("ecsummary", BASE_SHCEMA_ORG)
     ecsummary = Namespace(BASE_SHCEMA_ORG)
+    sosschema = Namespace(BASE_SHCEMA_ORG)
 
 
     for index, row in df.iterrows():
         logging.debug(f'dbg:{row}')
         gu=df["g"][index]
         graph_subject = URIRef(gu)
         #skip the small %of dups, that even new get_summary.txt * has
@@ -137,18 +139,25 @@
         ##############
         # output
         # write to f StringIO()
         # for RDF graph, using sub, verp object
         ###############
         s=row['subj']
 # RDF.TYPE
-        if rt == "tool":
-            g.add((graph_subject,RDF.type, Literal("SoftwareApplication")) )
-        else:
-            g.add((graph_subject, RDF.type, Literal("Dataset")))
+
+#         if rt == "tool":
+#             g.add((graph_subject,RDF.type, sosschema.SoftwareApplication) )
+#         else:
+#             g.add((graph_subject, RDF.type, sosschema.Dataset))
+
+        # original aummary query wrote out strings, then converted back to schema uri... just skip that step
+        # RDF.TYPE
+        rt = row['sosType']
+        g.add((graph_subject, RDF.type, URIRef(rt)))
+
 # ecsummary.name
         if (pandas.isnull( row.get('name'))):
             g.add((graph_subject, ecsummary.name, Literal("")))
         else:
             g.add( (graph_subject, ecsummary.name, Literal( row.get('name') ) ) )
 
 # ecsummary.description
```

