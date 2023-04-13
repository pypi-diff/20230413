# Comparing `tmp/autometrics-0.3.tar.gz` & `tmp/autometrics-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autometrics-0.3.tar", last modified: Tue Mar 28 09:16:20 2023, max compression
+gzip compressed data, was "autometrics-0.4.tar", max compression
```

## Comparing `autometrics-0.3.tar` & `autometrics-0.4.tar`

### file list

```diff
@@ -1,18 +1,13 @@
-drwxr-xr-x   0 aparna     (501) staff       (20)        0 2023-03-28 09:16:20.282305 autometrics-0.3/
--rw-r--r--   0 aparna     (501) staff       (20)     1022 2023-03-06 16:22:27.000000 autometrics-0.3/LICENSE
--rw-r--r--   0 aparna     (501) staff       (20)     2314 2023-03-28 09:16:20.282375 autometrics-0.3/PKG-INFO
--rw-r--r--   0 aparna     (501) staff       (20)     2097 2023-03-21 09:58:27.000000 autometrics-0.3/README.md
--rw-r--r--   0 aparna     (501) staff       (20)       86 2023-03-08 12:04:08.000000 autometrics-0.3/pyproject.toml
--rw-r--r--   0 aparna     (501) staff       (20)      319 2023-03-28 09:16:20.282619 autometrics-0.3/setup.cfg
--rw-r--r--   0 aparna     (501) staff       (20)      208 2023-03-28 09:15:58.000000 autometrics-0.3/setup.py
-drwxr-xr-x   0 aparna     (501) staff       (20)        0 2023-03-28 09:16:20.279723 autometrics-0.3/src/
-drwxr-xr-x   0 aparna     (501) staff       (20)        0 2023-03-28 09:16:20.281327 autometrics-0.3/src/autometrics/
--rw-r--r--   0 aparna     (501) staff       (20)        0 2023-03-06 14:16:36.000000 autometrics-0.3/src/autometrics/__init__.py
--rw-r--r--   0 aparna     (501) staff       (20)     2262 2023-03-27 13:49:23.000000 autometrics-0.3/src/autometrics/autometrics.py
--rw-r--r--   0 aparna     (501) staff       (20)     1463 2023-03-21 09:58:27.000000 autometrics-0.3/src/autometrics/prometheus_url.py
-drwxr-xr-x   0 aparna     (501) staff       (20)        0 2023-03-28 09:16:20.282184 autometrics-0.3/src/autometrics.egg-info/
--rw-r--r--   0 aparna     (501) staff       (20)     2314 2023-03-28 09:16:20.000000 autometrics-0.3/src/autometrics.egg-info/PKG-INFO
--rw-r--r--   0 aparna     (501) staff       (20)      338 2023-03-28 09:16:20.000000 autometrics-0.3/src/autometrics.egg-info/SOURCES.txt
--rw-r--r--   0 aparna     (501) staff       (20)        1 2023-03-28 09:16:20.000000 autometrics-0.3/src/autometrics.egg-info/dependency_links.txt
--rw-r--r--   0 aparna     (501) staff       (20)       32 2023-03-28 09:16:20.000000 autometrics-0.3/src/autometrics.egg-info/requires.txt
--rw-r--r--   0 aparna     (501) staff       (20)       12 2023-03-28 09:16:20.000000 autometrics-0.3/src/autometrics.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1022 2023-03-06 16:22:27.425939 autometrics-0.4/LICENSE
+-rw-r--r--   0        0        0     5439 2023-04-13 10:20:53.040055 autometrics-0.4/README.md
+-rw-r--r--   0        0        0     1825 2023-04-13 10:53:46.784179 autometrics-0.4/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-13 09:01:12.452935 autometrics-0.4/src/autometrics/__init__.py
+-rw-r--r--   0        0        0      843 2023-04-13 10:20:53.042912 autometrics-0.4/src/autometrics/constants.py
+-rw-r--r--   0        0        0     1913 2023-04-13 10:20:53.043762 autometrics-0.4/src/autometrics/decorator.py
+-rw-r--r--   0        0        0     2158 2023-04-13 10:20:53.044169 autometrics-0.4/src/autometrics/emit.py
+-rw-r--r--   0        0        0     3050 2023-04-13 10:20:53.044607 autometrics-0.4/src/autometrics/objectives.py
+-rw-r--r--   0        0        0     1956 2023-04-13 10:20:53.045139 autometrics-0.4/src/autometrics/prometheus_url.py
+-rw-r--r--   0        0        0     6787 2023-04-13 10:20:53.045649 autometrics-0.4/src/autometrics/test_decorator.py
+-rw-r--r--   0        0        0     1401 2023-04-13 10:20:53.045977 autometrics-0.4/src/autometrics/test_prometheus_url.py
+-rw-r--r--   0        0        0     1535 2023-04-13 10:20:53.046402 autometrics-0.4/src/autometrics/utils.py
+-rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 autometrics-0.4/PKG-INFO
```

### Comparing `autometrics-0.3/LICENSE` & `autometrics-0.4/LICENSE`

 * *Files identical despite different names*

