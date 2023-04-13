# Comparing `tmp/pynativeextractor-1.0.9.tar.gz` & `tmp/pynativeextractor-10.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynativeextractor-1.0.9.tar", last modified: Fri Jan  7 11:37:10 2022, max compression
+gzip compressed data, was "dist/pynativeextractor-10.0.12.tar", last modified: Wed Jul 13 11:32:01 2022, max compression
```

## Comparing `pynativeextractor-1.0.9.tar` & `pynativeextractor-10.0.12.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.543975 pynativeextractor-1.0.9/
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       65 2021-06-11 07:18:41.000000 pynativeextractor-1.0.9/MANIFEST.in
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2980 2022-01-07 11:37:10.543975 pynativeextractor-1.0.9/PKG-INFO
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1876 2021-06-11 07:17:43.000000 pynativeextractor-1.0.9/README.md
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.499975 pynativeextractor-1.0.9/nativeextractor/
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.499975 pynativeextractor-1.0.9/nativeextractor/include/
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.519975 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1465 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/common.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2275 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/csv_parser.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     4522 2021-11-15 12:26:22.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/extractor.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2095 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/finite_automaton.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    15656 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/miner.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1034 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/ner.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1019 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/occurrence.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1002 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/pair.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     7812 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/patricia.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1157 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/patricia_miner.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     4494 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/regex_generator.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     5952 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/stream.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2154 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/terminal.h
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     4178 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/unicode.h
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.535975 pynativeextractor-1.0.9/nativeextractor/src/
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     5596 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/csv_parser.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    15171 2021-11-15 12:26:22.000000 pynativeextractor-1.0.9/nativeextractor/src/extractor.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    10925 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/finite_automaton.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     9515 2021-11-15 12:26:22.000000 pynativeextractor-1.0.9/nativeextractor/src/miner.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1754 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/ner.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1075 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/occurrence.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1046 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/pair.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    18601 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/patricia.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1280 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/patricia_miner.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    34612 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/regex_generator.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     6088 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/stream.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1654 2021-07-12 10:42:20.000000 pynativeextractor-1.0.9/nativeextractor/src/unicode.c
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     8940 2021-11-15 12:26:12.000000 pynativeextractor-1.0.9/nativeextractormodule.c
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.539975 pynativeextractor-1.0.9/pynativeextractor/
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       24 2021-06-11 07:17:43.000000 pynativeextractor-1.0.9/pynativeextractor/__init__.py
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     5810 2021-11-15 12:26:12.000000 pynativeextractor-1.0.9/pynativeextractor/extractor.py
-drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-01-07 11:37:10.543975 pynativeextractor-1.0.9/pynativeextractor.egg-info/
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2980 2022-01-07 11:37:10.000000 pynativeextractor-1.0.9/pynativeextractor.egg-info/PKG-INFO
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1437 2022-01-07 11:37:10.000000 pynativeextractor-1.0.9/pynativeextractor.egg-info/SOURCES.txt
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)        1 2022-01-07 11:37:10.000000 pynativeextractor-1.0.9/pynativeextractor.egg-info/dependency_links.txt
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       38 2022-01-07 11:37:10.000000 pynativeextractor-1.0.9/pynativeextractor.egg-info/top_level.txt
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       38 2022-01-07 11:37:10.543975 pynativeextractor-1.0.9/setup.cfg
--rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1747 2022-01-07 11:35:17.000000 pynativeextractor-1.0.9/setup.py
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2982 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/PKG-INFO
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor/
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     5810 2022-07-12 08:27:28.000000 pynativeextractor-10.0.12/pynativeextractor/extractor.py
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       24 2022-07-12 08:27:28.000000 pynativeextractor-10.0.12/pynativeextractor/__init__.py
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2246 2022-07-13 11:25:04.000000 pynativeextractor-10.0.12/setup.py
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1876 2022-07-12 08:27:28.000000 pynativeextractor-10.0.12/README.md
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/nativeextractor/
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/nativeextractor/include/
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     4178 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/unicode.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1019 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/occurrence.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     4494 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/regex_generator.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1034 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/ner.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     5952 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/stream.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     4522 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/extractor.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    15656 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/miner.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1002 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/pair.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1465 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/common.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2154 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/terminal.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2275 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/csv_parser.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     7812 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/patricia.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2095 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/finite_automaton.h
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1157 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/patricia_miner.h
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/nativeextractor/src/
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    10925 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/finite_automaton.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    34612 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/regex_generator.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     5596 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/csv_parser.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    15194 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/extractor.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     6088 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/stream.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1046 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/pair.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1075 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/occurrence.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)    18601 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/patricia.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1280 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/patricia_miner.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1754 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/ner.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     9515 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/miner.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1654 2022-07-12 08:27:29.000000 pynativeextractor-10.0.12/nativeextractor/src/unicode.c
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       65 2022-07-12 08:27:28.000000 pynativeextractor-10.0.12/MANIFEST.in
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       38 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/setup.cfg
+drwxrwxr-x   0 mafiosso  (1000) mafiosso  (1000)        0 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor.egg-info/
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     2982 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor.egg-info/PKG-INFO
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     1477 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)        6 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor.egg-info/requires.txt
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)        1 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)       38 2022-07-13 11:32:01.000000 pynativeextractor-10.0.12/pynativeextractor.egg-info/top_level.txt
+-rw-rw-r--   0 mafiosso  (1000) mafiosso  (1000)     9001 2022-07-13 10:39:17.000000 pynativeextractor-10.0.12/nativeextractormodule.c
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pynativeextractor-1.0.9/PKG-INFO` & `pynativeextractor-10.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynativeextractor
-Version: 1.0.9
+Version: 10.0.12
 Summary: Python binding for nativeextractor
 Home-page: https://github.com/SpongeData-cz/pynativeextractor
 Author: SpongeData s.r.o.
 Author-email: info@spongedata.cz
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/SpongeData-cz/pynativeextractor/issues
 Description: # NativeExtractor module for Python
