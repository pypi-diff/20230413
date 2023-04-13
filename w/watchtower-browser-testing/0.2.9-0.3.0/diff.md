# Comparing `tmp/watchtower_browser_testing-0.2.9.tar.gz` & `tmp/watchtower_browser_testing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.2.9.tar", last modified: Wed Apr 12 13:40:30 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.0.tar", last modified: Thu Apr 13 18:01:57 2023, max compression
```

## Comparing `watchtower_browser_testing-0.2.9.tar` & `watchtower_browser_testing-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 13:40:30.564026 watchtower_browser_testing-0.2.9/
--rw-rw-rw-   0        0        0      310 2023-04-12 13:40:30.564026 watchtower_browser_testing-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 13:40:30.564026 watchtower_browser_testing-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:40:30.548401 watchtower_browser_testing-0.2.9/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0    11551 2023-04-12 13:40:18.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-12 13:40:18.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:40:30.548401 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:01:57.187871 watchtower_browser_testing-0.3.0/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:01:57.187871 watchtower_browser_testing-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:01:57.187871 watchtower_browser_testing-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:01:57.187871 watchtower_browser_testing-0.3.0/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-04-13 12:22:31.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1503 2023-04-13 18:01:14.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/helpers.py
+-rw-rw-rw-   0        0        0    13957 2023-04-13 18:01:14.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 18:01:14.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:01:57.187871 watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:01:56.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-13 18:01:57.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:01:56.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-13 18:01:56.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 18:01:56.000000 watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.2.9/setup.py` & `watchtower_browser_testing-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.9/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.0/watchtower_browser_testing/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,8 +4,16 @@
 VALIDATION_METHOD_PREFIX = 'validation_'
 DEFAULT_TEST_DESCRIPTION = ''
 DEFAULT_BROWSERS = ['chromium', 'firefox', 'webkit']
 HARVEST_USER_SS_COOKIE_NAME = '_harvest_ss_user'
 HARVEST_USER_WEB_COOKIE_NAME = '_harvest_web_user'
 OLD_HARVEST_USER_ID_KEY = 'oldHarvestUserId'
 GTM_WEB_PREVIEW_LINK_REGEX = r'^https://tagassistant[.]google[.]com/.*'
-DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION = r'tag_assistant'
+DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION = r'tag_assistant'
+
+VALIDATION_MD_STRING = '''<details>
+<summary>Open to see performed validation for {event_name}</summary>
+
+```
+{json_string}
+```
+</details>'''
```

### Comparing `watchtower_browser_testing-0.2.9/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.0/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.0/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 watchtower_browser_testing/__init__.py
 watchtower_browser_testing/config.py
 watchtower_browser_testing/exceptions.py
+watchtower_browser_testing/helpers.py
 watchtower_browser_testing/testsuite.py
 watchtower_browser_testing/tracking_validation.py
 watchtower_browser_testing/version.py
 watchtower_browser_testing.egg-info/PKG-INFO
 watchtower_browser_testing.egg-info/SOURCES.txt
 watchtower_browser_testing.egg-info/dependency_links.txt
 watchtower_browser_testing.egg-info/requires.txt
```

