# Comparing `tmp/whylabs_toolkit-0.0.6.tar.gz` & `tmp/whylabs_toolkit-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs_toolkit-0.0.6.tar", max compression
+gzip compressed data, was "whylabs_toolkit-0.0.6.dev0.tar", max compression
```

## Comparing `whylabs_toolkit-0.0.6.tar` & `whylabs_toolkit-0.0.6.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/LICENSE
--rw-r--r--   0        0        0     1409 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/README.md
--rw-r--r--   0        0        0      850 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/cli/__init__.py
--rw-r--r--   0        0        0      559 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/container/config_types.py
--rw-r--r--   0        0        0        0 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/__init__.py
--rw-r--r--   0        0        0      362 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/client.py
--rw-r--r--   0        0        0     1600 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/config.py
--rw-r--r--   0        0        0      960 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/dataset_profiles.py
--rw-r--r--   0        0        0     1458 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/models.py
--rw-r--r--   0        0        0     3398 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/monitor_helpers.py
--rw-r--r--   0        0        0     6066 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/schema.py
--rw-r--r--   0        0        0      922 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/utils.py
--rw-r--r--   0        0        0      121 2023-04-13 19:59:51.933188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/__init__.py
--rw-r--r--   0        0        0      178 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/__init__.py
--rw-r--r--   0        0        0      557 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/credentials.py
--rw-r--r--   0        0        0     5777 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/manager.py
--rw-r--r--   0        0        0     9551 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/monitor_setup.py
--rw-r--r--   0        0        0     1500 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/__init__.py
--rw-r--r--   0        0        0      841 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/__init__.py
--rw-r--r--   0        0        0    12589 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/algorithms.py
--rw-r--r--   0        0        0     4597 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/analyzer.py
--rw-r--r--   0        0        0     3242 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/baseline.py
--rw-r--r--   0        0        0     2071 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/targets.py
--rw-r--r--   0        0        0     4115 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/column_schema.py
--rw-r--r--   0        0        0     3363 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/commons.py
--rw-r--r--   0        0        0     2497 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/document.py
--rw-r--r--   0        0        0     9201 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/monitor.py
--rw-r--r--   0        0        0      574 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/segments.py
--rw-r--r--   0        0        0      961 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/utils.py
--rw-r--r--   0        0        0    75902 2023-04-13 19:59:51.937188 whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/schema/schema.json
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.6/setup.py
--rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 22:21:38.271279 whylabs_toolkit-0.0.6.dev0/LICENSE
+-rw-r--r--   0        0        0     1409 2023-04-10 22:21:38.271279 whylabs_toolkit-0.0.6.dev0/README.md
+-rw-r--r--   0        0        0      855 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/cli/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/container/config_types.py
+-rw-r--r--   0        0        0        0 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/client.py
+-rw-r--r--   0        0        0     1600 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/config.py
+-rw-r--r--   0        0        0      960 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/dataset_profiles.py
+-rw-r--r--   0        0        0     1458 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/models.py
+-rw-r--r--   0        0        0     3398 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/monitor_helpers.py
+-rw-r--r--   0        0        0     6066 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/schema.py
+-rw-r--r--   0        0        0      922 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/utils.py
+-rw-r--r--   0        0        0      121 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/__init__.py
+-rw-r--r--   0        0        0      557 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/credentials.py
+-rw-r--r--   0        0        0     5777 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/manager.py
+-rw-r--r--   0        0        0     9551 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/monitor_setup.py
+-rw-r--r--   0        0        0     1500 2023-04-10 22:21:38.275279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/__init__.py
+-rw-r--r--   0        0        0      841 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/__init__.py
+-rw-r--r--   0        0        0    12589 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/algorithms.py
+-rw-r--r--   0        0        0     4597 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3242 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/baseline.py
+-rw-r--r--   0        0        0     2071 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/targets.py
+-rw-r--r--   0        0        0     4115 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/column_schema.py
+-rw-r--r--   0        0        0     3363 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/commons.py
+-rw-r--r--   0        0        0     2497 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/document.py
+-rw-r--r--   0        0        0     9201 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/monitor.py
+-rw-r--r--   0        0        0      574 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/segments.py
+-rw-r--r--   0        0        0      961 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/utils.py
+-rw-r--r--   0        0        0    75902 2023-04-10 22:21:38.279279 whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/schema/schema.json
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.6.dev0/setup.py
+-rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 whylabs_toolkit-0.0.6.dev0/PKG-INFO
```

### Comparing `whylabs_toolkit-0.0.6/LICENSE` & `whylabs_toolkit-0.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/README.md` & `whylabs_toolkit-0.0.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/pyproject.toml` & `whylabs_toolkit-0.0.6.dev0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylabs-toolkit"
-version = "0.0.6"
+version = "0.0.6-dev0"
 description = "Whylabs CLI and Helpers package."
 authors = ["Anthony Naddeo <anthony.naddeo@gmail.com>", "Murilo Mendonca <murilommen@gmail.com>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 packages = [{include = "whylabs_toolkit/**/*.py"}]
 include = ["whylabs_toolkit/monitor/schema/schema.json"]
```

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/container/config_types.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/container/config_types.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/config.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/config.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/dataset_profiles.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/dataset_profiles.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/models.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/models.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/monitor_helpers.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/monitor_helpers.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/schema.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/helpers/utils.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/credentials.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/credentials.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/manager.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/manager.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/manager/monitor_setup.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/manager/monitor_setup.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/__init__.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/__init__.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/algorithms.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/algorithms.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/analyzer.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/baseline.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/baseline.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/analyzer/targets.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/analyzer/targets.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/column_schema.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/commons.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/commons.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/document.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/document.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/monitor.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/monitor.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/segments.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/segments.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/models/utils.py` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/models/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/whylabs_toolkit/monitor/schema/schema.json` & `whylabs_toolkit-0.0.6.dev0/whylabs_toolkit/monitor/schema/schema.json`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.0.6/setup.py` & `whylabs_toolkit-0.0.6.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pytz>=2022.7.1,<2023.0.0',
  'types-pytz>=2022.7.1.0,<2023.0.0.0',
  'whylabs-client>=0.4.4,<0.5.0',
  'whylogs>=1.1.26,<2.0.0']
 
 setup_kwargs = {
     'name': 'whylabs-toolkit',
-    'version': '0.0.6',
+    'version': '0.0.6.dev0',
     'description': 'Whylabs CLI and Helpers package.',
     'long_description': "# WhyLabs Toolkit\n\nThe WhyLabs Toolkit package contains helper methods to help users interact with our internal APIs. Users will benefit from using it if they want to abstract some of WhyLabs' internal logic and also automate recurring API calls.\n\n\n## Basic usage\nTo start using the `whylabs_toolkit` package, install it from PyPI with:\n```bash\npip install whylabs_toolkit\n``` \n\n## Packages\n\nThe available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.\n\n| Package             | Usage                |\n|---------------------|----------------------|\n| [Monitor Manager](/whylabs_toolkit/monitor/manager/README.md) | Author and modify existing WhyLabs monitor with Python |\n| [WhyLabs Helpers](/whylabs_toolkit/helpers/README.md) | Interact with and modify your Datasets and ML Models specs in WhyLabs. |\n\n## Development\n\nTo start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:\n\n```bash\nmake setup && poetry shell\n```\n\n## Get in touch\nIf you want to learn more how you can benefit from this package or if there is anything missing, please [contact our support](https://whylabs.ai/contact-us), we'll be more than happy to help you!",
     'author': 'Anthony Naddeo',
     'author_email': 'anthony.naddeo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `whylabs_toolkit-0.0.6/PKG-INFO` & `whylabs_toolkit-0.0.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-toolkit
-Version: 0.0.6
+Version: 0.0.6.dev0
 Summary: Whylabs CLI and Helpers package.
 License: Apache-2.0 license
 Author: Anthony Naddeo
 Author-email: anthony.naddeo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