```

### Comparing `pynativeextractor-1.0.9/README.md` & `pynativeextractor-10.0.12/README.md`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/common.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/common.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/csv_parser.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/csv_parser.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/extractor.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/extractor.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/finite_automaton.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/finite_automaton.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/miner.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/miner.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/ner.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/ner.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/occurrence.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/occurrence.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/pair.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/pair.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/patricia.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/patricia.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/patricia_miner.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/patricia_miner.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/regex_generator.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/regex_generator.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/stream.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/stream.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/terminal.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/terminal.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/include/nativeextractor/unicode.h` & `pynativeextractor-10.0.12/nativeextractor/include/nativeextractor/unicode.h`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/csv_parser.c` & `pynativeextractor-10.0.12/nativeextractor/src/csv_parser.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/extractor.c` & `pynativeextractor-10.0.12/nativeextractor/src/extractor.c`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,16 @@
     return false;
   }
 
   for (unsigned m = 0; m < self->miners_count; ++m) {
     self->miners[m]->set_stream(self->miners[m], self->stream);
   }
 
+  self->last_max = 0;
+
   pthread_mutex_unlock(&(self->mutex_extractor));
 
   return true;
 }
 
 void extractor_c_unset_stream(extractor_c* self) {
   pthread_mutex_lock(&(self->mutex_extractor));
```

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/finite_automaton.c` & `pynativeextractor-10.0.12/nativeextractor/src/finite_automaton.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/miner.c` & `pynativeextractor-10.0.12/nativeextractor/src/miner.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/ner.c` & `pynativeextractor-10.0.12/nativeextractor/src/ner.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/occurrence.c` & `pynativeextractor-10.0.12/nativeextractor/src/occurrence.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/pair.c` & `pynativeextractor-10.0.12/nativeextractor/src/pair.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/patricia.c` & `pynativeextractor-10.0.12/nativeextractor/src/patricia.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/patricia_miner.c` & `pynativeextractor-10.0.12/nativeextractor/src/patricia_miner.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/regex_generator.c` & `pynativeextractor-10.0.12/nativeextractor/src/regex_generator.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/stream.c` & `pynativeextractor-10.0.12/nativeextractor/src/stream.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractor/src/unicode.c` & `pynativeextractor-10.0.12/nativeextractor/src/unicode.c`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/nativeextractormodule.c` & `pynativeextractor-10.0.12/nativeextractormodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 /**
  * Copyright (c) 2021 SpongeData s.r.o.
  *
  * This software is released under the MIT License.
  * https://opensource.org/licenses/MIT
  */
 
+// Define Python 3.10+ macro
+#define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <string.h>
 #include <nativeextractor/extractor.h>
 #include <nativeextractor/miner.h>
 #include <nativeextractor/occurrence.h>
 
 static PyObject *stream_file_new(PyObject *self, PyObject *args) {
@@ -65,15 +67,15 @@
   DESTROY(stream);
 
   Py_RETURN_NONE;
 }
 
 static PyObject *stream_buffer_new(PyObject *self, PyObject *args) {
   const char *buffer;
-  int buflen;
+  Py_ssize_t buflen;
 
   if (!PyArg_ParseTuple(args, "s#", &buffer, &buflen)) {
     return NULL;
   }
 
   char * buffer_mem = malloc(buflen);
   memcpy(buffer_mem, buffer, buflen);
```

