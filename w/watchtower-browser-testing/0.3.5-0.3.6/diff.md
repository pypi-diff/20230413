# Comparing `tmp/watchtower_browser_testing-0.3.5.tar.gz` & `tmp/watchtower_browser_testing-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.5.tar", last modified: Thu Apr 13 18:41:35 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.6.tar", last modified: Thu Apr 13 18:51:35 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.5.tar` & `watchtower_browser_testing-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:41:35.602208 watchtower_browser_testing-0.3.5/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:41:35.602208 watchtower_browser_testing-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 18:41:35.602208 watchtower_browser_testing-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:41:35.586576 watchtower_browser_testing-0.3.5/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:41:35.602208 watchtower_browser_testing-0.3.5/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0      151 2023-04-13 18:24:13.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    14352 2023-04-13 18:35:07.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:41:35.602208 watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:41:35.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-13 18:41:35.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:41:35.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 18:41:35.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 18:41:35.000000 watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.890283 watchtower_browser_testing-0.3.6/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0      480 2023-04-13 18:51:23.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    14352 2023-04-13 18:35:07.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 18:51:23.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.5/setup.py` & `watchtower_browser_testing-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.5/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.6/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.5/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.6/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.5/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.6/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.5/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.6/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.5/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

