# Comparing `tmp/contact-energy-nz-0.1.4684335331.tar.gz` & `tmp/contact-energy-nz-0.1.4684953769.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-energy-nz-0.1.4684335331.tar", last modified: Thu Apr 13 00:55:55 2023, max compression
+gzip compressed data, was "contact-energy-nz-0.1.4684953769.tar", last modified: Thu Apr 13 02:42:51 2023, max compression
```

## Comparing `contact-energy-nz-0.1.4684335331.tar` & `contact-energy-nz-0.1.4684953769.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:55:55.793287 contact-energy-nz-0.1.4684335331/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 00:55:55.793287 contact-energy-nz-0.1.4684335331/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:55:55.793287 contact-energy-nz-0.1.4684335331/contact_energy_nz/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz/contact_energy_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz/usage_datum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:55:55.793287 contact-energy-nz-0.1.4684335331/contact_energy_nz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 00:55:55.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 00:55:55.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:55:55.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 00:55:55.000000 contact-energy-nz-0.1.4684335331/contact_energy_nz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 00:55:55.793287 contact-energy-nz-0.1.4684335331/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:55:55.793287 contact-energy-nz-0.1.4684335331/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 00:55:41.000000 contact-energy-nz-0.1.4684335331/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:42:51.557251 contact-energy-nz-0.1.4684953769/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 02:42:51.553251 contact-energy-nz-0.1.4684953769/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:42:51.553251 contact-energy-nz-0.1.4684953769/contact_energy_nz/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz/contact_energy_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz/usage_datum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:42:51.553251 contact-energy-nz-0.1.4684953769/contact_energy_nz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 02:42:51.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 02:42:51.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 02:42:51.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 02:42:51.000000 contact-energy-nz-0.1.4684953769/contact_energy_nz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 02:42:51.557251 contact-energy-nz-0.1.4684953769/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 02:42:51.553251 contact-energy-nz-0.1.4684953769/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 02:42:36.000000 contact-energy-nz-0.1.4684953769/tests/test_integration.py
```

### Comparing `contact-energy-nz-0.1.4684335331/LICENSE` & `contact-energy-nz-0.1.4684953769/LICENSE`

 * *Files identical despite different names*

### Comparing `contact-energy-nz-0.1.4684335331/contact_energy_nz/contact_energy_api.py` & `contact-energy-nz-0.1.4684953769/contact_energy_nz/contact_energy_api.py`

 * *Files identical despite different names*

### Comparing `contact-energy-nz-0.1.4684335331/contact_energy_nz/usage_datum.py` & `contact-energy-nz-0.1.4684953769/contact_energy_nz/usage_datum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import datetime
 
 from attr import dataclass
 
-
-@dataclass
 class UsageDatum:
     """Helper class for data manipulation"""
 
     def __init__(self, json_item) -> None:
         """Construct class out of json dictionary"""
         self.currency = json_item["currency"]
         self.date = datetime.datetime.strptime(
```

### Comparing `contact-energy-nz-0.1.4684335331/pyproject.toml` & `contact-energy-nz-0.1.4684953769/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "contact-energy-nz"
-version = "0.1.4684335331"
+version = "0.1.4684953769"
 description = "API Connector to fetch usage data from Contact Energy NZ utilities provider"
 authors = [
     {name = "Tkhadimullin", email = "hello@wiseowls.co.nz"}
 ]
 license = {text = "MIT"}
 
 [tool.poetry.dependencies]
```

### Comparing `contact-energy-nz-0.1.4684335331/tests/test_integration.py` & `contact-energy-nz-0.1.4684953769/tests/test_integration.py`

 * *Files identical despite different names*

