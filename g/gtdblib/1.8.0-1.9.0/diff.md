# Comparing `tmp/gtdblib-1.8.0.tar.gz` & `tmp/gtdblib-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gtdblib-1.8.0.tar", last modified: Thu Jan 12 00:42:51 2023, max compression
+gzip compressed data, was "dist/gtdblib-1.9.0.tar", last modified: Fri Mar  3 21:37:07 2023, max compression
```

## Comparing `gtdblib-1.8.0.tar` & `gtdblib-1.9.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-12 00:42:48.000000 gtdblib-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-01-12 00:42:51.000000 gtdblib-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-01-12 00:42:48.000000 gtdblib-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/cli/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/file/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/file/itol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/dataset_color_strip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/dataset_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/file/itol/tree_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/taxon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/taxon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/taxon/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/taxon/taxon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/taxonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/taxonomy/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/taxonomy/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/bootstrap_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/convert_accession.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/get_node_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/get_node_to_desc_taxa.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/get_unique_mrca_for_internal_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/tree/polytomy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/util/bio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/bio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/bio/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/bio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/bio/newick.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/bio/seq_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib/util/shell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/shell/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/shell/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/shell/filemgmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/shell/gtdbshutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-12 00:42:48.000000 gtdblib-1.8.0/gtdblib/util/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-12 00:42:51.000000 gtdblib-1.8.0/gtdblib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 00:42:51.000000 gtdblib-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-01-12 00:42:48.000000 gtdblib-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/test/test_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_tree/test_bootstrap_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_tree/test_convert_accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_tree/test_polytomy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/test/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:51.000000 gtdblib-1.8.0/test/test_util/test_bio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_util/test_bio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-01-12 00:42:48.000000 gtdblib-1.8.0/test/test_util/test_bio/test_accession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-03 21:37:01.000000 gtdblib-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-03 21:37:07.000000 gtdblib-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-03 21:37:01.000000 gtdblib-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/cli/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/file/itol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/dataset_color_strip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/dataset_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/file/itol/tree_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/taxon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/taxon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/taxon/rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/taxon/taxon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/taxonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/taxonomy/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/taxonomy/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/bootstrap_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/convert_accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/get_node_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/get_node_to_desc_taxa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/get_unique_mrca_for_internal_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/tree/polytomy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/util/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/bio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/bio/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/bio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/bio/newick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/bio/seq_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib/util/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/shell/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/shell/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/shell/filemgmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/shell/gtdbshutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-03 21:37:01.000000 gtdblib-1.9.0/gtdblib/util/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-03 21:37:07.000000 gtdblib-1.9.0/gtdblib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 21:37:07.000000 gtdblib-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-03 21:37:01.000000 gtdblib-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/test/test_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_tree/test_bootstrap_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_tree/test_convert_accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_tree/test_polytomy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/test/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:07.000000 gtdblib-1.9.0/test/test_util/test_bio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_util/test_bio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-03 21:37:01.000000 gtdblib-1.9.0/test/test_util/test_bio/test_accession.py
```

### Comparing `gtdblib-1.8.0/LICENSE` & `gtdblib-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/PKG-INFO` & `gtdblib-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdblib
-Version: 1.8.0
+Version: 1.9.0
 Summary: An abstraction of objects, files, and third-party tools used by the GTDB. Not intended for public use.
 Home-page: https://github.com/Ecogenomics/gtdb-lib
 Author: Aaron Mussig
 Author-email: aaronmussig@gmail.com
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Ecogenomics/gtdb-lib
 Project-URL: Documentation, https://github.com/Ecogenomics/gtdb-lib
```

### Comparing `gtdblib-1.8.0/README.md` & `gtdblib-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/__init__.py` & `gtdblib-1.9.0/gtdblib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __title__ = 'gtdblib'
 __description__ = 'An abstraction of objects, files, and third-party tools used by the GTDB. Not intended for public use.'
 __url__ = 'https://github.com/Ecogenomics/gtdb-lib'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 __author__ = 'Aaron Mussig'
 __author_email__ = 'aaronmussig@gmail.com'
 __license__ = 'GPL-3.0'
 __bug_url__ = 'https://github.com/Ecogenomics/gtdb-lib'
 __doc_url__ = 'https://github.com/Ecogenomics/gtdb-lib'
 __src_url__ = 'https://github.com/Ecogenomics/gtdb-lib'
```

### Comparing `gtdblib-1.8.0/gtdblib/__main__.py` & `gtdblib-1.9.0/gtdblib/__main__.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/cli/tree.py` & `gtdblib-1.9.0/gtdblib/cli/tree.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/file/itol/dataset_color_strip.py` & `gtdblib-1.9.0/gtdblib/file/itol/dataset_color_strip.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/file/itol/dataset_text.py` & `gtdblib-1.9.0/gtdblib/file/itol/dataset_text.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/file/itol/label.py` & `gtdblib-1.9.0/gtdblib/file/itol/label.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/file/itol/popup.py` & `gtdblib-1.9.0/gtdblib/file/itol/popup.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/file/itol/tree_colors.py` & `gtdblib-1.9.0/gtdblib/file/itol/tree_colors.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/taxonomy/taxonomy.py` & `gtdblib-1.9.0/gtdblib/taxonomy/taxonomy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from typing import Dict, List
 
 from gtdblib import log
 from gtdblib.taxon.taxon import Taxon
 from gtdblib.taxon.rank import TaxonRank
 from gtdblib.util.types import is_float