### Comparing `pynativeextractor-1.0.9/pynativeextractor/extractor.py` & `pynativeextractor-10.0.12/pynativeextractor/extractor.py`

 * *Files identical despite different names*

### Comparing `pynativeextractor-1.0.9/pynativeextractor.egg-info/PKG-INFO` & `pynativeextractor-10.0.12/pynativeextractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynativeextractor
-Version: 1.0.9
+Version: 10.0.12
 Summary: Python binding for nativeextractor
 Home-page: https://github.com/SpongeData-cz/pynativeextractor
 Author: SpongeData s.r.o.
 Author-email: info@spongedata.cz
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/SpongeData-cz/pynativeextractor/issues
 Description: # NativeExtractor module for Python
```

### Comparing `pynativeextractor-1.0.9/pynativeextractor.egg-info/SOURCES.txt` & `pynativeextractor-10.0.12/pynativeextractor.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 ./nativeextractor/src/stream.c
 ./nativeextractor/src/unicode.c
 pynativeextractor/__init__.py
 pynativeextractor/extractor.py
 pynativeextractor.egg-info/PKG-INFO
 pynativeextractor.egg-info/SOURCES.txt
 pynativeextractor.egg-info/dependency_links.txt
+pynativeextractor.egg-info/requires.txt
 pynativeextractor.egg-info/top_level.txt
```

### Comparing `pynativeextractor-1.0.9/setup.py` & `pynativeextractor-10.0.12/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import glob, setuptools
 import sys
-from distutils.core import setup, Extension
+from distutils.core import Extension
+from setuptools import setup
+import subprocess
+import re
 
 sources = ['nativeextractormodule.c'] + glob.glob('./nativeextractor/src/*.c')
 
 if sys.version_info >= (3, 0):
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 else:
     with open("README.md", "r") as fh:
         long_description = fh.read().decode("utf-8")
 
+def get_git_version():
+    tag = subprocess.check_output([ "git", "describe", "--tags", "--abbrev=0", ])
+    if sys.version_info >= (3, 0):
+        tag = tag.decode("utf-8")
+    found = re.search(r"v(?P<tag>\d+.\d+.\d+)", tag)
+    if found is None:
+        raise Exception("No tag in git!")
+    found = found.groupdict()
+    return found["tag"]
+
 kwargs = {
     "setup_requires": ['wheel'], # for future releases to support wheel by default
     "name": "pynativeextractor",
-    "version": "1.0.9",
+    "version": "10.0.12", #get_git_version(), - unable to install if you use
     "author": "SpongeData s.r.o.",
     "author_email": "info@spongedata.cz",
     "description": "Python binding for nativeextractor",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "ext_modules": [
         Extension(
@@ -43,11 +56,14 @@
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     "packages": setuptools.find_packages(),
     "python_requires":">=2.7",
+    "install_requires": [
+        "wheel",
+    ],
 }
 
 setup(**kwargs)
```

