# Comparing `tmp/watchtower_browser_testing-0.3.3.tar.gz` & `tmp/watchtower_browser_testing-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.3.tar", last modified: Thu Apr 13 18:29:17 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.4.tar", last modified: Thu Apr 13 18:32:22 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.3.tar` & `watchtower_browser_testing-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:29:17.249379 watchtower_browser_testing-0.3.3/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:29:17.233737 watchtower_browser_testing-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 18:29:17.249379 watchtower_browser_testing-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:29:17.233737 watchtower_browser_testing-0.3.3/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/helpers.py
--rw-rw-rw-   0        0        0    14194 2023-04-13 18:29:02.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 18:29:02.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:29:17.233737 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 18:29:17.000000 watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:32:22.192410 watchtower_browser_testing-0.3.4/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:32:22.192410 watchtower_browser_testing-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:32:22.192410 watchtower_browser_testing-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2023-04-13 18:32:14.000000 watchtower_browser_testing-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:32:22.192410 watchtower_browser_testing-0.3.4/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/helpers.py
+-rw-rw-rw-   0        0        0    14194 2023-04-13 18:29:02.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 18:32:14.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:32:22.192410 watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:32:22.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-13 18:32:22.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:32:22.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 18:32:22.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 18:32:22.000000 watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.3/setup.py` & `watchtower_browser_testing-0.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,12 +26,14 @@
     author='Jacob Noordmans',
     author_email='jacob@graindataconsultants.com',
     keywords=['Watchtower']
 )
 
 install_requires = [
     'playwright==1.32.1',
-    'Cerberus'
+    'Cerberus',
+    'marko',
+    'Jinja2'
 ]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

### Comparing `watchtower_browser_testing-0.3.3/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.4/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.3/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.4/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.3/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.4/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.3/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.4/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.3/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.4/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

