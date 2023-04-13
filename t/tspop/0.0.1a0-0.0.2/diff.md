# Comparing `tmp/tspop-0.0.1a0.tar.gz` & `tmp/tspop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tspop-0.0.1a0.tar", last modified: Thu Jul 21 03:41:15 2022, max compression
+gzip compressed data, was "tspop-0.0.2.tar", last modified: Thu Apr 13 21:08:31 2023, max compression
```

## Comparing `tspop-0.0.1a0.tar` & `tspop-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 gtsambos (1726227300) 1793139257        0 2022-07-21 03:41:15.544610 tspop-0.0.1a0/
--rw-r--r--   0 gtsambos (1726227300) 1793139257     1407 2022-07-21 03:41:15.544098 tspop-0.0.1a0/PKG-INFO
--rw-r--r--   0 gtsambos (1726227300) 1793139257      501 2022-07-05 00:46:19.000000 tspop-0.0.1a0/README.rst
--rw-r--r--   0 gtsambos (1726227300) 1793139257       38 2022-07-21 03:41:15.544783 tspop-0.0.1a0/setup.cfg
--rw-r--r--   0 gtsambos (1726227300) 1793139257     1026 2022-07-21 03:41:09.000000 tspop-0.0.1a0/setup.py
-drwxr-xr-x   0 gtsambos (1726227300) 1793139257        0 2022-07-21 03:41:15.483808 tspop-0.0.1a0/src/
-drwxr-xr-x   0 gtsambos (1726227300) 1793139257        0 2022-07-21 03:41:15.543451 tspop-0.0.1a0/src/tspop.egg-info/
--rw-r--r--   0 gtsambos (1726227300) 1793139257     1407 2022-07-21 03:41:14.000000 tspop-0.0.1a0/src/tspop.egg-info/PKG-INFO
--rw-r--r--   0 gtsambos (1726227300) 1793139257      196 2022-07-21 03:41:15.000000 tspop-0.0.1a0/src/tspop.egg-info/SOURCES.txt
--rw-r--r--   0 gtsambos (1726227300) 1793139257        1 2022-07-21 03:41:14.000000 tspop-0.0.1a0/src/tspop.egg-info/dependency_links.txt
--rw-r--r--   0 gtsambos (1726227300) 1793139257       75 2022-07-21 03:41:14.000000 tspop-0.0.1a0/src/tspop.egg-info/requires.txt
--rw-r--r--   0 gtsambos (1726227300) 1793139257        6 2022-07-21 03:41:14.000000 tspop-0.0.1a0/src/tspop.egg-info/top_level.txt
--rw-r--r--   0 gtsambos (1726227300) 1793139257     5485 2022-07-15 06:06:29.000000 tspop-0.0.1a0/src/tspop.py
+drwxr-xr-x   0 georgia    (501) staff       (20)        0 2023-04-13 21:08:31.124070 tspop-0.0.2/
+-rw-r--r--   0 georgia    (501) staff       (20)     1071 2022-07-07 04:54:28.000000 tspop-0.0.2/LICENCE.txt
+-rw-r--r--   0 georgia    (501) staff       (20)      901 2023-04-13 21:08:31.123575 tspop-0.0.2/PKG-INFO
+-rw-r--r--   0 georgia    (501) staff       (20)      282 2022-07-17 12:43:54.000000 tspop-0.0.2/README.rst
+-rw-r--r--   0 georgia    (501) staff       (20)       38 2023-04-13 21:08:31.124277 tspop-0.0.2/setup.cfg
+-rw-r--r--   0 georgia    (501) staff       (20)     1049 2022-07-29 02:36:40.000000 tspop-0.0.2/setup.py
+drwxr-xr-x   0 georgia    (501) staff       (20)        0 2023-04-13 21:08:31.118762 tspop-0.0.2/src/
+drwxr-xr-x   0 georgia    (501) staff       (20)        0 2023-04-13 21:08:31.122892 tspop-0.0.2/src/tspop.egg-info/
+-rw-r--r--   0 georgia    (501) staff       (20)      901 2023-04-13 21:08:31.000000 tspop-0.0.2/src/tspop.egg-info/PKG-INFO
+-rw-r--r--   0 georgia    (501) staff       (20)      208 2023-04-13 21:08:31.000000 tspop-0.0.2/src/tspop.egg-info/SOURCES.txt
+-rw-r--r--   0 georgia    (501) staff       (20)        1 2023-04-13 21:08:31.000000 tspop-0.0.2/src/tspop.egg-info/dependency_links.txt
+-rw-r--r--   0 georgia    (501) staff       (20)       93 2023-04-13 21:08:31.000000 tspop-0.0.2/src/tspop.egg-info/requires.txt
+-rw-r--r--   0 georgia    (501) staff       (20)        6 2023-04-13 21:08:31.000000 tspop-0.0.2/src/tspop.egg-info/top_level.txt
+-rw-r--r--   0 georgia    (501) staff       (20)    13858 2023-04-10 02:12:26.000000 tspop-0.0.2/src/tspop.py
```

### Comparing `tspop-0.0.1a0/setup.py` & `tspop-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 		"Natural Language :: English"
 	],
 	long_description = long_description,
 	long_description_content_type = "text/x-rst",
 	install_requires = [
 		"tskit>=0.2.3",
 		"pandas>=1.2.0",
-		"numpy>=1.21.0"
+		"numpy>=1.21.0",
+		"matplotlib>=3.4.0"
 	],
 	extras_require = {
 		"dev" : ["pytest>=3.7",
 				"msprime==1.1.1"
 				]
 	}
 	)
```

