# Comparing `tmp/zflow-2.2.3.tar.gz` & `tmp/zflow-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zflow-2.2.3.tar", last modified: Wed Apr 12 09:01:16 2023, max compression
+gzip compressed data, was "zflow-2.3.0.tar", last modified: Thu Apr 13 14:34:36 2023, max compression
```

## Comparing `zflow-2.2.3.tar` & `zflow-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:01:16.351802 zflow-2.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-12 09:01:15.000000 zflow-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-12 09:01:16.351802 zflow-2.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-12 09:01:15.000000 zflow-2.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-12 09:01:15.000000 zflow-2.2.3/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-12 09:01:16.351802 zflow-2.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-04-12 09:01:15.000000 zflow-2.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:01:16.351802 zflow-2.2.3/zflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-12 09:01:16.000000 zflow-2.2.3/zflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2023-04-12 09:01:16.000000 zflow-2.2.3/zflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:01:16.000000 zflow-2.2.3/zflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:01:16.000000 zflow-2.2.3/zflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 09:01:16.000000 zflow-2.2.3/zflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:34:36.034944 zflow-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-13 14:34:34.000000 zflow-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      244 2023-04-13 14:34:36.034944 zflow-2.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-13 14:34:34.000000 zflow-2.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-13 14:34:34.000000 zflow-2.3.0/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-13 14:34:36.034944 zflow-2.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-04-13 14:34:34.000000 zflow-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:34:36.034944 zflow-2.3.0/zflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-04-13 14:34:36.000000 zflow-2.3.0/zflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2023-04-13 14:34:36.000000 zflow-2.3.0/zflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 14:34:36.000000 zflow-2.3.0/zflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 14:34:36.000000 zflow-2.3.0/zflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 14:34:36.000000 zflow-2.3.0/zflow.egg-info/top_level.txt
```

### Comparing `zflow-2.2.3/LICENSE` & `zflow-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zflow-2.2.3/setup.py` & `zflow-2.3.0/setup.py`

 * *Files identical despite different names*

