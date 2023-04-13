# Comparing `tmp/vernac-0.0.0.tar.gz` & `tmp/vernac-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernac-0.0.0.tar", last modified: Thu Apr 13 17:34:12 2023, max compression
+gzip compressed data, was "vernac-0.0.1.tar", last modified: Thu Apr 13 17:51:15 2023, max compression
```

## Comparing `vernac-0.0.0.tar` & `vernac-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:34:12.639462 vernac-0.0.0/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1867 2023-04-13 17:01:30.000000 vernac-0.0.0/.gitignore
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.0/LICENSE
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      116 2023-04-13 17:34:12.639462 vernac-0.0.0/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1837 2023-04-13 16:57:36.000000 vernac-0.0.0/README.md
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1153 2023-04-13 16:59:44.000000 vernac-0.0.0/dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.0/local-dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      409 2023-04-13 17:29:48.000000 vernac-0.0.0/pyproject.toml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-13 17:34:12.639462 vernac-0.0.0/setup.cfg
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:34:12.635462 vernac-0.0.0/src/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:34:12.635462 vernac-0.0.0/src/vernac/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     5980 2023-04-13 16:59:08.000000 vernac-0.0.0/src/vernac/compile.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:34:12.635462 vernac-0.0.0/src/vernac.egg-info/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      116 2023-04-13 17:34:12.000000 vernac-0.0.0/src/vernac.egg-info/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      319 2023-04-13 17:34:12.000000 vernac-0.0.0/src/vernac.egg-info/SOURCES.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-13 17:34:12.000000 vernac-0.0.0/src/vernac.egg-info/dependency_links.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-13 17:34:12.000000 vernac-0.0.0/src/vernac.egg-info/entry_points.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       65 2023-04-13 17:34:12.000000 vernac-0.0.0/src/vernac.egg-info/requires.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-13 17:34:12.000000 vernac-0.0.0/src/vernac.egg-info/top_level.txt
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1867 2023-04-13 17:01:30.000000 vernac-0.0.1/.gitignore
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.1/LICENSE
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1994 2023-04-13 17:51:15.983838 vernac-0.0.1/PKG-INFO
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1837 2023-04-13 16:57:36.000000 vernac-0.0.1/README.md
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1153 2023-04-13 16:59:44.000000 vernac-0.0.1/dev-requirements.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.1/local-dev-requirements.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      452 2023-04-13 17:40:54.000000 vernac-0.0.1/pyproject.toml
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-13 17:51:15.983838 vernac-0.0.1/setup.cfg
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/src/
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/src/vernac/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     5980 2023-04-13 16:59:08.000000 vernac-0.0.1/src/vernac/compile.py
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/src/vernac.egg-info/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1994 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/PKG-INFO
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      319 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/entry_points.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       65 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/requires.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/top_level.txt
```

### Comparing `vernac-0.0.0/.gitignore` & `vernac-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vernac-0.0.0/LICENSE` & `vernac-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vernac-0.0.0/README.md` & `vernac-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vernac-0.0.0/dev-requirements.txt` & `vernac-0.0.1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `vernac-0.0.0/src/vernac/compile.py` & `vernac-0.0.1/src/vernac/compile.py`

 * *Files identical despite different names*

