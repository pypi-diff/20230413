# Comparing `tmp/mofikhatun530-checksum-1.0.tar.gz` & `tmp/mofikhatun530_checksum-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mofikhatun530-checksum-1.0.tar", last modified: Thu Apr 13 08:23:52 2023, max compression
+gzip compressed data, was "mofikhatun530_checksum-1.1.tar", last modified: Thu Apr 13 12:42:10 2023, max compression
```

## Comparing `mofikhatun530-checksum-1.0.tar` & `mofikhatun530_checksum-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 megapihar  (1001) megapihar  (1001)        0 2023-04-13 08:23:52.147772 mofikhatun530-checksum-1.0/
--rw-rw-r--   0 megapihar  (1001) megapihar  (1001)      235 2023-04-13 08:23:52.147772 mofikhatun530-checksum-1.0/PKG-INFO
--rw-r--r--   0 megapihar  (1001) megapihar  (1001)      482 2023-04-13 07:49:35.000000 mofikhatun530-checksum-1.0/README.rst
--rw-r--r--   0 megapihar  (1001) megapihar  (1001)      107 2023-04-13 08:23:52.151772 mofikhatun530-checksum-1.0/setup.cfg
--rw-r--r--   0 megapihar  (1001) megapihar  (1001)      380 2023-04-13 08:02:56.000000 mofikhatun530-checksum-1.0/setup.py
-drwxrwxr-x   0 megapihar  (1001) megapihar  (1001)        0 2023-04-13 08:23:52.147772 mofikhatun530-checksum-1.0/src/
-drwxrwxr-x   0 megapihar  (1001) megapihar  (1001)        0 2023-04-13 08:23:52.147772 mofikhatun530-checksum-1.0/src/mofikhatun530_checksum.egg-info/
--rw-rw-r--   0 megapihar  (1001) megapihar  (1001)      235 2023-04-13 08:23:51.000000 mofikhatun530-checksum-1.0/src/mofikhatun530_checksum.egg-info/PKG-INFO
--rw-rw-r--   0 megapihar  (1001) megapihar  (1001)      350 2023-04-13 08:23:51.000000 mofikhatun530-checksum-1.0/src/mofikhatun530_checksum.egg-info/SOURCES.txt
--rw-rw-r--   0 megapihar  (1001) megapihar  (1001)        1 2023-04-13 08:23:51.000000 mofikhatun530-checksum-1.0/src/mofikhatun530_checksum.egg-info/dependency_links.txt
--rw-rw-r--   0 megapihar  (1001) megapihar  (1001)       14 2023-04-13 08:23:51.000000 mofikhatun530-checksum-1.0/src/mofikhatun530_checksum.egg-info/requires.txt
--rw-rw-r--   0 megapihar  (1001) megapihar  (1001)       14 2023-04-13 08:23:51.000000 mofikhatun530-checksum-1.0/src/mofikhatun530_checksum.egg-info/top_level.txt
-drwxrwxr-x   0 megapihar  (1001) megapihar  (1001)        0 2023-04-13 08:23:52.147772 mofikhatun530-checksum-1.0/src/web3_checksum/
--rw-r--r--   0 megapihar  (1001) megapihar  (1001)        0 2023-04-13 07:39:09.000000 mofikhatun530-checksum-1.0/src/web3_checksum/__init__.py
--rw-r--r--   0 megapihar  (1001) megapihar  (1001)      707 2023-04-13 07:46:22.000000 mofikhatun530-checksum-1.0/src/web3_checksum/get_checksum_address.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:42:10.981948 mofikhatun530_checksum-1.1/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-13 12:42:10.981948 mofikhatun530_checksum-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-13 07:49:35.000000 mofikhatun530_checksum-1.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-13 12:42:10.981948 mofikhatun530_checksum-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-13 12:42:05.000000 mofikhatun530_checksum-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:42:10.977948 mofikhatun530_checksum-1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:42:10.981948 mofikhatun530_checksum-1.1/src/mofikhatun530_checksum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-13 12:42:10.000000 mofikhatun530_checksum-1.1/src/mofikhatun530_checksum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-13 12:42:10.000000 mofikhatun530_checksum-1.1/src/mofikhatun530_checksum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 12:42:10.000000 mofikhatun530_checksum-1.1/src/mofikhatun530_checksum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 12:42:10.000000 mofikhatun530_checksum-1.1/src/mofikhatun530_checksum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 12:42:10.000000 mofikhatun530_checksum-1.1/src/mofikhatun530_checksum.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 12:42:10.981948 mofikhatun530_checksum-1.1/src/web3_checksum/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 07:39:09.000000 mofikhatun530_checksum-1.1/src/web3_checksum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      707 2023-04-13 07:46:22.000000 mofikhatun530_checksum-1.1/src/web3_checksum/get_checksum_address.py
```

### Comparing `mofikhatun530-checksum-1.0/src/web3_checksum/get_checksum_address.py` & `mofikhatun530_checksum-1.1/src/web3_checksum/get_checksum_address.py`

 * *Files identical despite different names*

