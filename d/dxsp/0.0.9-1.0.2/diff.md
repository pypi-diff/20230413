# Comparing `tmp/dxsp-0.0.9.tar.gz` & `tmp/dxsp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.9.tar", last modified: Sun Apr  9 13:03:24 2023, max compression
+gzip compressed data, was "dxsp-1.0.2.tar", max compression
```

## Comparing `dxsp-0.0.9.tar` & `dxsp-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:03:24.916595 dxsp-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 13:03:12.000000 dxsp-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 13:03:24.916595 dxsp-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 13:03:12.000000 dxsp-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:03:24.916595 dxsp-0.0.9/dxsp/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 13:03:12.000000 dxsp-0.0.9/dxsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-09 13:03:12.000000 dxsp-0.0.9/dxsp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-09 13:03:12.000000 dxsp-0.0.9/dxsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:03:24.916595 dxsp-0.0.9/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 13:03:24.000000 dxsp-0.0.9/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 13:03:12.000000 dxsp-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:03:24.916595 dxsp-0.0.9/setup.cfg
+-rw-r--r--   0        0        0     1064 2023-04-13 06:48:08.521218 dxsp-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2889 2023-04-13 06:48:08.521218 dxsp-1.0.2/README.md
+-rw-r--r--   0        0        0       47 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8588 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    15860 2023-04-13 06:48:08.521218 dxsp-1.0.2/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 06:48:09.217226 dxsp-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 dxsp-1.0.2/PKG-INFO
```

### Comparing `dxsp-0.0.9/LICENSE` & `dxsp-1.0.2/LICENSE`

 * *Files identical despite different names*

