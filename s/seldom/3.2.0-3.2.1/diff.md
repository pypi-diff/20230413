# Comparing `tmp/seldom-3.2.0.tar.gz` & `tmp/seldom-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seldom-3.2.0.tar", last modified: Tue Mar 14 15:53:10 2023, max compression
+gzip compressed data, was "dist\seldom-3.2.1.tar", last modified: Thu Apr 13 16:55:00 2023, max compression
```

## Comparing `seldom-3.2.0.tar` & `seldom-3.2.1.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.673894 seldom-3.2.0/
--rw-rw-rw-   0        0        0    11565 2022-12-06 15:57:51.000000 seldom-3.2.0/LICENSE
--rw-rw-rw-   0        0        0       44 2022-12-06 15:57:51.000000 seldom-3.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1012 2023-03-14 15:53:10.671888 seldom-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9958 2022-12-14 16:56:26.000000 seldom-3.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.570778 seldom-3.2.0/demo/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-11 15:24:10.000000 seldom-3.2.0/demo/confrun.py
--rw-rw-rw-   0        0        0     1583 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/run.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.571777 seldom-3.2.0/demo/test_dir/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.572778 seldom-3.2.0/demo/test_dir/api_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/api_case/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-01-11 15:24:10.000000 seldom-3.2.0/demo/test_dir/api_case/test_http_demo.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.577807 seldom-3.2.0/demo/test_dir/app_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/app_case/__init__.py
--rw-rw-rw-   0        0        0      994 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/app_case/test_first_demo.py
--rw-rw-rw-   0        0        0     1243 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/app_case/test_po_demo.py
--rw-rw-rw-   0        0        0      875 2023-03-14 15:43:32.000000 seldom-3.2.0/demo/test_dir/app_case/test_u2_demo.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.583807 seldom-3.2.0/demo/test_dir/web_case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/web_case/__init__.py
--rw-rw-rw-   0        0        0      579 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/web_case/test_data_demo.py
--rw-rw-rw-   0        0        0     4287 2023-01-11 15:24:10.000000 seldom-3.2.0/demo/test_dir/web_case/test_ddt_demo.py
--rw-rw-rw-   0        0        0      589 2023-01-11 15:24:10.000000 seldom-3.2.0/demo/test_dir/web_case/test_first_demo.py
--rw-rw-rw-   0        0        0      846 2022-12-06 15:57:51.000000 seldom-3.2.0/demo/test_dir/web_case/test_fixture_demo.py
--rw-rw-rw-   0        0        0      953 2023-01-11 15:24:10.000000 seldom-3.2.0/demo/test_dir/web_case/test_playwright_demo.py
--rw-rw-rw-   0        0        0     1087 2023-03-11 17:21:24.000000 seldom-3.2.0/demo/test_dir/web_case/test_po_demo.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.588808 seldom-3.2.0/proj/
--rw-rw-rw-   0        0        0        0 2022-12-08 16:29:03.000000 seldom-3.2.0/proj/__init__.py
--rw-rw-rw-   0        0        0      110 2022-12-12 15:41:44.000000 seldom-3.2.0/proj/confrun.py
--rw-rw-rw-   0        0        0     1031 2022-12-12 15:42:40.000000 seldom-3.2.0/proj/loader.py
--rw-rw-rw-   0        0        0      293 2022-12-12 15:41:28.000000 seldom-3.2.0/proj/run.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.598899 seldom-3.2.0/seldom/
--rw-rw-rw-   0        0        0     1305 2023-03-14 15:51:03.000000 seldom-3.2.0/seldom/__init__.py
--rw-rw-rw-   0        0        0     5373 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/appdriver.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.611517 seldom-3.2.0/seldom/appium_lab/
--rw-rw-rw-   0        0        0     1669 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/appium_lab/__init__.py
--rw-rw-rw-   0        0        0     3909 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/appium_lab/action.py
--rw-rw-rw-   0        0        0     7248 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/appium_lab/find.py
--rw-rw-rw-   0        0        0     2997 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/appium_lab/keyboard.py
--rw-rw-rw-   0        0        0     1721 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/appium_lab/switch.py
--rw-rw-rw-   0        0        0    11006 2023-03-13 16:12:38.000000 seldom-3.2.0/seldom/case.py
--rw-rw-rw-   0        0        0    13177 2022-12-16 17:09:13.000000 seldom-3.2.0/seldom/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.617517 seldom-3.2.0/seldom/db_operation/
--rw-rw-rw-   0        0        0       64 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/db_operation/__init__.py
--rw-rw-rw-   0        0        0     1698 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/db_operation/base_db.py
--rw-rw-rw-   0        0        0      715 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/db_operation/mongo_db.py
--rw-rw-rw-   0        0        0     3610 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/db_operation/mssql_db.py
--rw-rw-rw-   0        0        0     3867 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/db_operation/mysql_db.py
--rw-rw-rw-   0        0        0     2856 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/db_operation/sqlite_db.py
--rw-rw-rw-   0        0        0     5665 2023-03-14 15:43:32.000000 seldom-3.2.0/seldom/driver.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.620516 seldom-3.2.0/seldom/har2case/
--rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/har2case/__init__.py
--rw-rw-rw-   0        0        0     4014 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/har2case/core.py
--rw-rw-rw-   0        0        0     1171 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/har2case/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.624520 seldom-3.2.0/seldom/logging/
--rw-rw-rw-   0        0        0       48 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/logging/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-01-02 07:33:41.000000 seldom-3.2.0/seldom/logging/exceptions.py
--rw-rw-rw-   0        0        0     1858 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/logging/log.py
--rw-rw-rw-   0        0        0    11786 2023-03-13 16:12:38.000000 seldom-3.2.0/seldom/request.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.631065 seldom-3.2.0/seldom/running/
--rw-rw-rw-   0        0        0     2477 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/running/DebugTestRunner.py
--rw-rw-rw-   0        0        0      803 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/running/__init__.py
--rw-rw-rw-   0        0        0      561 2023-03-14 15:43:32.000000 seldom-3.2.0/seldom/running/config.py
--rw-rw-rw-   0        0        0     1467 2022-12-07 17:25:01.000000 seldom-3.2.0/seldom/running/loader.py
--rw-rw-rw-   0        0        0     7450 2022-12-15 14:14:22.000000 seldom-3.2.0/seldom/running/loader_extend.py
--rw-rw-rw-   0        0        0     1006 2022-12-12 16:47:54.000000 seldom-3.2.0/seldom/running/loader_hook.py
--rw-rw-rw-   0        0        0    14706 2023-03-14 15:43:32.000000 seldom-3.2.0/seldom/running/runner.py
--rw-rw-rw-   0        0        0     2670 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/skip.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.636874 seldom-3.2.0/seldom/testdata/
--rw-rw-rw-   0        0        0       28 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/testdata/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/testdata/conversion.py
--rw-rw-rw-   0        0        0    10731 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/testdata/parameterization.py
--rw-rw-rw-   0        0        0    18847 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/testdata/random_data.py
--rw-rw-rw-   0        0        0    11986 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/testdata/random_func.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.651889 seldom-3.2.0/seldom/utils/
--rw-rw-rw-   0        0        0      206 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/__init__.py
--rw-rw-rw-   0        0        0     3594 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/utils/cache.py
--rw-rw-rw-   0        0        0     1067 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/curlify.py
--rw-rw-rw-   0        0        0     2395 2023-03-13 16:12:38.000000 seldom-3.2.0/seldom/utils/diff.py
--rw-rw-rw-   0        0        0     3280 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/file_extend.py
--rw-rw-rw-   0        0        0      438 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/genson.py
--rw-rw-rw-   0        0        0      243 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/jmespath.py
--rw-rw-rw-   0        0        0    10473 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/jsonpath.py
--rw-rw-rw-   0        0        0     3964 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/klook.py
--rw-rw-rw-   0        0        0     1500 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/utils/send_extend.py
--rw-rw-rw-   0        0        0     1577 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/utils/thread_lab.py
--rw-rw-rw-   0        0        0     1543 2022-12-06 15:42:11.000000 seldom-3.2.0/seldom/utils/webdriver_manager_extend.py
--rw-rw-rw-   0        0        0    32386 2023-03-13 16:12:23.000000 seldom-3.2.0/seldom/webdriver.py
--rw-rw-rw-   0        0        0    10549 2022-12-06 15:57:51.000000 seldom-3.2.0/seldom/webdriver_chaining.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.605503 seldom-3.2.0/seldom.egg-info/
--rw-rw-rw-   0        0        0     1012 2023-03-14 15:53:10.000000 seldom-3.2.0/seldom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2364 2023-03-14 15:53:10.000000 seldom-3.2.0/seldom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 15:53:10.000000 seldom-3.2.0/seldom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-03-14 15:53:10.000000 seldom-3.2.0/seldom.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 14:29:25.000000 seldom-3.2.0/seldom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      252 2023-03-14 15:53:10.000000 seldom-3.2.0/seldom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-14 15:53:10.000000 seldom-3.2.0/seldom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 15:53:10.673894 seldom-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1853 2023-03-13 16:12:23.000000 seldom-3.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-14 15:53:10.669889 seldom-3.2.0/test/
--rw-rw-rw-   0        0        0      594 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_cache.py
--rw-rw-rw-   0        0        0     8814 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_db_operation.py
--rw-rw-rw-   0        0        0      691 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_klook.py
--rw-rw-rw-   0        0        0     1062 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_log.py
--rw-rw-rw-   0        0        0     2204 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_testdata.py
--rw-rw-rw-   0        0        0     1658 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_thread.py
--rw-rw-rw-   0        0        0      999 2022-12-06 15:57:51.000000 seldom-3.2.0/test/test_thread2.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.427087 seldom-3.2.1/
+-rw-rw-rw-   0        0        0    11565 2022-12-06 15:57:51.000000 seldom-3.2.1/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-12-06 15:57:51.000000 seldom-3.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1118 2023-04-13 16:55:00.426085 seldom-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9605 2023-03-19 02:36:19.000000 seldom-3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.269780 seldom-3.2.1/demo/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/confrun.py
+-rw-rw-rw-   0        0        0     1583 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/run.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.272782 seldom-3.2.1/demo/test_dir/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.275785 seldom-3.2.1/demo/test_dir/api_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/api_case/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/api_case/test_http_demo.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.283790 seldom-3.2.1/demo/test_dir/app_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/app_case/__init__.py
+-rw-rw-rw-   0        0        0      994 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/app_case/test_first_demo.py
+-rw-rw-rw-   0        0        0     1231 2023-03-19 02:35:00.000000 seldom-3.2.1/demo/test_dir/app_case/test_po_demo.py
+-rw-rw-rw-   0        0        0      875 2023-03-14 15:43:32.000000 seldom-3.2.1/demo/test_dir/app_case/test_u2_demo.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.296793 seldom-3.2.1/demo/test_dir/web_case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/web_case/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/web_case/test_data_demo.py
+-rw-rw-rw-   0        0        0     4287 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/web_case/test_ddt_demo.py
+-rw-rw-rw-   0        0        0      589 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/web_case/test_first_demo.py
+-rw-rw-rw-   0        0        0      846 2022-12-06 15:57:51.000000 seldom-3.2.1/demo/test_dir/web_case/test_fixture_demo.py
+-rw-rw-rw-   0        0        0      953 2023-01-11 15:24:10.000000 seldom-3.2.1/demo/test_dir/web_case/test_playwright_demo.py
+-rw-rw-rw-   0        0        0     1194 2023-03-19 02:31:03.000000 seldom-3.2.1/demo/test_dir/web_case/test_po_demo.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.303852 seldom-3.2.1/proj/
+-rw-rw-rw-   0        0        0        0 2022-12-08 16:29:03.000000 seldom-3.2.1/proj/__init__.py
+-rw-rw-rw-   0        0        0      110 2022-12-12 15:41:44.000000 seldom-3.2.1/proj/confrun.py
+-rw-rw-rw-   0        0        0     1031 2022-12-12 15:42:40.000000 seldom-3.2.1/proj/loader.py
+-rw-rw-rw-   0        0        0      293 2022-12-12 15:41:28.000000 seldom-3.2.1/proj/run.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.318852 seldom-3.2.1/seldom/
+-rw-rw-rw-   0        0        0     1305 2023-04-13 16:51:46.000000 seldom-3.2.1/seldom/__init__.py
+-rw-rw-rw-   0        0        0     5373 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/appdriver.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.338853 seldom-3.2.1/seldom/appium_lab/
+-rw-rw-rw-   0        0        0     1669 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/appium_lab/__init__.py
+-rw-rw-rw-   0        0        0     3909 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/appium_lab/action.py
+-rw-rw-rw-   0        0        0     7248 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/appium_lab/find.py
+-rw-rw-rw-   0        0        0     2997 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/appium_lab/keyboard.py
+-rw-rw-rw-   0        0        0     1721 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/appium_lab/switch.py
+-rw-rw-rw-   0        0        0    11006 2023-03-13 16:12:38.000000 seldom-3.2.1/seldom/case.py
+-rw-rw-rw-   0        0        0    13177 2022-12-16 17:09:13.000000 seldom-3.2.1/seldom/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.348853 seldom-3.2.1/seldom/db_operation/
+-rw-rw-rw-   0        0        0       64 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/db_operation/__init__.py
+-rw-rw-rw-   0        0        0     1698 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/db_operation/base_db.py
+-rw-rw-rw-   0        0        0      715 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/db_operation/mongo_db.py
+-rw-rw-rw-   0        0        0     3958 2023-04-13 16:34:19.000000 seldom-3.2.1/seldom/db_operation/mssql_db.py
+-rw-rw-rw-   0        0        0     4265 2023-04-13 16:36:12.000000 seldom-3.2.1/seldom/db_operation/mysql_db.py
+-rw-rw-rw-   0        0        0     3159 2023-04-13 16:31:28.000000 seldom-3.2.1/seldom/db_operation/sqlite_db.py
+-rw-rw-rw-   0        0        0     5665 2023-03-14 15:43:32.000000 seldom-3.2.1/seldom/driver.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.352852 seldom-3.2.1/seldom/har2case/
+-rw-rw-rw-   0        0        0        0 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/har2case/__init__.py
+-rw-rw-rw-   0        0        0     4014 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/har2case/core.py
+-rw-rw-rw-   0        0        0     1171 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/har2case/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.358856 seldom-3.2.1/seldom/logging/
+-rw-rw-rw-   0        0        0       48 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/logging/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-01-02 07:33:41.000000 seldom-3.2.1/seldom/logging/exceptions.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 00:03:22.000000 seldom-3.2.1/seldom/logging/log.py
+-rw-rw-rw-   0        0        0    11842 2023-03-19 02:45:19.000000 seldom-3.2.1/seldom/request.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.371857 seldom-3.2.1/seldom/running/
+-rw-rw-rw-   0        0        0     2477 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/running/DebugTestRunner.py
+-rw-rw-rw-   0        0        0      803 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/running/__init__.py
+-rw-rw-rw-   0        0        0      561 2023-03-14 15:43:32.000000 seldom-3.2.1/seldom/running/config.py
+-rw-rw-rw-   0        0        0     1467 2022-12-07 17:25:01.000000 seldom-3.2.1/seldom/running/loader.py
+-rw-rw-rw-   0        0        0     7450 2022-12-15 14:14:22.000000 seldom-3.2.1/seldom/running/loader_extend.py
+-rw-rw-rw-   0        0        0     1006 2022-12-12 16:47:54.000000 seldom-3.2.1/seldom/running/loader_hook.py
+-rw-rw-rw-   0        0        0    14706 2023-03-14 15:43:32.000000 seldom-3.2.1/seldom/running/runner.py
+-rw-rw-rw-   0        0        0     2670 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/skip.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.381856 seldom-3.2.1/seldom/testdata/
+-rw-rw-rw-   0        0        0       28 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/testdata/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/testdata/conversion.py
+-rw-rw-rw-   0        0        0    10749 2023-04-03 16:11:58.000000 seldom-3.2.1/seldom/testdata/parameterization.py
+-rw-rw-rw-   0        0        0    18847 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/testdata/random_data.py
+-rw-rw-rw-   0        0        0    11986 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/testdata/random_func.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.407083 seldom-3.2.1/seldom/utils/
+-rw-rw-rw-   0        0        0      232 2023-04-01 06:05:16.000000 seldom-3.2.1/seldom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5564 2023-04-01 06:05:16.000000 seldom-3.2.1/seldom/utils/cache.py
+-rw-rw-rw-   0        0        0     1067 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/curlify.py
+-rw-rw-rw-   0        0        0     2395 2023-03-13 16:12:38.000000 seldom-3.2.1/seldom/utils/diff.py
+-rw-rw-rw-   0        0        0     3280 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/file_extend.py
+-rw-rw-rw-   0        0        0      438 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/genson.py
+-rw-rw-rw-   0        0        0      243 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/jmespath.py
+-rw-rw-rw-   0        0        0    10473 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/jsonpath.py
+-rw-rw-rw-   0        0        0     3964 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/klook.py
+-rw-rw-rw-   0        0        0     1500 2023-03-13 16:12:23.000000 seldom-3.2.1/seldom/utils/send_extend.py
+-rw-rw-rw-   0        0        0     1577 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/utils/thread_lab.py
+-rw-rw-rw-   0        0        0     1543 2022-12-06 15:42:11.000000 seldom-3.2.1/seldom/utils/webdriver_manager_extend.py
+-rw-rw-rw-   0        0        0    31413 2023-04-03 17:12:07.000000 seldom-3.2.1/seldom/webdriver.py
+-rw-rw-rw-   0        0        0    10549 2022-12-06 15:57:51.000000 seldom-3.2.1/seldom/webdriver_chaining.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.330852 seldom-3.2.1/seldom.egg-info/
+-rw-rw-rw-   0        0        0     1118 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2390 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 14:29:25.000000 seldom-3.2.1/seldom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      252 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 16:54:59.000000 seldom-3.2.1/seldom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 16:55:00.428083 seldom-3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1853 2023-03-13 16:12:23.000000 seldom-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:55:00.424083 seldom-3.2.1/test/
+-rw-rw-rw-   0        0        0      594 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_cache.py
+-rw-rw-rw-   0        0        0     8814 2023-04-13 16:38:59.000000 seldom-3.2.1/test/test_db_operation.py
+-rw-rw-rw-   0        0        0      691 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_klook.py
+-rw-rw-rw-   0        0        0     1062 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_log.py
+-rw-rw-rw-   0        0        0      761 2023-04-01 06:05:16.000000 seldom-3.2.1/test/test_memory_cache.py
+-rw-rw-rw-   0        0        0     2204 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_testdata.py
+-rw-rw-rw-   0        0        0     1658 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_thread.py
+-rw-rw-rw-   0        0        0      999 2022-12-06 15:57:51.000000 seldom-3.2.1/test/test_thread2.py
```

### Comparing `seldom-3.2.0/LICENSE` & `seldom-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/PKG-INFO` & `seldom-3.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: seldom
-Version: 3.2.0
+Version: 3.2.1
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://github.com/seldomQA/seldom/
 Author: bugmaster
 Author-email: fnngj@126.com
 License: BSD
