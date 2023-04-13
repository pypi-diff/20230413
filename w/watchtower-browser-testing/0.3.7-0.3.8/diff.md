# Comparing `tmp/watchtower_browser_testing-0.3.7.tar.gz` & `tmp/watchtower_browser_testing-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.7.tar", last modified: Thu Apr 13 19:16:51 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.8.tar", last modified: Thu Apr 13 19:27:57 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.7.tar` & `watchtower_browser_testing-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.850849 watchtower_browser_testing-0.3.7/
--rw-rw-rw-   0        0        0      310 2023-04-13 19:16:51.850849 watchtower_browser_testing-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 19:16:51.850849 watchtower_browser_testing-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.834741 watchtower_browser_testing-0.3.7/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.834741 watchtower_browser_testing-0.3.7/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     1721 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    14236 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.834741 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/
+-rw-rw-rw-   0        0        0      310 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.378186 watchtower_browser_testing-0.3.8/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     2613 2023-04-13 19:27:41.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    14236 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 19:27:48.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.7/setup.py` & `watchtower_browser_testing-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.7/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.8/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.7/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.8/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.7/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.8/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.7/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.8/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

