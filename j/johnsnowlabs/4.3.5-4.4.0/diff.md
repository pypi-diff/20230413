# Comparing `tmp/johnsnowlabs-4.3.5.tar.gz` & `tmp/johnsnowlabs-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-4.3.5.tar", last modified: Sat Mar 25 15:25:32 2023, max compression
+gzip compressed data, was "johnsnowlabs-4.4.0.tar", last modified: Thu Apr 13 00:49:50 2023, max compression
```

## Comparing `johnsnowlabs-4.3.5.tar` & `johnsnowlabs-4.4.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1339 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      389 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.702685 johnsnowlabs-4.3.5/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1001 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.702685 johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.702685 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.702685 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-23 15:02:44.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-23 15:02:44.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3188 2023-03-23 15:02:44.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4082 2023-03-19 17:22:02.000000 johnsnowlabs-4.3.5/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4015 2023-03-19 17:22:02.000000 johnsnowlabs-4.3.5/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4012 2023-03-23 15:02:44.000000 johnsnowlabs-4.3.5/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-23 15:02:44.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/py_models/url_dependency.py
--rw-r--r--   0 ckl       (1000) ckl       (1000)     2201 2023-03-25 15:22:36.000000 johnsnowlabs-4.3.5/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1687 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1290 2023-03-19 17:22:02.000000 johnsnowlabs-4.3.5/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.3.5/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-03-25 15:25:32.702685 johnsnowlabs-4.3.5/johnsnowlabs.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1339 2023-03-25 15:25:32.000000 johnsnowlabs-4.3.5/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2458 2023-03-25 15:25:32.000000 johnsnowlabs-4.3.5/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-03-25 15:25:32.000000 johnsnowlabs-4.3.5/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-03-25 15:25:32.000000 johnsnowlabs-4.3.5/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-03-25 15:25:32.000000 johnsnowlabs-4.3.5/johnsnowlabs.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-03-25 15:25:32.706685 johnsnowlabs-4.3.5/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2063 2023-03-21 12:20:46.000000 johnsnowlabs-4.3.5/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.799275 johnsnowlabs-4.4.0/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.0/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-13 00:49:50.799275 johnsnowlabs-4.4.0/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs-4.4.0/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.791275 johnsnowlabs-4.4.0/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1001 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-04-13 00:38:10.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3188 2023-04-11 22:53:57.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8828 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4419 2023-04-13 00:39:20.000000 johnsnowlabs-4.4.0/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4348 2023-04-13 00:40:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4315 2023-04-13 00:40:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-11 22:58:52.000000 johnsnowlabs-4.4.0/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2079 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-04-11 23:12:44.000000 johnsnowlabs-4.4.0/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1687 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8019 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.799275 johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1290 2023-03-19 17:22:02.000000 johnsnowlabs-4.4.0/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs-4.4.0/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-04-13 00:49:50.795275 johnsnowlabs-4.4.0/johnsnowlabs.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9278 2023-04-13 00:49:50.000000 johnsnowlabs-4.4.0/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2466 2023-04-13 00:49:50.000000 johnsnowlabs-4.4.0/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-04-13 00:49:50.000000 johnsnowlabs-4.4.0/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      126 2023-04-13 00:49:50.000000 johnsnowlabs-4.4.0/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-04-13 00:49:50.000000 johnsnowlabs-4.4.0/johnsnowlabs.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-04-13 00:49:50.799275 johnsnowlabs-4.4.0/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2063 2023-03-31 10:11:32.000000 johnsnowlabs-4.4.0/setup.py
```

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/__init__.py` & `johnsnowlabs-4.4.0/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-4.4.0/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,23 +51,23 @@
         }
     }
 
     compatible_spark_to_py_map = {
         SparkVersion.spark3xx: {
             # TODO HARDCODE HASH!!! OR grap from enum or somwhere comfy. Maybe configs/settings file?
             PyInstallTypes.wheel: UrlDependency(
-                url="https://files.pythonhosted.org/packages/b4/0a/4b8762712ffb333de51fbc0dc77ab4bde5c284e8784ba0ecec9e017b999f/spark_nlp-{lib_version}-py2.py3-none-any.whl",
+                url="https://files.pythonhosted.org/packages/e2/80/22d2fca3662ecb658ee43c8b4cad5bbfd899444ba004daf87298f1154d8e/spark_nlp-{lib_version}-py2.py3-none-any.whl",
                 dependency_type=PyInstallTypes.wheel,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
             PyInstallTypes.tar: UrlDependency(
-                url="https://files.pythonhosted.org/packages/40/a7/6d450edede7a7f54b3a5cd78fe3d521bad33ada0f69de0b542c1ab13f3bd/spark-nlp-{lib_version}.tar.gz",
+                url="https://files.pythonhosted.org/packages/2e/aa/19e34297e3cc22a0f361c22cc366418158612bca8f5b9e3959c1f066f747/spark-nlp-{lib_version}.tar.gz",
                 dependency_type=PyInstallTypes.tar,
                 spark_version=SparkVersion.spark3xx,
                 product_name=product_name,
                 file_name=product_name.name,
                 dependency_version=lib_version,
             ),
         }
```

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-4.4.0/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/finance.py` & `johnsnowlabs-4.4.0/johnsnowlabs/finance.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
 
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.base import FeaturesAssembler
+        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
+            WindowedSentenceModel,
+        )
+        from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.finance import (
-
             GenericClassifierModel,
             FinanceNerQuestionGenerator as NerQuestionGenerator,
             FinanceDocumentHashCoder as DocumentHashCoder,
             FinanceBertForTokenClassification as BertForTokenClassification,
             FinanceDocumentMLClassifierModel as DocumentMLClassifierModel,
             FinanceDocumentMLClassifierApproach as DocumentMLClassifierApproach,
             DocMapperApproach,
@@ -32,14 +35,17 @@
             AssertionDLModel,
             RelationExtractionDLModel,
             ZeroShotRelationExtractionModel,
             ChunkMapperApproach,
             SentenceEntityResolverApproach,
             AssertionDLApproach,
             ZeroShotNerModel,
+            FinanceQuestionAnswering as QuestionAnswering,
+            FinanceTextGenerator as TextGenerator,
+            FinanceSummarizer as Summarizer,
         )
 
         # These are licensed annos shared across all libs
         from sparknlp_jsl.annotator import (
             GenericSVMClassifierApproach,
             GenericSVMClassifierModel,
             GenericLogRegClassifierApproach,
@@ -85,15 +91,15 @@
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             Resolution2Chunk,
             ResolverMerger,
         )
 
         from sparknlp_jsl.modelTracer import ModelTracer
