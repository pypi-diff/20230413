# Comparing `tmp/dbldatagen-0.3.4.tar.gz` & `tmp/dbldatagen-0.3.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbldatagen-0.3.4.tar", last modified: Sun Apr  9 00:46:09 2023, max compression
+gzip compressed data, was "dbldatagen-0.3.4.post1.tar", last modified: Thu Apr 13 17:05:10 2023, max compression
```

## Comparing `dbldatagen-0.3.4.tar` & `dbldatagen-0.3.4.post1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/dbldatagen/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    59230 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/column_generation_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/column_spec_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57532 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/datagen_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/daterange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/dbldatagen/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/data_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/exponential_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/function_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/nrange.py
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/spark_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/text_generator_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/text_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/dbldatagen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/dbldatagen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 00:46:09.000000 dbldatagen-0.3.4/dbldatagen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 00:46:09.159940 dbldatagen-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-09 00:44:32.000000 dbldatagen-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.218521 dbldatagen-0.3.4.post1/dbldatagen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59147 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/column_generation_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/column_spec_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57532 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/datagen_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/daterange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/dbldatagen/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/data_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/exponential_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/function_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/nrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/spark_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/text_generator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/text_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/dbldatagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/setup.py
```

### Comparing `dbldatagen-0.3.4/CHANGELOG.md` & `dbldatagen-0.3.4.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/CONTRIBUTING.md` & `dbldatagen-0.3.4.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/LICENSE` & `dbldatagen-0.3.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/PKG-INFO` & `dbldatagen-0.3.4.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.4
+Version: 0.3.4.post1
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post1/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4/PULL_REQUEST_TEMPLATE.md` & `dbldatagen-0.3.4.post1/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/README.md` & `dbldatagen-0.3.4.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post1/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4/dbldatagen/__init__.py` & `dbldatagen-0.3.4.post1/dbldatagen/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/_version.py` & `dbldatagen-0.3.4.post1/dbldatagen/_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 
     :param version: version string to parse for version information
 
     Layout of version string must be compatible with `bump` package"""
     r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+){0,1}(?P<release>\D*)(?P<build>\d*)')
     major, minor, patch, release, build = r.match(version).groups()
     version_info = VersionInfo(major, minor, patch, release, build)
-    logging.info("Version : %s", version_info)
+    logger = logging.getLogger(__name__)
+    logger.info("Version : %s", version_info)
     return version_info
 
 
-__version__ = "0.3.4"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "0.3.4post1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
 
 
 def _get_spark_version(sparkVersion):
     try:
         r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>.*)')
         major, minor, patch, release = r.match(sparkVersion).groups()
```

### Comparing `dbldatagen-0.3.4/dbldatagen/column_generation_spec.py` & `dbldatagen-0.3.4.post1/dbldatagen/column_generation_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         'short': 65536
     }
 
     # set up logging
 
     # restrict spurious messages from java gateway
     logging.getLogger("py4j").setLevel(logging.WARNING)
-    logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.NOTSET)
 
     def __init__(self, name, colType=None, minValue=0, maxValue=None, step=1, prefix='', random=False,
                  distribution=None, baseColumn=None, randomSeed=None, randomSeedMethod=None,
                  implicit=False, omit=False, nullable=True, debug=False, verbose=False,
                  seedColumnName=DEFAULT_SEED_COLUMN,
                  **kwargs):
```

### Comparing `dbldatagen-0.3.4/dbldatagen/column_spec_options.py` & `dbldatagen-0.3.4.post1/dbldatagen/column_spec_options.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/data_analyzer.py` & `dbldatagen-0.3.4.post1/dbldatagen/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/data_generator.py` & `dbldatagen-0.3.4.post1/dbldatagen/data_generator.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/datagen_constants.py` & `dbldatagen-0.3.4.post1/dbldatagen/datagen_constants.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/datarange.py` & `dbldatagen-0.3.4.post1/dbldatagen/datarange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/daterange.py` & `dbldatagen-0.3.4.post1/dbldatagen/daterange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/distributions/__init__.py` & `dbldatagen-0.3.4.post1/dbldatagen/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/distributions/beta.py` & `dbldatagen-0.3.4.post1/dbldatagen/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/distributions/data_distribution.py` & `dbldatagen-0.3.4.post1/dbldatagen/distributions/data_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/distributions/exponential_distribution.py` & `dbldatagen-0.3.4.post1/dbldatagen/distributions/exponential_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/distributions/gamma.py` & `dbldatagen-0.3.4.post1/dbldatagen/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/distributions/normal_distribution.py` & `dbldatagen-0.3.4.post1/dbldatagen/distributions/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/function_builder.py` & `dbldatagen-0.3.4.post1/dbldatagen/function_builder.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/nrange.py` & `dbldatagen-0.3.4.post1/dbldatagen/nrange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/schema_parser.py` & `dbldatagen-0.3.4.post1/dbldatagen/schema_parser.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/spark_singleton.py` & `dbldatagen-0.3.4.post1/dbldatagen/spark_singleton.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/text_generator_plugins.py` & `dbldatagen-0.3.4.post1/dbldatagen/text_generator_plugins.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/text_generators.py` & `dbldatagen-0.3.4.post1/dbldatagen/text_generators.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen/utils.py` & `dbldatagen-0.3.4.post1/dbldatagen/utils.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/dbldatagen.egg-info/PKG-INFO` & `dbldatagen-0.3.4.post1/dbldatagen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.4
+Version: 0.3.4.post1
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post1/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4/dbldatagen.egg-info/SOURCES.txt` & `dbldatagen-0.3.4.post1/dbldatagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4/setup.py` & `dbldatagen-0.3.4.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     The Databricks Labs Data Generator can generate realistic synthetic data sets at scale for testing, 
     benchmarking, environment validation and other purposes.
     """
 
 setuptools.setup(
     name="dbldatagen",
-    version="0.3.4",
+    version="0.3.4post1",
     author="Ronan Stokes, Databricks",
     description="Databricks Labs -  PySpark Synthetic Data Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/databrickslabs/data-generator",
     project_urls={
         "Databricks Labs": "https://www.databricks.com/learn/labs",
```

