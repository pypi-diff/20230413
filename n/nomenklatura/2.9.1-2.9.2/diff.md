# Comparing `tmp/nomenklatura-2.9.1.tar.gz` & `tmp/nomenklatura-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-2.9.1.tar", last modified: Tue Mar 28 20:04:02 2023, max compression
+gzip compressed data, was "nomenklatura-2.9.2.tar", last modified: Thu Apr 13 11:43:14 2023, max compression
```

## Comparing `nomenklatura-2.9.1.tar` & `nomenklatura-2.9.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.495638 nomenklatura-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.487638 nomenklatura-2.9.1/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.487638 nomenklatura-2.9.1/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/data/match-regression.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/judgement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/matching/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/features/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/features/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/features/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/features/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/matching/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.491638 nomenklatura-2.9.1/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:04:02.487638 nomenklatura-2.9.1/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:03:26.000000 nomenklatura-2.9.1/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 20:04:02.000000 nomenklatura-2.9.1/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 20:04:02.495638 nomenklatura-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-28 20:01:56.000000 nomenklatura-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.246182 nomenklatura-2.9.2/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.250182 nomenklatura-2.9.2/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/data/match-regression.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.250182 nomenklatura-2.9.2/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.250182 nomenklatura-2.9.2/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.254182 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.254182 nomenklatura-2.9.2/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/judgement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.254182 nomenklatura-2.9.2/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/matching/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/features/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/matching/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.258182 nomenklatura-2.9.2/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:43:14.246182 nomenklatura-2.9.2/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:42:37.000000 nomenklatura-2.9.2/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 11:43:14.000000 nomenklatura-2.9.2/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 11:43:14.262182 nomenklatura-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-13 11:41:05.000000 nomenklatura-2.9.2/setup.py
```

### Comparing `nomenklatura-2.9.1/LICENSE` & `nomenklatura-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/PKG-INFO` & `nomenklatura-2.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.1
+Version: 2.9.2
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
@@ -30,24 +30,24 @@
 
 Much of the functionality of `nomenklatura` can be used as a command-line tool. In the following example, we'll assume that you have a file containing [Follow the Money](https://followthemoney.rtfd.org/) entities in your local directory, named `entities.ijson`. If you just want try it out, you can use the file `tests/fixtures/donations.ijson` in this repository for testing (it contains German campaign finance data).
 
 With the file in place, you will cross-reference the entities to generate de-duplication candidates, then run the interactive de-duplication UI in your console, and eventually apply the judgements to generate a new file with merged entities:
 
 ```bash
 # generate merge candidates using an in-memory index:
-$ nomenklatura xref entities.ijson
-# note there is now a new file, `entities.rslv.ijson` that contains de-duplication info.
-$ nomenklatura dedupe entiites.ijson
+$ nomenklatura xref -r resolver.json entities.ijson
+# note there is now a new file, `resolver.json` that contains de-duplication info.
+$ nomenklatura dedupe -r resolver.json entites.ijson
 # will pop up a user interface.
-$ nomenklatura apply entities.ijson -o merged.ijson
+$ nomenklatura apply entities.ijson -o merged.ijson -r resolver.json
 # de-duplicated data goes into `merged.ijson`:
 $ cat entities.ijson | wc -l 
-474 entities.ijson
-$ cat entities.ijson | wc -l 
-468 merged.ijson
+474
+$ cat merged.ijson | wc -l 
+468 
 ```
 
 ### Programmatic usage
 
 The command-line use of `nomenklatura` is targeted at small datasets which need to be de-duplicated. For more involved scenarios, the package also offers a Python API which can be used to control the semantics of de-duplication.
 
 * `nomenklatura.Dataset` - implements a basic dataset for describing a set of entities.
```

### Comparing `nomenklatura-2.9.1/README.md` & `nomenklatura-2.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 Much of the functionality of `nomenklatura` can be used as a command-line tool. In the following example, we'll assume that you have a file containing [Follow the Money](https://followthemoney.rtfd.org/) entities in your local directory, named `entities.ijson`. If you just want try it out, you can use the file `tests/fixtures/donations.ijson` in this repository for testing (it contains German campaign finance data).
 
 With the file in place, you will cross-reference the entities to generate de-duplication candidates, then run the interactive de-duplication UI in your console, and eventually apply the judgements to generate a new file with merged entities:
 
 ```bash
 # generate merge candidates using an in-memory index:
-$ nomenklatura xref entities.ijson
-# note there is now a new file, `entities.rslv.ijson` that contains de-duplication info.
-$ nomenklatura dedupe entiites.ijson
+$ nomenklatura xref -r resolver.json entities.ijson
+# note there is now a new file, `resolver.json` that contains de-duplication info.
+$ nomenklatura dedupe -r resolver.json entites.ijson
 # will pop up a user interface.
-$ nomenklatura apply entities.ijson -o merged.ijson
+$ nomenklatura apply entities.ijson -o merged.ijson -r resolver.json
 # de-duplicated data goes into `merged.ijson`:
 $ cat entities.ijson | wc -l 
-474 entities.ijson
-$ cat entities.ijson | wc -l 
-468 merged.ijson
+474
+$ cat merged.ijson | wc -l 
+468 
 ```
 
 ### Programmatic usage
 
 The command-line use of `nomenklatura` is targeted at small datasets which need to be de-duplicated. For more involved scenarios, the package also offers a Python API which can be used to control the semantics of de-duplication.
 
 * `nomenklatura.Dataset` - implements a basic dataset for describing a set of entities.