+Description: seldom
+        ---------------
+        
+        WebUI/HTTP automation testing framework based on unittest.
+        
+        Installation
+        ------------
+        
+            $ pip install seldom
+        
+        
+        Documentation
+        ++++++++++++++++++
+        
+        https://github.com/SeldomQA/seldom
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
-License-File: LICENSE
-
-seldom
----------------
-
-WebUI/HTTP automation testing framework based on unittest.
-
-Installation
-------------
-
-    $ pip install seldom
-
-
-Documentation
-++++++++++++++++++
-
-https://github.com/SeldomQA/seldom
-
-
```

### Comparing `seldom-3.2.0/README.md` & `seldom-3.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 - [x] 提供脚手架快速创建自动化项目
 - [x] 集成`XTestRunner`测试报告，现代美观
 - [x] 提供丰富的断言
 - [x] 提供强大的`数据驱动`
 - [x] 平台化支持
 
 ### Install
-> 2.10.0 为了解决[107](https://github.com/SeldomQA/seldom/issues/107) 问题，我们经过反复的讨论和优化，甚至对相关库XTestRunner做了修改；以为完美解决了这个问题，没想到还是引起了一些严重的错误。为此，我们感到非常沮丧，退回到2.9.0的实现方案。请升级到2.10.1以上版本。
 
 ```shell
-pip install seldom==3.1.0
+pip install seldom==3.2.0
 ```
 
 If you want to keep up with the latest version, you can install with github repository url:
 
 ```shell
 > pip install -U git+https://github.com/SeldomQA/seldom.git@master
 ```
```

### Comparing `seldom-3.2.0/demo/confrun.py` & `seldom-3.2.1/demo/confrun.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/run.py` & `seldom-3.2.1/demo/run.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/api_case/test_http_demo.py` & `seldom-3.2.1/demo/test_dir/api_case/test_http_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/app_case/test_first_demo.py` & `seldom-3.2.1/demo/test_dir/app_case/test_first_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/app_case/test_po_demo.py` & `seldom-3.2.1/demo/test_dir/app_case/test_po_demo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import seldom
 from poium import Page, Element, Elements
 
 
 class BBSPage(Page):
     """BBS Page"""
-    search_input = Element(id_="com.meizu.flyme.flymebbs:id/nw")
-    search_button = Element(id_="com.meizu.flyme.flymebbs:id/o1")
-    search_result = Elements(id_="com.meizu.flyme.flymebbs:id/a29")
+    search_input = Element("id=com.meizu.flyme.flymebbs:id/nw")
+    search_button = Element("id=com.meizu.flyme.flymebbs:id/o1")
+    search_result = Elements("id=com.meizu.flyme.flymebbs:id/a29")
 
 
 class TestBBS(seldom.TestCase):
     """
     Test BBS
     """
 
     def start(self):
-        self.bbs_page = BBSPage(self.driver)
+        self.bbs_page = BBSPage()
 
     def test_bbs(self):
         """
         test bbs search
         """
         self.sleep(5)
         self.bbs_page.search_input.click()
         self.bbs_page.search_input.send_keys("flyme")
         self.bbs_page.search_button.click()
-        elems = self.bbs_page.search_result
-        for title in elems:
+        titles = self.bbs_page.search_result
+        for title in titles:
             self.assertIn("flyme", title.text.lower())
 
 
 if __name__ == '__main__':
     desired_caps = {
         'deviceName': 'JEF_AN20',
         'automationName': 'UiAutomator2',
```

### Comparing `seldom-3.2.0/demo/test_dir/app_case/test_u2_demo.py` & `seldom-3.2.1/demo/test_dir/app_case/test_u2_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/web_case/test_data_demo.py` & `seldom-3.2.1/demo/test_dir/web_case/test_data_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/web_case/test_ddt_demo.py` & `seldom-3.2.1/demo/test_dir/web_case/test_ddt_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/web_case/test_first_demo.py` & `seldom-3.2.1/demo/test_dir/web_case/test_first_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/web_case/test_fixture_demo.py` & `seldom-3.2.1/demo/test_dir/web_case/test_fixture_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/web_case/test_playwright_demo.py` & `seldom-3.2.1/demo/test_dir/web_case/test_playwright_demo.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/demo/test_dir/web_case/test_po_demo.py` & `seldom-3.2.1/demo/test_dir/web_case/test_po_demo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 """
 page object model
 Using the poium Library
 https://github.com/SeldomQA/poium
 ```
-> pip install poium=1.2.0
+> pip install poium>=1.3.2
 ```
 """
 import seldom
 from poium import Page, Element, Elements
 
 
 class BaiduPage(Page):
     """baidu page"""
     input = Element("#kw", describe="搜索输入框")
     button = Element("id=su", describe="搜索按钮")
-    result = Elements("//div/h3/a", describe="结果")
+    result = Elements("//div/h3/a", describe="搜索结果")
 
 
 class BaiduTest(seldom.TestCase):
     """Baidu search test case"""
 
     def test_case(self):
         """
         A simple test
         """
-        page = BaiduPage(print_log=True)
+        page = BaiduPage()
         page.open("https://www.baidu.com")
         self.sleep(3)
-        # assert element
+
+        # assert element is exist
         self.assertTrue(page.input.is_exist())
+        self.assertTrue(page.button.is_exist())
+
+        # operation element
         page.input.send_keys("seldom")
         page.button.click()
         self.sleep(3)
+
         # assert title
         self.assertTitle("seldom_百度搜索")
 
+        # Loop assertion result
         for r in page.result:
             # assert text in
             self.assertIn("seldom", r.text)
 
 
 if __name__ == '__main__':
-    seldom.main(browser='chrome', debug=True)
+    seldom.main(browser='chrome')
```

### Comparing `seldom-3.2.0/proj/loader.py` & `seldom-3.2.1/proj/loader.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/__init__.py` & `seldom-3.2.1/seldom/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 from .skip import *
 from .driver import *
 from .testdata.parameterization import *
 
 
 __author__ = "bugmaster"
 
-__version__ = "3.2.0"
+__version__ = "3.2.1"
 
 __description__ = "WebUI/HTTP automation testing framework based on unittest."
```

### Comparing `seldom-3.2.0/seldom/appdriver.py` & `seldom-3.2.1/seldom/appdriver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/appium_lab/__init__.py` & `seldom-3.2.1/seldom/appium_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/appium_lab/action.py` & `seldom-3.2.1/seldom/appium_lab/action.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/appium_lab/find.py` & `seldom-3.2.1/seldom/appium_lab/find.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/appium_lab/keyboard.py` & `seldom-3.2.1/seldom/appium_lab/keyboard.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/appium_lab/switch.py` & `seldom-3.2.1/seldom/appium_lab/switch.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/case.py` & `seldom-3.2.1/seldom/case.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/cli.py` & `seldom-3.2.1/seldom/cli.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/db_operation/base_db.py` & `seldom-3.2.1/seldom/db_operation/base_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/db_operation/mongo_db.py` & `seldom-3.2.1/seldom/db_operation/mongo_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/db_operation/mssql_db.py` & `seldom-3.2.1/seldom/db_operation/mssql_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,26 @@
         """
         with self.connection.cursor() as cursor:
             cursor.execute(sql)
             row = cursor.fetchone()
             self.connection.commit()
             return row
 
+    def insert_get_last_id(self, sql: str) -> int:
+        """
+        insert sql and get last row id
+        :param sql:
+        :return:
+        """
+        with self.connection.cursor() as cursor:
+            cursor.execute(sql)
+            last_id = cursor.lastrowid
+            self.connection.commit()
+            return last_id
+
     def insert_data(self, table: str, data: dict) -> None:
         """
         insert sql statement
         """
         for key in data:
             data[key] = "'" + str(data[key]) + "'"
         key = ','.join(data.keys())
```

### Comparing `seldom-3.2.0/seldom/db_operation/mysql_db.py` & `seldom-3.2.1/seldom/db_operation/mysql_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,27 @@
         with self.connection.cursor() as cursor:
             self.connection.ping(reconnect=True)
             cursor.execute(sql)
             row = cursor.fetchone()
             self.connection.commit()
             return row
 
+    def insert_get_last_id(self, sql: str) -> int:
+        """
+        insert sql and get last row id
+        :param sql:
+        :return:
+        """
+        with self.connection.cursor() as cursor:
+            self.connection.ping(reconnect=True)
+            cursor.execute(sql)
+            last_id = cursor.lastrowid
+            self.connection.commit()
+            return last_id
+
     def insert_data(self, table: str, data: dict) -> None:
         """
         insert sql statement
         """
         for key in data:
             data[key] = "'" + str(data[key]) + "'"
         key = ','.join(data.keys())
```

### Comparing `seldom-3.2.0/seldom/db_operation/sqlite_db.py` & `seldom-3.2.1/seldom/db_operation/sqlite_db.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,25 @@
         Query one data SQL
         return: query data
         """
         self.cursor.execute(sql)
         row = self.cursor.fetchone()
         return row
 
+    def insert_get_last_id(self, sql: str) -> int:
+        """
+        insert sql and get last row id
+        :param sql:
+        :return: query data
+        """
+        self.cursor.execute(sql)
+        last_id = self.cursor.lastrowid
+        self.connection.commit()
+        return last_id
+
     def select_data(self, table: str, where: dict = None, one: bool = False) -> Any:
         """
         select sql statement
         """
         sql = f"""select * from {table} """
         if where is not None:
             sql += f""" where {self.dict_to_str_and(where)}"""
```

### Comparing `seldom-3.2.0/seldom/driver.py` & `seldom-3.2.1/seldom/driver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/har2case/core.py` & `seldom-3.2.1/seldom/har2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/har2case/utils.py` & `seldom-3.2.1/seldom/har2case/utils.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/logging/exceptions.py` & `seldom-3.2.1/seldom/logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/logging/log.py` & `seldom-3.2.1/seldom/logging/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         :param format:
         :param level:
         :return:
         """
         if format is None:
             format = self._console_format
         self.logger.remove()
+        self._level = level
         self.logger.add(sys.stderr, level=level, colorize=colorlog, format=format)
         self.logger.add(self.logfile, level=level, colorize=False, format=self._log_format, encoding="utf-8")
 
 
 # log level: TRACE < DEBUG < INFO < SUCCESS < WARNING < ERROR
 log_cfg = LogConfig(level="TRACE")
 log = logger
```

### Comparing `seldom-3.2.0/seldom/request.py` & `seldom-3.2.1/seldom/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         @request
         def get(self, url, **kwargs):
             r"""Sends a GET request. Returns :class:`Response` object.
             :param url: URL for the new :class:`Request` object.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
-            if (Seldom.base_url is not None) and ("http" not in url):
+            if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
             kwargs.setdefault('allow_redirects', True)
             return self.request('GET', url, **kwargs)
 
         @request
         def post(self, url, data=None, json=None, **kwargs):
             r"""Sends a POST request. Returns :class:`Response` object.
@@ -210,55 +210,54 @@
             :param url: URL for the new :class:`Request` object.
             :param data: (optional) Dictionary, list of tuples, bytes, or file-like
                 object to send in the body of the :class:`Request`.
             :param json: (optional) json to send in the body of the :class:`Request`.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
-            if (Seldom.base_url is not None) and ("http" not in url):
+            if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
             return self.request('POST', url, data=data, json=json, **kwargs)
 
         @request
         def put(self, url, data=None, **kwargs):
             r"""Sends a PUT request. Returns :class:`Response` object.
 
             :param url: URL for the new :class:`Request` object.
             :param data: (optional) Dictionary, list of tuples, bytes, or file-like
                 object to send in the body of the :class:`Request`.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
-            if (Seldom.base_url is not None) and ("http" not in url):
+            if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
             return self.request('PUT', url, data=data, **kwargs)
 
         @request
         def delete(self, url, **kwargs):
             r"""Sends a DELETE request. Returns :class:`Response` object.
 
             :param url: URL for the new :class:`Request` object.
             :param \*\*kwargs: Optional arguments that ``request`` takes.
             :rtype: requests.Response
             """
-            if (Seldom.base_url is not None) and ("http" not in url):
+            if (Seldom.base_url is not None) and (url.startswith("http") is False):
                 url = Seldom.base_url + url
             return self.request('DELETE', url, **kwargs)
 
     @staticmethod
     def json_to_dict(data: str, replace_quotes: bool = True) -> dict:
         """
         json to dict
         :param data: json data.
         :param replace_quotes: whether to replace single quotes.
         """
         if isinstance(data, dict):
             return data
-
-        if isinstance(data, str):
+        elif isinstance(data, str):
             try:
                 data_dict = ast.literal_eval(data)
             except ValueError:
                 try:
                     if replace_quotes:
                         data = data.replace('\'', '\"')
                     data_dict = json.loads(data)
```

### Comparing `seldom-3.2.0/seldom/running/DebugTestRunner.py` & `seldom-3.2.1/seldom/running/DebugTestRunner.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/running/__init__.py` & `seldom-3.2.1/seldom/running/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/running/config.py` & `seldom-3.2.1/seldom/running/config.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/running/loader.py` & `seldom-3.2.1/seldom/running/loader.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/running/loader_extend.py` & `seldom-3.2.1/seldom/running/loader_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/running/loader_hook.py` & `seldom-3.2.1/seldom/running/loader_hook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/running/runner.py` & `seldom-3.2.1/seldom/running/runner.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/skip.py` & `seldom-3.2.1/seldom/skip.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/testdata/conversion.py` & `seldom-3.2.1/seldom/testdata/conversion.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/testdata/parameterization.py` & `seldom-3.2.1/seldom/testdata/parameterization.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,19 +259,19 @@
         delete_patches_if_need(f)
 
         f.__test__ = False
 
     return parameterized_expand_wrapper
 
 
-def data_class(attrs, input_values):
+def data_class(attrs, input_values=None):
     """
     Parameterizes a test class by setting attributes on the class.
     """
-    return parameterized_class(attrs, input_values)
+    return parameterized_class(attrs, input_values=input_values)
 
 
 def default_name_func(func, num, p):
     """
     return test function name
     """
     base_name = func.__name__
```

### Comparing `seldom-3.2.0/seldom/testdata/random_data.py` & `seldom-3.2.1/seldom/testdata/random_data.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/testdata/random_func.py` & `seldom-3.2.1/seldom/testdata/random_func.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/curlify.py` & `seldom-3.2.1/seldom/utils/curlify.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/diff.py` & `seldom-3.2.1/seldom/utils/diff.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/file_extend.py` & `seldom-3.2.1/seldom/utils/file_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/jsonpath.py` & `seldom-3.2.1/seldom/utils/jsonpath.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/klook.py` & `seldom-3.2.1/seldom/utils/klook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/send_extend.py` & `seldom-3.2.1/seldom/utils/send_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/thread_lab.py` & `seldom-3.2.1/seldom/utils/thread_lab.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/utils/webdriver_manager_extend.py` & `seldom-3.2.1/seldom/utils/webdriver_manager_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom/webdriver.py` & `seldom-3.2.1/seldom/webdriver.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from selenium.webdriver import Chrome
 from selenium.webdriver.remote.webdriver import WebDriver as SeleniumWebDriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.chrome.service import Service as cService
+from appium.webdriver.common.appiumby import AppiumBy
 from seldom.logging import log
 from seldom.running.config import Seldom
 from seldom.logging.exceptions import NotFindElementError
 from seldom.utils.webdriver_manager_extend import ChromeDriverManager
 from seldom.testdata import get_timestamp
 
 
@@ -27,86 +28,66 @@
     'id_': By.ID,
     'name': By.NAME,
     'xpath': By.XPATH,
     'link_text': By.LINK_TEXT,
     'partial_link_text': By.PARTIAL_LINK_TEXT,
     'tag': By.TAG_NAME,
     'class_name': By.CLASS_NAME,
+    'ios_uiautomation': AppiumBy.IOS_UIAUTOMATION,
+    'ios_predicate': AppiumBy.IOS_PREDICATE,
+    'ios_class_chain': AppiumBy.IOS_CLASS_CHAIN,
+    'android_uiautomator': AppiumBy.ANDROID_UIAUTOMATOR,
+    'android_viewtag': AppiumBy.ANDROID_VIEWTAG,
+    'android_data_matcher': AppiumBy.ANDROID_DATA_MATCHER,
+    'android_view_matcher': AppiumBy.ANDROID_VIEW_MATCHER,
+    'windows_uiautomation': AppiumBy.WINDOWS_UI_AUTOMATION,
+    'accessibility_id': AppiumBy.ACCESSIBILITY_ID,
+    'image': AppiumBy.IMAGE,
+    'custom': AppiumBy.CUSTOM,
 }
 
 
 class WebElement:
     """web element API"""
 
     def __init__(self, **kwargs) -> None:
         if not kwargs:
             raise ValueError("Please specify a locator")
         if len(kwargs) > 1:
             raise ValueError("Please specify only one locator")
 
-        self.by, self.value = next(iter(kwargs.items()))
-        try:
-            LOCATOR_LIST[self.by]
-        except KeyError:
-            raise ValueError(f"Element positioning of type '{self.by}' is not supported. ")
+        by, self.value = next(iter(kwargs.items()))
+
+        self.by = LOCATOR_LIST.get(by)
+        if self.by is None:
+            raise ValueError(f"The find element is not supported: {by}. ")
         self.find_elem_info = None
         self.find_elem_warn = None
 
-    def __find_element(self, elem: tuple) -> None:
+    def get_elements(self, index: int = None):
         """
-        Find if the element exists.
+        Judge element positioning way, and returns the element.
         """
+
         for _ in range(Seldom.timeout):
-            elems = Seldom.driver.find_elements(by=elem[0], value=elem[1])
+            elems = Seldom.driver.find_elements(by=self.by, value=self.value)
             if len(elems) >= 1:
-                self.find_elem_info = f"Find {len(elems)} element: {elem[0]}={elem[1]} "
+                self.find_elem_info = f"Find {len(elems)} element: {self.by}={self.value} "
                 break
             time.sleep(1)
         else:
-            self.find_elem_warn = f"❌ Find 0 element through: {elem[0]}={elem[1]}"
+            self.find_elem_warn = f"❌ Find 0 element through: {self.by}={self.value}"
 
-    def get_elements(self, index: int = None):
-        """
-        Judge element positioning way, and returns the element.
-        """
-
-        if self.by == "id_":
-            self.__find_element((By.ID, self.value))
-            elem = Seldom.driver.find_elements(By.ID, self.value)
-        elif self.by == "name":
-            self.__find_element((By.NAME, self.value))
-            elem = Seldom.driver.find_elements(By.NAME, self.value)
-        elif self.by == "class_name":
-            self.__find_element((By.CLASS_NAME, self.value))
-            elem = Seldom.driver.find_elements(By.CLASS_NAME, self.value)
-        elif self.by == "tag":
-            self.__find_element((By.TAG_NAME, self.value))
-            elem = Seldom.driver.find_elements(By.TAG_NAME, self.value)
-        elif self.by == "link_text":
-            self.__find_element((By.LINK_TEXT, self.value))
-            elem = Seldom.driver.find_elements(By.LINK_TEXT, self.value)
-        elif self.by == "partial_link_text":
-            self.__find_element((By.PARTIAL_LINK_TEXT, self.value))
-            elem = Seldom.driver.find_elements(By.PARTIAL_LINK_TEXT, self.value)
-        elif self.by == "xpath":
-            self.__find_element((By.XPATH, self.value))
-            elem = Seldom.driver.find_elements(By.XPATH, self.value)
-        elif self.by == "css":
-            self.__find_element((By.CSS_SELECTOR, self.value))
-            elem = Seldom.driver.find_elements(By.CSS_SELECTOR, self.value)
-        else:
-            raise NameError(
-                "Please enter the correct targeting elements,'id_/name/class_name/tag/link_text/xpath/css'.")
+        elem = Seldom.driver.find_elements(self.by, self.value)
+        if len(elem) == 0:
+            raise NotFindElementError(self.find_elem_warn)
 
         if index is None:
             return elem
 
-        if len(elem) == 0:
-            raise NotFindElementError(self.find_elem_warn)
-
         return elem[index]
 
     @staticmethod
     def show_element(elem) -> None:
         """
         Show the elements of the operation
         :param elem:
```

### Comparing `seldom-3.2.0/seldom/webdriver_chaining.py` & `seldom-3.2.1/seldom/webdriver_chaining.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/seldom.egg-info/PKG-INFO` & `seldom-3.2.1/seldom.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: seldom
-Version: 3.2.0
+Version: 3.2.1
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://github.com/seldomQA/seldom/
 Author: bugmaster
 Author-email: fnngj@126.com
 License: BSD
+Description: seldom
+        ---------------
+        
+        WebUI/HTTP automation testing framework based on unittest.
+        
+        Installation
+        ------------
+        
+            $ pip install seldom
+        
+        
+        Documentation
+        ++++++++++++++++++
+        
+        https://github.com/SeldomQA/seldom
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
-License-File: LICENSE
-
-seldom
----------------
-
-WebUI/HTTP automation testing framework based on unittest.
-
-Installation
-------------
-
-    $ pip install seldom
-
-
-Documentation
-++++++++++++++++++
-
-https://github.com/SeldomQA/seldom
-
-
```

### Comparing `seldom-3.2.0/seldom.egg-info/SOURCES.txt` & `seldom-3.2.1/seldom.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,10 +80,11 @@
 seldom/utils/send_extend.py
 seldom/utils/thread_lab.py
 seldom/utils/webdriver_manager_extend.py
 test/test_cache.py
 test/test_db_operation.py
 test/test_klook.py
 test/test_log.py
+test/test_memory_cache.py
 test/test_testdata.py
 test/test_thread.py
 test/test_thread2.py
```

### Comparing `seldom-3.2.0/setup.py` & `seldom-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_cache.py` & `seldom-3.2.1/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_db_operation.py` & `seldom-3.2.1/test/test_db_operation.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_klook.py` & `seldom-3.2.1/test/test_klook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_log.py` & `seldom-3.2.1/test/test_log.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_testdata.py` & `seldom-3.2.1/test/test_testdata.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_thread.py` & `seldom-3.2.1/test/test_thread.py`

 * *Files identical despite different names*

### Comparing `seldom-3.2.0/test/test_thread2.py` & `seldom-3.2.1/test/test_thread2.py`

 * *Files identical despite different names*