-        from sparknlp_jsl import (training_log_parser, Deid)
+        from sparknlp_jsl import training_log_parser, Deid
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
             NerDLMetrics,
             NerDLEvaluation,
             SymSpellEvaluation,
             POSEvaluation,
```

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/legal.py` & `johnsnowlabs-4.4.0/johnsnowlabs/legal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import traceback
 
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.utils.print_messages import log_broken_lib
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
+        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
+            WindowedSentenceModel,
+        )
+        from sparknlp_jsl.training_log_parser import ner_log_parser
+
         from sparknlp_jsl.base import FeaturesAssembler
 
         from sparknlp_jsl.legal import (
             LegalDocumentHashCoder as DocumentHashCoder,
             LegalNerQuestionGenerator as NerQuestionGenerator,
             LegalBertForSequenceClassification as BertForSequenceClassification,
             LegalDocumentMLClassifierModel as DocumentMLClassifierModel,
@@ -26,14 +31,17 @@
             AssertionDLModel,
             RelationExtractionDLModel,
             ZeroShotRelationExtractionModel,
             ChunkMapperApproach,
             SentenceEntityResolverApproach,
             AssertionDLApproach,
             ZeroShotNerModel,
+            LegalQuestionAnswering as QuestionAnswering,
+            LegalTextGenerator as TextGenerator,
+            LegalSummarizer as Summarizer,
         )
 
         # These are licensed annos shared across all libs
         from sparknlp_jsl.annotator import (
             GenericSVMClassifierApproach,
             GenericSVMClassifierModel,
             GenericLogRegClassifierApproach,
@@ -82,15 +90,15 @@
             # Resolution2Chunk,
             ResolverMerger,
         )
         from sparknlp_jsl.modelTracer import ModelTracer
 
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
 
-        from sparknlp_jsl import (training_log_parser, Deid)
+        from sparknlp_jsl import training_log_parser, Deid
 
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
             NerDLMetrics,
             NerDLEvaluation,
             SymSpellEvaluation,
```

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/medical.py` & `johnsnowlabs-4.4.0/johnsnowlabs/medical.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import traceback
 
