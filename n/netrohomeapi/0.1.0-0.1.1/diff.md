# Comparing `tmp/netrohomeapi-0.1.0.tar.gz` & `tmp/netrohomeapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netrohomeapi-0.1.0.tar", last modified: Thu Apr 13 13:09:02 2023, max compression
+gzip compressed data, was "netrohomeapi-0.1.1.tar", last modified: Thu Apr 13 14:01:51 2023, max compression
```

## Comparing `netrohomeapi-0.1.0.tar` & `netrohomeapi-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jorgebarca   (501) staff       (20)        0 2023-04-13 13:09:02.172346 netrohomeapi-0.1.0/
--rw-r--r--   0 jorgebarca   (501) staff       (20)     1087 2023-04-13 12:55:44.000000 netrohomeapi-0.1.0/LICENSE
--rw-r--r--   0 jorgebarca   (501) staff       (20)      778 2023-04-13 13:09:02.174676 netrohomeapi-0.1.0/PKG-INFO
--rw-r--r--   0 jorgebarca   (501) staff       (20)      428 2023-04-13 12:54:32.000000 netrohomeapi-0.1.0/README.md
-drwxr-xr-x   0 jorgebarca   (501) staff       (20)        0 2023-04-13 13:09:02.157527 netrohomeapi-0.1.0/netrohomeapi/
--rw-r--r--   0 jorgebarca   (501) staff       (20)        0 2023-03-27 17:04:09.000000 netrohomeapi-0.1.0/netrohomeapi/__init__.py
--rw-r--r--   0 jorgebarca   (501) staff       (20)     3822 2023-04-12 14:53:57.000000 netrohomeapi-0.1.0/netrohomeapi/models.py
--rw-r--r--   0 jorgebarca   (501) staff       (20)     8772 2023-04-13 13:04:27.000000 netrohomeapi-0.1.0/netrohomeapi/netrohomeapi.py
-drwxr-xr-x   0 jorgebarca   (501) staff       (20)        0 2023-04-13 13:09:02.169896 netrohomeapi-0.1.0/netrohomeapi.egg-info/
--rw-r--r--   0 jorgebarca   (501) staff       (20)      778 2023-04-13 13:09:02.000000 netrohomeapi-0.1.0/netrohomeapi.egg-info/PKG-INFO
--rw-r--r--   0 jorgebarca   (501) staff       (20)      292 2023-04-13 13:09:02.000000 netrohomeapi-0.1.0/netrohomeapi.egg-info/SOURCES.txt
--rw-r--r--   0 jorgebarca   (501) staff       (20)        1 2023-04-13 13:09:02.000000 netrohomeapi-0.1.0/netrohomeapi.egg-info/dependency_links.txt
--rw-r--r--   0 jorgebarca   (501) staff       (20)       17 2023-04-13 13:09:02.000000 netrohomeapi-0.1.0/netrohomeapi.egg-info/requires.txt
--rw-r--r--   0 jorgebarca   (501) staff       (20)       13 2023-04-13 13:09:02.000000 netrohomeapi-0.1.0/netrohomeapi.egg-info/top_level.txt
--rw-r--r--   0 jorgebarca   (501) staff       (20)       79 2023-04-13 13:09:02.179505 netrohomeapi-0.1.0/setup.cfg
--rw-r--r--   0 jorgebarca   (501) staff       (20)      934 2023-04-13 13:03:45.000000 netrohomeapi-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:01:51.167073 netrohomeapi-0.1.1/netrohomeapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/netrohomeapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/netrohomeapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/netrohomeapi/netrohomeapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/netrohomeapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 14:01:51.000000 netrohomeapi-0.1.1/netrohomeapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 14:01:51.171073 netrohomeapi-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 14:01:34.000000 netrohomeapi-0.1.1/setup.py
```

### Comparing `netrohomeapi-0.1.0/LICENSE` & `netrohomeapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netrohomeapi-0.1.0/netrohomeapi/models.py` & `netrohomeapi-0.1.1/netrohomeapi/models.py`

 * *Files identical despite different names*

### Comparing `netrohomeapi-0.1.0/netrohomeapi/netrohomeapi.py` & `netrohomeapi-0.1.1/netrohomeapi/netrohomeapi.py`

 * *Files identical despite different names*

