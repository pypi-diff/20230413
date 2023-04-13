# Comparing `tmp/webdriver_manager-3.8.5.tar.gz` & `tmp/webdriver_manager-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_manager-3.8.5.tar", last modified: Wed Nov 16 16:55:01 2022, max compression
+gzip compressed data, was "webdriver_manager-3.8.6.tar", last modified: Thu Apr 13 20:11:36 2023, max compression
```

## Comparing `webdriver_manager-3.8.5.tar` & `webdriver_manager-3.8.6.tar`

### file list

```diff
@@ -1,46 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/
--rw-r--r--   0 runner    (1001) docker     (121)    11328 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10605 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9589 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-16 16:55:00.998548 webdriver_manager-3.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.990548 webdriver_manager-3.8.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/tests/xdist/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/tests/xdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/tests/xdist/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/tests/xdist/test_cuncurent_1.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/tests/xdist/test_cuncurent_2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/tests_negative/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/tests_negative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/tests_negative/test_browsers_not_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/webdriver_manager/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/webdriver_manager/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/archive.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/driver.py
--rw-r--r--   0 runner    (1001) docker     (121)     4742 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/driver_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/http.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    12469 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/webdriver_manager/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/drivers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/drivers/edge.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/drivers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/drivers/ie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/drivers/opera.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/microsoft.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1743 2022-11-16 16:54:41.000000 webdriver_manager-3.8.5/webdriver_manager/opera.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:55:00.994548 webdriver_manager-3.8.5/webdriver_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10605 2022-11-16 16:55:00.000000 webdriver_manager-3.8.5/webdriver_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-11-16 16:55:00.000000 webdriver_manager-3.8.5/webdriver_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 16:55:00.000000 webdriver_manager-3.8.5/webdriver_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 16:55:00.000000 webdriver_manager-3.8.5/webdriver_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-16 16:55:00.000000 webdriver_manager-3.8.5/webdriver_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 20:11:36.439015 webdriver_manager-3.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_brave_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_chromium_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_custom_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_edge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_firefox_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_ie_driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_opera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_silent_global_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/tests_negative/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_negative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_negative/test_browsers_not_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/tests_xdist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/test_cuncurent_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/tests_xdist/test_cuncurent_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/driver_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/ie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/drivers/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/microsoft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1743 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:15.000000 webdriver_manager-3.8.6/webdriver_manager/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:11:36.435014 webdriver_manager-3.8.6/webdriver_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 20:11:36.000000 webdriver_manager-3.8.6/webdriver_manager.egg-info/top_level.txt
```

### Comparing `webdriver_manager-3.8.5/LICENSE` & `webdriver_manager-3.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/PKG-INFO` & `webdriver_manager-3.8.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: webdriver_manager
-Version: 3.8.5
+Version: 3.8.6
 Summary: Library provides the way to automatically manage drivers for different browsers
 Home-page: https://github.com/SergeyPirogov/webdriver_manager
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -25,30 +26,26 @@
 # Webdriver Manager for Python
 
 [![Tests](https://github.com/SergeyPirogov/webdriver_manager/actions/workflows/test.yml/badge.svg)](https://github.com/SergeyPirogov/webdriver_manager/actions/workflows/test.yml)
 [![PyPI](https://img.shields.io/pypi/v/webdriver_manager.svg)](https://pypi.org/project/webdriver-manager)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/webdriver_manager.svg)](https://pypi.org/project/webdriver-manager/)
 [![codecov](https://codecov.io/gh/SergeyPirogov/webdriver_manager/branch/master/graph/badge.svg)](https://codecov.io/gh/SergeyPirogov/webdriver_manager)
 
-[Patreon](https://www.patreon.com/automation_remarks)
+## Support the library on [Patreon](https://www.patreon.com/automation_remarks)
 
 The main idea is to simplify management of binary drivers for different browsers.
 
 For now support:
 
 - [ChromeDriver](#use-with-chrome)
-
+- [EdgeChromiumDriver](#use-with-edge)
 - [GeckoDriver](#use-with-firefox)
-
 - [IEDriver](#use-with-ie)
-
 - [OperaDriver](#use-with-opera)
 
-- [EdgeChromiumDriver](#use-with-edge)
-
 Compatible with Selenium 4.x and below.
 
 Before:
 You need to download the chromedriver binary, unzip it somewhere on your PC and set the path to this driver like this:
 
 ```python
 from selenium import webdriver
@@ -121,14 +118,33 @@
 from selenium.webdriver.chrome.service import Service as BraveService
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 driver = webdriver.Chrome(service=BraveService(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
 ```
 
+
+#### Use with Edge
+
+```python
+# selenium 3
+from selenium import webdriver
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+```
+```python
+# selenium 4
+from selenium import webdriver
+from selenium.webdriver.edge.service import Service as EdgeService
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+```
+
 #### Use with Firefox
 
 ```python
 # selenium 3
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 
@@ -157,53 +173,50 @@
 from selenium import webdriver
 from selenium.webdriver.ie.service import Service as IEService
 from webdriver_manager.microsoft import IEDriverManager
 
 driver = webdriver.Ie(service=IEService(IEDriverManager().install()))
 ```
 
-#### Use with Edge
+
+#### Use with Opera
 
 ```python
 # selenium 3
 from selenium import webdriver
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
+
+driver = webdriver.Remote(webdriver_service.service_url, webdriver.DesiredCapabilities.OPERA)
 ```
 ```python
 # selenium 4
 from selenium import webdriver
-from selenium.webdriver.edge.service import Service as EdgeService
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
-
-driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
-```
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-#### Use with Opera
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
 
-```python
-# selenium 3 & 4
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
+options = webdriver.ChromeOptions()
+options.add_experimental_option('w3c', True)
 
-driver = webdriver.Opera(executable_path=OperaDriverManager().install())
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 If the Opera browser is installed in a location other than `C:/Program Files` or `C:/Program Files (x86)` on windows
 and `/usr/bin/opera` for all unix variants and mac, then use the below code,
 
 ```python
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
-
 options = webdriver.ChromeOptions()
-options.add_argument('allow-elevated-browser')
-options.binary_location = "C:\\Users\\USERNAME\\FOLDERLOCATION\\Opera\\VERSION\\opera.exe"
-driver = webdriver.Opera(executable_path=OperaDriverManager().install(), options=options)
+options.binary_location = "path/to/opera.exe"
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 #### Get browser version from path
 
 To get the version of the browser from the executable of the browser itself:
 
 ```python
@@ -243,14 +256,23 @@
 ```python
 import logging
 import os
 
 os.environ['WDM_LOG'] = str(logging.NOTSET)
 ```
 
+### `WDM_PROGRESS_BAR`
+Turn off the progress bar which is displayed on downloads:
+
+```python
+import os
+
+os.environ['WDM_PROGRESS_BAR'] = str(0)
+```
+
 ### `WDM_LOCAL`
 By default, all driver binaries are saved to user.home/.wdm folder. You can override this setting and save binaries to project.root/.wdm.
 
 ```python
 import os
 
 os.environ['WDM_LOCAL'] = '1'
```

### Comparing `webdriver_manager-3.8.5/README.md` & `webdriver_manager-3.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # Webdriver Manager for Python
 
 [![Tests](https://github.com/SergeyPirogov/webdriver_manager/actions/workflows/test.yml/badge.svg)](https://github.com/SergeyPirogov/webdriver_manager/actions/workflows/test.yml)
 [![PyPI](https://img.shields.io/pypi/v/webdriver_manager.svg)](https://pypi.org/project/webdriver-manager)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/webdriver_manager.svg)](https://pypi.org/project/webdriver-manager/)
 [![codecov](https://codecov.io/gh/SergeyPirogov/webdriver_manager/branch/master/graph/badge.svg)](https://codecov.io/gh/SergeyPirogov/webdriver_manager)
 
-[Patreon](https://www.patreon.com/automation_remarks)
+## Support the library on [Patreon](https://www.patreon.com/automation_remarks)
 
 The main idea is to simplify management of binary drivers for different browsers.
 
 For now support:
 
 - [ChromeDriver](#use-with-chrome)
-
+- [EdgeChromiumDriver](#use-with-edge)
 - [GeckoDriver](#use-with-firefox)
-
 - [IEDriver](#use-with-ie)
-
 - [OperaDriver](#use-with-opera)
 
-- [EdgeChromiumDriver](#use-with-edge)
-
 Compatible with Selenium 4.x and below.
 
 Before:
 You need to download the chromedriver binary, unzip it somewhere on your PC and set the path to this driver like this:
 
 ```python
 from selenium import webdriver
@@ -97,14 +93,33 @@
 from selenium.webdriver.chrome.service import Service as BraveService
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 driver = webdriver.Chrome(service=BraveService(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
 ```
 
+
+#### Use with Edge
+
+```python
+# selenium 3
+from selenium import webdriver
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+```
+```python
+# selenium 4
+from selenium import webdriver
+from selenium.webdriver.edge.service import Service as EdgeService
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+```
+
 #### Use with Firefox
 
 ```python
 # selenium 3
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 
@@ -133,53 +148,50 @@
 from selenium import webdriver
 from selenium.webdriver.ie.service import Service as IEService
 from webdriver_manager.microsoft import IEDriverManager
 
 driver = webdriver.Ie(service=IEService(IEDriverManager().install()))
 ```
 
-#### Use with Edge
+
+#### Use with Opera
 
 ```python
 # selenium 3
 from selenium import webdriver
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
+
+driver = webdriver.Remote(webdriver_service.service_url, webdriver.DesiredCapabilities.OPERA)
 ```
 ```python
 # selenium 4
 from selenium import webdriver
-from selenium.webdriver.edge.service import Service as EdgeService
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
-
-driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
-```
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-#### Use with Opera
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
 
-```python
-# selenium 3 & 4
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
+options = webdriver.ChromeOptions()
+options.add_experimental_option('w3c', True)
 
-driver = webdriver.Opera(executable_path=OperaDriverManager().install())
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 If the Opera browser is installed in a location other than `C:/Program Files` or `C:/Program Files (x86)` on windows
 and `/usr/bin/opera` for all unix variants and mac, then use the below code,
 
 ```python
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
-
 options = webdriver.ChromeOptions()
-options.add_argument('allow-elevated-browser')
-options.binary_location = "C:\\Users\\USERNAME\\FOLDERLOCATION\\Opera\\VERSION\\opera.exe"
-driver = webdriver.Opera(executable_path=OperaDriverManager().install(), options=options)
+options.binary_location = "path/to/opera.exe"
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 #### Get browser version from path
 
 To get the version of the browser from the executable of the browser itself:
 
 ```python
@@ -219,14 +231,23 @@
 ```python
 import logging
 import os
 
 os.environ['WDM_LOG'] = str(logging.NOTSET)
 ```
 
+### `WDM_PROGRESS_BAR`
+Turn off the progress bar which is displayed on downloads:
+
+```python
+import os
+
+os.environ['WDM_PROGRESS_BAR'] = str(0)
+```
+
 ### `WDM_LOCAL`
 By default, all driver binaries are saved to user.home/.wdm folder. You can override this setting and save binaries to project.root/.wdm.
 
 ```python
 import os
 
 os.environ['WDM_LOCAL'] = '1'
```

### Comparing `webdriver_manager-3.8.5/setup.py` & `webdriver_manager-3.8.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,35 +19,39 @@
 setuptools.setup(
     name='webdriver_manager',
     python_requires=">=3.7",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=['tests']),
     include_package_data=True,
-    version='3.8.5',
+    version='3.8.6',
     description='Library provides the way to automatically manage drivers for different browsers',
     author='Sergey Pirogov',
     author_email='automationremarks@gmail.com',
     url='https://github.com/SergeyPirogov/webdriver_manager',
     keywords=['testing', 'selenium', 'driver', 'test automation'],
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: '
         'Libraries :: Python Modules',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Operating System :: Unix',
         'Operating System :: MacOS',
     ],
     install_requires=[
         'requests',
         'python-dotenv',
         'tqdm',
         'packaging'
     ],
+    package_data={
+        "webdriver_manager": ["py.typed"]
+    },
 )
```

### Comparing `webdriver_manager-3.8.5/tests_negative/test_browsers_not_installed.py` & `webdriver_manager-3.8.6/tests_negative/test_browsers_not_installed.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/chrome.py` & `webdriver_manager-3.8.6/webdriver_manager/chrome.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/archive.py` & `webdriver_manager-3.8.6/webdriver_manager/core/archive.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/config.py` & `webdriver_manager-3.8.6/webdriver_manager/core/config.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/download_manager.py` & `webdriver_manager-3.8.6/webdriver_manager/core/download_manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/driver.py` & `webdriver_manager-3.8.6/webdriver_manager/drivers/chrome.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,63 @@
-from webdriver_manager.core import utils
+from packaging import version
+
+from webdriver_manager.core.driver import Driver
 from webdriver_manager.core.logger import log
-from webdriver_manager.core.config import gh_token
-from webdriver_manager.core.utils import get_browser_version_from_os
+from webdriver_manager.core.utils import ChromeType, is_arch, is_mac_os
+
 
+class ChromeDriver(Driver):
 
-class Driver(object):
     def __init__(
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
-            http_client):
-        self._name = name
-        self._url = url
-        self._version = version
-        self._os_type = os_type
-        if os_type is None:
-            self._os_type = utils.os_type()
-        self._latest_release_url = latest_release_url
-        self._http_client = http_client
-
-    @property
-    def auth_header(self):
-        token = gh_token()
-        if token:
-            log("GH_TOKEN will be used to perform requests")
-            return {"Authorization": f"token {token}"}
-        return None
-
-    def get_name(self):
-        return self._name
+            http_client,
+            chrome_type=ChromeType.GOOGLE,
+    ):
+        super(ChromeDriver, self).__init__(
+            name, version, os_type, url, latest_release_url, http_client
+        )
+        self._browser_type = chrome_type
+        self._os_type = self.get_os_type()
 
     def get_os_type(self):
-        return self._os_type
+        os_type = super().get_os_type()
+        if "win" in os_type:
+            return "win32"
+
+        if not is_mac_os(os_type):
+            return os_type
+
+        if is_arch(os_type):
+            return "mac_arm64"
+
+        return os_type
+
+    def get_driver_download_url(self):
+        driver_version_to_download = self.get_driver_version_to_download()
+        os_type = self._os_type
+        # For Mac ARM CPUs after version 106.0.5249.61 the format of OS type changed
+        # to more unified "mac_arm64". For newer versions, it'll be "mac_arm64"
+        # by default, for lower versions we replace "mac_arm64" to old format - "mac64_m1".
+        if version.parse(driver_version_to_download) < version.parse("106.0.5249.61"):
+            os_type = os_type.replace("mac_arm64", "mac64_m1")
 
-    def get_url(self):
-        return f"{self._url}/{self.get_version()}/{self.get_name()}_{self.get_os_type()}.zip"
+        return f"{self._url}/{driver_version_to_download}/{self.get_name()}_{os_type}.zip"
 
-    def get_version(self):
-        if not self._version:
-            try:
-                return self.get_latest_release_version()
-            except Exception:
-                return self.get_browser_version()
-        return self._version
+    def get_browser_type(self):
+        return self._browser_type
 
     def get_latest_release_version(self):
-        # type: () -> str
-        raise NotImplementedError("Please implement this method")
+        determined_browser_version = self.get_browser_version_from_os()
 
-    def get_browser_version(self):
-        return get_browser_version_from_os(self.get_browser_type())
-
-    def get_browser_type(self):
-        raise NotImplementedError("Please implement this method")
-
-    def get_binary_name(self):
-        driver_name = self.get_name()
-        driver_binary_name = (
-            "msedgedriver" if driver_name == "edgedriver" else driver_name
-        )
-        driver_binary_name = (
-            f"{driver_binary_name}.exe" if "win" in self.get_os_type() else driver_binary_name
+        log(f"Get LATEST {self._name} version for {self._browser_type}")
+        latest_release_url = (
+            self._latest_release_url
+            if (self._version == "latest" or determined_browser_version is None)
+            else f"{self._latest_release_url}_{determined_browser_version}"
         )
-        return driver_binary_name
+        resp = self._http_client.get(url=latest_release_url)
+        return resp.text.rstrip()
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/driver_cache.py` & `webdriver_manager-3.8.6/webdriver_manager/core/driver_cache.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import os
 
 from webdriver_manager.core.config import wdm_local, get_xdist_worker_id
 from webdriver_manager.core.constants import (
     DEFAULT_PROJECT_ROOT_CACHE_PATH,
     DEFAULT_USER_HOME_CACHE_PATH, ROOT_FOLDER_NAME,
 )
+from webdriver_manager.core.driver import Driver
 from webdriver_manager.core.logger import log
-from webdriver_manager.core.utils import get_date_diff, File, save_file, format_version
+from webdriver_manager.core.utils import get_date_diff, File, save_file
 
 
 class DriverCache(object):
     def __init__(self, root_dir=None, valid_range=1):
         self._root_dir = DEFAULT_USER_HOME_CACHE_PATH
         is_wdm_local = wdm_local()
         xdist_worker_id = get_xdist_worker_id()
@@ -26,111 +27,108 @@
             self._root_dir = os.path.join(DEFAULT_PROJECT_ROOT_CACHE_PATH, xdist_worker_id)
 
         self._drivers_root = "drivers"
         self._drivers_json_path = os.path.join(self._root_dir, "drivers.json")
         self._date_format = "%d/%m/%Y"
         self._drivers_directory = os.path.join(self._root_dir, self._drivers_root)
         self.valid_range = valid_range
+        self._cache_key_driver_version = None
+        self._metadata_key = None
+        self._driver_binary_path = None
 
-    def save_file_to_cache(self, driver, file: File):
-        driver_name = driver.get_name()
-        os_type = driver.get_os_type()
-        driver_version = driver.get_version()
-        browser_version = driver.get_browser_version()
-        browser_type = driver.get_browser_type()
-        unified_version = format_version(browser_type, driver_version)
-
-        path = os.path.join(
-            self._drivers_directory, driver_name, os_type, unified_version
-        )
+    def save_file_to_cache(self, driver: Driver, file: File):
+        path = self.__get_path(driver)
         archive = save_file(file, path)
         files = archive.unpack(path)
-        binary = self.__get_binary(files, driver_name)
+        binary = self.__get_binary(files, driver.get_name())
         binary_path = os.path.join(path, binary)
-        self.__save_metadata(
-            browser_version, driver_name, os_type, unified_version, binary_path
-        )
+        self.__save_metadata(driver, binary_path)
         log(f"Driver has been saved in cache [{path}]")
         return binary_path
 
     def __get_binary(self, files, driver_name):
         if len(files) == 1:
             return files[0]
 
         for f in files:
             if driver_name in f:
                 return f
 
         raise Exception(f"Can't find binary for {driver_name} among {files}")
 
-    def __save_metadata(
-            self,
-            browser_version,
-            driver_name,
-            os_type,
-            driver_version,
-            binary_path,
-            date=None,
-    ):
+    def __save_metadata(self, driver: Driver, binary_path, date=None):
         if date is None:
             date = datetime.date.today()
 
-        metadata = self.get_metadata()
-
-        key = f"{os_type}_{driver_name}_{driver_version}_for_{browser_version}"
-
+        metadata = self.load_metadata_content()
+        key = self.__get_metadata_key(driver)
         data = {
             key: {
                 "timestamp": date.strftime(self._date_format),
                 "binary_path": binary_path,
             }
         }
 
         metadata.update(data)
         with open(self._drivers_json_path, "w+") as outfile:
             json.dump(metadata, outfile, indent=4)
 
-    def find_driver(self, driver):
+    def find_driver(self, driver: Driver):
         """Find driver by '{os_type}_{driver_name}_{driver_version}_{browser_version}'."""
         os_type = driver.get_os_type()
         driver_name = driver.get_name()
-        driver_version = driver.get_version()
-        browser_version = driver.get_browser_version()
+        browser_version = driver.get_browser_version_from_os()
+        driver_version = self.get_cache_key_driver_version(driver)
         browser_type = driver.get_browser_type()
-        unified_version = format_version(browser_type, driver_version)
-
-        metadata = self.get_metadata()
+        metadata = self.load_metadata_content()
 
-        key = f"{os_type}_{driver_name}_{unified_version}_for_{browser_version}"
+        key = self.__get_metadata_key(driver)
         if key not in metadata:
-            log(
-                f"There is no [{os_type}] {driver_name} for browser {browser_version} in cache"
-            )
-            return None
-
-        path = os.path.join(self._drivers_directory, driver_name, os_type, unified_version)
-
-        driver_binary_name = driver.get_binary_name()
-        binary_path = os.path.join(path, driver_binary_name)
-        if not os.path.exists(binary_path):
+            log(f'There is no [{os_type}] {driver_name} "{driver_version}" for browser {browser_type} "{browser_version}" in cache')
             return None
 
         driver_info = metadata[key]
+        path = driver_info["binary_path"]
+        if not os.path.exists(path):
+            return None
 
         if not self.__is_valid(driver_info):
             return None
 
         path = driver_info["binary_path"]
         log(f"Driver [{path}] found in cache")
         return path
 
     def __is_valid(self, driver_info):
         dates_diff = get_date_diff(
             driver_info["timestamp"], datetime.date.today(), self._date_format
         )
         return dates_diff < self.valid_range
 
-    def get_metadata(self):
+    def load_metadata_content(self):
         if os.path.exists(self._drivers_json_path):
             with open(self._drivers_json_path, "r") as outfile:
                 return json.load(outfile)
         return {}
+
+    def __get_metadata_key(self, driver: Driver):
+        if self._metadata_key is None:
+            driver_version = self.get_cache_key_driver_version(driver)
+            browser_version = driver.get_browser_version_from_os()
+            browser_version = browser_version if browser_version else ""
+            self._metadata_key = f"{driver.get_os_type()}_{driver.get_name()}_{driver_version}_for_{browser_version}"
+        return self._metadata_key
+
+    def get_cache_key_driver_version(self, driver: Driver):
+        if self._cache_key_driver_version is None:
+            self._cache_key_driver_version = "latest" if driver._version in (None, "latest") else driver._version
+        return self._cache_key_driver_version
+
+    def __get_path(self, driver: Driver):
+        if self._driver_binary_path is None:
+            self._driver_binary_path = os.path.join(
+                self._drivers_directory,
+                driver.get_name(),
+                driver.get_os_type(),
+                driver.get_driver_version_to_download(),
+            )
+        return self._driver_binary_path
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/http.py` & `webdriver_manager-3.8.6/webdriver_manager/core/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from requests import Response
+from requests import Response, exceptions
 
 from webdriver_manager.core.config import ssl_verify, wdm_progress_bar
 from webdriver_manager.core.utils import show_download_progress
 
 
 class HttpClient:
     def get(self, url, params=None, **kwargs) -> Response:
@@ -25,13 +25,17 @@
 
 
 class WDMHttpClient(HttpClient):
     def __init__(self):
         self._ssl_verify = ssl_verify()
 
     def get(self, url, **kwargs) -> Response:
-        resp = requests.get(url=url, verify=self._ssl_verify, stream=True, **kwargs)
+        try:
+            resp = requests.get(
+                url=url, verify=self._ssl_verify, stream=True, **kwargs)
+        except exceptions.ConnectionError:
+            raise ConnectionError(f"Could not reach host. Are you offline?")
         self.validate_response(resp)
         if wdm_progress_bar():
             show_download_progress(resp)
         return resp
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/logger.py` & `webdriver_manager-3.8.6/webdriver_manager/core/logger.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/manager.py` & `webdriver_manager-3.8.6/webdriver_manager/core/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,10 +23,10 @@
         raise NotImplementedError("Please Implement this method")
 
     def _get_driver_path(self, driver):
         binary_path = self.driver_cache.find_driver(driver)
         if binary_path:
             return binary_path
 
-        file = self._download_manager.download_file(driver.get_url())
+        file = self._download_manager.download_file(driver.get_driver_download_url())
         binary_path = self.driver_cache.save_file_to_cache(driver, file)
         return binary_path
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/core/utils.py` & `webdriver_manager-3.8.6/webdriver_manager/core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 def save_file(file: File, directory: str):
     os.makedirs(directory, exist_ok=True)
 
     archive_path = f"{directory}{os.sep}{file.filename}"
     with open(archive_path, "wb") as code:
         code.write(file.content)
+    if not os.path.exists(archive_path):
+        raise FileExistsError(f"No file has been saved on such path {archive_path}")
     return Archive(archive_path, os_type=os_name())
 
 
 class OSType(object):
     LINUX = "linux"
     MAC = "mac"
     WIN = "win"
@@ -218,42 +220,15 @@
 
     try:
         cmd_mapping = cmd_mapping[browser_type][os_name()]
         pattern = PATTERN[browser_type]
         version = read_version_from_cmd(cmd_mapping, pattern)
         return version
     except Exception:
-        raise Exception(f"Can not find browser {browser_type} installed in your system!!!")
-
-
-def format_version(browser_type, version):
-    if not version or version == 'latest':
-        return 'latest'
-    try:
-        pattern = PATTERN[browser_type]
-        result = re.search(pattern, version)
-        return result.group(0) if result else version
-    except:
-        return "latest"
-
-
-def get_browser_version(browser_type, metadata):
-    pattern = PATTERN[browser_type]
-    version_from_os = metadata['version']
-    result = re.search(pattern, version_from_os)
-    version = result.group(0) if version_from_os else None
-    if not version:
-        log(
-            f"Could not get version for {browser_type}. "
-            f"Is {browser_type} installed?"
-        )
-    else:
-        log(f"Current {browser_type} version is {version}")
-
-    return version
+        return None
 
 
 def read_version_from_cmd(cmd, pattern):
     with subprocess.Popen(
             cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.DEVNULL,
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/drivers/edge.py` & `webdriver_manager-3.8.6/webdriver_manager/drivers/edge.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,35 +18,38 @@
             name,
             version,
             os_type,
             url,
             latest_release_url,
             http_client
         )
+        self._os_type = self.get_os_type()
 
     def get_stable_release_version(self):
         """Stable driver version when browser version was not determined."""
-        stable_url = self._latest_release_url.replace(
-            "LATEST_RELEASE", "LATEST_STABLE")
+        stable_url = self._latest_release_url.replace("LATEST_RELEASE", "LATEST_STABLE")
         resp = self._http_client.get(url=stable_url)
         return resp.text.rstrip()
 
     def get_latest_release_version(self) -> str:
-        browser_version = self.get_browser_version()
-        browser_version = (
-            browser_version if browser_version else self.get_stable_release_version())
-        log(f"Get LATEST {self._name} version for {browser_version} Edge")
-        major_edge_version = browser_version.split(".")[0]
+        determined_browser_version = self.get_browser_version_from_os()
+        log(f"Get LATEST {self._name} version for Edge {determined_browser_version}")
+
+        edge_driver_version_to_download = (
+            self.get_stable_release_version()
+            if (self._version == "latest" or determined_browser_version is None)
+            else determined_browser_version
+        )
+        major_edge_version = edge_driver_version_to_download.split(".")[0]
         latest_release_url = {
             OSType.WIN
-            in self.get_os_type(): f"{self._latest_release_url}_{major_edge_version}_WINDOWS",
+            in self._os_type: f"{self._latest_release_url}_{major_edge_version}_WINDOWS",
             OSType.MAC
-            in self.get_os_type(): f"{self._latest_release_url}_{major_edge_version}_MACOS",
+            in self._os_type: f"{self._latest_release_url}_{major_edge_version}_MACOS",
             OSType.LINUX
-            in self.get_os_type(): f"{self._latest_release_url}_{major_edge_version}_LINUX",
+            in self._os_type: f"{self._latest_release_url}_{major_edge_version}_LINUX",
         }[True]
         resp = self._http_client.get(url=latest_release_url)
-        self._version = resp.text.rstrip()
-        return self._version
+        return resp.text.rstrip()
 
     def get_browser_type(self):
         return ChromeType.MSEDGE
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/drivers/firefox.py` & `webdriver_manager-3.8.6/webdriver_manager/drivers/firefox.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,45 +8,46 @@
             self,
             name,
             version,
             os_type,
             url,
             latest_release_url,
             mozila_release_tag,
-            http_client
+            http_client,
     ):
         super(GeckoDriver, self).__init__(
             name,
             version,
             os_type,
             url,
             latest_release_url,
-            http_client
+            http_client,
         )
         self._mozila_release_tag = mozila_release_tag
+        self._os_type = self.get_os_type()
 
     def get_latest_release_version(self) -> str:
-        browser_version = self.get_browser_version()
-        log(f"Get LATEST {self._name} version for {browser_version} firefox")
+        determined_browser_version = self.get_browser_version_from_os()
+        log(f"Get LATEST {self._name} version for {determined_browser_version} firefox")
         resp = self._http_client.get(
             url=self.latest_release_url,
             headers=self.auth_header
         )
-        self._version = resp.json()["tag_name"]
-        return self._version
+        return resp.json()["tag_name"]
 
-    def get_url(self):
+    def get_driver_download_url(self):
         """Like https://github.com/mozilla/geckodriver/releases/download/v0.11.1/geckodriver-v0.11.1-linux64.tar.gz"""
-        log(f"Getting latest mozilla release info for {self.get_version()}")
+        driver_version_to_download = self.get_driver_version_to_download()
+        log(f"Getting latest mozilla release info for {driver_version_to_download}")
         resp = self._http_client.get(
-            url=self.tagged_release_url(self.get_version()),
+            url=self.tagged_release_url(driver_version_to_download),
             headers=self.auth_header
         )
         assets = resp.json()["assets"]
-        name = f"{self.get_name()}-{self.get_version()}-{self.get_os_type()}."
+        name = f"{self.get_name()}-{driver_version_to_download}-{self._os_type}."
         output_dict = [
             asset for asset in assets if asset["name"].startswith(name)]
         return output_dict[0]["browser_download_url"]
 
     def get_os_type(self):
         os_type = super().get_os_type()
         if not is_mac_os(os_type):
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/drivers/ie.py` & `webdriver_manager-3.8.6/webdriver_manager/drivers/ie.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,41 +24,41 @@
         )
         self.os_type = "x64" if os_type == "win64" else "Win32"
         self._ie_release_tag = ie_release_tag
         # todo: for 'browser_version' implement installed IE version detection
         #       like chrome or firefox
 
     def get_latest_release_version(self) -> str:
-        log(f"Get LATEST driver version for {self.get_browser_version()}")
+        log(f"Get LATEST driver version for Internet Explorer")
         resp = self._http_client.get(
             url=self.latest_release_url,
             headers=self.auth_header
         )
 
         releases = resp.json()
         release = next(
             release
             for release in releases
             for asset in release["assets"]
             if asset["name"].startswith(self.get_name())
         )
-        self._version = release["tag_name"].replace("selenium-", "")
-        return self._version
+        return release["tag_name"].replace("selenium-", "")
 
-    def get_url(self):
+    def get_driver_download_url(self):
         """Like https://github.com/seleniumhq/selenium/releases/download/3.141.59/IEDriverServer_Win32_3.141.59.zip"""
-        log(f"Getting latest ie release info for {self.get_version()}")
+        driver_version_to_download = self.get_driver_version_to_download()
+        log(f"Getting latest ie release info for {driver_version_to_download}")
         resp = self._http_client.get(
-            url=self.tagged_release_url(self.get_version()),
+            url=self.tagged_release_url(driver_version_to_download),
             headers=self.auth_header
         )
 
         assets = resp.json()["assets"]
 
-        name = f"{self.get_name()}_{self.os_type}_{self.get_version()}" + "."
+        name = f"{self._name}_{self.os_type}_{driver_version_to_download}" + "."
         output_dict = [
             asset for asset in assets if asset["name"].startswith(name)]
         return output_dict[0]["browser_download_url"]
 
     @property
     def latest_release_url(self):
         return self._latest_release_url
@@ -77,13 +77,7 @@
             raise ValueError(
                 "Version must consist of major, minor and/or patch, "
                 "but given was: '{version}'".format(version=version)
             )
 
     def get_browser_type(self):
         return "msie"
-
-    def get_browser_version(self):
-        try:
-            return super().get_browser_version()
-        except:
-            return "latest"
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/drivers/opera.py` & `webdriver_manager-3.8.6/webdriver_manager/drivers/opera.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,23 +18,22 @@
         self.opera_release_tag = opera_release_tag
 
     def get_latest_release_version(self) -> str:
         resp = self._http_client.get(
             url=self.latest_release_url,
             headers=self.auth_header
         )
-        self._version = resp.json()["tag_name"]
-        return self._version
+        return resp.json()["tag_name"]
 
-    def get_url(self) -> str:
-        # https://github.com/operasoftware/operachromiumdriver/releases/download/v.2.45/operadriver_linux64.zip
-        version = self.get_version()
-        log(f"Getting latest opera release info for {version}")
+    def get_driver_download_url(self) -> str:
+        """Like https://github.com/operasoftware/operachromiumdriver/releases/download/v.2.45/operadriver_linux64.zip"""
+        driver_version_to_download = self.get_driver_version_to_download()
+        log(f"Getting latest opera release info for {driver_version_to_download}")
         resp = self._http_client.get(
-            url=self.tagged_release_url(version),
+            url=self.tagged_release_url(driver_version_to_download),
             headers=self.auth_header
         )
         assets = resp.json()["assets"]
         name = "{0}_{1}".format(self.get_name(), self.get_os_type())
         output_dict = [
             asset for asset in assets if asset["name"].startswith(name)]
         return output_dict[0]["browser_download_url"]
@@ -44,13 +43,7 @@
         return self._latest_release_url
 
     def tagged_release_url(self, version):
         return self.opera_release_tag.format(version)
 
     def get_browser_type(self):
         return "opera"
-
-    def get_browser_version(self):
-        try:
-            return super().get_browser_version()
-        except:
-            return "latest"
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager/firefox.py` & `webdriver_manager-3.8.6/webdriver_manager/firefox.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/microsoft.py` & `webdriver_manager-3.8.6/webdriver_manager/microsoft.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager/opera.py` & `webdriver_manager-3.8.6/webdriver_manager/opera.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.8.5/webdriver_manager.egg-info/PKG-INFO` & `webdriver_manager-3.8.6/webdriver_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: webdriver-manager
-Version: 3.8.5
+Version: 3.8.6
 Summary: Library provides the way to automatically manage drivers for different browsers
 Home-page: https://github.com/SergeyPirogov/webdriver_manager
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -25,30 +26,26 @@
 # Webdriver Manager for Python
 
 [![Tests](https://github.com/SergeyPirogov/webdriver_manager/actions/workflows/test.yml/badge.svg)](https://github.com/SergeyPirogov/webdriver_manager/actions/workflows/test.yml)
 [![PyPI](https://img.shields.io/pypi/v/webdriver_manager.svg)](https://pypi.org/project/webdriver-manager)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/webdriver_manager.svg)](https://pypi.org/project/webdriver-manager/)
 [![codecov](https://codecov.io/gh/SergeyPirogov/webdriver_manager/branch/master/graph/badge.svg)](https://codecov.io/gh/SergeyPirogov/webdriver_manager)
 
-[Patreon](https://www.patreon.com/automation_remarks)
+## Support the library on [Patreon](https://www.patreon.com/automation_remarks)
 
 The main idea is to simplify management of binary drivers for different browsers.
 
 For now support:
 
 - [ChromeDriver](#use-with-chrome)
-
+- [EdgeChromiumDriver](#use-with-edge)
 - [GeckoDriver](#use-with-firefox)
-
 - [IEDriver](#use-with-ie)
-
 - [OperaDriver](#use-with-opera)
 
-- [EdgeChromiumDriver](#use-with-edge)
-
 Compatible with Selenium 4.x and below.
 
 Before:
 You need to download the chromedriver binary, unzip it somewhere on your PC and set the path to this driver like this:
 
 ```python
 from selenium import webdriver
@@ -121,14 +118,33 @@
 from selenium.webdriver.chrome.service import Service as BraveService
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 driver = webdriver.Chrome(service=BraveService(ChromeDriverManager(chrome_type=ChromeType.BRAVE).install()))
 ```
 
+
+#### Use with Edge
+
+```python
+# selenium 3
+from selenium import webdriver
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+```
+```python
+# selenium 4
+from selenium import webdriver
+from selenium.webdriver.edge.service import Service as EdgeService
+from webdriver_manager.microsoft import EdgeChromiumDriverManager
+
+driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
+```
+
 #### Use with Firefox
 
 ```python
 # selenium 3
 from selenium import webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 
@@ -157,53 +173,50 @@
 from selenium import webdriver
 from selenium.webdriver.ie.service import Service as IEService
 from webdriver_manager.microsoft import IEDriverManager
 
 driver = webdriver.Ie(service=IEService(IEDriverManager().install()))
 ```
 
-#### Use with Edge
+
+#### Use with Opera
 
 ```python
 # selenium 3
 from selenium import webdriver
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-driver = webdriver.Edge(EdgeChromiumDriverManager().install())
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
+
+driver = webdriver.Remote(webdriver_service.service_url, webdriver.DesiredCapabilities.OPERA)
 ```
 ```python
 # selenium 4
 from selenium import webdriver
-from selenium.webdriver.edge.service import Service as EdgeService
-from webdriver_manager.microsoft import EdgeChromiumDriverManager
-
-driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))
-```
+from selenium.webdriver.chrome import service
+from webdriver_manager.opera import OperaDriverManager
 
-#### Use with Opera
+webdriver_service = service.Service(OperaDriverManager().install())
+webdriver_service.start()
 
-```python
-# selenium 3 & 4
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
+options = webdriver.ChromeOptions()
+options.add_experimental_option('w3c', True)
 
-driver = webdriver.Opera(executable_path=OperaDriverManager().install())
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 If the Opera browser is installed in a location other than `C:/Program Files` or `C:/Program Files (x86)` on windows
 and `/usr/bin/opera` for all unix variants and mac, then use the below code,
 
 ```python
-from selenium import webdriver
-from webdriver_manager.opera import OperaDriverManager
-
 options = webdriver.ChromeOptions()
-options.add_argument('allow-elevated-browser')
-options.binary_location = "C:\\Users\\USERNAME\\FOLDERLOCATION\\Opera\\VERSION\\opera.exe"
-driver = webdriver.Opera(executable_path=OperaDriverManager().install(), options=options)
+options.binary_location = "path/to/opera.exe"
+driver = webdriver.Remote(webdriver_service.service_url, options=options)
 ```
 
 #### Get browser version from path
 
 To get the version of the browser from the executable of the browser itself:
 
 ```python
@@ -243,14 +256,23 @@
 ```python
 import logging
 import os
 
 os.environ['WDM_LOG'] = str(logging.NOTSET)
 ```
 
+### `WDM_PROGRESS_BAR`
+Turn off the progress bar which is displayed on downloads:
+
+```python
+import os
+
+os.environ['WDM_PROGRESS_BAR'] = str(0)
+```
+
 ### `WDM_LOCAL`
 By default, all driver binaries are saved to user.home/.wdm folder. You can override this setting and save binaries to project.root/.wdm.
 
 ```python
 import os
 
 os.environ['WDM_LOCAL'] = '1'
```

### Comparing `webdriver_manager-3.8.5/webdriver_manager.egg-info/SOURCES.txt` & `webdriver_manager-3.8.6/webdriver_manager.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-tests/xdist/__init__.py
-tests/xdist/conftest.py
-tests/xdist/test_cuncurent_1.py
-tests/xdist/test_cuncurent_2.py
+tests/test_brave_driver.py
+tests/test_chrome_driver.py
+tests/test_chromium_driver.py
+tests/test_custom_http_client.py
+tests/test_custom_logger.py
+tests/test_downloader.py
+tests/test_edge_driver.py
+tests/test_firefox_manager.py
+tests/test_ie_driver.py
+tests/test_opera_manager.py
+tests/test_silent_global_logs.py
+tests/test_utils.py
 tests_negative/__init__.py
 tests_negative/test_browsers_not_installed.py
+tests_xdist/__init__.py
+tests_xdist/conftest.py
+tests_xdist/test_cuncurent_1.py
+tests_xdist/test_cuncurent_2.py
 webdriver_manager/__init__.py
 webdriver_manager/chrome.py
 webdriver_manager/firefox.py
 webdriver_manager/microsoft.py
 webdriver_manager/opera.py
+webdriver_manager/py.typed
 webdriver_manager.egg-info/PKG-INFO
 webdriver_manager.egg-info/SOURCES.txt
 webdriver_manager.egg-info/dependency_links.txt
 webdriver_manager.egg-info/requires.txt
 webdriver_manager.egg-info/top_level.txt
 webdriver_manager/core/__init__.py
 webdriver_manager/core/archive.py
```

