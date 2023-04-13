# Comparing `tmp/ruphonetic-0.1.4.tar.gz` & `tmp/ruphonetic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruphonetic-0.1.4.tar", last modified: Sun Jun 26 09:18:20 2022, max compression
+gzip compressed data, was "ruphonetic-0.1.5.tar", last modified: Thu Apr 13 19:28:46 2023, max compression
```

## Comparing `ruphonetic-0.1.4.tar` & `ruphonetic-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-06-26 09:18:20.401859 ruphonetic-0.1.4/
--rw-rw-rw-   0        0        0      373 2022-06-26 09:16:38.000000 ruphonetic-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2022-06-25 19:33:55.000000 ruphonetic-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       31 2022-06-12 12:18:34.000000 ruphonetic-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      950 2022-06-26 09:18:20.401859 ruphonetic-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       32 2022-06-25 19:34:04.000000 ruphonetic-0.1.4/README.txt
-drwxrwxrwx   0        0        0        0 2022-06-26 09:18:20.255778 ruphonetic-0.1.4/ruphonetic/
--rw-rw-rw-   0        0        0     4499 2022-06-26 09:17:56.000000 ruphonetic-0.1.4/ruphonetic/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-26 09:18:20.269281 ruphonetic-0.1.4/ruphonetic/accentuation/
--rw-rw-rw-   0        0        0        0 2022-06-25 20:10:13.000000 ruphonetic-0.1.4/ruphonetic/accentuation/__init__.py
--rw-rw-rw-   0        0        0  2023355 2021-08-25 03:07:42.000000 ruphonetic-0.1.4/ruphonetic/accentuation/lemmas.dat
--rw-rw-rw-   0        0        0     6813 2022-06-25 20:14:12.000000 ruphonetic-0.1.4/ruphonetic/accentuation/stress.py
--rw-rw-rw-   0        0        0 70568821 2021-08-25 03:07:42.000000 ruphonetic-0.1.4/ruphonetic/accentuation/wordforms.dat
--rw-rw-rw-   0        0        0     6533 2022-06-25 20:01:49.000000 ruphonetic-0.1.4/ruphonetic/transcriptor.py
--rw-rw-rw-   0        0        0      707 2022-06-26 09:15:09.000000 ruphonetic-0.1.4/ruphonetic/utils.py
-drwxrwxrwx   0        0        0        0 2022-06-26 09:18:20.259279 ruphonetic-0.1.4/ruphonetic.egg-info/
--rw-rw-rw-   0        0        0      950 2022-06-26 09:18:20.000000 ruphonetic-0.1.4/ruphonetic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2022-06-26 09:18:20.000000 ruphonetic-0.1.4/ruphonetic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-26 09:18:20.000000 ruphonetic-0.1.4/ruphonetic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-06-26 09:18:20.000000 ruphonetic-0.1.4/ruphonetic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-06-26 09:18:20.000000 ruphonetic-0.1.4/ruphonetic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-26 09:18:20.402859 ruphonetic-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      751 2022-06-26 09:16:04.000000 ruphonetic-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:28:46.306441 ruphonetic-0.1.5/
+-rw-rw-rw-   0        0        0      436 2023-04-13 18:58:30.000000 ruphonetic-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2022-06-25 19:33:55.000000 ruphonetic-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       31 2022-06-12 12:18:34.000000 ruphonetic-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      985 2023-04-13 19:28:46.306441 ruphonetic-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2022-06-25 19:34:04.000000 ruphonetic-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:28:46.222443 ruphonetic-0.1.5/ruphonetic/
+-rw-rw-rw-   0        0        0     4499 2022-06-26 09:17:56.000000 ruphonetic-0.1.5/ruphonetic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:28:46.231939 ruphonetic-0.1.5/ruphonetic/accentuation/
+-rw-rw-rw-   0        0        0        0 2022-06-25 20:10:13.000000 ruphonetic-0.1.5/ruphonetic/accentuation/__init__.py
+-rw-rw-rw-   0        0        0  2023355 2021-08-25 03:07:42.000000 ruphonetic-0.1.5/ruphonetic/accentuation/lemmas.dat
+-rw-rw-rw-   0        0        0     6813 2022-06-25 20:14:12.000000 ruphonetic-0.1.5/ruphonetic/accentuation/stress.py
+-rw-rw-rw-   0        0        0 70568821 2021-08-25 03:07:42.000000 ruphonetic-0.1.5/ruphonetic/accentuation/wordforms.dat
+-rw-rw-rw-   0        0        0     6533 2022-06-25 20:01:49.000000 ruphonetic-0.1.5/ruphonetic/transcriptor.py
+-rw-rw-rw-   0        0        0      707 2022-06-26 09:15:09.000000 ruphonetic-0.1.5/ruphonetic/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:28:46.226443 ruphonetic-0.1.5/ruphonetic.egg-info/
+-rw-rw-rw-   0        0        0      985 2023-04-13 19:28:46.000000 ruphonetic-0.1.5/ruphonetic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-13 19:28:46.000000 ruphonetic-0.1.5/ruphonetic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:28:46.000000 ruphonetic-0.1.5/ruphonetic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-13 19:28:46.000000 ruphonetic-0.1.5/ruphonetic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 19:28:46.000000 ruphonetic-0.1.5/ruphonetic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:28:46.307442 ruphonetic-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-04-13 19:28:44.000000 ruphonetic-0.1.5/setup.py
```

### Comparing `ruphonetic-0.1.4/LICENSE.txt` & `ruphonetic-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/PKG-INFO` & `ruphonetic-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: ruphonetic
-Version: 0.1.4
+Version: 0.1.5
 Summary: Russian Phonetic Analysis Module
