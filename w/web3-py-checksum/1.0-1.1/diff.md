# Comparing `tmp/web3_py_checksum-1.0.tar.gz` & `tmp/web3_py_checksum-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3_py_checksum-1.0.tar", last modified: Thu Apr 13 07:36:03 2023, max compression
+gzip compressed data, was "web3_py_checksum-1.1.tar", last modified: Thu Apr 13 08:09:40 2023, max compression
```

## Comparing `web3_py_checksum-1.0.tar` & `web3_py_checksum-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 07:36:03.826324 web3_py_checksum-1.0/
--rw-rw-rw-   0        0        0       26 2023-04-13 07:36:02.000000 web3_py_checksum-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      329 2023-04-13 07:36:03.826324 web3_py_checksum-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-13 07:36:03.832370 web3_py_checksum-1.0/setup.cfg
--rw-rw-rw-   0        0        0      402 2023-04-13 07:36:02.000000 web3_py_checksum-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:36:03.802322 web3_py_checksum-1.0/web3_py_checksum/
--rw-rw-rw-   0        0        0      814 2023-04-12 12:54:31.000000 web3_py_checksum-1.0/web3_py_checksum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:36:03.826324 web3_py_checksum-1.0/web3_py_checksum.egg-info/
--rw-rw-rw-   0        0        0      329 2023-04-13 07:36:03.000000 web3_py_checksum-1.0/web3_py_checksum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-04-13 07:36:03.000000 web3_py_checksum-1.0/web3_py_checksum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 07:36:03.000000 web3_py_checksum-1.0/web3_py_checksum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 07:36:03.000000 web3_py_checksum-1.0/web3_py_checksum.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 08:09:40.446495 web3_py_checksum-1.1/
+-rw-rw-rw-   0        0        0       26 2023-04-13 08:09:39.000000 web3_py_checksum-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      329 2023-04-13 08:09:40.446495 web3_py_checksum-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-13 08:09:40.446495 web3_py_checksum-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      402 2023-04-13 08:09:39.000000 web3_py_checksum-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:09:40.415242 web3_py_checksum-1.1/web3_py_checksum/
+-rw-rw-rw-   0        0        0        0 2023-04-13 08:07:39.000000 web3_py_checksum-1.1/web3_py_checksum/__init.py
+-rw-rw-rw-   0        0        0      814 2023-04-12 12:54:31.000000 web3_py_checksum-1.1/web3_py_checksum/get_checksum_address.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:09:40.446495 web3_py_checksum-1.1/web3_py_checksum.egg-info/
+-rw-rw-rw-   0        0        0      329 2023-04-13 08:09:40.000000 web3_py_checksum-1.1/web3_py_checksum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-13 08:09:40.000000 web3_py_checksum-1.1/web3_py_checksum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 08:09:40.000000 web3_py_checksum-1.1/web3_py_checksum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 08:09:40.000000 web3_py_checksum-1.1/web3_py_checksum.egg-info/top_level.txt
```

### Comparing `web3_py_checksum-1.0/web3_py_checksum/__init__.py` & `web3_py_checksum-1.1/web3_py_checksum/get_checksum_address.py`

 * *Files identical despite different names*

