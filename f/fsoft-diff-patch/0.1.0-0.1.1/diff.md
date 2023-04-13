# Comparing `tmp/fsoft_diff_patch-0.1.0.tar.gz` & `tmp/fsoft_diff_patch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsoft_diff_patch-0.1.0.tar", last modified: Wed Apr 12 17:46:04 2023, max compression
+gzip compressed data, was "fsoft_diff_patch-0.1.1.tar", last modified: Thu Apr 13 05:54:43 2023, max compression
```

## Comparing `fsoft_diff_patch-0.1.0.tar` & `fsoft_diff_patch-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2023-04-12 17:46:04.746146 fsoft_diff_patch-0.1.0/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      365 2023-04-12 17:46:04.746146 fsoft_diff_patch-0.1.0/PKG-INFO
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2023-04-12 17:46:04.746146 fsoft_diff_patch-0.1.0/fsoft_diff_patch/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)     3720 2023-04-12 17:34:10.000000 fsoft_diff_patch-0.1.0/fsoft_diff_patch/__init__.py
-drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2023-04-12 17:46:04.746146 fsoft_diff_patch-0.1.0/fsoft_diff_patch.egg-info/
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      365 2023-04-12 17:46:04.000000 fsoft_diff_patch-0.1.0/fsoft_diff_patch.egg-info/PKG-INFO
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      197 2023-04-12 17:46:04.000000 fsoft_diff_patch-0.1.0/fsoft_diff_patch.egg-info/SOURCES.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)        1 2023-04-12 17:46:04.000000 fsoft_diff_patch-0.1.0/fsoft_diff_patch.egg-info/dependency_links.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       17 2023-04-12 17:46:04.000000 fsoft_diff_patch-0.1.0/fsoft_diff_patch.egg-info/top_level.txt
--rw-rw-r--   0 fabio     (1000) fabio     (1000)       38 2023-04-12 17:46:04.746146 fsoft_diff_patch-0.1.0/setup.cfg
--rw-rw-r--   0 fabio     (1000) fabio     (1000)      557 2023-04-12 17:45:31.000000 fsoft_diff_patch-0.1.0/setup.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2023-04-13 05:54:43.825632 fsoft_diff_patch-0.1.1/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     3075 2023-04-13 05:54:43.825632 fsoft_diff_patch-0.1.1/PKG-INFO
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     2669 2023-04-13 05:52:33.000000 fsoft_diff_patch-0.1.1/README.md
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2023-04-13 05:54:43.821632 fsoft_diff_patch-0.1.1/fsoft_diff_patch/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     3720 2023-04-12 17:34:10.000000 fsoft_diff_patch-0.1.1/fsoft_diff_patch/__init__.py
+drwxrwxr-x   0 fabio     (1000) fabio     (1000)        0 2023-04-13 05:54:43.825632 fsoft_diff_patch-0.1.1/fsoft_diff_patch.egg-info/
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)     3075 2023-04-13 05:54:43.000000 fsoft_diff_patch-0.1.1/fsoft_diff_patch.egg-info/PKG-INFO
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      207 2023-04-13 05:54:43.000000 fsoft_diff_patch-0.1.1/fsoft_diff_patch.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)        1 2023-04-13 05:54:43.000000 fsoft_diff_patch-0.1.1/fsoft_diff_patch.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       17 2023-04-13 05:54:43.000000 fsoft_diff_patch-0.1.1/fsoft_diff_patch.egg-info/top_level.txt
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)       38 2023-04-13 05:54:43.825632 fsoft_diff_patch-0.1.1/setup.cfg
+-rw-rw-r--   0 fabio     (1000) fabio     (1000)      802 2023-04-13 05:54:39.000000 fsoft_diff_patch-0.1.1/setup.py
```

### Comparing `fsoft_diff_patch-0.1.0/fsoft_diff_patch/__init__.py` & `fsoft_diff_patch-0.1.1/fsoft_diff_patch/__init__.py`

 * *Files identical despite different names*