```

### Comparing `nomenklatura-2.9.1/nomenklatura/cache.py` & `nomenklatura-2.9.2/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/cli.py` & `nomenklatura-2.9.2/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/data/match-regression.pkl` & `nomenklatura-2.9.2/nomenklatura/data/match-regression.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/dataset/catalog.py` & `nomenklatura-2.9.2/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/dataset/coverage.py` & `nomenklatura-2.9.2/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/dataset/dataset.py` & `nomenklatura-2.9.2/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/dataset/publisher.py` & `nomenklatura-2.9.2/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/dataset/resource.py` & `nomenklatura-2.9.2/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/dataset/util.py` & `nomenklatura-2.9.2/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/db.py` & `nomenklatura-2.9.2/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/__init__.py` & `nomenklatura-2.9.2/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/aleph.py` & `nomenklatura-2.9.2/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/common.py` & `nomenklatura-2.9.2/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/nominatim.py` & `nomenklatura-2.9.2/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/opencorporates.py` & `nomenklatura-2.9.2/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-2.9.2/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/enrich/yente.py` & `nomenklatura-2.9.2/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/entity.py` & `nomenklatura-2.9.2/nomenklatura/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from hashlib import sha1
+from banal import hash_data
 from datetime import datetime
 from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
 from typing import Generator, Iterable, Tuple, Type, TypeVar
 from followthemoney import model
 from followthemoney.model import Model
 from followthemoney.exc import InvalidData
@@ -75,24 +77,31 @@
     def _properties(self) -> Dict[str, List[str]]:  # type: ignore
         return {p: [s.value for s in v] for p, v in self._statements.items()}
 
     def _iter_stmt(self) -> Generator[Statement, None, None]:
         for stmts in self._statements.values():
             yield from stmts
 
+    def checksum(self) -> str:
+        hash = sha1(self.schema.name.encode("utf-8"))
+        for stmt in sorted(self._iter_stmt()):
+            if stmt.id is not None:
+                hash.update(stmt.id.encode("utf-8"))
+        return hash.hexdigest()
+
     @property
     def statements(self) -> Generator[Statement, None, None]:
         if self.id is not None:
             yield Statement(
                 canonical_id=self.id,
                 entity_id=self.id,
                 prop=Statement.BASE,
                 prop_type=Statement.BASE,
                 schema=self.schema.name,
-                value=self.id,
+                value=self.checksum(),
                 dataset=self.default_dataset,
             )
         yield from self._iter_stmt()
 
     @property
     def first_seen(self) -> Optional[datetime]:
         seen = (s.first_seen for s in self._iter_stmt() if s.first_seen is not None)
```

### Comparing `nomenklatura-2.9.1/nomenklatura/index/entry.py` & `nomenklatura-2.9.2/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/index/index.py` & `nomenklatura-2.9.2/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/index/tokenizer.py` & `nomenklatura-2.9.2/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/judgement.py` & `nomenklatura-2.9.2/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/loader.py` & `nomenklatura-2.9.2/nomenklatura/loader.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/features/__init__.py` & `nomenklatura-2.9.2/nomenklatura/matching/features/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/features/dates.py` & `nomenklatura-2.9.2/nomenklatura/matching/features/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/features/misc.py` & `nomenklatura-2.9.2/nomenklatura/matching/features/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/features/names.py` & `nomenklatura-2.9.2/nomenklatura/matching/features/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/features/util.py` & `nomenklatura-2.9.2/nomenklatura/matching/features/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/model.py` & `nomenklatura-2.9.2/nomenklatura/matching/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/pairs.py` & `nomenklatura-2.9.2/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/matching/train.py` & `nomenklatura-2.9.2/nomenklatura/matching/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/publish/dates.py` & `nomenklatura-2.9.2/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/publish/edges.py` & `nomenklatura-2.9.2/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/publish/names.py` & `nomenklatura-2.9.2/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/resolver/edge.py` & `nomenklatura-2.9.2/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/resolver/identifier.py` & `nomenklatura-2.9.2/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/resolver/resolver.py` & `nomenklatura-2.9.2/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/senzing.py` & `nomenklatura-2.9.2/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/statement/serialize.py` & `nomenklatura-2.9.2/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/statement/statement.py` & `nomenklatura-2.9.2/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/tui/app.py` & `nomenklatura-2.9.2/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/tui/comparison.py` & `nomenklatura-2.9.2/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/tui/util.py` & `nomenklatura-2.9.2/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/util.py` & `nomenklatura-2.9.2/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/nomenklatura/xref.py` & `nomenklatura-2.9.2/nomenklatura/xref.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nomenklatura.dataset import DS
 from nomenklatura.entity import CE
 from nomenklatura.loader import Loader
 from nomenklatura.resolver import Resolver
 from nomenklatura.judgement import Judgement
 from nomenklatura.index import Index
 from nomenklatura.matching import compare_scored