-Home-page: UNKNOWN
+Home-page: 
 Author: Igor Furkalo
 Author-email: igor.furkalo@gmail.com
 License: MIT
 Keywords: quantanalysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 Russian Phonetic Analysis Module
 
 Change Log
 ===============
 
-0.1.3 (25.06.2022)
+0.1.5 (13.04.2023)
+--------------------
+-Add package data
+
+0.1.4 (25.06.2022)
 --------------------
 -Add pie, bar plot support
 
 0.1.3 (25.06.2022)
 --------------------
 -Spacy model installation workaround
 
@@ -35,8 +38,7 @@
 0.1.1 (25.06.2022)
 --------------------
 -Remove pprint
 
 0.1 (25.06.2022)
 --------------------
 -First Release
-
```

### Comparing `ruphonetic-0.1.4/ruphonetic/__init__.py` & `ruphonetic-0.1.5/ruphonetic/__init__.py`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/ruphonetic/accentuation/lemmas.dat` & `ruphonetic-0.1.5/ruphonetic/accentuation/lemmas.dat`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/ruphonetic/accentuation/stress.py` & `ruphonetic-0.1.5/ruphonetic/accentuation/stress.py`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/ruphonetic/accentuation/wordforms.dat` & `ruphonetic-0.1.5/ruphonetic/accentuation/wordforms.dat`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/ruphonetic/transcriptor.py` & `ruphonetic-0.1.5/ruphonetic/transcriptor.py`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/ruphonetic/utils.py` & `ruphonetic-0.1.5/ruphonetic/utils.py`

 * *Files identical despite different names*

### Comparing `ruphonetic-0.1.4/ruphonetic.egg-info/PKG-INFO` & `ruphonetic-0.1.5/ruphonetic.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: ruphonetic
-Version: 0.1.4
+Version: 0.1.5
 Summary: Russian Phonetic Analysis Module
-Home-page: UNKNOWN
+Home-page: 
 Author: Igor Furkalo
 Author-email: igor.furkalo@gmail.com
 License: MIT
 Keywords: quantanalysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 Russian Phonetic Analysis Module
 
 Change Log
 ===============
 
-0.1.3 (25.06.2022)
+0.1.5 (13.04.2023)
+--------------------
+-Add package data
+
+0.1.4 (25.06.2022)
 --------------------
 -Add pie, bar plot support
 
 0.1.3 (25.06.2022)
 --------------------
 -Spacy model installation workaround
 
@@ -35,8 +38,7 @@
 0.1.1 (25.06.2022)
 --------------------
 -Remove pprint
 
 0.1 (25.06.2022)
 --------------------
 -First Release
-
```

