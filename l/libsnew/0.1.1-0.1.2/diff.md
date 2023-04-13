# Comparing `tmp/libsnew-0.1.1.tar.gz` & `tmp/libsnew-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsnew-0.1.1.tar", last modified: Thu Apr 13 06:20:22 2023, max compression
+gzip compressed data, was "libsnew-0.1.2.tar", last modified: Thu Apr 13 06:26:22 2023, max compression
```

## Comparing `libsnew-0.1.1.tar` & `libsnew-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.956553 libsnew-0.1.1/
--rw-rw-rw-   0        0        0     1073 2023-04-01 06:22:30.000000 libsnew-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3719 2023-04-13 06:20:22.954556 libsnew-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-04-03 14:37:58.000000 libsnew-0.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.846509 libsnew-0.1.1/libsnew/
--rw-rw-rw-   0        0        0      449 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/Extract.py
--rw-rw-rw-   0        0        0      452 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/Load.py
--rw-rw-rw-   0        0        0      617 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/Ml.py
--rw-rw-rw-   0        0        0     8881 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/Step.py
--rw-rw-rw-   0        0        0      482 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/Transform.py
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.886142 libsnew-0.1.1/libsnew/connectors/
--rw-rw-rw-   0        0        0      946 2023-04-04 12:55:16.000000 libsnew-0.1.1/libsnew/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.891138 libsnew-0.1.1/libsnew/connectors/destination_3TLIPFS/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_3TLIPFS/__init__.py
--rw-rw-rw-   0        0        0     3593 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_3TLIPFS/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.895161 libsnew-0.1.1/libsnew/connectors/destination_IPFS/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_IPFS/__init__.py
--rw-rw-rw-   0        0        0     2628 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_IPFS/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.900558 libsnew-0.1.1/libsnew/connectors/destination_azblob/
--rw-rw-rw-   0        0        0        2 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_azblob/__init__.py
--rw-rw-rw-   0        0        0      652 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_azblob/destination.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.906635 libsnew-0.1.1/libsnew/connectors/destination_mysql/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_mysql/__init__.py
--rw-rw-rw-   0        0        0     7936 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_mysql/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.910953 libsnew-0.1.1/libsnew/connectors/destination_postgres/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_postgres/__init__.py
--rw-rw-rw-   0        0        0     7315 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_postgres/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.921181 libsnew-0.1.1/libsnew/connectors/destination_sftp_json/
--rw-rw-rw-   0        0        0        2 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_sftp_json/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_sftp_json/client.py
--rw-rw-rw-   0        0        0     4226 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/destination_sftp_json/destination.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.924179 libsnew-0.1.1/libsnew/connectors/source_3TLIPFS/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_3TLIPFS/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_3TLIPFS/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.928645 libsnew-0.1.1/libsnew/connectors/source_IPFS/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_IPFS/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_IPFS/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.934655 libsnew-0.1.1/libsnew/connectors/source_exchange_rates/
--rw-rw-rw-   0        0        0        0 2023-04-04 11:22:01.000000 libsnew-0.1.1/libsnew/connectors/source_exchange_rates/__init__.py
--rw-rw-rw-   0        0        0     4772 2023-04-04 11:22:51.000000 libsnew-0.1.1/libsnew/connectors/source_exchange_rates/source.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.941889 libsnew-0.1.1/libsnew/connectors/source_file/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_file/__init__.py
--rw-rw-rw-   0        0        0    16972 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_file/client.py
--rw-rw-rw-   0        0        0     6307 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_file/source.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.945885 libsnew-0.1.1/libsnew/connectors/source_mysql/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_mysql/__init__.py
--rw-rw-rw-   0        0        0     5596 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_mysql/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.952566 libsnew-0.1.1/libsnew/connectors/source_postgres/
--rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_postgres/__init__.py
--rw-rw-rw-   0        0        0     5408 2023-04-01 06:22:30.000000 libsnew-0.1.1/libsnew/connectors/source_postgres/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:20:22.882138 libsnew-0.1.1/libsnew.egg-info/
--rw-rw-rw-   0        0        0     3719 2023-04-13 06:20:22.000000 libsnew-0.1.1/libsnew.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2023-04-13 06:20:22.000000 libsnew-0.1.1/libsnew.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:20:22.000000 libsnew-0.1.1/libsnew.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      389 2023-04-13 06:20:22.000000 libsnew-0.1.1/libsnew.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 06:20:22.000000 libsnew-0.1.1/libsnew.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:20:22.956553 libsnew-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1757 2023-04-13 06:20:00.000000 libsnew-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.236503 libsnew-0.1.2/
+-rw-rw-rw-   0        0        0     1073 2023-04-01 06:22:30.000000 libsnew-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3719 2023-04-13 06:26:22.235504 libsnew-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-04-03 14:37:58.000000 libsnew-0.1.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.146726 libsnew-0.1.2/libsnew/
+-rw-rw-rw-   0        0        0      449 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/Extract.py
+-rw-rw-rw-   0        0        0      452 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/Load.py
+-rw-rw-rw-   0        0        0      617 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/Ml.py
+-rw-rw-rw-   0        0        0     8881 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/Step.py
+-rw-rw-rw-   0        0        0      482 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/Transform.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.174779 libsnew-0.1.2/libsnew/connectors/
+-rw-rw-rw-   0        0        0      946 2023-04-04 12:55:16.000000 libsnew-0.1.2/libsnew/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.180167 libsnew-0.1.2/libsnew/connectors/destination_3TLIPFS/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_3TLIPFS/__init__.py
+-rw-rw-rw-   0        0        0     3593 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_3TLIPFS/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.184164 libsnew-0.1.2/libsnew/connectors/destination_IPFS/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_IPFS/__init__.py
+-rw-rw-rw-   0        0        0     2628 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_IPFS/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.187471 libsnew-0.1.2/libsnew/connectors/destination_azblob/
+-rw-rw-rw-   0        0        0        2 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_azblob/__init__.py
+-rw-rw-rw-   0        0        0      652 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_azblob/destination.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.193467 libsnew-0.1.2/libsnew/connectors/destination_mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_mysql/__init__.py
+-rw-rw-rw-   0        0        0     7936 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_mysql/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.198471 libsnew-0.1.2/libsnew/connectors/destination_postgres/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_postgres/__init__.py
+-rw-rw-rw-   0        0        0     7315 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_postgres/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.204718 libsnew-0.1.2/libsnew/connectors/destination_sftp_json/
+-rw-rw-rw-   0        0        0        2 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_sftp_json/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_sftp_json/client.py
+-rw-rw-rw-   0        0        0     4226 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/destination_sftp_json/destination.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.210134 libsnew-0.1.2/libsnew/connectors/source_3TLIPFS/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_3TLIPFS/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_3TLIPFS/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.214133 libsnew-0.1.2/libsnew/connectors/source_IPFS/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_IPFS/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_IPFS/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.218156 libsnew-0.1.2/libsnew/connectors/source_exchange_rates/
+-rw-rw-rw-   0        0        0        0 2023-04-04 11:22:01.000000 libsnew-0.1.2/libsnew/connectors/source_exchange_rates/__init__.py
+-rw-rw-rw-   0        0        0     4772 2023-04-04 11:22:51.000000 libsnew-0.1.2/libsnew/connectors/source_exchange_rates/source.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.225518 libsnew-0.1.2/libsnew/connectors/source_file/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_file/__init__.py
+-rw-rw-rw-   0        0        0    16972 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_file/client.py
+-rw-rw-rw-   0        0        0     6307 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_file/source.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.229511 libsnew-0.1.2/libsnew/connectors/source_mysql/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_mysql/__init__.py
+-rw-rw-rw-   0        0        0     5596 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_mysql/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.233510 libsnew-0.1.2/libsnew/connectors/source_postgres/
+-rw-rw-rw-   0        0        0        0 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_postgres/__init__.py
+-rw-rw-rw-   0        0        0     5408 2023-04-01 06:22:30.000000 libsnew-0.1.2/libsnew/connectors/source_postgres/client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:26:22.172772 libsnew-0.1.2/libsnew.egg-info/
+-rw-rw-rw-   0        0        0     3719 2023-04-13 06:26:21.000000 libsnew-0.1.2/libsnew.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2023-04-13 06:26:22.000000 libsnew-0.1.2/libsnew.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:26:21.000000 libsnew-0.1.2/libsnew.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      389 2023-04-13 06:26:21.000000 libsnew-0.1.2/libsnew.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 06:26:22.000000 libsnew-0.1.2/libsnew.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:26:22.237508 libsnew-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2023-04-13 06:26:10.000000 libsnew-0.1.2/setup.py
```

### Comparing `libsnew-0.1.1/LICENSE.txt` & `libsnew-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/PKG-INFO` & `libsnew-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsnew
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a 3TL module for pipeline creation
 Home-page: https://3tl.dev
 Author: Thinkartha
 Author-email: navin.naik@thinkartha.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `libsnew-0.1.1/README.txt` & `libsnew-0.1.2/README.txt`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/Ml.py` & `libsnew-0.1.2/libsnew/Ml.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/Step.py` & `libsnew-0.1.2/libsnew/Step.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/__init__.py` & `libsnew-0.1.2/libsnew/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_3TLIPFS/client.py` & `libsnew-0.1.2/libsnew/connectors/destination_3TLIPFS/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_IPFS/client.py` & `libsnew-0.1.2/libsnew/connectors/destination_IPFS/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_azblob/destination.py` & `libsnew-0.1.2/libsnew/connectors/destination_azblob/destination.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_mysql/client.py` & `libsnew-0.1.2/libsnew/connectors/destination_mysql/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_postgres/client.py` & `libsnew-0.1.2/libsnew/connectors/destination_postgres/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_sftp_json/client.py` & `libsnew-0.1.2/libsnew/connectors/destination_sftp_json/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/destination_sftp_json/destination.py` & `libsnew-0.1.2/libsnew/connectors/destination_sftp_json/destination.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_3TLIPFS/client.py` & `libsnew-0.1.2/libsnew/connectors/source_3TLIPFS/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_IPFS/client.py` & `libsnew-0.1.2/libsnew/connectors/source_IPFS/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_exchange_rates/source.py` & `libsnew-0.1.2/libsnew/connectors/source_exchange_rates/source.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_file/client.py` & `libsnew-0.1.2/libsnew/connectors/source_file/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_file/source.py` & `libsnew-0.1.2/libsnew/connectors/source_file/source.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_mysql/client.py` & `libsnew-0.1.2/libsnew/connectors/source_mysql/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew/connectors/source_postgres/client.py` & `libsnew-0.1.2/libsnew/connectors/source_postgres/client.py`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/libsnew.egg-info/PKG-INFO` & `libsnew-0.1.2/libsnew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsnew
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a 3TL module for pipeline creation
 Home-page: https://3tl.dev
 Author: Thinkartha
 Author-email: navin.naik@thinkartha.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `libsnew-0.1.1/libsnew.egg-info/SOURCES.txt` & `libsnew-0.1.2/libsnew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libsnew-0.1.1/setup.py` & `libsnew-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='libsnew',
     packages=find_packages(include=('libsnew*',)),
-    version='0.1.1',
+    version='0.1.2',
     description='This is a 3TL module for pipeline creation',
     long_description_content_type=open('README.txt').read(),
     url='https://3tl.dev',
     author='Thinkartha',
     author_email='navin.naik@thinkartha.com',
     license='BSD 2-clause',
     # packages=['libsnew'],
@@ -22,15 +22,15 @@
                       'genson==1.2.2',
                       'google-cloud-storage==2.5.0',
                       'pandas==2.0.0',
                       'paramiko==2.11.0',
                       's3fs==2022.7.1',
                       'boto3==1.21.21',
                       'smart-open[all]==6.0.0',
-                      'lxml==4.9.1',
+                      'lxml==4.9.2',
                       'html5lib==1.1',
                       'pyarrow==11.0.0',
                       'xlrd==2.0.1',
                       'openpyxl==3.0.10',
                       'PyMySQL==1.0.2',
                       'pyxlsb==1.0.9',
                       'azure-storage-blob==12.14.1',
```

