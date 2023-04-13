# Comparing `tmp/azure-monitor-opentelemetry-distro-1.0.0b8.tar.gz` & `tmp/azure-monitor-opentelemetry-distro-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-monitor-opentelemetry-distro-1.0.0b8.tar", last modified: Tue Sep 27 00:44:19 2022, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-distro-1.0.0b9.tar", last modified: Thu Apr 13 19:06:12 2023, max compression
```

## Comparing `azure-monitor-opentelemetry-distro-1.0.0b8.tar` & `azure-monitor-opentelemetry-distro-1.0.0b9.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.452691 azure-monitor-opentelemetry-distro-1.0.0b8/
--rw-rw-rw-   0        0        0     3130 2022-09-27 00:44:19.455052 azure-monitor-opentelemetry-distro-1.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     2365 2022-09-26 21:21:50.000000 azure-monitor-opentelemetry-distro-1.0.0b8/README.md
--rw-rw-rw-   0        0        0     1457 2022-09-27 00:44:19.458546 azure-monitor-opentelemetry-distro-1.0.0b8/setup.cfg
--rw-rw-rw-   0        0        0      672 2022-09-21 22:26:59.000000 azure-monitor-opentelemetry-distro-1.0.0b8/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.125179 azure-monitor-opentelemetry-distro-1.0.0b8/src/
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.113020 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.113772 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.114275 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.333628 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/distro/
--rw-rw-rw-   0        0        0      449 2022-09-21 22:26:59.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/distro/configurator.py
--rw-rw-rw-   0        0        0     1365 2022-09-06 23:08:33.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/distro/constants.py
--rw-rw-rw-   0        0        0      978 2022-09-22 20:39:19.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/distro/distro.py
--rw-rw-rw-   0        0        0      334 2022-09-27 00:40:19.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/distro/version.py
-drwxrwxrwx   0        0        0        0 2022-09-27 00:44:19.444919 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/
--rw-rw-rw-   0        0        0     3130 2022-09-27 00:44:18.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2022-09-27 00:44:19.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-27 00:44:18.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2022-09-27 00:44:18.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-09-07 22:25:25.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      222 2022-09-27 00:44:18.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-27 00:44:18.000000 azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:12.002394 azure-monitor-opentelemetry-distro-1.0.0b9/
+-rw-rw-rw-   0        0        0     1005 2023-04-13 19:06:12.002394 azure-monitor-opentelemetry-distro-1.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-13 18:29:55.000000 azure-monitor-opentelemetry-distro-1.0.0b9/README.md
+-rw-rw-rw-   0        0        0     1457 2023-04-13 19:06:12.006390 azure-monitor-opentelemetry-distro-1.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-04-13 18:27:02.000000 azure-monitor-opentelemetry-distro-1.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:11.851810 azure-monitor-opentelemetry-distro-1.0.0b9/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:11.848661 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:11.848661 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:11.849788 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/opentelemetry/
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:11.896438 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/opentelemetry/distro/
+-rw-rw-rw-   0        0        0      449 2023-04-13 18:27:02.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/opentelemetry/distro/configurator.py
+-rw-rw-rw-   0        0        0      978 2023-04-13 18:27:02.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/opentelemetry/distro/distro.py
+-rw-rw-rw-   0        0        0      334 2023-04-13 18:44:29.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/opentelemetry/distro/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:11.967171 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/
+-rw-rw-rw-   0        0        0     1005 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      222 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 19:06:11.000000 azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:06:12.000382 azure-monitor-opentelemetry-distro-1.0.0b9/tests/
+-rw-rw-rw-   0        0        0      540 2023-04-13 18:27:02.000000 azure-monitor-opentelemetry-distro-1.0.0b9/tests/test_flask.py
+-rw-rw-rw-   0        0        0      474 2023-04-13 18:27:02.000000 azure-monitor-opentelemetry-distro-1.0.0b9/tests/test_psycopg2.py
+-rw-rw-rw-   0        0        0      474 2023-04-13 18:27:02.000000 azure-monitor-opentelemetry-distro-1.0.0b9/tests/test_requests.py
```

### Comparing `azure-monitor-opentelemetry-distro-1.0.0b8/setup.cfg` & `azure-monitor-opentelemetry-distro-1.0.0b9/setup.cfg`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-distro-1.0.0b8/setup.py` & `azure-monitor-opentelemetry-distro-1.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-distro-1.0.0b8/src/azure/monitor/opentelemetry/distro/distro.py` & `azure-monitor-opentelemetry-distro-1.0.0b9/src/azure/monitor/opentelemetry/distro/distro.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-distro-1.0.0b8/src/azure_monitor_opentelemetry_distro.egg-info/SOURCES.txt` & `azure-monitor-opentelemetry-distro-1.0.0b9/src/azure_monitor_opentelemetry_distro.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 setup.cfg
 setup.py
 src/azure/monitor/opentelemetry/distro/configurator.py
-src/azure/monitor/opentelemetry/distro/constants.py
 src/azure/monitor/opentelemetry/distro/distro.py
 src/azure/monitor/opentelemetry/distro/version.py
 src/azure_monitor_opentelemetry_distro.egg-info/PKG-INFO
 src/azure_monitor_opentelemetry_distro.egg-info/SOURCES.txt
 src/azure_monitor_opentelemetry_distro.egg-info/dependency_links.txt
 src/azure_monitor_opentelemetry_distro.egg-info/entry_points.txt
 src/azure_monitor_opentelemetry_distro.egg-info/not-zip-safe
 src/azure_monitor_opentelemetry_distro.egg-info/requires.txt
-src/azure_monitor_opentelemetry_distro.egg-info/top_level.txt
+src/azure_monitor_opentelemetry_distro.egg-info/top_level.txt
+tests/test_flask.py
+tests/test_psycopg2.py
+tests/test_requests.py
```

