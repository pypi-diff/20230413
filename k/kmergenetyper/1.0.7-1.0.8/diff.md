# Comparing `tmp/kmergenetyper-1.0.7.tar.gz` & `tmp/kmergenetyper-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmergenetyper-1.0.7.tar", last modified: Tue Apr 11 12:08:10 2023, max compression
+gzip compressed data, was "kmergenetyper-1.0.8.tar", last modified: Thu Apr 13 12:05:07 2023, max compression
```

## Comparing `kmergenetyper-1.0.7.tar` & `kmergenetyper-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.554905 kmergenetyper-1.0.7/
--rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.7/LICENSE
--rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 12:08:10.554787 kmergenetyper-1.0.7/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      195 2023-04-04 09:02:07.000000 kmergenetyper-1.0.7/README.md
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.553209 kmergenetyper-1.0.7/bin/
--rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.7/bin/kmergenetyper
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.554163 kmergenetyper-1.0.7/kmergenetyper/
--rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.7/kmergenetyper/__init__.py
--rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.7/kmergenetyper/kma.py
--rw-r--r--   0 malhal     (502) staff       (20)     4010 2023-04-11 12:06:05.000000 kmergenetyper-1.0.7/kmergenetyper/realignConsensus.py
--rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.7/kmergenetyper/typeGenes.py
--rw-r--r--   0 malhal     (502) staff       (20)       21 2023-04-11 12:08:05.000000 kmergenetyper-1.0.7/kmergenetyper/version.py
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-11 12:08:10.554620 kmergenetyper-1.0.7/kmergenetyper.egg-info/
--rw-r--r--   0 malhal     (502) staff       (20)      243 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/SOURCES.txt
--rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/dependency_links.txt
--rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-11 12:08:10.000000 kmergenetyper-1.0.7/kmergenetyper.egg-info/top_level.txt
--rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-11 12:08:10.554957 kmergenetyper-1.0.7/setup.cfg
--rw-r--r--   0 malhal     (502) staff       (20)      442 2023-04-11 12:08:05.000000 kmergenetyper-1.0.7/setup.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.641918 kmergenetyper-1.0.8/
+-rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.8/LICENSE
+-rw-r--r--   0 malhal     (502) staff       (20)      645 2023-04-13 12:05:07.641797 kmergenetyper-1.0.8/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      361 2023-04-13 12:04:26.000000 kmergenetyper-1.0.8/README.md
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.639987 kmergenetyper-1.0.8/bin/
+-rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.8/bin/kmergenetyper
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.641168 kmergenetyper-1.0.8/kmergenetyper/
+-rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.8/kmergenetyper/__init__.py
+-rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.8/kmergenetyper/kma.py
+-rw-r--r--   0 malhal     (502) staff       (20)     4010 2023-04-11 12:06:05.000000 kmergenetyper-1.0.8/kmergenetyper/realignConsensus.py
+-rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.8/kmergenetyper/typeGenes.py
+-rw-r--r--   0 malhal     (502) staff       (20)       21 2023-04-13 12:04:58.000000 kmergenetyper-1.0.8/kmergenetyper/version.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-04-13 12:05:07.641610 kmergenetyper-1.0.8/kmergenetyper.egg-info/
+-rw-r--r--   0 malhal     (502) staff       (20)      645 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      325 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/SOURCES.txt
+-rw-r--r--   0 malhal     (502) staff       (20)        1 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/dependency_links.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       14 2023-04-13 12:05:07.000000 kmergenetyper-1.0.8/kmergenetyper.egg-info/top_level.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       38 2023-04-13 12:05:07.641963 kmergenetyper-1.0.8/setup.cfg
+-rw-r--r--   0 malhal     (502) staff       (20)      659 2023-04-13 12:05:04.000000 kmergenetyper-1.0.8/setup.py
```

### Comparing `kmergenetyper-1.0.7/LICENSE` & `kmergenetyper-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.7/bin/kmergenetyper` & `kmergenetyper-1.0.8/bin/kmergenetyper`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.7/kmergenetyper/kma.py` & `kmergenetyper-1.0.8/kmergenetyper/kma.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.7/kmergenetyper/realignConsensus.py` & `kmergenetyper-1.0.8/kmergenetyper/realignConsensus.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.7/kmergenetyper/typeGenes.py` & `kmergenetyper-1.0.8/kmergenetyper/typeGenes.py`

 * *Files identical despite different names*