+
 from johnsnowlabs.abstract_base.lib_resolver import try_import_lib
 from johnsnowlabs.auto_install.softwares import Software
 from johnsnowlabs.utils.print_messages import log_outdated_lib, log_broken_lib
 
 warning_logged = False
 
 try:
     if try_import_lib("sparknlp_jsl") and try_import_lib("sparknlp"):
         # Pretrained
+        from sparknlp_jsl.annotator.windowed.windowed_sentence import (
+            WindowedSentenceModel,
+        )
         from sparknlp_jsl.annotator import (
             GenericSVMClassifierApproach,
             GenericSVMClassifierModel,
             GenericLogRegClassifierApproach,
             GenericClassifierModel,
             AssertionLogRegModel,
             AssertionDLModel,
@@ -63,30 +67,33 @@
             DocMapperModel,
             DocMapperApproach,
             NameChunkObfuscatorApproach,
             NameChunkObfuscator,
             DocumentMLClassifierApproach,
             DocumentMLClassifierModel,
             Resolution2Chunk,
-            MedicalQuestionAnswering,
         )
         from sparknlp_jsl.structured_deidentification import StructuredDeidentification
         from sparknlp_jsl.modelTracer import ModelTracer
         from sparknlp_jsl import training_log_parser, Deid
+        from sparknlp_jsl.training_log_parser import ner_log_parser
 
         from sparknlp_jsl.base import FeaturesAssembler
 
         from sparknlp_jsl.annotator.resolution.resolver_merger import ResolverMerger
 
         from sparknlp_jsl.annotator import (
             MedicalDistilBertForSequenceClassification as DistilBertForSequenceClassification,
             MedicalBertForSequenceClassification as BertForSequenceClassification,
             MedicalBertForTokenClassifier as BertForTokenClassification,
             MedicalNerModel as NerModel,
             MedicalNerApproach as NerApproach,
+            MedicalQuestionAnswering as QuestionAnswering,
+            MedicalTextGenerator as TextGenerator,
+            MedicalSummarizer as Summarizer,
         )
         from sparknlp_jsl.compatibility import Compatibility
         from sparknlp_jsl.pretrained import InternalResourceDownloader
         from sparknlp_jsl.eval import (
             NerDLMetrics,
             NerDLEvaluation,
             SymSpellEvaluation,
```

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/nlp.py` & `johnsnowlabs-4.4.0/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-4.4.0/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-4.4.0/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-4.4.0/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-4.4.0/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/settings.py` & `johnsnowlabs-4.4.0/johnsnowlabs/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.3.5"
-raw_version_nlp = "4.3.2"
+raw_version_jsl_lib = "4.4.0"
+raw_version_nlp = "4.4.0"
 raw_version_nlu = "4.2.0"
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
-raw_version_medical = "4.3.2"
-raw_version_secret_medical = "4.3.2"
+raw_version_medical = "4.4.0"
+raw_version_secret_medical = "4.4.0"
 
 raw_version_secret_ocr = "4.3.3"
 raw_version_ocr = "4.3.3"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 
 json_indent = 4
```

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/enums.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/functional.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-4.4.0/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs/visual.py` & `johnsnowlabs-4.4.0/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-4.3.5/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-4.4.0/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 johnsnowlabs/__init__.py
 johnsnowlabs/finance.py
 johnsnowlabs/lab.py
 johnsnowlabs/legal.py
 johnsnowlabs/medical.py
```

### Comparing `johnsnowlabs-4.3.5/setup.py` & `johnsnowlabs-4.4.0/setup.py`

 * *Files identical despite different names*