+from nomenklatura.util import is_qid
 
 log = logging.getLogger(__name__)
 
 
 def _print_stats(pairs: int, suggested: int, scores: List[float]) -> None:
     matches = len(scores)
     log.info(
@@ -45,14 +46,17 @@
         for idx, ((left_id, right_id), score) in enumerate(index.pairs()):
             if idx % 1000 == 0 and idx > 0:
                 _print_stats(idx, suggested, scores)
 
             if not resolver.check_candidate(left_id, right_id):
                 continue
 
+            if is_qid(left_id.id) and is_qid(right_id.id):
+                continue
+
             left = loader.get_entity(left_id.id)
             right = loader.get_entity(right_id.id)
             if left is None or left.id is None or right is None or right.id is None:
                 continue
 
             if not left.schema.can_match(right.schema):
                 continue
@@ -76,14 +80,20 @@
             #         resolver.decide(left_id, right_id, Judgement.POSITIVE)
             #         continue
 
             # Not sure this is globally a good idea.
             if len(left.datasets.intersection(right.datasets)) > 0:
                 score = score * 0.7
 
+            # promote = "us_cia_world_leaders"
+            # if promote in left.datasets and promote not in right.datasets:
+            #     score = (score + 1.0) / 2.0
+            # if promote not in left.datasets and promote in right.datasets:
+            #     score = (score + 1.0) / 2.0
+
             if auto_threshold is not None and score > auto_threshold:
                 log.info("Auto-merge [%.2f]: %s <> %s", score, left, right)
                 resolver.decide(left_id, right_id, Judgement.POSITIVE, user=user)
                 continue
             resolver.suggest(left.id, right.id, score, user=user)
             if suggested > limit:
                 break
```

### Comparing `nomenklatura-2.9.1/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-2.9.2/nomenklatura.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.1
+Version: 2.9.2
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
@@ -30,24 +30,24 @@
 
 Much of the functionality of `nomenklatura` can be used as a command-line tool. In the following example, we'll assume that you have a file containing [Follow the Money](https://followthemoney.rtfd.org/) entities in your local directory, named `entities.ijson`. If you just want try it out, you can use the file `tests/fixtures/donations.ijson` in this repository for testing (it contains German campaign finance data).
 
 With the file in place, you will cross-reference the entities to generate de-duplication candidates, then run the interactive de-duplication UI in your console, and eventually apply the judgements to generate a new file with merged entities:
 
 ```bash
 # generate merge candidates using an in-memory index:
-$ nomenklatura xref entities.ijson
-# note there is now a new file, `entities.rslv.ijson` that contains de-duplication info.
-$ nomenklatura dedupe entiites.ijson
+$ nomenklatura xref -r resolver.json entities.ijson
+# note there is now a new file, `resolver.json` that contains de-duplication info.
+$ nomenklatura dedupe -r resolver.json entites.ijson
 # will pop up a user interface.
-$ nomenklatura apply entities.ijson -o merged.ijson
+$ nomenklatura apply entities.ijson -o merged.ijson -r resolver.json
 # de-duplicated data goes into `merged.ijson`:
 $ cat entities.ijson | wc -l 
-474 entities.ijson
-$ cat entities.ijson | wc -l 
-468 merged.ijson
+474
+$ cat merged.ijson | wc -l 
+468 
 ```
 
 ### Programmatic usage
 
 The command-line use of `nomenklatura` is targeted at small datasets which need to be de-duplicated. For more involved scenarios, the package also offers a Python API which can be used to control the semantics of de-duplication.
 
 * `nomenklatura.Dataset` - implements a basic dataset for describing a set of entities.
```

### Comparing `nomenklatura-2.9.1/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-2.9.2/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.1/setup.py` & `nomenklatura-2.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="2.9.1",
+    version="2.9.2",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
@@ -20,15 +20,15 @@
     include_package_data=True,
     package_data={"": ["nomenklatura/data/*", "nomenklatura/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.3.0, < 4.0.0",
         "shortuuid >= 1.0.11, < 2.0.0",
         "rich >= 10.9.0, < 14.0.0",
-        "textual >= 0.3.0, < 0.11.0",
+        "textual >= 0.19.0, < 0.20.0",
         "scikit-learn == 1.2.1",
         "click >= 8.0.0, < 9.0.0",
     ],
     tests_require=[],
     entry_points={
         "console_scripts": [
             "nk = nomenklatura.cli:cli",
```