-from gtdblib.utilshell.gtdbshutil import check_file_exists
+from gtdblib.util.shell.gtdbshutil import check_file_exists
 from gtdblib.util.bio.accession import canonical_gid
 
 
 def read_taxonomy(taxonomy_file: str, use_canonical_gid: bool = False) -> Dict[str, List[str]]:
     """Read Greengenes-style taxonomy file.
 
     This method is generic in that it can read any Greengenes-style taxonomy string
@@ -143,14 +143,28 @@
 
     return taxonomy
 
 
 class Taxonomy:
     __slots__ = ('d', 'p', 'c', 'o', 'f', 'g', 's')
 
+    RANK_PREFIXES = ('d__', 'p__', 'c__', 'o__', 'f__', 'g__', 's__')
+    RANK_LABELS = ('domain', 'phylum', 'class', 'order',
+                   'family', 'genus', 'species')
+    RANK_INDEX = {'d__': 0, 'p__': 1, 'c__': 2,
+                  'o__': 3, 'f__': 4, 'g__': 5, 's__': 6}
+
+    DOMAIN_INDEX = 0
+    PHYLUM_INDEX = 1
+    CLASS_INDEX = 2
+    ORDER_INDEX = 3
+    FAMILY_INDEX = 4
+    GENUS_INDEX = 5
+    SPECIES_INDEX = 6
+
     def __init__(self, d: Taxon, p: Taxon, c: Taxon, o: Taxon, f: Taxon, g: Taxon, s: Taxon):
         self.d = d
         self.p = p
         self.c = c
         self.o = o
         self.f = f
         self.g = g
```

### Comparing `gtdblib-1.8.0/gtdblib/taxonomy/validation.py` & `gtdblib-1.9.0/gtdblib/taxonomy/validation.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/tree/bootstrap_merge.py` & `gtdblib-1.9.0/gtdblib/tree/bootstrap_merge.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/tree/convert_accession.py` & `gtdblib-1.9.0/gtdblib/tree/convert_accession.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/tree/get_node_depth.py` & `gtdblib-1.9.0/gtdblib/tree/get_node_depth.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/tree/get_node_to_desc_taxa.py` & `gtdblib-1.9.0/gtdblib/tree/get_node_to_desc_taxa.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/tree/get_unique_mrca_for_internal_nodes.py` & `gtdblib-1.9.0/gtdblib/tree/get_unique_mrca_for_internal_nodes.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/tree/polytomy.py` & `gtdblib-1.9.0/gtdblib/tree/polytomy.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/bio/accession.py` & `gtdblib-1.9.0/gtdblib/util/bio/accession.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/bio/exceptions.py` & `gtdblib-1.9.0/gtdblib/util/bio/exceptions.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/bio/newick.py` & `gtdblib-1.9.0/gtdblib/util/bio/newick.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/bio/seq_io.py` & `gtdblib-1.9.0/gtdblib/util/bio/seq_io.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/color.py` & `gtdblib-1.9.0/gtdblib/util/color.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/shell/filemgmt.py` & `gtdblib-1.9.0/gtdblib/util/shell/filemgmt.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib/util/shell/gtdbshutil.py` & `gtdblib-1.9.0/gtdblib/util/shell/gtdbshutil.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/gtdblib.egg-info/PKG-INFO` & `gtdblib-1.9.0/gtdblib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtdblib
-Version: 1.8.0
+Version: 1.9.0
 Summary: An abstraction of objects, files, and third-party tools used by the GTDB. Not intended for public use.
 Home-page: https://github.com/Ecogenomics/gtdb-lib
 Author: Aaron Mussig
 Author-email: aaronmussig@gmail.com
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Ecogenomics/gtdb-lib
 Project-URL: Documentation, https://github.com/Ecogenomics/gtdb-lib
```

### Comparing `gtdblib-1.8.0/gtdblib.egg-info/SOURCES.txt` & `gtdblib-1.9.0/gtdblib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/setup.py` & `gtdblib-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/test/test_tree/test_bootstrap_merge.py` & `gtdblib-1.9.0/test/test_tree/test_bootstrap_merge.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/test/test_tree/test_polytomy.py` & `gtdblib-1.9.0/test/test_tree/test_polytomy.py`

 * *Files identical despite different names*

### Comparing `gtdblib-1.8.0/test/test_util/test_bio/test_accession.py` & `gtdblib-1.9.0/test/test_util/test_bio/test_accession.py`

 * *Files identical despite different names*

